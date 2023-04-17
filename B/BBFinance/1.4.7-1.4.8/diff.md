# Comparing `tmp/BBFinance-1.4.7.tar.gz` & `tmp/BBFinance-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.7.tar", last modified: Tue Apr 11 15:10:21 2023, max compression
+gzip compressed data, was "BBFinance-1.4.8.tar", last modified: Mon Apr 17 19:25:57 2023, max compression
```

## Comparing `BBFinance-1.4.7.tar` & `BBFinance-1.4.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.959608 BBFinance-1.4.7/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.004850 BBFinance-1.4.7/BBFdocs/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.239243 BBFinance-1.4.7/BBFdocs/docs/
--rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.4.7/BBFdocs/docs/index.md
--rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.4.7/BBFdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.364258 BBFinance-1.4.7/BBFdocs/site/
--rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/404.html
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.801819 BBFinance-1.4.7/BBFdocs/site/css/
--rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/base.css
--rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/base.min.css
--rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.css
--rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.min.css
--rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/cinder.css
--rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/cinder.min.css
--rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/highlight.css
--rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/highlight.min.css
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:41.286723 BBFinance-1.4.7/BBFdocs/site/fonts/
--rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.woff
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.286930 BBFinance-1.4.7/BBFdocs/site/img/
--rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/favicon.ico
--rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/grid1.png
--rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/grid10.png
--rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid11.png
--rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid12.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid13.png
--rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid14.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid15.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid16.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid17.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid18.png
--rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid19.png
--rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid2.png
--rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid20.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid3.png
--rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid4.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid5.png
--rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid6.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid7.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid8.png
--rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid9.png
--rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/index.html
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.536957 BBFinance-1.4.7/BBFdocs/site/js/
--rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/base.js
--rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/bootstrap-3.0.3.min.js
--rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/highlight.pack.js
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.880753 BBFinance-1.4.7/BBFdocs/site/search/
--rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/lunr.js
--rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/main.js
--rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/search_index.json
--rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/worker.js
--rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/sitemap.xml
--rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/sitemap.xml.gz
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.005764 BBFinance-1.4.7/BBFinance/
--rw-rw-rw-   0        0        0    38842 2023-04-10 19:06:27.000000 BBFinance-1.4.7/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      312 2023-04-10 15:30:26.000000 BBFinance-1.4.7/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.412650 BBFinance-1.4.7/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    23312 2023-04-10 17:41:27.000000 BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.7/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      422 2023-04-10 17:41:27.000000 BBFinance-1.4.7/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.334516 BBFinance-1.4.7/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1918 2023-04-11 15:13:35.000000 BBFinance-1.4.7/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      283 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.709559 BBFinance-1.4.7/Data/
--rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.7/Data/AtivosIbov.xlsx
--rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2023 2023-04-11 15:13:44.975215 BBFinance-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.865867 BBFinance-1.4.7/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.7/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.7/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     1354 2023-04-11 15:11:55.000000 BBFinance-1.4.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 15:13:45.006488 BBFinance-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-04-11 15:12:33.000000 BBFinance-1.4.7/setup.py
--rw-rw-rw-   0        0        0       59 2023-04-10 17:42:02.000000 BBFinance-1.4.7/teste.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:35.259688 BBFinance-1.4.8/
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:15.250270 BBFinance-1.4.8/BBFdocs/
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:18.677462 BBFinance-1.4.8/BBFdocs/docs/
+-rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.4.8/BBFdocs/docs/index.md
+-rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.4.8/BBFdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:19.240188 BBFinance-1.4.8/BBFdocs/site/
+-rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/404.html
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:22.657860 BBFinance-1.4.8/BBFdocs/site/css/
+-rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/base.css
+-rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/base.min.css
+-rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/bootstrap-custom.css
+-rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/bootstrap-custom.min.css
+-rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/cinder.css
+-rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/cinder.min.css
+-rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/highlight.css
+-rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/css/highlight.min.css
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:26.767380 BBFinance-1.4.8/BBFdocs/site/fonts/
+-rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.woff
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:33.118232 BBFinance-1.4.8/BBFdocs/site/img/
+-rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/img/favicon.ico
+-rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/img/grid1.png
+-rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.4.8/BBFdocs/site/img/grid10.png
+-rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid11.png
+-rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid12.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid13.png
+-rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid14.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid15.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid16.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid17.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid18.png
+-rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid19.png
+-rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid2.png
+-rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid20.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid3.png
+-rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid4.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid5.png
+-rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid6.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid7.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid8.png
+-rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/img/grid9.png
+-rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/index.html
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:33.383943 BBFinance-1.4.8/BBFdocs/site/js/
+-rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/js/base.js
+-rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/js/bootstrap-3.0.3.min.js
+-rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/js/highlight.pack.js
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:33.962301 BBFinance-1.4.8/BBFdocs/site/search/
+-rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/search/lunr.js
+-rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/search/main.js
+-rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/search/search_index.json
+-rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/search/worker.js
+-rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/sitemap.xml
+-rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.4.8/BBFdocs/site/sitemap.xml.gz
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:34.118613 BBFinance-1.4.8/BBFinance/
+-rw-rw-rw-   0        0        0    42818 2023-04-17 19:25:32.000000 BBFinance-1.4.8/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      340 2023-04-17 19:24:24.000000 BBFinance-1.4.8/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:34.665702 BBFinance-1.4.8/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.8/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23404 2023-04-12 17:50:16.000000 BBFinance-1.4.8/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.8/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      422 2023-04-10 17:41:27.000000 BBFinance-1.4.8/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:34.603177 BBFinance-1.4.8/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     5070 2023-04-17 19:28:54.000000 BBFinance-1.4.8/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1908 2023-04-17 19:29:13.000000 BBFinance-1.4.8/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 19:28:54.000000 BBFinance-1.4.8/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2023-04-17 19:28:54.000000 BBFinance-1.4.8/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 19:28:54.000000 BBFinance-1.4.8/BBFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     5070 2023-04-17 19:29:35.244069 BBFinance-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4445 2023-04-11 17:27:42.000000 BBFinance-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:35.087746 BBFinance-1.4.8/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.8/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.8/__pycache__/main.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-17 19:29:35.165900 BBFinance-1.4.8/docs/
+-rw-rw-rw-   0        0        0       17 2023-04-11 17:09:57.000000 BBFinance-1.4.8/docs/CNAME
+-rw-rw-rw-   0        0        0     1354 2023-04-11 15:11:55.000000 BBFinance-1.4.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 19:29:35.259688 BBFinance-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1364 2023-04-17 19:26:02.000000 BBFinance-1.4.8/setup.py
+-rw-rw-rw-   0        0        0      361 2023-04-13 13:10:02.000000 BBFinance-1.4.8/teste.py
```

### Comparing `BBFinance-1.4.7/BBFdocs/docs/index.md` & `BBFinance-1.4.8/BBFdocs/docs/index.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/404.html` & `BBFinance-1.4.8/BBFdocs/site/404.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/base.css` & `BBFinance-1.4.8/BBFdocs/site/css/base.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/base.min.css` & `BBFinance-1.4.8/BBFdocs/site/css/base.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.css` & `BBFinance-1.4.8/BBFdocs/site/css/bootstrap-custom.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.min.css` & `BBFinance-1.4.8/BBFdocs/site/css/bootstrap-custom.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/cinder.css` & `BBFinance-1.4.8/BBFdocs/site/css/cinder.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/cinder.min.css` & `BBFinance-1.4.8/BBFdocs/site/css/cinder.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/highlight.css` & `BBFinance-1.4.8/BBFdocs/site/css/highlight.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/css/highlight.min.css` & `BBFinance-1.4.8/BBFdocs/site/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.eot` & `BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.svg` & `BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.ttf` & `BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.woff` & `BBFinance-1.4.8/BBFdocs/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/img/favicon.ico` & `BBFinance-1.4.8/BBFdocs/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/index.html` & `BBFinance-1.4.8/BBFdocs/site/index.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/js/base.js` & `BBFinance-1.4.8/BBFdocs/site/js/base.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/js/bootstrap-3.0.3.min.js` & `BBFinance-1.4.8/BBFdocs/site/js/bootstrap-3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/js/highlight.pack.js` & `BBFinance-1.4.8/BBFdocs/site/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/search/lunr.js` & `BBFinance-1.4.8/BBFdocs/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/search/main.js` & `BBFinance-1.4.8/BBFdocs/site/search/main.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/search/search_index.json` & `BBFinance-1.4.8/BBFdocs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFdocs/site/search/worker.js` & `BBFinance-1.4.8/BBFdocs/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFinance/BBFinance.py` & `BBFinance-1.4.8/BBFinance/BBFinance.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,44 +5,49 @@
 from sklearn.linear_model import LinearRegression
 
 #BIBLIOTECAS PARA WEBSCRAPING
 from selenium import webdriver
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
-# import chromedriver_autoinstaller
+import chromedriver_autoinstaller
 import requests
 from bs4 import BeautifulSoup
+import time
 
 #BIBLIOTECAS DE CHAMADAS DE API
 from fastapi import FastAPI, Response, Request
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 import json
 import uvicorn
-import BBFinance as bb
+
 #BIBLIOTECAS DE ANALISE DE DATAFRAMES, DADOS E CRIAÇAO DE CLASSES
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 from typing import Union
 
 import warnings
 warnings.filterwarnings("ignore")
 
-# chromedriver_autoinstaller.install()
 yf.pdr_override()
 
 today = datetime.today()
 # Data de um ano atrás
 one_year_ago = today - timedelta(days=365)
+one_days_ago = today - timedelta(days=1)
+seven_days_ago = today - timedelta(days=7)
 
 # Convertendo as datas para strings com formato yyyy-mm-dd
 oneY = one_year_ago.strftime('%Y-%m-%d')
+oneD = one_days_ago.strftime('%Y-%m-%d')
+sevenD = seven_days_ago.strftime('%Y-%m-%d')
+
 currently = today.strftime('%Y-%m-%d')
 
 app = FastAPI()
 # templates = Jinja2Templates(directory="Site")
 # app.mount("/Static", StaticFiles(directory="Static"), name="Static")
 
 # @app.get("/", response_class=HTMLResponse)
@@ -200,15 +205,17 @@
     """
     ## Usabilidade 
     - cálculo envolve a comparação da média de ganhos em um período de tempo com a média de perdas em um período de tempo. \n
     
     ## Como interpretar 
     - Quando o RSI está acima de 70, o ativo é considerado sobrecomprado, o que significa que pode estar prestes a sofrer uma correção para baixo. 
     Quando o RSI está abaixo de 30, o ativo é considerado sobrevendido, o que significa que pode estar prestes a subir novamente. \n 
-    
+    - sma_50 -> Media movel dos 50 periodos
+    - sma_200 -> media movel dos 200 peridos
+
     ## Parâmetros
     - symbol -> Nome do Ativo para a busca \n
     
     """
     
     stock = yf.Ticker(symbol)
     info = stock.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
@@ -300,15 +307,15 @@
     
     ## Parâmetros
     - symbol -> Nome do Ativo para a busca \n
     - market -> Como padrao, Mercado: IBOVESPA / BVSP
     """
     
     # Obter os dados do ativo e do mercado
-    asset = yf.Ticker('PETR4.SA')
+    asset = yf.Ticker(symbol)
     market = yf.Ticker("^BVSP") # Índice Bovespa como mercado de referência
     info = asset.info #DADO Q VEM COMO UM DICIONARIO, SE NAO FOR UM DICIONARIO VAI APRESENTAR TICKER INVALIDO, SENAO VAI PASSAR
     infoMarket = market.info
     tipoInfo = type(info)
     if tipoInfo == dict or infoMarket == dict:
         pass 
     else:
@@ -735,15 +742,15 @@
             return valuerisk
                         
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/compareFunds")
 responseHistory = Response(media_type="application/json")
 
 
-## SIMULADOR DE AÇOES ##
+## SIMULADORES DE AÇOES ##
 
 @app.get("/bestAssets", response_model=None)
 def best_assets(perfil= str) -> pd.DataFrame:
     
     """
     ## Usabilidade
     - Função que analisa os principais ativos listados no mercado que com base no perfil escolhido mostra quais podem ser suas escolhas e quantos porcento se deve ter na carteira
@@ -891,15 +898,34 @@
     ## Parâmetros
     
     - valor -> Valor do investimento, por padrão 0
 
     """
     
     # Lista de ativos
-    ativos = pd.read_excel(r'Q:\Risco\Novo Risco\pythonrisco\BBFinance\Data\AtivosIbov.xlsx')
+    chromedriver_autoinstaller.install()
+    chrome_options = Options()
+    chrome_options.add_argument('--headless')
+    driver = webdriver.Chrome(options=chrome_options)
+
+    url = f'https://www.b3.com.br/pt_br/market-data-e-indices/indices/indices-amplos/indice-ibovespa-ibovespa-composicao-da-carteira.htm'
+    driver.get(url)
+    time.sleep(2)
+    cookies = driver.find_element(By.ID, 'onetrust-accept-btn-handler').click()
+    driver.switch_to.frame(driver.find_element(By.XPATH, '//*[@id="bvmf_iframe"]'))
+    select = driver.find_element(By.XPATH, '//*[@id="selectPage"]').click()
+    all = driver.find_element(By.CSS_SELECTOR, '#selectPage > option:nth-child(4)').click()
+
+    table = driver.find_element(By.CSS_SELECTOR, '#divContainerIframeB3 > div > div.col-lg-9.col-12.order-2.order-lg-1 > form > div:nth-child(4) > div > table')
+    table_html = table.get_attribute('outerHTML')
+    ativos = pd.read_html(str(table_html), decimal=',', thousands='.')
+    ativos = ativos[0]
+    ativos = ativos[['Código', 'Ação']]
+    ativos = ativos.drop([88,89])
+
     ativos['Código'] = ativos['Código'].apply(lambda x: x+'.SA')
 
     # Baixa os dados históricos dos ativos nos últimos 12 meses
     precos = yf.download(ativos['Código'].tolist(), period='1y')['Close']
 
     # Remove colunas com valores ausentes
     precos = precos.dropna(axis=1)
@@ -941,41 +967,119 @@
     return ativos_df[['Ativos', 'Qtd Necessaria (R$)', 'Retorno Aprox.']]
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/bestAssetsValues")
 responseHistory = Response(media_type="application/json")
 
 
-#################################################################
 
-def prever_taxa_retorno(ativo):
+## INFORMAÇÕES DE OPÇÕES ##
+
+@app.get("/options/{symbol}/info", response_model=None)
+def get_opc(symbol: str, call: True | False, put: True | False) -> pd.DataFrame():
+
+    """
+    ## Usabilidade
+
+    - Função que apresenta as principais informações das opções do ativo selecionado, informações como: Strike, Var, Gregas, dentre outras.
+
+    ## Parâmetros
+
+    - symbol -> Nome do ativo para buscar as opções referentes a ele.
+    - call -> Recebe True ou False, se True for selecionado a função ira filtrar so as CALL.
+    - put -> Recebe True ou False, se True for selecionado a função ira filtrar so as PUT.
+
+
+    """
+
+
+    if symbol.endswith('.SA'):
+        symbol = symbol.replace('.SA', '')
+    else:
+        print('Procurando dados de opções do ativo selecionado...')
+        pass
+    chromedriver_autoinstaller.install()
+    chrome_options = Options()
+    chrome_options.add_argument('--headless')
+    driver = webdriver.Chrome(options=chrome_options)
+
+    url = f'https://opcoes.net.br/opcoes/bovespa/{symbol}'
+    driver.get(url)
+    time.sleep(1.5)
+    table = driver.find_element(By.CSS_SELECTOR, '#tblListaOpc')
+    table_html = table.get_attribute('outerHTML')
+    dfOPC = pd.read_html(str(table_html), decimal=',', thousands='.')
+    dfOPC = dfOPC[0]
+    dfOPC = dfOPC[['Ticker', 'Tipo', 'Strike', 'A/I/OTM', 'Dist. (%) do Strike', 'Último', 'Var. (%)', 'Núm. de Neg.', 'Vol. Financeiro', 'Delta', 'Gamma', 'Theta ($)', 'Vega']]
+    if call == True:
+        dfCall = dfOPC.loc[dfOPC['Tipo'] == 'CALL']
+        return dfCall
+    elif put == True:
+        dfPut = dfOPC.loc[dfOPC['Tipo'] == 'PUT']
+        return dfPut
+    else:
+        return dfOPC
+
+if __name__ == "__main__":
+    uvicorn.run(app, host="127.0.0.1", port=8000, default="/options/{symbol}/info")
+responseHistory = Response(media_type="application/json")
+
+
+@app.get("/options/blackScholes", response_model=None)
+def black_scholes(Call_or_Put = Union['call', 'put'], ativo= str, preco = float, strike= float, diasUteis= int) -> str:
     
-    dados_historicos = yf.download('PETR4.SA', period='1y')
-    dados_historicos = dados_historicos.reset_index()
+    """
+    ## Usabilidade
+
+    - Função que simula o caculo do black-scholes, modelo no qual é utilizado para precificar opções no mercado de derivativos.
+    - Por se tratar de uma função em desenvolvimento não levar o resultado como verdade absoluta, mas um valor a se basear.
+
+    ## Parâmetros
+
+    - Call_or_Put -> Recebe os valores "call" e "put", por serem calculos diferentes parada cada tipo, é necessario a seleção
+    - ativo -> Inserir o ativo correspondente da função (Exemplo: 'PETR4.SA')
+    - preco -> inserir o preço do ativo selecionado
+    - strike -> Inserir o strike da opção
+    - diasUteis -> Adicionar a quantidade de dias úteis ate o vencimento da opção.
+
+    ## Exemplo
 
-    # Seleciona os dados históricos do ativo
-    # dados_ativo = dados_historicos.loc[dados_historicos['Ativo'] == ativo]
+    ```
+    >>> bb.black_scholes(Call_or_Put= 'call', ativo= 'PETR4.SA', preco= 26.25, strike= 26.25, diasUteis= 22 )
+    ```
 
-    # Separa as variáveis independentes (datas) e dependentes (preços)
-    datas = pd.to_numeric(dados_historicos['Date'].astype(str).str.replace('-', ''))
-    precos = dados_historicos['Close']
+    """
+
+    volatilidadeD = get_volatility(ativo, sevenD, currently)
+    volatilidade = volatilidadeD * 252**2
+    taxaLR= 5.4563 # == 0.1375/252 CDI AO ANO
+    
+    d1 = (np.log(preco/strike) + (taxaLR + (volatilidade**2/2)*diasUteis) * (volatilidade * np.sqrt(diasUteis)))
+    d2 = d1 = (volatilidade * np.sqrt(diasUteis))
+
+    if Call_or_Put == 'call':
+        print('Selecionado Call')
+        C = preco * norm.cdf(d1) - strike * np.exp(-taxaLR*diasUteis) * norm.cdf(d2)
+        return C
+    elif Call_or_Put == 'put':
+        print('Selecionado Put')
+        P = strike * np.exp(-taxaLR*diasUteis) * norm.cdf(d2) - preco * norm.cdf(-d1)
+        return P
+    else:
+        print('As opções validas sao somente as de CALL e PUT')
+
+if __name__ == "__main__":
+    uvicorn.run(app, host="127.0.0.1", port=8000, default="/options/blackScholes")
+responseHistory = Response(media_type="application/json")
 
-    # Cria o modelo de regressão linear
-    modelo = LinearRegression()
 
-    # Treina o modelo com os dados históricos
-    modelo.fit(datas.values.reshape(-1, 1), precos)
 
-    # Faz a previsão da taxa de retorno para o próximo período
-    data_atual = pd.Timestamp.today().strftime('%Y-%m-%d')
-    data_futura = (pd.Timestamp.today() + pd.DateOffset(days=365)).strftime('%Y-%m-%d')
-    taxa_retorno = (modelo.predict(pd.to_numeric([data_futura.replace('-', '')]).reshape(-1, 1)) / 
-                    modelo.predict(pd.to_numeric([data_atual.replace('-', '')]).reshape(-1, 1)) - 1)
 
-    return taxa_retorno[0] * -1
+
+#################################################################
 
 
 # QUANTO MAIOR A TAXA DE RETORNO EM MENOS TEMPO VAI TER O RETORNO EM DIVIDENDO, A QUESTAO É PEGAR UMA TAXA DE RETORNO JUSTA OU UMA PADRAO
 
 def retornos_dividendos(ativos: Union[str, list], investimento: Union[int, float], taxa_desconto= 0.23):
     data = pd.DataFrame(columns=['Ativo', 'Retorno com Dividendos', 'Tempo para Atingir Retorno'])
```

### Comparing `BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.4.8/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.4.8/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 10 17:27:31 2023 UTC, .py size: 38822 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 0347 3464 a697 0000  a........G4d....
+00000000: 610d 0d0a 0000 0000 3ba7 3564 1198 0000  a.......;.5d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5405 0000 6400  .....@...sT...d.
+00000020: 0006 0000 0040 0000 0073 5e05 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6408 6c0e 6d0f 5a0f 0100 6400 6401 6c10  d.l.m.Z...d.d.l.
 00000090: 5a10 6400 6409 6c11 6d12 5a12 0100 6400  Z.d.d.l.m.Z...d.
@@ -75,1383 +75,1389 @@
 000004a0: 6537 641b 6b02 9004 728e 651e 6a38 6531  e7d.k...r.e.j8e1
 000004b0: 641d 641e 644c 6420 8d04 0100 6515 6421  d.d.dLd ....e.d!
 000004c0: 6422 8d01 5a3c 6531 6a33 6450 6401 6417  d"..Z<e1j3dPd.d.
 000004d0: 8d02 6534 6601 6522 6a3a 644d 9c01 6451  ..e4f.e"j:dM..dQ
 000004e0: 6452 8405 8301 5a4a 6537 641b 6b02 9004  dR....ZJe7d.k...
 000004f0: 72d6 651e 6a38 6531 641d 641e 6450 6420  r.e.j8e1d.d.dPd 
 00000500: 8d04 0100 6515 6421 6422 8d01 5a3c 6531  ....e.d!d"..Z<e1
-00000510: 6a33 6453 6401 6417 8d02 645e 6522 6a3a  j3dSd.d...d^e"j:
-00000520: 644d 9c01 6454 6455 8405 8301 5a4b 6537  dM..dTdU....ZKe7
-00000530: 641b 6b02 9005 721c 651e 6a38 6531 641d  d.k...r.e.j8e1d.
-00000540: 641e 6453 6420 8d04 0100 6515 6421 6422  d.dSd ....e.d!d"
-00000550: 8d01 5a3c 6456 6457 8400 5a4c 645f 6528  ..Z<dVdW..ZLd_e(
-00000560: 6534 6544 6602 1900 6528 6542 6541 6602  e4eDf...e(eBeAf.
-00000570: 1900 6459 9c02 645a 645b 8405 5a4d 6401  ..dY..dZd[..ZMd.
-00000580: 5300 2960 e900 0000 004e 2901 da04 6e6f  S.)`.....N)...no
-00000590: 726d 2901 da08 6d69 6e69 6d69 7a65 2901  rm)...minimize).
-000005a0: da10 4c69 6e65 6172 5265 6772 6573 7369  ..LinearRegressi
-000005b0: 6f6e 2901 da09 7765 6264 7269 7665 7229  on)...webdriver)
-000005c0: 01da 044b 6579 7329 01da 074f 7074 696f  ...Keys)...Optio
-000005d0: 6e73 2901 da02 4279 2901 da0d 4265 6175  ns)...By)...Beau
-000005e0: 7469 6675 6c53 6f75 7029 03da 0746 6173  tifulSoup)...Fas
-000005f0: 7441 5049 da08 5265 7370 6f6e 7365 da07  tAPI..Response..
-00000600: 5265 7175 6573 7429 01da 0c48 544d 4c52  Request)...HTMLR
-00000610: 6573 706f 6e73 6529 01da 0b53 7461 7469  esponse)...Stati
-00000620: 6346 696c 6573 2901 da0f 4a69 6e6a 6132  cFiles)...Jinja2
-00000630: 5465 6d70 6c61 7465 7329 02da 0864 6174  Templates)...dat
-00000640: 6574 696d 65da 0974 696d 6564 656c 7461  etime..timedelta
-00000650: 2901 da05 556e 696f 6eda 0669 676e 6f72  )...Union..ignor
-00000660: 65e9 6d01 0000 a901 da04 6461 7973 fa08  e.m.......days..
-00000670: 2559 2d25 6d2d 2564 6302 0000 0000 0000  %Y-%m-%dc.......
-00000680: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00000690: 0073 5e00 0000 7c00 7c01 1900 6a00 6401  .s^...|.|...j.d.
-000006a0: 6402 6403 6404 8d03 7c00 7c01 3c00 7c00  d.d.d...|.|.<.|.
-000006b0: 7c01 1900 6a00 6405 6402 6403 6404 8d03  |...j.d.d.d.d...
-000006c0: 7c00 7c01 3c00 7c00 7c01 1900 6a00 6406  |.|.<.|.|...j.d.
-000006d0: 6407 6403 6404 8d03 7c00 7c01 3c00 7c00  d.d.d...|.|.<.|.
-000006e0: 7c01 1900 a001 7402 a101 7c00 7c01 3c00  |.....t...|.|.<.
-000006f0: 7c00 5300 2908 4e7a 035b 2e5d da00 5429  |.S.).Nz.[.]..T)
-00000700: 01da 0572 6567 6578 7a03 5b25 5d7a 035b  ...regexz.[%]z.[
-00000710: 2c5d da01 2e29 03da 0772 6570 6c61 6365  ,]...)...replace
-00000720: da06 6173 7479 7065 da05 666c 6f61 7429  ..astype..float)
-00000730: 02da 0264 665a 0a6e 6f6d 6543 6f6c 756e  ...dfZ.nomeColun
-00000740: 61a9 0072 1f00 0000 fa40 713a 5c52 6973  a..r.....@q:\Ris
-00000750: 636f 5c4e 6f76 6f20 5269 7363 6f5c 7079  co\Novo Risco\py
-00000760: 7468 6f6e 7269 7363 6f5c 4242 4669 6e61  thonrisco\BBFina
-00000770: 6e63 655c 4242 4669 6e61 6e63 655c 4242  nce\BBFinance\BB
-00000780: 4669 6e61 6e63 652e 7079 da14 666f 726d  Finance.py..form
-00000790: 6174 6156 616c 6f72 6573 4e75 6d65 726f  ataValoresNumero
-000007a0: 3800 0000 730a 0000 0000 0118 0118 0118  8...s...........
-000007b0: 0112 0272 2100 0000 7a15 2f73 746f 636b  ...r!...z./stock
-000007c0: 732f 7b73 796d 626f 6c7d 2f69 6e66 6f29  s/{symbol}/info)
-000007d0: 015a 0e72 6573 706f 6e73 655f 6d6f 6465  .Z.response_mode
-000007e0: 6c29 02da 0673 796d 626f 6cda 0672 6574  l)...symbol..ret
-000007f0: 7572 6e63 0100 0000 0000 0000 0000 0000  urnc............
-00000800: 0800 0000 0500 0000 4300 0000 7368 0000  ........C...sh..
-00000810: 0074 00a0 017c 00a1 017d 017c 016a 027d  .t...|...}.|.j.}
-00000820: 0274 037c 0283 017d 037c 0374 046b 0272  .t.|...}.|.t.k.r
-00000830: 226e 0874 0564 0183 0101 007c 016a 0264  "n.t.d.....|.j.d
-00000840: 0219 007d 047c 016a 0264 0319 007d 057c  ...}.|.j.d...}.|
-00000850: 016a 067d 067c 066a 0764 0464 0585 0219  .j.}.|.j.d.d....
-00000860: 00a0 08a1 007d 067c 007c 047c 057c 0664  .....}.|.|.|.|.d
-00000870: 069c 047d 077c 0753 0029 0775 bf00 0000  ...}.|.S.).u....
-00000880: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
-00000890: 6164 6520 0a20 2020 202d 2042 7573 6361  ade .    - Busca
-000008a0: 2061 7320 7072 696e 6369 7061 6973 2069   as principais i
-000008b0: 6e66 6f72 6d61 c3a7 6f65 7320 736f 6272  nforma..oes sobr
-000008c0: 6520 6f20 6174 6976 6f20 7365 6c65 6369  e o ativo seleci
-000008d0: 6f6e 6164 6f20 636f 6d6f 2050 7265 c3a7  onado como Pre..
-000008e0: 6f20 6520 4469 7669 6465 6e64 6f73 200a  o e Dividendos .
-000008f0: 0a20 2020 200a 2020 2020 2323 2050 6172  .    .    ## Par
-00000900: c3a2 6d65 7472 6f73 0a20 2020 202d 2073  ..metros.    - s
-00000910: 796d 626f 6c20 2d3e 204e 6f6d 6520 646f  ymbol -> Nome do
-00000920: 2041 7469 766f 2070 6172 6120 6120 6275   Ativo para a bu
-00000930: 7363 6120 0a0a 2020 2020 0a20 2020 20fa  sca ..    .    .
-00000940: 0f54 6963 6b65 7220 496e 7661 6c69 646f  .Ticker Invalido
-00000950: da12 7265 6775 6c61 724d 6172 6b65 7450  ..regularMarketP
-00000960: 7269 6365 5a08 6c6f 6e67 4e61 6d65 e9ff  riceZ.longName..
-00000970: ffff ff4e 2904 7222 0000 00da 0d63 7572  ...N).r".....cur
-00000980: 7265 6e74 5f70 7269 6365 da0c 636f 6d70  rent_price..comp
-00000990: 616e 795f 6e61 6d65 da09 6469 7669 6465  any_name..divide
-000009a0: 6e64 7329 09da 0279 66da 0654 6963 6b65  nds)...yf..Ticke
-000009b0: 72da 0469 6e66 6fda 0474 7970 65da 0464  r..info..type..d
-000009c0: 6963 74da 0570 7269 6e74 7229 0000 00da  ict..printr)....
-000009d0: 0469 6c6f 63da 0373 756d 2908 7222 0000  .iloc..sum).r"..
-000009e0: 00da 0573 746f 636b 722c 0000 00da 0874  ...stockr,.....t
-000009f0: 6970 6f49 6e66 6f72 2700 0000 7228 0000  ipoInfor'...r(..
-00000a00: 005a 0864 6976 6964 656e 64da 096a 736f  .Z.dividend..jso
-00000a10: 6e5f 6461 7461 721f 0000 0072 1f00 0000  n_datar....r....
-00000a20: 7220 0000 00da 0867 6574 5f69 6e66 6f41  r .....get_infoA
-00000a30: 0000 0073 2000 0000 000c 0a01 0601 0801  ...s ...........
-00000a40: 0801 0202 0802 0a03 0a03 0601 1203 0201  ................
-00000a50: 0201 0201 02fd 0607 7235 0000 00da 085f  ........r5....._
-00000a60: 5f6d 6169 6e5f 5f7a 086d 6169 6e3a 6170  _main__z.main:ap
-00000a70: 707a 0931 3237 2e30 2e30 2e31 6940 1f00  pz.127.0.0.1i@..
-00000a80: 007a 1473 746f 636b 732f 7b73 796d 626f  .z.stocks/{symbo
-00000a90: 6c7d 2f69 6e66 6f29 03da 0468 6f73 74da  l}/info)...host.
-00000aa0: 0470 6f72 74da 0764 6566 6175 6c74 7a10  .port..defaultz.
-00000ab0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00000ac0: 2901 5a0a 6d65 6469 615f 7479 7065 7a18  ).Z.media_typez.
-00000ad0: 2f73 746f 636b 732f 7b73 796d 626f 6c7d  /stocks/{symbol}
-00000ae0: 2f68 6973 746f 7279 da02 3179 2903 7222  /history..1y).r"
-00000af0: 0000 00da 0670 6572 696f 6472 2300 0000  .....periodr#...
-00000b00: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
-00000b10: 0003 0000 0043 0000 0073 7000 0000 7400  .....C...sp...t.
-00000b20: a001 7c00 a101 7d02 7c02 6a02 7d03 7403  ..|...}.|.j.}.t.
-00000b30: 7c03 8301 7d04 7c04 7404 6b02 7222 6e08  |...}.|.t.k.r"n.
-00000b40: 7405 6401 8301 0100 7c02 6a06 7c01 6402  t.d.....|.j.|.d.
-00000b50: 8d01 7d05 7c05 6a07 7248 6403 7405 6404  ..}.|.j.rHd.t.d.
-00000b60: 8301 6901 5300 7c05 6a08 6405 6406 8d01  ..i.S.|.j.d.d...
-00000b70: 7d06 7409 6a0a a00b 7c06 a101 6a0c 6407  }.t.j...|...j.d.
-00000b80: 6408 8d01 7d07 7c07 5300 6409 5300 290a  d...}.|.S.d.S.).
-00000b90: 75ff 0000 000a 2020 2020 2323 2055 7361  u.....    ## Usa
-00000ba0: 6269 6c69 6461 6465 200a 2020 2020 2d20  bilidade .    - 
-00000bb0: 5573 6164 6120 7061 7261 2076 6572 6966  Usada para verif
-00000bc0: 6963 6172 206f 2068 6973 74c3 b372 6963  icar o hist..ric
-00000bd0: 6f20 6461 2061 c3a7 616f 2073 656c 6563  o da a..ao selec
-00000be0: 696f 6e61 6461 2065 2065 6d20 7175 616c  ionada e em qual
-00000bf0: 2070 6572 696f 646f 200a 0a20 2020 200a   periodo ..    .
-00000c00: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
-00000c10: 6f73 0a20 2020 200a 2020 2020 2d20 7379  os.    .    - sy
-00000c20: 6d62 6f6c 202d 3e20 4e6f 6d65 2064 6f20  mbol -> Nome do 
-00000c30: 4174 6976 6f20 7061 7261 2061 2062 7573  Ativo para a bus
-00000c40: 6361 200a 0a20 2020 202d 2070 6572 696f  ca ..    - perio
-00000c50: 6420 2d3e 2044 6174 6120 656d 2041 4e4f  d -> Data em ANO
-00000c60: 5320 7061 7261 2061 2062 7573 6361 2064  S para a busca d
-00000c70: 6173 2069 6e66 6f72 6d61 c3a7 6f65 7320  as informa..oes 
-00000c80: 646f 2041 7469 766f 200a 0a20 2020 200a  do Ativo ..    .
-00000c90: 2020 2020 7224 0000 00a9 0172 3b00 0000      r$.....r;...
-00000ca0: da05 6572 726f 727a 0d4e 6f20 6461 7461  ..errorz.No data
-00000cb0: 2066 6f75 6e64 da04 6c69 7374 2901 5a06   found..list).Z.
-00000cc0: 6f72 6965 6e74 4629 01da 0464 726f 704e  orientF)...dropN
-00000cd0: 290d 722a 0000 0072 2b00 0000 722c 0000  ).r*...r+...r,..
-00000ce0: 0072 2d00 0000 722e 0000 0072 2f00 0000  .r-...r....r/...
-00000cf0: da07 6869 7374 6f72 79da 0565 6d70 7479  ..history..empty
-00000d00: da07 746f 5f64 6963 74da 0270 64da 0944  ..to_dict..pd..D
-00000d10: 6174 6146 7261 6d65 da09 6672 6f6d 5f64  ataFrame..from_d
-00000d20: 6963 74da 0b72 6573 6574 5f69 6e64 6578  ict..reset_index
-00000d30: 2908 7222 0000 0072 3b00 0000 7232 0000  ).r"...r;...r2..
-00000d40: 0072 2c00 0000 7233 0000 0072 4000 0000  .r,...r3...r@...
-00000d50: 5a0c 6869 7374 6f72 795f 6469 6374 5a0a  Z.history_dictZ.
-00000d60: 6869 7374 6f72 795f 6466 721f 0000 0072  history_dfr....r
-00000d70: 1f00 0000 7220 0000 00da 1167 6574 5f73  ....r .....get_s
-00000d80: 746f 636b 5f68 6973 746f 7279 6f00 0000  tock_historyo...
-00000d90: 7318 0000 0000 0e0a 0106 0108 0108 0102  s...............
-00000da0: 0208 020c 0206 010c 020c 0114 0272 4700  .............rG.
-00000db0: 0000 7a17 7374 6f63 6b73 2f7b 7379 6d62  ..z.stocks/{symb
-00000dc0: 6f6c 7d2f 6869 7374 6f72 797a 152f 7374  ol}/historyz./st
-00000dd0: 6f63 6b2f 7b73 796d 626f 6c7d 2f74 7265  ock/{symbol}/tre
-00000de0: 6e64 6301 0000 0000 0000 0000 0000 0008  ndc.............
-00000df0: 0000 0003 0000 0043 0000 0073 6800 0000  .......C...sh...
-00000e00: 7400 a001 7c00 a101 7d01 7c01 6a02 7d02  t...|...}.|.j.}.
-00000e10: 7403 7c02 8301 7d03 7c03 7404 6b02 7222  t.|...}.|.t.k.r"
-00000e20: 6e08 7405 6401 8301 0100 7c01 6a06 6402  n.t.d.....|.j.d.
-00000e30: 6403 8d01 7d04 7c04 6404 1900 7d05 7c05  d...}.|.d...}.|.
-00000e40: 6a07 6405 1900 7c05 6a07 6406 1900 6b04  j.d...|.j.d...k.
-00000e50: 7256 6407 6e02 6408 7d06 7c00 7c06 6409  rVd.n.d.}.|.|.d.
-00000e60: 9c02 7d07 7c07 5300 290a 75b9 0000 000a  ..}.|.S.).u.....
-00000e70: 2020 2020 2323 2055 7361 6269 6c69 6461      ## Usabilida
-00000e80: 6465 200a 2020 2020 2d20 4964 656e 7469  de .    - Identi
-00000e90: 6669 6361 2061 2074 656e 6465 6e63 6961  fica a tendencia
-00000ea0: 2064 6520 7072 65c3 a76f 2064 6520 756d   de pre..o de um
-00000eb0: 6120 61c3 a761 6f2c 2073 6520 6972 6120  a a..ao, se ira 
-00000ec0: 7365 7220 6465 2041 4c54 4120 6f75 2042  ser de ALTA ou B
-00000ed0: 4149 5841 0a20 2020 200a 2020 2020 2323  AIXA.    .    ##
-00000ee0: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
-00000ef0: 200a 2020 2020 2d20 7379 6d62 6f6c 202d   .    - symbol -
-00000f00: 3e20 4e6f 6d65 2064 6f20 4174 6976 6f20  > Nome do Ativo 
-00000f10: 7061 7261 2061 2062 7573 6361 200a 0a20  para a busca .. 
-00000f20: 2020 200a 2020 2020 7224 0000 005a 0231     .    r$...Z.1
-00000f30: 6472 3c00 0000 da05 436c 6f73 6572 2600  dr<.....Closer&.
-00000f40: 0000 7201 0000 00da 0275 70da 0464 6f77  ..r......up..dow
-00000f50: 6e29 0272 2200 0000 da05 7472 656e 6429  n).r".....trend)
-00000f60: 0872 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000f70: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00000f80: 4000 0000 7230 0000 0029 0872 2200 0000  @...r0...).r"...
-00000f90: 7232 0000 0072 2c00 0000 7233 0000 0072  r2...r,...r3...r
-00000fa0: 4000 0000 da0c 636c 6f73 655f 7072 6963  @.....close_pric
-00000fb0: 6573 724b 0000 0072 3400 0000 721f 0000  esrK...r4...r...
-00000fc0: 0072 1f00 0000 7220 0000 00da 0f67 6574  .r....r .....get
-00000fd0: 5f73 746f 636b 5f74 7265 6e64 9d00 0000  _stock_trend....
-00000fe0: 731a 0000 0000 0d0a 0106 0108 0108 0102  s...............
-00000ff0: 0208 020c 0108 011c 0202 0102 ff06 0672  ...............r
-00001000: 4d00 0000 7a15 7374 6f63 6b73 2f7b 7379  M...z.stocks/{sy
-00001010: 6d62 6f6c 7d2f 7472 656e 647a 192f 7374  mbol}/trendz./st
-00001020: 6f63 6b2f 7b73 796d 626f 6c7d 2f74 6563  ock/{symbol}/tec
-00001030: 686e 6963 616c 6301 0000 0000 0000 0000  hnicalc.........
-00001040: 0000 0011 0000 0006 0000 0043 0000 0073  ...........C...s
-00001050: f800 0000 7400 a001 7c00 a101 7d01 7c01  ....t...|...}.|.
-00001060: 6a02 7d02 7403 7c02 8301 7d03 7c03 7404  j.}.t.|...}.|.t.
-00001070: 6b02 7222 6e08 7405 6401 8301 0100 7c01  k.r"n.t.d.....|.
-00001080: 6a06 6402 6403 8d01 7d04 7c04 6404 1900  j.d.d...}.|.d...
-00001090: 7d05 7c05 6a07 6405 6406 8d01 a008 a100  }.|.j.d.d.......
-000010a0: 6a09 6407 1900 7d06 7c05 6a07 6408 6406  j.d...}.|.j.d.d.
-000010b0: 8d01 a008 a100 6a09 6407 1900 7d07 7c05  ......j.d...}.|.
-000010c0: a00a a100 7d08 7c08 a00b 7c08 6409 6b04  ....}.|...|.d.k.
-000010d0: 6409 a102 7d09 7c08 a00b 7c08 6409 6b00  d...}.|...|.d.k.
-000010e0: 6409 a102 0b00 7d0a 7c09 6a07 640a 6406  d.....}.|.j.d.d.
-000010f0: 8d01 a008 a100 7d0b 7c0a 6a07 640a 6406  ......}.|.j.d.d.
-00001100: 8d01 a008 a100 7d0c 7c0b 7c0c 1b00 7d0d  ......}.|.|...}.
-00001110: 640b 640b 640c 7c0d 1700 1b00 6a09 6407  d.d.d.|.....j.d.
-00001120: 1900 1800 7d0e 7c0e 640d 6b05 72e0 640e  ....}.|.d.k.r.d.
-00001130: 7d0f 6e04 640f 7d0f 7c00 7c06 7c07 7c0e  }.n.d.}.|.|.|.|.
-00001140: 7c0f 6410 9c05 7d10 7c10 5300 2911 7524  |.d...}.|.S.).u$
-00001150: 0200 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00001160: 6c69 6461 6465 200a 2020 2020 2d20 63c3  lidade .    - c.
-00001170: a16c 6375 6c6f 2065 6e76 6f6c 7665 2061  .lculo envolve a
-00001180: 2063 6f6d 7061 7261 c3a7 c3a3 6f20 6461   compara....o da
-00001190: 206d c3a9 6469 6120 6465 2067 616e 686f   m..dia de ganho
-000011a0: 7320 656d 2075 6d20 7065 72c3 ad6f 646f  s em um per..odo
-000011b0: 2064 6520 7465 6d70 6f20 636f 6d20 6120   de tempo com a 
-000011c0: 6dc3 a964 6961 2064 6520 7065 7264 6173  m..dia de perdas
-000011d0: 2065 6d20 756d 2070 6572 c3ad 6f64 6f20   em um per..odo 
-000011e0: 6465 2074 656d 706f 2e20 0a0a 2020 2020  de tempo. ..    
-000011f0: 0a20 2020 2023 2320 436f 6d6f 2069 6e74  .    ## Como int
-00001200: 6572 7072 6574 6172 200a 2020 2020 2d20  erpretar .    - 
-00001210: 5175 616e 646f 206f 2052 5349 2065 7374  Quando o RSI est
-00001220: c3a1 2061 6369 6d61 2064 6520 3730 2c20  .. acima de 70, 
-00001230: 6f20 6174 6976 6f20 c3a9 2063 6f6e 7369  o ativo .. consi
-00001240: 6465 7261 646f 2073 6f62 7265 636f 6d70  derado sobrecomp
-00001250: 7261 646f 2c20 6f20 7175 6520 7369 676e  rado, o que sign
-00001260: 6966 6963 6120 7175 6520 706f 6465 2065  ifica que pode e
-00001270: 7374 6172 2070 7265 7374 6573 2061 2073  star prestes a s
-00001280: 6f66 7265 7220 756d 6120 636f 7272 65c3  ofrer uma corre.
-00001290: a7c3 a36f 2070 6172 6120 6261 6978 6f2e  ...o para baixo.
-000012a0: 200a 2020 2020 5175 616e 646f 206f 2052   .    Quando o R
-000012b0: 5349 2065 7374 c3a1 2061 6261 6978 6f20  SI est.. abaixo 
-000012c0: 6465 2033 302c 206f 2061 7469 766f 20c3  de 30, o ativo .
-000012d0: a920 636f 6e73 6964 6572 6164 6f20 736f  . considerado so
-000012e0: 6272 6576 656e 6469 646f 2c20 6f20 7175  brevendido, o qu
-000012f0: 6520 7369 676e 6966 6963 6120 7175 6520  e significa que 
-00001300: 706f 6465 2065 7374 6172 2070 7265 7374  pode estar prest
-00001310: 6573 2061 2073 7562 6972 206e 6f76 616d  es a subir novam
-00001320: 656e 7465 2e20 0a20 0a20 2020 200a 2020  ente. . .    .  
-00001330: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
-00001340: 0a20 2020 202d 2073 796d 626f 6c20 2d3e  .    - symbol ->
-00001350: 204e 6f6d 6520 646f 2041 7469 766f 2070   Nome do Ativo p
-00001360: 6172 6120 6120 6275 7363 6120 0a0a 2020  ara a busca ..  
-00001370: 2020 0a20 2020 2072 2400 0000 da03 6d61    .    r$.....ma
-00001380: 7872 3c00 0000 7248 0000 00e9 3200 0000  xr<...rH....2...
-00001390: 2901 da06 7769 6e64 6f77 7226 0000 00e9  )...windowr&....
-000013a0: c800 0000 7201 0000 00e9 0e00 0000 e964  ....r..........d
-000013b0: 0000 00e9 0100 0000 e946 0000 007a 1f41  .........F...z.A
-000013c0: 2063 6861 6e63 6520 646f 2070 7265 636f   chance do preco
-000013d0: 2064 6f20 6174 6976 6f20 4341 4952 7a20   do ativo CAIRz 
-000013e0: 4120 6368 616e 6365 2064 6f20 7072 6563  A chance do prec
-000013f0: 6f20 646f 2061 7469 766f 2053 5542 4952  o do ativo SUBIR
-00001400: 2905 7222 0000 00da 0673 6d61 5f35 30da  ).r".....sma_50.
-00001410: 0773 6d61 5f32 3030 da03 7273 695a 0874  .sma_200..rsiZ.t
-00001420: 656e 6465 6e63 7929 0c72 2a00 0000 722b  endency).r*...r+
-00001430: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00001440: 0000 722f 0000 0072 4000 0000 5a07 726f  ..r/...r@...Z.ro
-00001450: 6c6c 696e 67da 046d 6561 6e72 3000 0000  lling..meanr0...
-00001460: da04 6469 6666 da05 7768 6572 6529 1172  ..diff..where).r
-00001470: 2200 0000 7232 0000 0072 2c00 0000 7233  "...r2...r,...r3
-00001480: 0000 0072 4000 0000 724c 0000 0072 5600  ...r@...rL...rV.
-00001490: 0000 7257 0000 00da 0564 656c 7461 5a04  ..rW.....deltaZ.
-000014a0: 6761 696e 5a04 6c6f 7373 5a08 6176 675f  gainZ.lossZ.avg_
-000014b0: 6761 696e 5a08 6176 675f 6c6f 7373 da02  gainZ.avg_loss..
-000014c0: 7273 7258 0000 00da 0673 7461 7475 7372  rsrX.....statusr
-000014d0: 3400 0000 721f 0000 0072 1f00 0000 7220  4...r....r....r 
-000014e0: 0000 00da 1467 6574 5f73 746f 636b 5f74  .....get_stock_t
-000014f0: 6563 686e 6963 616c 73c5 0000 0073 3600  echnicals....s6.
-00001500: 0000 0010 0a01 0601 0801 0801 0202 0802  ................
-00001510: 0c01 0803 1601 1603 0801 1001 1201 1001  ................
-00001520: 1001 0801 1602 0801 0602 0403 0201 0201  ................
-00001530: 0201 0201 02fb 060a 725f 0000 007a 1973  ........r_...z.s
-00001540: 746f 636b 732f 7b73 796d 626f 6c7d 2f74  tocks/{symbol}/t
-00001550: 6563 686e 6963 616c 7a1a 7374 6f63 6b73  echnicalz.stocks
-00001560: 2f7b 7379 6d62 6f6c 7d2f 766f 6c61 7469  /{symbol}/volati
-00001570: 6c69 7479 2904 7222 0000 00da 0a73 7461  lity).r".....sta
-00001580: 7274 5f64 6174 65da 0865 6e64 5f64 6174  rt_date..end_dat
-00001590: 6572 2300 0000 6303 0000 0000 0000 0000  er#...c.........
-000015a0: 0000 0006 0000 0006 0000 0043 0000 0073  ...........C...s
-000015b0: 6800 0000 7a28 7400 6a01 7c00 7c01 7c02  h...z(t.j.|.|.|.
-000015c0: 6401 8d03 7d03 7c03 6a02 7226 6402 7403  d...}.|.j.r&d.t.
-000015d0: 6403 8301 6901 5700 5300 5700 6e0c 0100  d...i.W.S.W.n...
-000015e0: 0100 0100 5900 6e02 3000 7404 a005 7c03  ....Y.n.0.t...|.
-000015f0: 6404 1900 7c03 6404 1900 a006 6405 a101  d...|.d.....d...
-00001600: 1b00 a101 7d04 7404 a007 6406 7c04 a008  ....}.t...d.|...
-00001610: a100 1400 a101 7d05 7c05 5300 2907 756e  ......}.|.S.).un
-00001620: 0100 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00001630: 6c69 6461 6465 200a 2020 2020 2d20 4dc3  lidade .    - M.
-00001640: a974 6f64 6f20 7573 6164 6f20 7061 7261  .todo usado para
-00001650: 2076 6572 6966 6963 6172 2061 2076 6f6c   verificar a vol
-00001660: 6174 696c 6964 6164 6520 6465 2075 6d20  atilidade de um 
-00001670: 6174 6976 6f20 656d 2063 6f6d 7061 7261  ativo em compara
-00001680: 6361 6f20 616f 206d 6572 6361 646f 2065  cao ao mercado e
-00001690: 6d20 7175 6520 6573 7461 2020 0a0a 2020  m que esta  ..  
-000016a0: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
-000016b0: 6574 726f 730a 2020 2020 2d20 7379 6d62  etros.    - symb
-000016c0: 6f6c 202d 3e20 4e6f 6d65 2064 6f20 4174  ol -> Nome do At
-000016d0: 6976 6f20 7061 7261 2061 2062 7573 6361  ivo para a busca
-000016e0: 200a 0a20 2020 202d 2073 7461 7274 5f64   ..    - start_d
-000016f0: 6174 6520 2d3e 2044 6174 6120 6465 2049  ate -> Data de I
-00001700: 6e69 6369 6f20 6461 2062 7573 6361 2064  nicio da busca d
-00001710: 6173 2069 6e66 6f73 2028 7072 6563 6f2c  as infos (preco,
-00001720: 2076 6f6c 756d 652c 2065 7463 2920 646f   volume, etc) do
-00001730: 2061 7469 766f 200a 0a20 2020 202d 2065   ativo ..    - e
-00001740: 6e64 5f64 6174 6520 2d3e 2044 6174 6120  nd_date -> Data 
-00001750: 4669 6e61 6c20 7061 7261 2061 2062 7573  Final para a bus
-00001760: 6361 2064 6173 2069 6e66 6f73 2028 7072  ca das infos (pr
-00001770: 6563 6f2c 2076 6f6c 756d 652c 2065 7463  eco, volume, etc
-00001780: 2920 646f 2061 7469 766f 200a 0a20 2020  ) do ativo ..   
-00001790: 20a9 02da 0573 7461 7274 da03 656e 6472   ....start..endr
-000017a0: 3d00 0000 7a38 4e61 6f20 666f 6920 656e  =...z8Nao foi en
-000017b0: 636f 6e74 7261 646f 206f 2068 6973 746f  contrado o histo
-000017c0: 7269 636f 206e 6573 7365 2070 6572 696f  rico nesse perio
-000017d0: 646f 2c20 7665 7269 6669 6361 722e 7248  do, verificar.rH
-000017e0: 0000 0072 5400 0000 e9fc 0000 0029 0972  ...rT........).r
-000017f0: 2a00 0000 da08 646f 776e 6c6f 6164 7241  *.....downloadrA
-00001800: 0000 0072 2f00 0000 da02 6e70 da03 6c6f  ...r/.....np..lo
-00001810: 67da 0573 6869 6674 da04 7371 7274 da03  g..shift..sqrt..
-00001820: 7661 7229 0672 2200 0000 7260 0000 0072  var).r"...r`...r
-00001830: 6100 0000 5a0a 7374 6f63 6b5f 6461 7461  a...Z.stock_data
-00001840: 5a0b 6c6f 675f 7265 7475 726e 735a 0a76  Z.log_returnsZ.v
-00001850: 6f6c 6174 696c 6974 7972 1f00 0000 721f  olatilityr....r.
-00001860: 0000 0072 2000 0000 da0e 6765 745f 766f  ...r .....get_vo
-00001870: 6c61 7469 6c69 7479 0501 0000 7312 0000  latility....s...
-00001880: 0000 0d02 0110 0106 0112 0106 0106 021c  ................
-00001890: 0112 0272 6c00 0000 7a14 7374 6f63 6b73  ...rl...z.stocks
-000018a0: 2f7b 7379 6d62 6f6c 7d2f 6265 7461 6301  /{symbol}/betac.
-000018b0: 0000 0000 0000 0000 0000 000f 0000 0003  ................
-000018c0: 0000 0043 0000 0073 be00 0000 7400 a001  ...C...s....t...
-000018d0: 6401 a101 7d01 7400 a001 6402 a101 7d02  d...}.t...d...}.
-000018e0: 7c01 6a02 7d03 7c02 6a02 7d04 7403 7c03  |.j.}.|.j.}.t.|.
-000018f0: 8301 7d05 7c05 7404 6b02 7342 7c04 7404  ..}.|.t.k.sB|.t.
-00001900: 6b02 723a 6e08 7405 6403 8301 0100 7c01  k.r:n.t.d.....|.
-00001910: 6a06 6404 6405 8d01 7d06 7c02 6a06 6404  j.d.d...}.|.j.d.
-00001920: 6405 8d01 7d07 7c06 6406 1900 a007 a100  d...}.|.d.......
-00001930: 7d08 7c07 6406 1900 a007 a100 7d09 7c08  }.|.d.......}.|.
-00001940: a008 7c09 a101 7d0a 7c09 a009 a100 7d0b  ..|...}.|.....}.
-00001950: 7c0a 7c0b 1b00 7d0c 7c0c 6407 6b04 7298  |.|...}.|.d.k.r.
-00001960: 6408 7d0d 7c0c 6407 6b00 72a4 6409 7d0d  d.}.|.d.k.r.d.}.
-00001970: 7c0c 6407 6b02 72b0 640a 7d0d 7c0c 7c0d  |.d.k.r.d.}.|.|.
-00001980: 640b 9c02 7d0e 7c0e 5300 290c 7595 0100  d...}.|.S.).u...
-00001990: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-000019a0: 6461 6465 200a 2020 2020 2d20 4f20 6265  dade .    - O be
-000019b0: 7461 20c3 a920 756d 6120 6d65 6469 6461  ta .. uma medida
-000019c0: 2065 7374 6174 c3ad 7374 6963 6120 7175   estat..stica qu
-000019d0: 6520 696e 6469 6361 2061 2072 656c 61c3  e indica a rela.
-000019e0: a7c3 a36f 2065 6e74 7265 2061 2076 6f6c  ...o entre a vol
-000019f0: 6174 696c 6964 6164 6520 6465 2075 6d61  atilidade de uma
-00001a00: 2061 c3a7 c3a3 6f20 6520 6120 766f 6c61   a....o e a vola
-00001a10: 7469 6c69 6461 6465 2064 6f20 6d65 7263  tilidade do merc
-00001a20: 6164 6f20 636f 6d6f 2075 6d20 746f 646f  ado como um todo
-00001a30: 2e0a 2020 2020 4f20 7661 6c6f 7220 646f  ..    O valor do
-00001a40: 2062 6574 6120 c3a9 2075 7469 6c69 7a61   beta .. utiliza
-00001a50: 646f 2070 6172 6120 6d65 6469 7220 6f20  do para medir o 
-00001a60: 7269 7363 6f20 6465 2075 6d61 2061 c3a7  risco de uma a..
-00001a70: c3a3 6f20 656d 2072 656c 61c3 a7c3 a36f  ..o em rela....o
-00001a80: 2061 6f20 6d65 7263 6164 6f20 656d 2071   ao mercado em q
-00001a90: 7565 2065 6c61 20c3 a920 6e65 676f 6369  ue ela .. negoci
-00001aa0: 6164 612e 200a 0a20 2020 200a 2020 2020  ada. ..    .    
-00001ab0: 2323 2050 6172 c3a2 6d65 7472 6f73 0a20  ## Par..metros. 
-00001ac0: 2020 202d 2073 796d 626f 6c20 2d3e 204e     - symbol -> N
-00001ad0: 6f6d 6520 646f 2041 7469 766f 2070 6172  ome do Ativo par
-00001ae0: 6120 6120 6275 7363 6120 0a0a 2020 2020  a a busca ..    
-00001af0: 2d20 6d61 726b 6574 202d 3e20 436f 6d6f  - market -> Como
-00001b00: 2070 6164 7261 6f2c 204d 6572 6361 646f   padrao, Mercado
-00001b10: 3a20 4942 4f56 4553 5041 202f 2042 5653  : IBOVESPA / BVS
-00001b20: 500a 2020 2020 fa08 5045 5452 342e 5341  P.    ..PETR4.SA
-00001b30: 7a05 5e42 5653 5072 2400 0000 724e 0000  z.^BVSPr$...rN..
-00001b40: 0072 3c00 0000 7248 0000 0072 5400 0000  .r<...rH...rT...
-00001b50: 7a28 4163 616f 206d 6169 7320 566f 6c61  z(Acao mais Vola
-00001b60: 7469 6c20 7175 6520 6f20 6d65 7263 6164  til que o mercad
-00001b70: 6f20 656d 2067 6572 616c 7a29 4163 616f  o em geralz)Acao
-00001b80: 206d 656e 6f73 2056 6f6c 6174 696c 2071   menos Volatil q
-00001b90: 7565 206f 206d 6572 6361 646f 2065 6d20  ue o mercado em 
-00001ba0: 6765 7261 6c7a 3441 6361 6f20 636f 6d20  geralz4Acao com 
-00001bb0: 6120 6d65 736d 6120 566f 6c61 7469 6c69  a mesma Volatili
-00001bc0: 6461 6465 2071 7565 206f 206d 6572 6361  dade que o merca
-00001bd0: 646f 2065 6d20 6765 7261 6c29 02da 0462  do em geral)...b
-00001be0: 6574 6172 5e00 0000 290a 722a 0000 0072  etar^...).r*...r
-00001bf0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
-00001c00: 0000 0072 2f00 0000 7240 0000 00da 0a70  ...r/...r@.....p
-00001c10: 6374 5f63 6861 6e67 65da 0363 6f76 726b  ct_change..covrk
-00001c20: 0000 0029 0f72 2200 0000 5a05 6173 7365  ...).r"...Z.asse
-00001c30: 745a 066d 6172 6b65 7472 2c00 0000 5a0a  tZ.marketr,...Z.
-00001c40: 696e 666f 4d61 726b 6574 7233 0000 005a  infoMarketr3...Z
-00001c50: 0d61 7373 6574 5f68 6973 746f 7279 5a0e  .asset_historyZ.
-00001c60: 6d61 726b 6574 5f68 6973 746f 7279 5a0d  market_historyZ.
-00001c70: 6173 7365 745f 7265 7475 726e 735a 0e6d  asset_returnsZ.m
-00001c80: 6172 6b65 745f 7265 7475 726e 7372 7000  arket_returnsrp.
-00001c90: 0000 726b 0000 0072 6e00 0000 725e 0000  ..rk...rn...r^..
-00001ca0: 0072 3400 0000 721f 0000 0072 1f00 0000  .r4...r....r....
-00001cb0: 7220 0000 00da 0867 6574 5f62 6574 6125  r .....get_beta%
-00001cc0: 0100 0073 3200 0000 000e 0a01 0a01 0601  ...s2...........
-00001cd0: 0601 0801 1001 0202 0802 0c01 0c03 0c01  ................
-00001ce0: 0c03 0a01 0801 0802 0801 0401 0801 0401  ................
-00001cf0: 0801 0403 0201 02ff 0605 7271 0000 007a  ..........rq...z
-00001d00: 1373 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-00001d10: 2f56 6152 2904 7222 0000 00da 1063 6f6e  /VaR).r".....con
-00001d20: 6669 6465 6e63 655f 6c65 7665 6cda 0f6c  fidence_level..l
-00001d30: 6f6f 6b62 6163 6b5f 7065 7269 6f64 7223  ookback_periodr#
-00001d40: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00001d50: 0b00 0000 0600 0000 4300 0000 739e 0000  ........C...s...
-00001d60: 0074 00a0 017c 00a1 017d 037c 036a 027d  .t...|...}.|.j.}
-00001d70: 0474 037c 0483 017d 057c 0574 046b 0272  .t.|...}.|.t.k.r
-00001d80: 226e 0874 0564 0183 0101 007c 036a 067c  "n.t.d.....|.j.|
-00001d90: 029b 0064 029d 0264 038d 0164 0419 007d  ...d...d...d...}
-00001da0: 0674 07a0 087c 067c 06a0 0964 05a1 011b  .t...|.|...d....
-00001db0: 00a1 017d 077c 07a0 0aa1 007d 087c 0874  ...}.|.....}.|.t
-00001dc0: 0ba0 0c64 057c 0118 00a1 0114 007d 0974  ...d.|.......}.t
-00001dd0: 0564 0674 0d7c 097c 0664 0719 0014 0064  .d.t.|.|.d.....d
-00001de0: 0883 0269 0183 0101 0074 0d7c 097c 0664  ...i.....t.|.|.d
-00001df0: 0719 0014 0064 0883 027d 0a7c 0a53 0029  .....d...}.|.S.)
-00001e00: 0975 c801 0000 0a20 2020 2023 2320 5573  .u.....    ## Us
-00001e10: 6162 696c 6964 6164 6520 0a20 2020 202d  abilidade .    -
-00001e20: 204f 2056 616c 7565 2061 7420 5269 736b   O Value at Risk
-00001e30: 2028 5661 5229 20c3 a920 756d 6120 6d65   (VaR) .. uma me
-00001e40: 6469 6461 2064 6520 7269 7363 6f20 7175  dida de risco qu
-00001e50: 6520 696e 6469 6361 2061 2070 6572 6461  e indica a perda
-00001e60: 206d c3a1 7869 6d61 2065 7370 6572 6164   m..xima esperad
-00001e70: 612c 2063 6f6d 2075 6d20 6465 7465 726d  a, com um determ
-00001e80: 696e 6164 6f20 6ec3 ad76 656c 2064 6520  inado n..vel de 
-00001e90: 636f 6e66 6961 6ec3 a761 2c20 656d 2075  confian..a, em u
-00001ea0: 6d20 696e 7465 7276 616c 6f20 6465 2074  m intervalo de t
-00001eb0: 656d 706f 2070 72c3 a92d 6465 7465 726d  empo pr..-determ
-00001ec0: 696e 6164 6f2e 200a 0a20 2020 200a 2020  inado. ..    .  
-00001ed0: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
-00001ee0: 0a20 2020 200a 2020 2020 2d20 7379 6d62  .    .    - symb
-00001ef0: 6f6c 202d 3e20 4e6f 6d65 2064 6f20 4174  ol -> Nome do At
-00001f00: 6976 6f20 7061 7261 2066 617a 6572 2061  ivo para fazer a
-00001f10: 2062 7573 6361 200a 0a20 2020 202d 2063   busca ..    - c
-00001f20: 6f6e 6669 6465 6e63 655f 6c65 7665 6c20  onfidence_level 
-00001f30: 2d3e 204e 6976 656c 2064 6520 636f 6e66  -> Nivel de conf
-00001f40: 6961 6ec3 a761 2070 6172 6120 6f20 5641  ian..a para o VA
-00001f50: 5220 2830 2061 2031 292c 206e 6f72 6d61  R (0 a 1), norma
-00001f60: 6c6d 656e 7465 2075 7361 646f 2065 6d20  lmente usado em 
-00001f70: 302e 3935 200a 0a20 2020 202d 206c 6f6f  0.95 ..    - loo
-00001f80: 6b62 6163 6b5f 7065 7269 6f64 202d 3e20  kback_period -> 
-00001f90: 5065 7269 6f64 6f20 454d 2044 4941 5320  Periodo EM DIAS 
-00001fa0: 6120 7365 7220 636f 6e73 6964 6572 6164  a ser considerad
-00001fb0: 6f20 7061 7261 206f 2063 c3a1 6c63 756c  o para o c..lcul
-00001fc0: 6f20 646f 2056 6152 0a0a 2020 2020 7224  o do VaR..    r$
-00001fd0: 0000 00da 0164 723c 0000 0072 4800 0000  .....dr<...rH...
-00001fe0: 7254 0000 005a 0356 6152 7226 0000 00e9  rT...Z.VaRr&....
-00001ff0: 0200 0000 290e 722a 0000 0072 2b00 0000  ....).r*...r+...
-00002000: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
-00002010: 2f00 0000 7240 0000 0072 6700 0000 7268  /...r@...rg...rh
-00002020: 0000 0072 6900 0000 da03 7374 6472 0200  ...ri.....stdr..
-00002030: 0000 5a03 7070 66da 0572 6f75 6e64 290b  ..Z.ppf..round).
-00002040: 7222 0000 0072 7200 0000 7273 0000 0072  r"...rr...rs...r
-00002050: 3200 0000 722c 0000 0072 3300 0000 5a06  2...r,...r3...Z.
-00002060: 7072 6963 6573 da07 7265 7475 726e 735a  prices..returnsZ
-00002070: 0773 7464 5f64 6576 726b 0000 005a 0356  .std_devrk...Z.V
-00002080: 6172 721f 0000 0072 1f00 0000 7220 0000  arr....r....r ..
-00002090: 00da 0767 6574 5f76 6172 5f01 0000 731a  ...get_var_...s.
-000020a0: 0000 0000 0f0a 0106 0108 0108 0102 0208  ................
-000020b0: 0316 0314 0308 0112 011a 0112 0172 7900  .............ry.
-000020c0: 0000 7a1c 7374 6f63 6b73 2f7b 7379 6d62  ..z.stocks/{symb
-000020d0: 6f6c 7d2f 416e 6e75 616c 5265 7475 726e  ol}/AnnualReturn
-000020e0: 2904 da07 7379 6d62 6f6c 7372 6000 0000  )...symbolsr`...
-000020f0: 7261 0000 0072 2300 0000 6303 0000 0000  ra...r#...c.....
-00002100: 0000 0000 0000 0011 0000 0007 0000 0043  ...............C
-00002110: 0000 0073 9201 0000 7400 7c00 7401 8302  ...s....t.|.t...
-00002120: 72c8 7402 6401 7c00 9b00 9d02 8301 0100  r.t.d.|.........
-00002130: 7403 6a04 7c00 7c01 7c02 6402 6403 8d04  t.j.|.|.|.d.d...
-00002140: 7d03 7a86 7403 a005 7c00 a101 6a06 7d04  }.z.t...|...j.}.
-00002150: 7c04 6404 1900 7d05 7c03 6405 1900 7d06  |.d...}.|.d...}.
-00002160: 7c06 a007 a100 7d07 7c07 a008 a100 6406  |.....}.|.....d.
-00002170: 1400 7d08 7c07 a009 a100 6407 1400 7d09  ..}.|.....d...}.
-00002180: 7c06 6a0a 6408 1900 6409 1400 7d0a 7c06  |.j.d...d...}.|.
-00002190: 6a0a 640a 1900 6409 1400 7d0b 7c0b 7c0a  j.d...d...}.|.|.
-000021a0: 1800 7c0a 1b00 7d0c 740b 6a0c 7c00 7c05  ..|...}.t.j.|.|.
-000021b0: 7c08 7c09 7c0c 640b 9c05 640c 6701 640d  |.|.|.d...d.g.d.
-000021c0: 8d02 7d0d 7c0d 5700 5300 0100 0100 0100  ..}.|.W.S.......
-000021d0: 7402 640e 8301 0100 5900 6e02 3000 6ec6  t.d.....Y.n.0.n.
-000021e0: 7400 7c00 740d 8302 9001 7286 740b a00c  t.|.t.....r.t...
-000021f0: a100 7d0e 7402 640f 7c00 9b00 9d02 8301  ..}.t.d.|.......
-00002200: 0100 7c00 4400 5d92 7d0f 7403 6a04 7c0f  ..|.D.].}.t.j.|.
-00002210: 7c01 7c02 6402 6403 8d04 7d03 7c03 6405  |.|.d.d...}.|.d.
-00002220: 1900 7d06 7c06 a007 a100 7d07 7c07 a008  ..}.|.....}.|...
-00002230: a100 6406 1400 7d08 7c07 a009 a100 6407  ..d...}.|.....d.
-00002240: 1400 7d09 7c06 6a0a 6408 1900 6409 1400  ..}.|.j.d...d...
-00002250: 7d0a 7c06 6a0a 640a 1900 6409 1400 7d0b  }.|.j.d...d...}.
-00002260: 7c0b 7c0a 1800 7c0a 1b00 7d0c 740b 6a0c  |.|...|...}.t.j.
-00002270: 7c0f 7c08 7c09 7c0c 6410 9c04 740e 7c00  |.|.|.|.d...t.|.
-00002280: 8301 6701 640d 8d02 7d10 740b a00f 7c10  ..g.d...}.t...|.
-00002290: 7c0e 6702 a101 7d0e 71ee 7c0e 5300 7402  |.g...}.q.|.S.t.
-000022a0: 6411 8301 0100 6412 5300 2913 759b 0100  d.....d.S.).u...
-000022b0: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-000022c0: 6461 6465 0a20 2020 202d 2052 6563 6562  dade.    - Receb
-000022d0: 6520 756d 6120 6c69 7374 6120 6520 7265  e uma lista e re
-000022e0: 746f 726e 6120 756d 2044 6174 6146 7261  torna um DataFra
-000022f0: 6d65 2063 6f6d 2061 7320 696e 666f 726d  me com as inform
-00002300: 61c3 a7c3 b565 7320 646f 7320 6174 6976  a....es dos ativ
-00002310: 6f73 2065 2061 6c67 756d 6173 2065 7374  os e algumas est
-00002320: 6174 c3ad 7374 6963 6173 2062 c3a1 7369  at..sticas b..si
-00002330: 6361 732e 200a 0a20 2020 200a 2020 2020  cas. ..    .    
-00002340: 2323 2050 6172 c3a2 6d65 7472 6f73 0a20  ## Par..metros. 
-00002350: 2020 202d 2073 796d 626f 6c73 202d 3e20     - symbols -> 
-00002360: 5265 6365 6265 2075 6d61 206c 6973 7461  Recebe uma lista
-00002370: 206f 7520 756d 2075 6e69 636f 2061 7469   ou um unico ati
-00002380: 766f 2070 6172 6120 6275 7363 6172 206e  vo para buscar n
-00002390: 6120 6261 7365 200a 0a20 2020 202d 2073  a base ..    - s
-000023a0: 7461 7274 5f64 6174 6520 2d3e 2044 6174  tart_date -> Dat
-000023b0: 6120 6465 2049 6e69 6369 6f20 6461 2062  a de Inicio da b
-000023c0: 7573 6361 2064 6173 2069 6e66 6f73 2028  usca das infos (
-000023d0: 7072 6563 6f2c 2076 6f6c 756d 652c 2065  preco, volume, e
-000023e0: 7463 2920 646f 2061 7469 766f 200a 0a20  tc) do ativo .. 
-000023f0: 2020 202d 2065 6e64 5f64 6174 6520 2d3e     - end_date ->
-00002400: 2044 6174 6120 4669 6e61 6c20 7061 7261   Data Final para
-00002410: 2061 2062 7573 6361 2064 6173 2069 6e66   a busca das inf
-00002420: 6f73 2028 7072 6563 6f2c 2076 6f6c 756d  os (preco, volum
-00002430: 652c 2065 7463 2920 646f 2061 7469 766f  e, etc) do ativo
-00002440: 200a 0a20 2020 200a 2020 2020 751a 0000   ..    .    u...
-00002450: 0056 6f63 c3aa 2064 6967 6974 6f75 2075  .Voc.. digitou u
-00002460: 6d61 2073 7472 696e 673a 20da 0674 6963  ma string: ..tic
-00002470: 6b65 7229 045a 0774 6963 6b65 7273 7263  ker).Z.tickersrc
-00002480: 0000 0072 6400 0000 5a08 6772 6f75 705f  ...rd...Z.group_
-00002490: 6279 7225 0000 0072 4800 0000 7265 0000  byr%...rH...re..
-000024a0: 0067 5f75 bc7e bfbf 2f40 7201 0000 0072  .g_u.~../@r....r
-000024b0: 5300 0000 7226 0000 0029 05da 0541 7469  S...r&...)...Ati
-000024c0: 766f 7510 0000 0050 7265 c3a7 6f20 6120  vou....Pre..o a 
-000024d0: 4d65 7263 6164 6ffa 0d52 6574 6f72 6e6f  Mercado..Retorno
-000024e0: 2061 6e75 616c f514 0000 0044 6573 7669   anual.....Desvi
-000024f0: 6f20 7061 6472 c3a3 6f20 616e 7561 6cfa  o padr..o anual.
-00002500: 0d52 6574 6f72 6e6f 2074 6f74 616c 7254  .Retorno totalrT
-00002510: 0000 00a9 01da 0569 6e64 6578 7510 0000  .......indexu...
-00002520: 0054 6963 6b65 7220 696e 76c3 a16c 6964  .Ticker inv..lid
-00002530: 6f75 1900 0000 566f 63c3 aa20 6469 6769  ou....Voc.. digi
-00002540: 746f 7520 756d 6120 6c69 7374 613a 2029  tou uma lista: )
-00002550: 0472 7c00 0000 727d 0000 0072 7e00 0000  .r|...r}...r~...
-00002560: 727f 0000 0075 2f00 0000 5469 706f 2069  r....u/...Tipo i
-00002570: 6e76 c3a1 6c69 646f 2e20 4469 6769 7465  nv..lido. Digite
-00002580: 2075 6d61 2073 7472 696e 6720 6f75 2075   uma string ou u
-00002590: 6d61 206c 6973 7461 2e4e 2910 da0a 6973  ma lista.N)...is
-000025a0: 696e 7374 616e 6365 da03 7374 7272 2f00  instance..strr/.
-000025b0: 0000 722a 0000 0072 6600 0000 722b 0000  ..r*...rf...r+..
-000025c0: 0072 2c00 0000 726f 0000 0072 5900 0000  .r,...ro...rY...
-000025d0: 7276 0000 0072 3000 0000 7243 0000 0072  rv...r0...rC...r
-000025e0: 4400 0000 723e 0000 00da 036c 656e da06  D...r>.....len..
-000025f0: 636f 6e63 6174 2911 727a 0000 0072 6000  concat).rz...r`.
-00002600: 0000 7261 0000 00da 0564 6164 6f73 da04  ..ra.....dados..
-00002610: 6461 7461 5a0b 7661 6c75 654d 6172 6b65  dataZ.valueMarke
-00002620: 74da 0563 6c6f 7365 5a0e 7265 746f 726e  t..closeZ.retorn
-00002630: 6f5f 6469 6172 696f 5a0d 7265 746f 726e  o_diarioZ.retorn
-00002640: 6f5f 616e 7561 6c5a 1364 6573 7669 6f5f  o_anualZ.desvio_
-00002650: 7061 6472 616f 5f61 6e75 616c 5a0f 7661  padrao_anualZ.va
-00002660: 6c6f 725f 696e 7665 7374 6964 6f5a 0b76  lor_investidoZ.v
-00002670: 616c 6f72 5f61 7475 616c 5a0d 7265 746f  alor_atualZ.reto
-00002680: 726e 6f5f 746f 7461 6c5a 0c76 616c 7565  rno_totalZ.value
-00002690: 5379 6d62 6f6c 735a 0776 616c 7565 4446  SymbolsZ.valueDF
-000026a0: 5a07 7369 6d62 6f6c 6f5a 0d72 6574 7572  Z.simboloZ.retur
-000026b0: 6e53 796d 626f 6c73 721f 0000 0072 1f00  nSymbolsr....r..
-000026c0: 0000 7220 0000 00da 0f61 7373 6574 5f70  ..r .....asset_p
-000026d0: 6f72 7466 6f6c 696f 8a01 0000 7360 0000  ortfolio....s`..
-000026e0: 0000 0e0a 010e 0112 0202 020c 0108 0308  ................
-000026f0: 0308 030c 030c 030e 030e 030c 0304 0102  ................
-00002700: 0102 0102 0102 0102 fb04 0604 fa06 0806  ................
-00002710: 0206 0110 020c 0108 010e 0108 0112 0308  ................
-00002720: 0308 030c 030c 030e 030e 030c 0304 0102  ................
-00002730: 0102 0102 0102 fc04 0508 fb06 0710 0204  ................
-00002740: 0272 8900 0000 7a24 7374 6f63 6b73 2f7b  .r....z$stocks/{
-00002750: 7379 6d62 6f6c 7d2f 4d61 726b 6f77 6974  symbol}/Markowit
-00002760: 7a41 6c6c 6f63 6174 696f 6e6e 2904 727a  zAllocationn).rz
-00002770: 0000 00da 0973 7461 725f 6461 7465 7261  .....star_datera
-00002780: 0000 0072 2300 0000 6303 0000 0000 0000  ...r#...c.......
-00002790: 0000 0000 0011 0000 0009 0000 0043 0000  .............C..
-000027a0: 0073 3a01 0000 7400 6a01 7c00 7c01 7c02  .s:...t.j.|.|.|.
-000027b0: 6401 8d03 6402 1900 7d03 7c03 a002 a100  d...d...}.|.....
-000027c0: a003 a100 7d04 7c04 a004 a100 7d05 7405  ....}.|.....}.t.
-000027d0: a006 6403 7407 7c00 8301 1b00 6701 7407  ..d.t.|.....g.t.
-000027e0: 7c00 8301 1400 a101 7d06 7405 a008 7c04  |.......}.t...|.
-000027f0: a009 a100 7c06 1400 a101 6404 1400 7d07  ....|.....d...}.
-00002800: 7405 a00a 7405 a00b 7c06 6a0c 7405 a00b  t...t...|.j.t...
-00002810: 7c05 7c06 a102 a102 a101 7405 a00a 6404  |.|.......t...d.
-00002820: a101 1400 7d08 6405 7405 a00d 7c05 a101  ....}.d.t...|...
-00002830: 1400 7d09 7405 6a0e a00f 7c05 7c09 7405  ..}.t.j...|.|.t.
-00002840: a010 7c05 6a11 6406 1900 a101 1400 1700  ..|.j.d.........
-00002850: a101 7d0a 7405 a012 7407 7c00 8301 6403  ..}.t...t.|...d.
-00002860: 6602 a101 7d0b 7405 a00b 7c0a 7c0b a102  f...}.t...|.|...
-00002870: 7405 a00b 7405 a00b 7c0b 6a0c 7c0a a102  t...t...|.j.|...
-00002880: 7c0b a102 1b00 7d0c 7c0c a013 a100 7d0c  |.....}.|.....}.
-00002890: 6700 7d0d 7414 7407 7c00 8301 8301 4400  g.}.t.t.|.....D.
-000028a0: 5d2e 7d0e 6407 7c00 7c0e 1900 9b00 6408  ].}.d.|.|.....d.
-000028b0: 7c0c 7c0e 1900 6409 1400 640a 9b04 640b  |.|...d...d...d.
-000028c0: 9d05 7d0f 7c0d a015 7c0f a101 0100 71fa  ..}.|...|.....q.
-000028d0: 7c07 7c08 7c0d 640c 9c03 7d10 7c10 5300  |.|.|.d...}.|.S.
-000028e0: 290d 7522 0300 000a 2020 2020 2323 2055  ).u"....    ## U
-000028f0: 7361 6269 6c69 6461 6465 7320 0a20 2020  sabilidades .   
-00002900: 2041 6c6f 6361 c3a7 c3a3 6f20 6465 204d   Aloca....o de M
-00002910: 6172 6b6f 7769 747a 20c3 a920 756d 6120  arkowitz .. uma 
-00002920: 74c3 a963 6e69 6361 2064 6520 6f74 696d  t..cnica de otim
-00002930: 697a 61c3 a7c3 a36f 2064 6520 706f 7274  iza....o de port
-00002940: 66c3 b36c 696f 2071 7565 2076 6973 6120  f..lio que visa 
-00002950: 656e 636f 6e74 7261 7220 6120 636f 6d62  encontrar a comb
-00002960: 696e 61c3 a7c3 a36f 2069 6465 616c 2064  ina....o ideal d
-00002970: 6520 6174 6976 6f73 2070 6172 6120 6d61  e ativos para ma
-00002980: 7869 6d69 7a61 7220 6f20 7265 746f 726e  ximizar o retorn
-00002990: 6f20 646f 2069 6e76 6573 7469 6d65 6e74  o do investiment
-000029a0: 6f20 656e 7175 616e 746f 206d 696e 696d  o enquanto minim
-000029b0: 697a 6120 6f20 7269 7363 6f2e 200a 0a0a  iza o risco. ...
-000029c0: 2020 2020 2323 204f 2052 6574 6f72 6e6f      ## O Retorno
-000029d0: 2045 7370 6572 6164 6f0a 2020 2020 2d20   Esperado.    - 
-000029e0: 7265 7072 6573 656e 7461 2061 2074 6178  representa a tax
-000029f0: 6120 6465 2072 6574 6f72 6e6f 206d c3a9  a de retorno m..
-00002a00: 6469 6120 7175 6520 7365 2065 7370 6572  dia que se esper
-00002a10: 6120 6f62 7465 7220 646f 2070 6f72 7466  a obter do portf
-00002a20: c3b3 6c69 6f20 6465 2069 6e76 6573 7469  ..lio de investi
-00002a30: 6d65 6e74 6f73 200a 0a20 2020 2023 2320  mentos ..    ## 
-00002a40: 4f20 5269 7363 6f20 0a20 2020 202d 2072  O Risco .    - r
-00002a50: 6570 7265 7365 6e74 6120 6120 6d65 6469  epresenta a medi
-00002a60: 6461 2064 6520 766f 6c61 7469 6c69 6461  da de volatilida
-00002a70: 6465 2064 6f20 706f 7274 66c3 b36c 696f  de do portf..lio
-00002a80: 2c20 6f75 2073 656a 612c 200a 2020 2020  , ou seja, .    
-00002a90: 7175 616e 746f 206d 6169 7320 696e 7374  quanto mais inst
-00002aa0: c3a1 7665 6c20 666f 7220 6f20 7265 746f  ..vel for o reto
-00002ab0: 726e 6f20 646f 7320 6174 6976 6f73 2c20  rno dos ativos, 
-00002ac0: 6d61 696f 7220 7365 72c3 a120 6f20 7269  maior ser.. o ri
-00002ad0: 7363 6f20 646f 2070 6f72 7466 c3b3 6c69  sco do portf..li
-00002ae0: 6f20 636f 6d6f 2075 6d20 746f 646f 200a  o como um todo .
-00002af0: 0a20 2020 200a 2020 2020 0a20 2020 200a  .    .    .    .
-00002b00: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
-00002b10: 6f73 0a20 2020 200a 2020 2020 2d20 7379  os.    .    - sy
-00002b20: 6d62 6f6c 7320 2d3e 2052 6563 6562 6520  mbols -> Recebe 
-00002b30: 756d 6120 6c69 7374 6120 6465 2061 7469  uma lista de ati
-00002b40: 766f 7320 7061 7261 2062 7573 6361 7220  vos para buscar 
-00002b50: 6e61 2062 6173 6520 0a0a 2020 2020 2d20  na base ..    - 
-00002b60: 7374 6172 745f 6461 7465 202d 3e20 4461  start_date -> Da
-00002b70: 7461 2064 6520 496e 6963 696f 2064 6120  ta de Inicio da 
-00002b80: 6275 7363 6120 6461 7320 696e 666f 7320  busca das infos 
-00002b90: 2870 7265 636f 2c20 766f 6c75 6d65 2c20  (preco, volume, 
-00002ba0: 6574 6329 2064 6f20 6174 6976 6f20 0a0a  etc) do ativo ..
-00002bb0: 2020 2020 2d20 656e 645f 6461 7465 202d      - end_date -
-00002bc0: 3e20 4461 7461 2046 696e 616c 2070 6172  > Data Final par
-00002bd0: 6120 6120 6275 7363 6120 6461 7320 696e  a a busca das in
-00002be0: 666f 7320 2870 7265 636f 2c20 766f 6c75  fos (preco, volu
-00002bf0: 6d65 2c20 6574 6329 2064 6f20 6174 6976  me, etc) do ativ
-00002c00: 6f20 0a0a 0a20 2020 2072 6200 0000 7a09  o ...    rb...z.
-00002c10: 4164 6a20 436c 6f73 6572 5400 0000 7265  Adj CloserT...re
-00002c20: 0000 0067 9a99 9999 9999 b93f 7201 0000  ...g.......?r...
-00002c30: 007a 084f 2061 7469 766f 207a 1520 6465  .z.O ativo z. de
-00002c40: 7665 2073 6572 2061 6c6f 6361 646f 2065  ve ser alocado e
-00002c50: 6d20 7253 0000 007a 032e 3266 7a0d 2520  m rS...z..2fz.% 
-00002c60: 6461 2063 6172 7465 6972 6129 03fa 1052  da carteira)...R
-00002c70: 6574 6f72 6e6f 2045 7370 6572 6164 6ffa  etorno Esperado.
-00002c80: 1152 6973 636f 2064 6120 4361 7274 6569  .Risco da Cartei
-00002c90: 7261 fa12 416c 6f63 6163 616f 204d 6172  ra..Alocacao Mar
-00002ca0: 6b6f 7769 747a 2916 722a 0000 0072 6600  kowitz).r*...rf.
-00002cb0: 0000 726f 0000 00da 0664 726f 706e 6172  ..ro.....dropnar
-00002cc0: 7000 0000 7267 0000 00da 0561 7272 6179  p...rg.....array
-00002cd0: 7284 0000 0072 3100 0000 7259 0000 0072  r....r1...rY...r
-00002ce0: 6a00 0000 da03 646f 74da 0154 da05 7472  j.....dot..T..tr
-00002cf0: 6163 655a 066c 696e 616c 67da 0369 6e76  aceZ.linalg..inv
-00002d00: da03 6579 65da 0573 6861 7065 da04 6f6e  ..eye..shape..on
-00002d10: 6573 da07 666c 6174 7465 6eda 0572 616e  es..flatten..ran
-00002d20: 6765 da06 6170 7065 6e64 2911 727a 0000  ge..append).rz..
-00002d30: 0072 8a00 0000 7261 0000 0072 8600 0000  .r....ra...r....
-00002d40: 5a08 7265 746f 726e 6f73 5a12 6d61 7472  Z.retornosZ.matr
-00002d50: 697a 5f63 6f76 6172 6961 6e63 6961 5a05  iz_covarianciaZ.
-00002d60: 7065 736f 73da 1072 6574 6f72 6e6f 5f65  pesos..retorno_e
-00002d70: 7370 6572 6164 6fda 0572 6973 636f 5a07  sperado..riscoZ.
-00002d80: 6c61 6d62 6461 5f5a 0763 6f76 5f69 6e76  lambda_Z.cov_inv
-00002d90: 5a09 7665 746f 725f 756e 735a 0b77 5f6d  Z.vetor_unsZ.w_m
-00002da0: 6172 6b6f 7769 747a 5a0d 6d61 726b 6f77  arkowitzZ.markow
-00002db0: 6974 7a4c 6973 74da 0169 5a05 7461 7861  itzList..iZ.taxa
-00002dc0: 7372 3400 0000 721f 0000 0072 1f00 0000  sr4...r....r....
-00002dd0: 7220 0000 00da 146d 6172 6b6f 7769 747a  r .....markowitz
-00002de0: 5f61 6c6c 6f63 6174 696f 6ef4 0100 0073  _allocation....s
-00002df0: 2800 0000 0016 1403 0c03 0803 1c03 1603  (...............
-00002e00: 2603 0e01 2001 1201 2201 0803 0401 1001  &... ...".......
-00002e10: 2001 0c01 0201 0201 02fe 0606 729d 0000   ...........r...
-00002e20: 007a 2373 746f 636b 732f 7b73 796d 626f  .z#stocks/{symbo
-00002e30: 6c7d 2f4d 6172 6b6f 7769 747a 416c 6c6f  l}/MarkowitzAllo
-00002e40: 6361 7469 6f6e 7a0a 2f69 6e66 6f46 756e  cationz./infoFun
-00002e50: 6473 6301 0000 0000 0000 0000 0000 0007  dsc.............
-00002e60: 0000 0004 0000 0043 0000 0073 7200 0000  .......C...sr...
-00002e70: 6401 7d01 7400 a001 7c01 a101 7d02 7402  d.}.t...|...}.t.
-00002e80: 7c02 6a03 6402 8302 7d03 7c03 a004 6403  |.j.d...}.|...d.
-00002e90: a101 6404 1900 7d04 7405 a006 7407 7c04  ..d...}.t...t.|.
-00002ea0: 8301 a101 6404 1900 7d05 7c05 6405 1900  ....d...}.|.d...
-00002eb0: a008 6406 6407 8400 a101 7c05 6405 3c00  ..d.d.....|.d.<.
-00002ec0: 7c05 6a09 7c05 6405 1900 7c00 6b02 1900  |.j.|.d...|.k...
-00002ed0: 7d06 7c06 6700 6408 a201 1900 7d06 7c06  }.|.g.d.....}.|.
-00002ee0: 5300 2909 75c8 0000 000a 2020 2020 2323  S.).u.....    ##
-00002ef0: 2055 7361 6269 6c69 6461 6465 0a20 2020   Usabilidade.   
-00002f00: 2046 756e c3a7 616f 2075 7469 6c69 7a61   Fun..ao utiliza
-00002f10: 6461 2070 6172 6120 6164 7175 6972 6972  da para adquirir
-00002f20: 2061 7320 7072 696e 6369 7061 6973 2063   as principais c
-00002f30: 6172 6163 7465 7269 7374 6963 6173 2065  aracteristicas e
-00002f40: 2069 6e66 6f72 6d61 c3a7 c3b5 6573 2064   informa....es d
-00002f50: 6f20 6675 6e64 6f20 7365 6c65 6369 6f6e  o fundo selecion
-00002f60: 6164 6f0a 0a20 2020 2023 2320 5061 72c3  ado..    ## Par.
-00002f70: a26d 6574 726f 730a 0a20 2020 202d 2073  .metros..    - s
-00002f80: 796d 626f 6c20 2d3e 204e 6f6d 6520 646f  ymbol -> Nome do
-00002f90: 2046 756e 646f 2070 6172 6120 6661 7a65   Fundo para faze
-00002fa0: 7220 6120 6275 7363 6120 0a0a 0a20 2020  r a busca ...   
-00002fb0: 20fa 2868 7474 7073 3a2f 2f77 7777 2e66   .(https://www.f
-00002fc0: 756e 6473 6578 706c 6f72 6572 2e63 6f6d  undsexplorer.com
-00002fd0: 2e62 722f 7261 6e6b 696e 67fa 0b68 746d  .br/ranking..htm
-00002fe0: 6c2e 7061 7273 6572 da05 7461 626c 6572  l.parser..tabler
-00002ff0: 0100 0000 f510 0000 0043 c3b3 6469 676f  .........C..digo
-00003000: 2064 6f20 6675 6e64 6f63 0100 0000 0000   do fundoc......
-00003010: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00003020: 0000 7308 0000 007c 0064 0117 0053 00a9  ..s....|.d...S..
-00003030: 024e 7a03 2e53 4172 1f00 0000 a901 da01  .Nz..SAr........
-00003040: 7872 1f00 0000 721f 0000 0072 2000 0000  xr....r....r ...
-00003050: da08 3c6c 616d 6264 613e 4802 0000 f300  ..<lambda>H.....
-00003060: 0000 007a 1b67 6574 5f66 756e 6473 2e3c  ...z.get_funds.<
-00003070: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00003080: a906 72a1 0000 00da 0553 6574 6f72 f50c  ..r......Setor..
-00003090: 0000 0050 7265 c3a7 6f20 4174 7561 6cda  ...Pre..o Atual.
-000030a0: 0944 6976 6964 656e 646f f511 0000 0056  .Dividendo.....V
-000030b0: 6172 6961 c3a7 c3a3 6f20 5072 65c3 a76f  aria....o Pre..o
-000030c0: f510 0000 0052 656e 7461 622e 2050 6572  .....Rentab. Per
-000030d0: c3ad 6f64 6f29 0ada 0872 6571 7565 7374  ..odo)...request
-000030e0: 73da 0367 6574 7209 0000 00da 0763 6f6e  s..getr......con
-000030f0: 7465 6e74 da08 6669 6e64 5f61 6c6c 7243  tent..find_allrC
-00003100: 0000 00da 0972 6561 645f 6874 6d6c 7283  .....read_htmlr.
-00003110: 0000 00da 0561 7070 6c79 da03 6c6f 6329  .....apply..loc)
-00003120: 0772 2200 0000 da03 7572 6cda 0872 6573  .r".....url..res
-00003130: 706f 6e73 65da 0473 6f75 7072 a000 0000  ponse..soupr....
-00003140: da07 6675 6e64 7344 46da 0876 616c 7565  ..fundsDF..value
-00003150: 7346 4972 1f00 0000 721f 0000 0072 2000  sFIr....r....r .
-00003160: 0000 da09 6765 745f 6675 6e64 7336 0200  ....get_funds6..
-00003170: 0073 1200 0000 000d 0401 0a01 0c01 0e01  .s..............
-00003180: 1201 1602 1201 0c02 72b9 0000 007a 122f  ........r....z./
-00003190: 636f 6d70 6172 6553 6574 6f72 4675 6e64  compareSetorFund
-000031a0: 7329 02da 0573 6574 6f72 7223 0000 0063  s)...setorr#...c
-000031b0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
-000031c0: 0600 0000 4300 0000 731e 0100 0064 017d  ....C...s....d.}
-000031d0: 0274 00a0 017c 02a1 017d 0374 027c 036a  .t...|...}.t.|.j
-000031e0: 0364 0283 027d 047c 04a0 0464 03a1 0164  .d...}.|...d...d
-000031f0: 0419 007d 0574 05a0 0674 077c 0583 01a1  ...}.t...t.|....
-00003200: 0164 0419 007d 0674 087c 0664 0583 0201  .d...}.t.|.d....
-00003210: 007c 0164 061b 007d 017c 066a 097c 0664  .|.d...}.|.j.|.d
-00003220: 0519 0064 061b 007c 016b 0419 007d 077c  ...d...|.k...}.|
-00003230: 0767 0064 07a2 0119 007d 077c 07a0 0aa1  .g.d.....}.|....
-00003240: 007d 077c 0764 0519 00a0 0ba1 007d 087c  .}.|.d.......}.|
-00003250: 0064 086b 0272 aa64 097d 007c 076a 097c  .d.k.r.d.}.|.j.|
-00003260: 0764 0a19 007c 006b 0219 0064 0519 00a0  .d...|.k...d....
-00003270: 0ba1 007d 096e 427c 0064 0b6b 0272 d264  ...}.nB|.d.k.r.d
-00003280: 0c7d 007c 076a 097c 0764 0a19 007c 006b  .}.|.j.|.d...|.k
-00003290: 0219 0064 0519 00a0 0ba1 007d 096e 1a7c  ...d.......}.n.|
-000032a0: 076a 097c 0764 0a19 007c 006b 0219 0064  .j.|.d...|.k...d
-000032b0: 0519 00a0 0ba1 007d 097c 0764 0519 00a0  .......}.|.d....
-000032c0: 0ca1 007d 0a74 05a0 0d7c 0867 017c 0967  ...}.t...|.g.|.g
-000032d0: 017c 0a67 0164 0d9c 03a1 017d 0b7c 0ba0  .|.g.d.....}.|..
-000032e0: 0e64 0ea1 017d 0b7c 0b53 0029 0f75 0603  .d...}.|.S.).u..
-000032f0: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
-00003300: 6964 6164 650a 2020 2020 0a20 2020 202d  idade.    .    -
-00003310: 2046 756e c3a7 616f 2071 7565 2075 7469   Fun..ao que uti
-00003320: 6c69 7a61 2061 7320 6d65 7472 6963 6173  liza as metricas
-00003330: 2065 206d 6564 6961 7320 646f 7320 6675   e medias dos fu
-00003340: 6e64 6f20 636f 6d20 6261 7365 206e 6f20  ndo com base no 
-00003350: 7365 7520 5365 746f 7220 7061 7261 2075  seu Setor para u
-00003360: 6d61 2061 6e61 6c69 7365 206d 6169 7320  ma analise mais 
-00003370: 7265 7374 7269 7461 0a20 2020 200a 2020  restrita.    .  
-00003380: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
-00003390: 0a20 2020 200a 2020 2020 2d20 7265 6e74  .    .    - rent
-000033a0: 6162 696c 6964 6164 655f 6d69 6e20 2d3e  abilidade_min ->
-000033b0: 2056 616c 6f72 2065 6d20 2520 7061 7261   Valor em % para
-000033c0: 2062 7573 6361 7220 6120 7265 6e74 6162   buscar a rentab
-000033d0: 696c 6964 6164 6520 6d69 6e69 6d61 2064  ilidade minima d
-000033e0: 6f20 6675 6e64 6f20 6573 636f 6c68 6964  o fundo escolhid
-000033f0: 6f0a 2020 2020 2d20 7365 746f 7220 2d3e  o.    - setor ->
-00003400: 2053 6574 6f72 6573 2064 6520 6675 6e64   Setores de fund
-00003410: 6f73 2071 7565 2070 6f64 6572 616d 2073  os que poderam s
-00003420: 6572 2065 7363 6f6c 6869 646f 732c 2073  er escolhidos, s
-00003430: 6567 7565 2061 206c 6973 7461 3a0a 2020  egue a lista:.  
-00003440: 2020 0a20 2020 2060 6060 0a20 2020 2054    .    ```.    T
-00003450: 6970 6f73 5365 746f 7265 733a 0a20 2020  iposSetores:.   
-00003460: 202d 2043 6f72 706f 7261 7469 7661 7320   - Corporativas 
-00003470: 3d20 224c 616a 6573 2043 6f72 706f 7261  = "Lajes Corpora
-00003480: 7469 7661 7322 200a 2020 2020 2d20 4d6f  tivas" .    - Mo
-00003490: 6269 6c69 6172 696f 7320 3d20 2254 c3ad  biliarios = "T..
-000034a0: 7475 6c6f 7320 6520 5661 6c2e 204d 6f62  tulos e Val. Mob
-000034b0: 2e22 0a20 2020 202d 2053 686f 7070 696e  .".    - Shoppin
-000034c0: 6773 203d 2022 5368 6f70 7069 6e67 7322  gs = "Shoppings"
-000034d0: 0a20 2020 202d 2048 c3ad 6272 6964 6f20  .    - H..brido 
-000034e0: 3d20 2748 c3ad 6272 6964 6f27 0a20 2020  = 'H..brido'.   
-000034f0: 202d 2052 656e 6461 203d 2027 5265 6e64   - Renda = 'Rend
-00003500: 6127 0a20 2020 202d 204c 6f67 c3ad 7374  a'.    - Log..st
-00003510: 6963 6120 3d20 274c 6f67 c3ad 7374 6963  ica = 'Log..stic
-00003520: 6127 0a20 2020 202d 2048 6f73 7069 7461  a'.    - Hospita
-00003530: 6c20 3d20 2748 6f73 7069 7461 6c27 0a20  l = 'Hospital'. 
-00003540: 2020 202d 2052 6573 6964 656e 6369 616c     - Residencial
-00003550: 203d 2027 5265 7369 6465 6e63 6961 6c27   = 'Residencial'
-00003560: 0a20 2020 202d 204f 7574 726f 7320 3d20  .    - Outros = 
-00003570: 274f 7574 726f 7327 0a0a 2020 2020 6060  'Outros'..    ``
-00003580: 600a 2020 2020 2323 2045 7865 6d70 6c6f  `.    ## Exemplo
-00003590: 3a0a 2020 2020 0a20 2020 2060 6060 0a20  :.    .    ```. 
-000035a0: 2020 203e 3e3e 2062 622e 636f 6d70 6172     >>> bb.compar
-000035b0: 655f 7365 746f 725f 6675 6e64 7328 7365  e_setor_funds(se
-000035c0: 746f 723d 2743 6f72 706f 7261 7469 7661  tor='Corporativa
-000035d0: 7327 2c20 7265 6e74 6162 696c 6964 6164  s', rentabilidad
-000035e0: 655f 6d69 6e20 3d20 3329 0a20 2020 2060  e_min = 3).    `
-000035f0: 6060 0a0a 2020 2020 729e 0000 0072 9f00  ``..    r....r..
-00003600: 0000 72a0 0000 0072 0100 0000 72ac 0000  ..r....r....r...
-00003610: 0072 5300 0000 72a7 0000 005a 0c43 6f72  .rS...r....Z.Cor
-00003620: 706f 7261 7469 7661 737a 124c 616a 6573  porativasz.Lajes
-00003630: 2043 6f72 706f 7261 7469 7661 7372 a800   Corporativasr..
-00003640: 0000 5a0b 4d6f 6269 6c69 6172 696f 7375  ..Z.Mobiliariosu
-00003650: 1400 0000 54c3 ad74 756c 6f73 2065 2056  ....T..tulos e V
-00003660: 616c 2e20 4d6f 622e 2903 752a 0000 0052  al. Mob.).u*...R
-00003670: 656e 7461 6269 6c69 6461 6465 204d c3a9  entabilidade M..
-00003680: 6469 6120 646f 7320 4649 4973 2053 656c  dia dos FIIs Sel
-00003690: 6563 696f 6e61 646f 7375 1f00 0000 5265  ecionadosu....Re
-000036a0: 6e74 6162 696c 6964 6164 6520 4dc3 a964  ntabilidade M..d
-000036b0: 6961 2064 6f20 4d65 7263 6164 6f75 3700  ia do Mercadou7.
-000036c0: 0000 4465 7376 696f 2050 6164 72c3 a36f  ..Desvio Padr..o
-000036d0: 2064 6173 2052 656e 7461 6269 6c69 6461   das Rentabilida
-000036e0: 6465 7320 646f 7320 4649 4973 2053 656c  des dos FIIs Sel
-000036f0: 6563 696f 6e61 646f 737a 204f 2073 6574  ecionadosz O set
-00003700: 6f72 2f76 616c 6f72 206e 616f 2066 6f69  or/valor nao foi
-00003710: 2065 6e63 6f6e 7472 6164 6f29 0f72 ad00   encontrado).r..
-00003720: 0000 72ae 0000 0072 0900 0000 72af 0000  ..r....r....r...
-00003730: 0072 b000 0000 7243 0000 0072 b100 0000  .r....rC...r....
-00003740: 7283 0000 0072 2100 0000 72b3 0000 0072  r....r!...r....r
-00003750: 8e00 0000 7259 0000 0072 7600 0000 7244  ....rY...rv...rD
-00003760: 0000 005a 0666 696c 6c6e 6129 0c72 ba00  ...Z.fillna).r..
-00003770: 0000 5a11 7265 6e74 6162 696c 6964 6164  ..Z.rentabilidad
-00003780: 655f 6d69 6e72 b400 0000 72b5 0000 0072  e_minr....r....r
-00003790: b600 0000 72a0 0000 0072 b700 0000 72b8  ....r....r....r.
-000037a0: 0000 005a 1372 656e 7461 6269 6c69 6461  ...Z.rentabilida
-000037b0: 6465 5f6d 6564 6961 5a15 7265 6e74 6162  de_mediaZ.rentab
-000037c0: 696c 6964 6164 655f 6d65 7263 6164 6fda  ilidade_mercado.
-000037d0: 0d64 6573 7669 6f5f 7061 6472 616f 5a0a  .desvio_padraoZ.
-000037e0: 7265 7375 6c74 6164 6f73 721f 0000 0072  resultadosr....r
-000037f0: 1f00 0000 7220 0000 00da 1363 6f6d 7061  ....r .....compa
-00003800: 7265 5f73 6574 6f72 5f66 756e 6473 5602  re_setor_fundsV.
-00003810: 0000 7334 0000 0000 2204 010a 010c 010e  ..s4....".......
-00003820: 0112 020a 0108 0116 010c 0108 010c 0108  ................
-00003830: 0104 011c 0108 0104 011c 021a 020c 0204  ................
-00003840: 0104 0104 0104 fd08 060a 0272 bc00 0000  ...........r....
-00003850: 7a0d 2f63 6f6d 7061 7265 4675 6e64 7329  z./compareFunds)
-00003860: 0172 2300 0000 6303 0000 0000 0000 0000  .r#...c.........
-00003870: 0000 0012 0000 0004 0000 0043 0000 0073  ...........C...s
-00003880: 4a01 0000 7c01 72bc 7c02 6401 6b03 72bc  J...|.r.|.d.k.r.
-00003890: 6402 7d03 7400 a001 7c03 a101 7d04 7402  d.}.t...|...}.t.
-000038a0: 7c04 6a03 6403 8302 7d05 7c05 a004 6404  |.j.d...}.|...d.
-000038b0: a101 6405 1900 7d06 7405 a006 7407 7c06  ..d...}.t...t.|.
-000038c0: 8301 a101 6405 1900 7d07 7c07 6406 1900  ....d...}.|.d...
-000038d0: a008 6407 6408 8400 a101 7c07 6406 3c00  ..d.d.....|.d.<.
-000038e0: 7c07 6700 6409 a201 1900 7d07 7c07 6a09  |.g.d.....}.|.j.
-000038f0: 6406 6701 640a 8d01 7d07 7c07 6a0a 7c07  d.g.d...}.|.j.|.
-00003900: 6406 1900 7c01 6b02 1900 7d08 7c07 6a0a  d...|.k...}.|.j.
-00003910: 7c07 6406 1900 7c02 6b02 1900 7d09 7405  |.d...|.k...}.t.
-00003920: a00b 7c08 7c09 6702 a101 7d0a 7c0a 6a0c  ..|.|.g...}.|.j.
-00003930: 72b8 740d 640b 8301 0100 6e04 7c0a 5300  r.t.d.....n.|.S.
-00003940: 7c00 6401 7500 72ca 6700 7d00 6e7c 640c  |.d.u.r.g.}.n|d.
-00003950: 7d0b 640d 7d0c 7c00 4400 5d3a 7d0d 740e  }.d.}.|.D.]:}.t.
-00003960: a00f 7c0d a101 7d0e 7c0e 6a10 640e 640f  ..|...}.|.j.d.d.
-00003970: 8d01 7d0f 7c0f 6410 1900 a011 a100 a012  ..}.|.d.........
-00003980: a100 7d10 7c10 7c0b 6b04 72d6 7c10 7d0b  ..}.|.|.k.r.|.}.
-00003990: 7c0d 7d0c 71d6 7405 6a13 7c0c 7c0b 6411  |.}.q.t.j.|.|.d.
-000039a0: 1400 6412 9c02 7414 7c00 8301 6701 6413  ..d...t.|...g.d.
-000039b0: 8d02 7d11 7c11 6a0c 9001 7242 740d 6414  ..}.|.j...rBt.d.
-000039c0: 8301 0100 6e04 7c11 5300 6401 5300 2915  ....n.|.S.d.S.).
-000039d0: 7524 0300 000a 2020 2020 2323 2055 7361  u$....    ## Usa
-000039e0: 6269 6c69 6461 6465 0a20 2020 200a 2020  bilidade.    .  
-000039f0: 2020 2d20 4675 6ec3 a761 6f20 7175 6520    - Fun..ao que 
-00003a00: 7265 616c 697a 6120 6120 636f 6d70 6172  realiza a compar
-00003a10: 61c3 a761 6f20 656e 7472 6520 646f 6973  a..ao entre dois
-00003a20: 2066 756e 646f 732c 2073 656a 6120 6665   fundos, seja fe
-00003a30: 6974 6120 6120 7265 7175 6973 69c3 a761  ita a requisi..a
-00003a40: 6f20 646f 7320 6675 6e64 6f73 2076 6961  o dos fundos via
-00003a50: 206c 6973 7461 206f 7520 756e 6963 6f73   lista ou unicos
-00003a60: 200a 2020 2020 2d20 5265 7175 6973 69c3   .    - Requisi.
-00003a70: a761 6f20 4c69 7374 6173 3a20 5265 746f  .ao Listas: Reto
-00003a80: 726e 6120 6f20 6675 6e64 6f20 636f 6d20  rna o fundo com 
-00003a90: 6d61 696f 7220 706f 7263 656e 7461 6765  maior porcentage
-00003aa0: 6d20 6465 2072 6973 636f 2028 6120 7661  m de risco (a va
-00003ab0: 7269 61c3 a7c3 a36f 2070 6572 6365 6e74  ria....o percent
-00003ac0: 7561 6c20 646f 7320 7072 65c3 a76f 7320  ual dos pre..os 
-00003ad0: 646f 7320 6174 6976 6f73 2c20 6361 6c63  dos ativos, calc
-00003ae0: 756c 6f20 7265 616c 697a 6164 6f20 636f  ulo realizado co
-00003af0: 6d20 6261 7365 206e 6f20 6465 7376 696f  m base no desvio
-00003b00: 2070 6164 72c3 a36f 290a 2020 2020 2d20   padr..o).    - 
-00003b10: 5265 7175 6973 69c3 a761 6f20 556e 6963  Requisi..ao Unic
-00003b20: 613a 2052 6574 6f72 6e61 2075 6d20 4461  a: Retorna um Da
-00003b30: 7461 6672 616d 6520 636f 6d20 6173 2070  taframe com as p
-00003b40: 7269 6e63 6970 6169 7320 696e 666f 726d  rincipais inform
-00003b50: 61c3 a76f 6573 2064 6f73 2066 756e 646f  a..oes dos fundo
-00003b60: 732c 2061 6669 6d20 6465 2075 6d61 2063  s, afim de uma c
-00003b70: 6f6d 7061 7261 c3a7 616f 2065 6e74 7265  ompara..ao entre
-00003b80: 2073 6575 7320 7661 6c6f 7265 7320 0a0a   seus valores ..
-00003b90: 2020 2020 0a20 2020 2023 2320 5061 72c3      .    ## Par.
-00003ba0: a26d 6574 726f 730a 2020 2020 0a20 2020  .metros.    .   
-00003bb0: 202d 206c 6973 7466 756e 6420 2d3e 204c   - listfund -> L
-00003bc0: 6973 7461 2064 6f73 2066 756e 646f 7320  ista dos fundos 
-00003bd0: 7061 7261 2061 6e61 6c69 7365 2064 6520  para analise de 
-00003be0: 7269 7363 6f0a 2020 2020 2d20 6675 6e64  risco.    - fund
-00003bf0: 5f31 202d 3e20 5072 696d 6569 726f 2066  _1 -> Primeiro f
-00003c00: 756e 646f 2070 6172 6120 616e 616c 6973  undo para analis
-00003c10: 6520 756e 6963 610a 2020 2020 2d20 6675  e unica.    - fu
-00003c20: 6e64 5f32 202d 3e20 5365 6775 6e64 6f20  nd_2 -> Segundo 
-00003c30: 6675 6e64 6f20 7061 7261 2061 6e61 6c69  fundo para anali
-00003c40: 7365 2075 6e69 6361 0a20 2020 200a 2020  se unica.    .  
-00003c50: 2020 2323 2045 7865 6d70 6c6f 733a 0a20    ## Exemplos:. 
-00003c60: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
-00003c70: 3e3e 3e20 6262 2e63 6f6d 7061 7265 5f66  >>> bb.compare_f
-00003c80: 756e 6473 286c 6973 7466 756e 643d 206c  unds(listfund= l
-00003c90: 6973 7429 200a 2020 2020 2020 2020 2020  ist) .          
-00003ca0: 2020 2020 2020 2020 2020 6f75 0a20 2020            ou.   
-00003cb0: 203e 3e3e 2062 622e 636f 6d70 6172 655f   >>> bb.compare_
-00003cc0: 6675 6e64 7328 6675 6e64 5f31 3d20 2766  funds(fund_1= 'f
-00003cd0: 756e 6431 272c 2066 756e 645f 323d 2027  und1', fund_2= '
-00003ce0: 6675 6e64 3227 290a 2020 2020 6060 600a  fund2').    ```.
-00003cf0: 2020 2020 0a20 2020 204e 729e 0000 0072      .    Nr....r
-00003d00: 9f00 0000 72a0 0000 0072 0100 0000 72a1  ....r....r....r.
-00003d10: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00003d20: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
-00003d30: 007c 0064 0117 0053 0072 a200 0000 721f  .|.d...S.r....r.
-00003d40: 0000 0072 a300 0000 721f 0000 0072 1f00  ...r....r....r..
-00003d50: 0000 7220 0000 0072 a500 0000 bf02 0000  ..r ...r........
-00003d60: 72a6 0000 007a 1f63 6f6d 7061 7265 5f66  r....z.compare_f
-00003d70: 756e 6473 2e3c 6c6f 6361 6c73 3e2e 3c6c  unds.<locals>.<l
-00003d80: 616d 6264 613e 2908 72a1 0000 0072 a800  ambda>).r....r..
-00003d90: 0000 72a9 0000 0072 aa00 0000 72ab 0000  ..r....r....r...
-00003da0: 0072 ac00 0000 7a0e 4469 7669 6465 6e64  .r....z.Dividend
-00003db0: 2059 6965 6c64 7a11 4459 2028 334d 2920   Yieldz.DY (3M) 
-00003dc0: 4163 756d 756c 6164 6f29 015a 0673 7562  Acumulado).Z.sub
-00003dd0: 7365 7475 3e00 0000 4e61 6f20 666f 7261  setu>...Nao fora
-00003de0: 6d20 6170 7265 7365 6e74 6164 6f20 6461  m apresentado da
-00003df0: 646f 7320 646f 7320 6675 6e64 6f73 2070  dos dos fundos p
-00003e00: 6172 6120 7665 7269 6669 6361 c3a7 616f  ara verifica..ao
-00003e10: 2075 6e69 6361 7226 0000 0072 1800 0000   unicar&...r....
-00003e20: 724e 0000 0072 3c00 0000 7248 0000 0072  rN...r<...rH...r
-00003e30: 5300 0000 2902 5a04 4675 6e64 7a0c 4d61  S...).Z.Fundz.Ma
-00003e40: 7820 7269 736b 2028 2529 7280 0000 0075  x risk (%)r....u
-00003e50: 4200 0000 4e61 6f20 666f 7261 6d20 6170  B...Nao foram ap
-00003e60: 7265 7365 6e74 6164 6f20 6461 646f 7320  resentado dados 
-00003e70: 646f 7320 6675 6e64 6f73 2070 6172 6120  dos fundos para 
-00003e80: 7665 7269 6669 6361 c3a7 616f 206d c3ba  verifica..ao m..
-00003e90: 6c74 6970 6c61 2915 72ad 0000 0072 ae00  ltipla).r....r..
-00003ea0: 0000 7209 0000 0072 af00 0000 72b0 0000  ..r....r....r...
-00003eb0: 0072 4300 0000 72b1 0000 0072 8300 0000  .rC...r....r....
-00003ec0: 72b2 0000 00da 0f64 726f 705f 6475 706c  r......drop_dupl
-00003ed0: 6963 6174 6573 72b3 0000 0072 8500 0000  icatesr....r....
-00003ee0: 7241 0000 0072 2f00 0000 722a 0000 0072  rA...r/...r*...r
-00003ef0: 2b00 0000 7240 0000 0072 6f00 0000 7276  +...r@...ro...rv
-00003f00: 0000 0072 4400 0000 7284 0000 0029 125a  ...rD...r....).Z
-00003f10: 086c 6973 7466 756e 645a 0666 756e 645f  .listfundZ.fund_
-00003f20: 315a 0666 756e 645f 3272 b400 0000 72b5  1Z.fund_2r....r.
-00003f30: 0000 0072 b600 0000 72a0 0000 0072 b700  ...r....r....r..
-00003f40: 0000 5a05 6675 6e64 315a 0566 756e 6432  ..Z.fund1Z.fund2
-00003f50: da04 756e 6974 5a09 6d61 785f 7269 7363  ..unitZ.max_risc
-00003f60: 6f5a 1074 6963 6b65 725f 6d61 785f 7269  oZ.ticker_max_ri
-00003f70: 7363 6f72 7b00 0000 5a05 6675 6e64 6f72  scor{...Z.fundor
-00003f80: 1e00 0000 72bb 0000 005a 0976 616c 7565  ....r....Z.value
-00003f90: 7269 736b 721f 0000 0072 1f00 0000 7220  riskr....r....r 
-00003fa0: 0000 00da 0d63 6f6d 7061 7265 5f66 756e  .....compare_fun
-00003fb0: 6473 a002 0000 7344 0000 0000 190c 0104  ds....sD........
-00003fc0: 010a 010c 010e 0112 0116 010c 010e 0212  ................
-00003fd0: 0112 020e 0106 010a 0204 0208 0106 0204  ................
-00003fe0: 0104 0108 010a 010c 0110 0108 0104 0106  ................
-00003ff0: 0206 0106 ff04 0108 ff06 0308 010a 0272  ...............r
-00004000: bf00 0000 7a0b 2f62 6573 7441 7373 6574  ....z./bestAsset
-00004010: 7363 0100 0000 0000 0000 0000 0000 1900  sc..............
-00004020: 0000 0500 0000 4300 0000 73fa 0200 0064  ......C...s....d
-00004030: 017d 0174 00a0 017c 01a1 017d 027c 026a  .}.t...|...}.|.j
-00004040: 0264 026b 0372 2474 0364 0383 0101 0090  .d.k.r$t.d......
-00004050: 026e d274 047c 026a 0564 0483 027d 037c  .n.t.|.j.d...}.|
-00004060: 03a0 0664 05a1 0164 0619 007d 0474 076a  ...d...d...}.t.j
-00004070: 0874 097c 0483 0164 0764 0864 098d 0364  .t.|...d.d.d...d
-00004080: 0619 007d 057c 0564 0a19 00a0 0a64 0b64  ...}.|.d.....d.d
-00004090: 0c84 00a1 017c 0564 0a3c 0074 0364 0d83  .....|.d.<.t.d..
-000040a0: 0101 0074 0b6a 0c7c 0564 0a19 00a0 0da1  ...t.j.|.d......
-000040b0: 0064 0e64 0f8d 0264 1019 007d 0664 1164  .d.d...d...}.d.d
-000040c0: 1284 007d 0764 1364 1484 007d 0869 007d  ...}.d.d...}.i.}
-000040d0: 0969 007d 0a7c 066a 0e44 005d 247d 0b7c  .i.}.|.j.D.]$}.|
-000040e0: 067c 0b19 007d 0c7c 077c 0c83 017c 097c  .|...}.|.|...|.|
-000040f0: 0b3c 007c 087c 0c83 017c 0a7c 0b3c 0071  .<.|.|...|.|.<.q
-00004100: ac7c 0064 156b 0290 0172 8867 007d 0d7c  .|.d.k...r.g.}.|
-00004110: 066a 0e44 005d 267d 0b7c 097c 0b19 0064  .j.D.]&}.|.|...d
-00004120: 166b 0472 e67c 0a7c 0b19 0064 176b 0472  .k.r.|.|...d.k.r
-00004130: e67c 0da0 0f7c 0ba1 0101 0071 e674 076a  .|...|.....q.t.j
-00004140: 107c 0d64 1867 0164 198d 027d 0e74 0364  .|.d.g.d...}.t.d
-00004150: 1a83 0101 0074 117c 0d74 1274 1364 1b8d  .....t.|.t.t.d..
-00004160: 037d 0f7c 0f67 017d 0f74 07a0 107c 0fa1  .}.|.g.}.t...|..
-00004170: 017d 107c 10a0 1464 1ca1 017d 107c 1064  .}.|...d...}.|.d
-00004180: 1d19 00a0 15a1 00a0 16a1 007c 1064 1d3c  ...........|.d.<
-00004190: 007c 1064 1e19 00a0 15a1 00a0 16a1 007c  .|.d...........|
-000041a0: 1064 1e3c 007c 106a 1790 0172 806e 047c  .d.<.|.j...r.n.|
-000041b0: 1053 0090 016e 6e7c 0064 1f6b 0290 0272  .S...nn|.d.k...r
-000041c0: 4267 007d 117c 066a 0e44 005d 2c7d 0b7c  Bg.}.|.j.D.],}.|
-000041d0: 097c 0b19 0064 206b 0490 0172 9c7c 0a7c  .|...d k...r.|.|
-000041e0: 0b19 0064 216b 0090 0172 9c7c 11a0 0f7c  ...d!k...r.|...|
-000041f0: 0ba1 0101 0090 0171 9c74 076a 107c 1164  .......q.t.j.|.d
-00004200: 2267 0164 198d 027d 1274 0364 1a83 0101  "g.d...}.t.d....
-00004210: 0074 117c 1174 1274 1364 1b8d 037d 137c  .t.|.t.t.d...}.|
-00004220: 1367 017d 1374 07a0 107c 13a1 017d 147c  .g.}.t...|...}.|
-00004230: 14a0 1464 1ca1 017d 147c 1464 1d19 00a0  ...d...}.|.d....
-00004240: 15a1 00a0 16a1 007c 1464 1d3c 007c 1464  .......|.d.<.|.d
-00004250: 1e19 00a0 15a1 00a0 16a1 007c 1464 1e3c  ...........|.d.<
-00004260: 007c 146a 1790 0272 3c6e 047c 1453 006e  .|.j...r<n.|.S.n
-00004270: b47c 0064 236b 0290 0272 ee67 007d 157c  .|.d#k...r.g.}.|
-00004280: 066a 0e44 005d 1e7d 0b7c 0a7c 0b19 0064  .j.D.].}.|.|...d
-00004290: 176b 0090 0272 567c 15a0 0f7c 0ba1 0101  .k...rV|...|....
-000042a0: 0090 0271 5674 076a 107c 1564 2467 0164  ...qVt.j.|.d$g.d
-000042b0: 198d 027d 1674 0364 1a83 0101 0074 117c  ...}.t.d.....t.|
-000042c0: 1574 1274 1364 1b8d 037d 177c 1767 017d  .t.t.d...}.|.g.}
-000042d0: 1774 07a0 107c 17a1 017d 187c 18a0 1464  .t...|...}.|...d
-000042e0: 1ca1 017d 187c 1864 1d19 00a0 15a1 00a0  ...}.|.d........
-000042f0: 16a1 007c 1864 1d3c 007c 1864 1e19 00a0  ...|.d.<.|.d....
-00004300: 15a1 00a0 16a1 007c 1864 1e3c 007c 186a  .......|.d.<.|.j
-00004310: 1790 0272 e86e 047c 1853 006e 0874 0364  ...r.n.|.S.n.t.d
-00004320: 2583 0101 0064 2653 0029 2775 0c02 0000  %....d&S.)'u....
-00004330: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
-00004340: 6164 650a 2020 2020 2d20 4675 6ec3 a7c3  ade.    - Fun...
-00004350: a36f 2071 7565 2061 6e61 6c69 7361 206f  .o que analisa o
-00004360: 7320 7072 696e 6369 7061 6973 2061 7469  s principais ati
-00004370: 766f 7320 6c69 7374 6164 6f73 206e 6f20  vos listados no 
-00004380: 6d65 7263 6164 6f20 7175 6520 636f 6d20  mercado que com 
-00004390: 6261 7365 206e 6f20 7065 7266 696c 2065  base no perfil e
-000043a0: 7363 6f6c 6869 646f 206d 6f73 7472 6120  scolhido mostra 
-000043b0: 7175 6169 7320 706f 6465 6d20 7365 7220  quais podem ser 
-000043c0: 7375 6173 2065 7363 6f6c 6861 7320 6520  suas escolhas e 
-000043d0: 7175 616e 746f 7320 706f 7263 656e 746f  quantos porcento
-000043e0: 2073 6520 6465 7665 2074 6572 206e 6120   se deve ter na 
-000043f0: 6361 7274 6569 7261 0a20 2020 200a 2020  carteira.    .  
-00004400: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
-00004410: 0a20 2020 200a 2020 2020 2d20 7065 7266  .    .    - perf
-00004420: 696c 202d 3e20 5065 7266 6973 2071 7565  il -> Perfis que
-00004430: 2070 6f64 656d 2073 6572 2065 7363 6f6c   podem ser escol
-00004440: 6869 646f 7320 7061 7261 2072 6561 6c69  hidos para reali
-00004450: 7a61 7220 6120 616e c3a1 6c69 7365 2c20  zar a an..lise, 
-00004460: 7365 6775 6520 6120 6c69 7374 613a 200a  segue a lista: .
-00004470: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
-00004480: 2020 5469 706f 5065 7266 6973 3a0a 2020    TipoPerfis:.  
-00004490: 2020 2a20 4167 7265 7373 6976 6f0a 2020    * Agressivo.  
-000044a0: 2020 2a20 4d6f 6465 7261 646f 0a20 2020    * Moderado.   
-000044b0: 202a 2043 6f6e 7365 7276 6164 6f72 0a20   * Conservador. 
-000044c0: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
-000044d0: 0a20 2020 2023 2320 4578 656d 706c 6f0a  .    ## Exemplo.
-000044e0: 2020 2020 0a20 2020 2060 6060 0a20 2020      .    ```.   
-000044f0: 200a 2020 2020 3e3e 3e20 616c 6f63 6174   .    >>> alocat
-00004500: 696f 6e20 3d20 6265 7374 5f61 7373 6574  ion = best_asset
-00004510: 7328 7065 7266 696c 3d27 4167 7265 7373  s(perfil='Agress
-00004520: 6976 6f27 290a 2020 2020 0a20 2020 2060  ivo').    .    `
-00004530: 6060 0a20 2020 200a 2020 2020 7a2d 6874  ``.    .    z-ht
-00004540: 7470 733a 2f2f 7777 772e 6461 646f 7364  tps://www.dadosd
-00004550: 656d 6572 6361 646f 2e63 6f6d 2e62 722f  emercado.com.br/
-00004560: 626f 6c73 612f 6163 6f65 7372 5100 0000  bolsa/acoesrQ...
-00004570: 7a31 4163 6573 736f 206e 6567 6164 6f20  z1Acesso negado 
-00004580: 6120 6261 7365 2c20 7465 6e74 6520 6e6f  a base, tente no
-00004590: 7661 6d65 6e74 6520 6d61 6973 2074 6172  vamente mais tar
-000045a0: 6465 2e72 9f00 0000 72a0 0000 0072 0100  de.r....r....r..
-000045b0: 0000 fa01 2c72 1a00 0000 2902 da07 6465  ....,r....)...de
-000045c0: 6369 6d61 6c5a 0974 686f 7573 616e 6473  cimalZ.thousands
-000045d0: f507 0000 0043 c3b3 6469 676f 6301 0000  .....C..digoc...
-000045e0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000045f0: 0053 0000 0073 0800 0000 7c00 6401 1700  .S...s....|.d...
-00004600: 5300 72a2 0000 0072 1f00 0000 72a3 0000  S.r....r....r...
-00004610: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00004620: 72a5 0000 000e 0300 0072 a600 0000 7a1d  r........r....z.
-00004630: 6265 7374 5f61 7373 6574 732e 3c6c 6f63  best_assets.<loc
-00004640: 616c 733e 2e3c 6c61 6d62 6461 3e7a 1342  als>.<lambda>z.B
-00004650: 7573 6361 6e64 6f20 6174 6976 6f73 2e2e  uscando ativos..
-00004660: 2e2e 723a 0000 0072 3c00 0000 7248 0000  ..r:...r<...rH..
-00004670: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-00004680: 0000 0200 0000 5300 0000 7314 0000 007c  ......S...s....|
-00004690: 00a0 00a1 007d 017c 01a0 01a1 007d 027c  .....}.|.....}.|
-000046a0: 0253 00a9 014e 2902 726f 0000 0072 5900  .S...N).ro...rY.
-000046b0: 0000 2903 da06 7072 6563 6f73 da07 7265  ..)...precos..re
-000046c0: 746f 726e 6f5a 0d72 6574 6f72 6e6f 5f6d  tornoZ.retorno_m
-000046d0: 6564 696f 721f 0000 0072 1f00 0000 7220  edior....r....r 
-000046e0: 0000 00da 1063 616c 6375 6c61 725f 7265  .....calcular_re
-000046f0: 746f 726e 6f13 0300 0073 0600 0000 0001  torno....s......
-00004700: 0801 0801 7a25 6265 7374 5f61 7373 6574  ....z%best_asset
-00004710: 732e 3c6c 6f63 616c 733e 2e63 616c 6375  s.<locals>.calcu
-00004720: 6c61 725f 7265 746f 726e 6f63 0100 0000  lar_retornoc....
-00004730: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00004740: 5300 0000 7314 0000 007c 00a0 00a1 007d  S...s....|.....}
-00004750: 017c 01a0 01a1 007d 027c 0253 0072 c300  .|.....}.|.S.r..
-00004760: 0000 2902 726f 0000 0072 7600 0000 2903  ..).ro...rv...).
-00004770: 72c4 0000 0072 c500 0000 729b 0000 0072  r....r....r....r
-00004780: 1f00 0000 721f 0000 0072 2000 0000 da0e  ....r....r .....
-00004790: 6361 6c63 756c 6172 5f72 6973 636f 1903  calcular_risco..
-000047a0: 0000 7306 0000 0000 0108 0108 017a 2362  ..s..........z#b
-000047b0: 6573 745f 6173 7365 7473 2e3c 6c6f 6361  est_assets.<loca
-000047c0: 6c73 3e2e 6361 6c63 756c 6172 5f72 6973  ls>.calcular_ris
-000047d0: 636f 5a09 4167 7265 7373 6976 6f67 2d43  coZ.Agressivog-C
-000047e0: 1ceb e236 1a3f e77b 14ae 47e1 7a84 3f7a  ...6.?.{..G.z.?z
-000047f0: 1241 7469 766f 7320 502f 4167 7265 7373  .Ativos P/Agress
-00004800: 6976 6fa9 01da 0763 6f6c 756d 6e73 7a3f  ivo....columnsz?
-00004810: 5265 616c 697a 616e 646f 2063 616c 6375  Realizando calcu
-00004820: 6c6f 7320 7061 7261 2061 2073 7561 2063  los para a sua c
-00004830: 6172 7465 6972 6120 636f 6d20 6261 7365  arteira com base
-00004840: 206e 6f20 7365 7520 7065 7266 696c 2e29   no seu perfil.)
-00004850: 0272 8a00 0000 7261 0000 0072 8d00 0000  .r....ra...r....
-00004860: 728b 0000 0072 8c00 0000 5a08 4d6f 6465  r....r....Z.Mode
-00004870: 7261 646f 6761 3255 302a a933 3f67 b81e  radoga2U0*.3?g..
-00004880: 85eb 51b8 9e3f 7a11 4174 6976 6f73 2050  ..Q..?z.Ativos P
-00004890: 2f4d 6f64 6572 6164 6f5a 0b43 6f6e 7365  /ModeradoZ.Conse
-000048a0: 7276 6164 6f72 7a14 4174 6976 6f73 2050  rvadorz.Ativos P
-000048b0: 2f43 6f6e 7365 7276 6164 6f72 755a 0000  /ConservadoruZ..
-000048c0: 0050 6572 6669 6c20 6ec3 a36f 2072 6563  .Perfil n..o rec
-000048d0: 6f6e 6865 6369 646f 2c20 6f73 2070 6572  onhecido, os per
-000048e0: 6669 7320 6469 7370 6f6e 6976 6569 7320  fis disponiveis 
-000048f0: 6573 7461 6f20 7072 6573 656e 7465 7320  estao presentes 
-00004900: 6e61 2065 7870 6c69 6361 c3a7 c3a3 6f20  na explica....o 
-00004910: 6461 2066 756e c3a7 c3a3 6f4e 2918 72ad  da fun....oN).r.
-00004920: 0000 0072 ae00 0000 5a0b 7374 6174 7573  ...r....Z.status
-00004930: 5f63 6f64 6572 2f00 0000 7209 0000 0072  _coder/...r....r
-00004940: af00 0000 72b0 0000 0072 4300 0000 72b1  ....r....rC...r.
-00004950: 0000 0072 8300 0000 72b2 0000 0072 2a00  ...r....r....r*.
-00004960: 0000 7266 0000 00da 0674 6f6c 6973 7472  ..rf.....tolistr
-00004970: ca00 0000 7299 0000 0072 4400 0000 729d  ....r....rD...r.
-00004980: 0000 00da 046f 6e65 59da 0963 7572 7265  .....oneY..curre
-00004990: 6e74 6c79 5a07 6578 706c 6f64 6572 bd00  ntlyZ.exploder..
-000049a0: 0000 728e 0000 0072 4100 0000 2919 5a06  ..r....rA...).Z.
-000049b0: 7065 7266 696c 72b4 0000 0072 b500 0000  perfilr....r....
-000049c0: 72b6 0000 0072 a000 0000 72b7 0000 0072  r....r....r....r
-000049d0: c400 0000 72c6 0000 0072 c700 0000 72c5  ....r....r....r.
-000049e0: 0000 0072 9b00 0000 da05 6174 6976 6f5a  ...r......ativoZ
-000049f0: 0c70 7265 636f 735f 6174 6976 6f5a 0961  .precos_ativoZ.a
-00004a00: 6772 6573 7369 766f 5a0b 4466 4167 7265  gressivoZ.DfAgre
-00004a10: 7373 6976 6f5a 1361 6c6f 6361 7469 6f6e  ssivoZ.alocation
-00004a20: 5f41 6772 6573 7369 7665 5a17 6461 7461  _AgressiveZ.data
-00004a30: 416c 6f63 6174 696f 6e5f 4167 7265 7373  Alocation_Agress
-00004a40: 6976 655a 086d 6f64 6572 6164 6f5a 0a44  iveZ.moderadoZ.D
-00004a50: 664d 6f64 6572 6164 6f5a 1261 6c6f 6361  fModeradoZ.aloca
-00004a60: 7469 6f6e 5f4d 6f64 6572 6164 655a 1664  tion_ModeradeZ.d
-00004a70: 6174 6141 6c6f 6361 7469 6f6e 5f4d 6f64  ataAlocation_Mod
-00004a80: 6572 6164 655a 0b63 6f6e 7365 7276 6164  eradeZ.conservad
-00004a90: 6f72 5a0d 4466 436f 6e73 6572 7661 646f  orZ.DfConservado
-00004aa0: 725a 1661 6c6f 6361 7469 6f6e 5f43 6f6e  rZ.alocation_Con
-00004ab0: 7365 7276 6174 6976 655a 1a64 6174 6141  servativeZ.dataA
-00004ac0: 6c6f 6361 7469 6f6e 5f43 6f6e 7365 7276  location_Conserv
-00004ad0: 6174 6976 6572 1f00 0000 721f 0000 0072  ativer....r....r
-00004ae0: 2000 0000 da0b 6265 7374 5f61 7373 6574   .....best_asset
-00004af0: 73e8 0200 0073 8600 0000 001e 0401 0a01  s....s..........
-00004b00: 0a01 0c02 0c01 0e01 1801 1601 0801 1a03  ................
-00004b10: 0806 0806 0401 0401 0a01 0801 0c01 0e03  ................
-00004b20: 0a01 0401 0a01 1801 0c02 1001 0801 0e01  ................
-00004b30: 0601 0a01 0a04 1401 1402 0801 0202 0802  ................
-00004b40: 0a02 0401 0a01 1c01 0e02 1001 0801 0e01  ................
-00004b50: 0601 0a01 0a04 1401 1402 0801 0202 0602  ................
-00004b60: 0a02 0401 0a01 0e01 0e01 1002 0801 0e01  ................
-00004b70: 0601 0a01 0a03 1401 1402 0801 0202 0602  ................
-00004b80: 72cf 0000 007a 112f 6265 7374 4173 7365  r....z./bestAsse
-00004b90: 7473 5661 6c75 6573 6301 0000 0000 0000  tsValuesc.......
-00004ba0: 0000 0000 0009 0000 0005 0000 0003 0000  ................
-00004bb0: 0073 6c01 0000 7400 a001 6401 a101 7d01  .sl...t...d...}.
-00004bc0: 7c01 6402 1900 a002 6403 6404 8400 a101  |.d.....d.d.....
-00004bd0: 7c01 6402 3c00 7403 6a04 7c01 6402 1900  |.d.<.t.j.|.d...
-00004be0: a005 a100 6405 6406 8d02 6407 1900 7d02  ....d.d...d...}.
-00004bf0: 7c02 6a06 6408 6409 8d01 7d02 7c02 a007  |.j.d.d...}.|...
-00004c00: a100 a008 a100 640a 1400 8900 7c02 a007  ......d.....|...
-00004c10: a100 a009 a100 740a a00b 640a a101 1400  ......t...d.....
-00004c20: 7d03 7400 a00c 8800 7c03 640b 9c02 a101  }.t.....|.d.....
-00004c30: 7d04 7c04 640c 1900 7c04 640d 1900 1b00  }.|.d...|.d.....
-00004c40: 7c04 640e 3c00 7c04 6a0d 640e 640f 6410  |.d.<.|.j.d.d.d.
-00004c50: 8d02 a00e 6411 a101 7d04 7c04 640e 1900  ....d...}.|.d...
-00004c60: 7c04 640e 1900 a00f a100 1b00 7c04 6412  |.d.........|.d.
-00004c70: 3c00 7c04 6412 1900 8801 1400 7c04 6413  <.|.d.......|.d.
-00004c80: 3c00 7c04 a010 a100 7d04 7c04 6a11 6414  <.|.....}.|.j.d.
-00004c90: 6415 6416 9c02 6417 8d01 7d04 7c04 6414  d.d...d...}.|.d.
-00004ca0: 1900 4400 5d40 7d05 7403 6a04 7c05 6405  ..D.]@}.t.j.|.d.
-00004cb0: 6406 8d02 7d06 7c06 6407 1900 6a12 6418  d...}.|.d...j.d.
-00004cc0: 1900 7c06 6407 1900 6a12 6419 1900 1800  ..|.d...j.d.....
-00004cd0: 7c06 6407 1900 6a12 6419 1900 1b00 8800  |.d...j.d.......
-00004ce0: 7c05 3c00 71ee 8700 8701 6602 641a 641b  |.<.q.....f.d.d.
-00004cf0: 8408 7c04 6414 1900 4400 8301 7d07 7c07  ..|.d...D...}.|.
-00004d00: a013 a100 7d08 7414 7c08 8301 7d08 7c08  ....}.t.|...}.|.
-00004d10: 7c04 641c 3c00 7c04 6700 641d a201 1900  |.d.<.|.g.d.....
-00004d20: 5300 291e 751a 0200 000a 2020 2020 2323  S.).u.....    ##
-00004d30: 2055 7361 6269 6c69 6461 6465 0a20 2020   Usabilidade.   
-00004d40: 202d 2046 756e c3a7 c3a3 6f20 7175 6520   - Fun....o que 
-00004d50: 616e 616c 6973 6120 6f73 2061 7469 766f  analisa os ativo
-00004d60: 7320 646f 2049 424f 5645 5350 4120 7175  s do IBOVESPA qu
-00004d70: 6520 636f 6d20 6261 7365 206e 6f20 7661  e com base no va
-00004d80: 6c6f 7220 6465 2069 6e76 6573 7469 6d65  lor de investime
-00004d90: 6e74 6f20 6573 636f 6c68 6964 6f20 6d6f  nto escolhido mo
-00004da0: 7374 7261 2071 7561 6973 2070 6f64 656d  stra quais podem
-00004db0: 2073 6572 2073 7561 7320 6573 636f 6c68   ser suas escolh
-00004dc0: 6173 2c20 6f20 7175 616e 746f 2069 7261  as, o quanto ira
-00004dd0: 2074 6572 2071 7565 2069 6e76 6573 7469   ter que investi
-00004de0: 7220 7061 7261 2063 6164 6120 6174 6976  r para cada ativ
-00004df0: 6f20 6520 6f20 7265 746f 726e 6f20 6170  o e o retorno ap
-00004e00: 726f 7869 6d61 646f 2070 6172 6120 6361  roximado para ca
-00004e10: 6461 2075 6d20 6465 6c65 7320 0a0a 2020  da um deles ..  
-00004e20: 2020 2d20 5573 616d 6f73 2063 6f6d 6f20    - Usamos como 
-00004e30: 6d65 746f 646f 2064 6520 63c3 a16c 6375  metodo de c..lcu
-00004e40: 6c6f 206f 2061 206d 6564 6964 6120 5368  lo o a medida Sh
-00004e50: 6172 7065 2071 7565 206e 6164 6120 6d61  arpe que nada ma
-00004e60: 6973 20c3 a920 7175 6520 756d 6120 206d  is .. que uma  m
-00004e70: 6564 6964 6120 6465 2064 6573 656d 7065  edida de desempe
-00004e80: 6e68 6f20 6465 2069 6e76 6573 7469 6d65  nho de investime
-00004e90: 6e74 6f73 2071 7565 206c 6576 6120 656d  ntos que leva em
-00004ea0: 2063 6f6e 7369 6465 7261 c3a7 c3a3 6f20   considera....o 
-00004eb0: 6f20 7265 746f 726e 6f20 6f62 7469 646f  o retorno obtido
-00004ec0: 2070 656c 6f20 696e 7665 7374 696d 656e   pelo investimen
-00004ed0: 746f 2065 6d20 7265 6c61 c3a7 c3a3 6f20  to em rela....o 
-00004ee0: 616f 2072 6973 636f 2061 7373 756d 6964  ao risco assumid
-00004ef0: 6f0a 2020 2020 2323 2050 6172 c3a2 6d65  o.    ## Par..me
-00004f00: 7472 6f73 0a20 2020 200a 2020 2020 2d20  tros.    .    - 
-00004f10: 7661 6c6f 7220 2d3e 2056 616c 6f72 2064  valor -> Valor d
-00004f20: 6f20 696e 7665 7374 696d 656e 746f 2c20  o investimento, 
-00004f30: 706f 7220 7061 6472 c3a3 6f20 300a 0a20  por padr..o 0.. 
-00004f40: 2020 207a 3e51 3a5c 5269 7363 6f5c 4e6f     z>Q:\Risco\No
-00004f50: 766f 2052 6973 636f 5c70 7974 686f 6e72  vo Risco\pythonr
-00004f60: 6973 636f 5c42 4246 696e 616e 6365 5c44  isco\BBFinance\D
-00004f70: 6174 615c 4174 6976 6f73 4962 6f76 2e78  ata\AtivosIbov.x
-00004f80: 6c73 7872 c200 0000 6301 0000 0000 0000  lsxr....c.......
-00004f90: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00004fa0: 0073 0800 0000 7c00 6401 1700 5300 72a2  .s....|.d...S.r.
-00004fb0: 0000 0072 1f00 0000 72a3 0000 0072 1f00  ...r....r....r..
-00004fc0: 0000 721f 0000 0072 2000 0000 72a5 0000  ..r....r ...r...
-00004fd0: 0083 0300 0072 a600 0000 7a23 6265 7374  .....r....z#best
-00004fe0: 5f61 7373 6574 735f 7661 6c75 652e 3c6c  _assets_value.<l
-00004ff0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00005000: 3a00 0000 723c 0000 0072 4800 0000 7254  :...r<...rH...rT
-00005010: 0000 0029 015a 0461 7869 7372 6500 0000  ...).Z.axisre...
-00005020: 2902 729a 0000 0072 9b00 0000 729a 0000  ).r....r....r...
-00005030: 0072 9b00 0000 5a06 7368 6172 7065 4629  .r....Z.sharpeF)
-00005040: 015a 0961 7363 656e 6469 6e67 e906 0000  .Z.ascending....
-00005050: 005a 0861 6c6f 6361 6361 6fda 0576 616c  .Z.alocacao..val
-00005060: 6f72 da06 4174 6976 6f73 fa13 5174 6420  or..Ativos..Qtd 
-00005070: 4e65 6365 7373 6172 6961 2028 5224 2929  Necessaria (R$))
-00005080: 0272 8100 0000 72d1 0000 0072 c900 0000  .r....r....r....
-00005090: 7226 0000 0072 0100 0000 6301 0000 0000  r&...r....c.....
-000050a0: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-000050b0: 0000 0073 1a00 0000 6900 7c00 5d12 7d01  ...s....i.|.].}.
-000050c0: 7c01 8800 7c01 1900 8801 1400 9302 7104  |...|.........q.
-000050d0: 5300 721f 0000 0072 1f00 0000 2902 da02  S.r....r....)...
-000050e0: 2e30 72ce 0000 00a9 0272 9a00 0000 72d1  .0r......r....r.
-000050f0: 0000 0072 1f00 0000 7220 0000 00da 0a3c  ...r....r .....<
-00005100: 6469 6374 636f 6d70 3ea6 0300 0072 a600  dictcomp>....r..
-00005110: 0000 7a25 6265 7374 5f61 7373 6574 735f  ..z%best_assets_
-00005120: 7661 6c75 652e 3c6c 6f63 616c 733e 2e3c  value.<locals>.<
-00005130: 6469 6374 636f 6d70 3efa 0e52 6574 6f72  dictcomp>..Retor
-00005140: 6e6f 2041 7072 6f78 2e29 0372 d200 0000  no Aprox.).r....
-00005150: 72d3 0000 0072 d700 0000 2915 7243 0000  r....r....).rC..
-00005160: 005a 0a72 6561 645f 6578 6365 6c72 b200  .Z.read_excelr..
-00005170: 0000 722a 0000 0072 6600 0000 72cb 0000  ..r*...rf...r...
-00005180: 0072 8e00 0000 726f 0000 0072 5900 0000  .r....ro...rY...
-00005190: 7276 0000 0072 6700 0000 726a 0000 0072  rv...rg...rj...r
-000051a0: 4400 0000 5a0b 736f 7274 5f76 616c 7565  D...Z.sort_value
-000051b0: 73da 0468 6561 6472 3100 0000 7246 0000  s..headr1...rF..
-000051c0: 00da 0672 656e 616d 6572 3000 0000 da06  ...renamer0.....
-000051d0: 7661 6c75 6573 723e 0000 0029 0972 d100  valuesr>...).r..
-000051e0: 0000 da06 6174 6976 6f73 72c4 0000 0072  ....ativosr....r
-000051f0: 9b00 0000 5a09 6174 6976 6f73 5f64 6672  ....Z.ativos_dfr
-00005200: ce00 0000 7287 0000 005a 1172 6574 6f72  ....r....Z.retor
-00005210: 6e6f 5f70 6f72 5f61 7469 766f 5a0c 4c69  no_por_ativoZ.Li
-00005220: 7374 6152 6574 6f72 6e6f 721f 0000 0072  staRetornor....r
-00005230: d500 0000 7220 0000 00da 1162 6573 745f  ....r .....best_
-00005240: 6173 7365 7473 5f76 616c 7565 7403 0000  assets_valuet...
-00005250: 732a 0000 0000 0e0a 0116 031a 030c 0310  s*..............
-00005260: 0116 0310 0314 0314 0318 0310 0108 0212  ................
-00005270: 020c 010e 0130 0318 0108 0108 0208 0372  .....0.........r
-00005280: dc00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00005290: 0008 0000 0009 0000 0043 0000 0073 d800  .........C...s..
-000052a0: 0000 7400 6a01 6401 6402 6403 8d02 7d01  ..t.j.d.d.d...}.
-000052b0: 7c01 a002 a100 7d01 7403 a004 7c01 6404  |.....}.t...|.d.
-000052c0: 1900 a005 7406 a101 6a06 a007 6405 6406  ....t...j...d.d.
-000052d0: a102 a101 7d02 7c01 6407 1900 7d03 7408  ....}.|.d...}.t.
-000052e0: 8300 7d04 7c04 a009 7c02 6a0a a00b 6408  ..}.|...|.j...d.
-000052f0: 6409 a102 7c03 a102 0100 7403 6a0c a00d  d...|.....t.j...
-00005300: a100 a00e 640a a101 7d05 7403 6a0c a00d  ....d...}.t.j...
-00005310: a100 7403 6a0f 640b 640c 8d01 1700 a00e  ..t.j.d.d.......
-00005320: 640a a101 7d06 7c04 a010 7403 a004 7c06  d...}.|...t...|.
-00005330: a007 6405 6406 a102 6701 a101 a00b 6408  ..d.d...g.....d.
-00005340: 6409 a102 a101 7c04 a010 7403 a004 7c05  d.....|...t...|.
-00005350: a007 6405 6406 a102 6701 a101 a00b 6408  ..d.d...g.....d.
-00005360: 6409 a102 a101 1b00 6409 1800 7d07 7c07  d.......d...}.|.
-00005370: 640d 1900 6408 1400 5300 290e 4e72 6d00  d...d...S.).Nrm.
-00005380: 0000 723a 0000 0072 3c00 0000 da04 4461  ..r:...r<.....Da
-00005390: 7465 fa01 2d72 1800 0000 7248 0000 0072  te..-r....rH...r
-000053a0: 2600 0000 7254 0000 0072 1700 0000 7214  &...rT...r....r.
-000053b0: 0000 0072 1500 0000 7201 0000 0029 1172  ...r....r....).r
-000053c0: 2a00 0000 7266 0000 0072 4600 0000 7243  *...rf...rF...rC
-000053d0: 0000 005a 0a74 6f5f 6e75 6d65 7269 6372  ...Z.to_numericr
-000053e0: 1c00 0000 7283 0000 0072 1b00 0000 7204  ....r....r....r.
-000053f0: 0000 005a 0366 6974 72da 0000 00da 0772  ...Z.fitr......r
-00005400: 6573 6861 7065 da09 5469 6d65 7374 616d  eshape..Timestam
-00005410: 70da 0574 6f64 6179 da08 7374 7266 7469  p..today..strfti
-00005420: 6d65 5a0a 4461 7465 4f66 6673 6574 5a07  meZ.DateOffsetZ.
-00005430: 7072 6564 6963 7429 0872 ce00 0000 5a10  predict).r....Z.
-00005440: 6461 646f 735f 6869 7374 6f72 6963 6f73  dados_historicos
-00005450: 5a05 6461 7461 7372 c400 0000 5a06 6d6f  Z.datasr....Z.mo
-00005460: 6465 6c6f 5a0a 6461 7461 5f61 7475 616c  deloZ.data_atual
-00005470: 5a0b 6461 7461 5f66 7574 7572 615a 0c74  Z.data_futuraZ.t
-00005480: 6178 615f 7265 746f 726e 6f72 1f00 0000  axa_retornor....
-00005490: 721f 0000 0072 2000 0000 da13 7072 6576  r....r .....prev
-000054a0: 6572 5f74 6178 615f 7265 746f 726e 6fb6  er_taxa_retorno.
-000054b0: 0300 0073 1c00 0000 0002 0e01 0806 1e01  ...s............
-000054c0: 0803 0603 1603 1001 1c01 2001 20ff 0201  .......... . ...
-000054d0: 02ff 0403 72e3 0000 00e7 713d 0ad7 a370  ....r.....q=...p
-000054e0: cd3f 2902 72db 0000 00da 0c69 6e76 6573  .?).r......inves
-000054f0: 7469 6d65 6e74 6f63 0300 0000 0000 0000  timentoc........
-00005500: 0000 0000 0a00 0000 0700 0000 4300 0000  ............C...
-00005510: 731e 0100 0074 006a 0167 0064 01a2 0164  s....t.j.g.d...d
-00005520: 028d 017d 0374 027c 0074 0383 0272 9674  ...}.t.|.t...r.t
-00005530: 04a0 057c 00a1 017d 047c 046a 0664 0364  ...|...}.|.j.d.d
-00005540: 048d 0164 0519 0064 0619 007d 057c 046a  ...d...d...}.|.j
-00005550: 07a0 08a1 007d 067c 057c 0617 007c 051b  .....}.|.|...|..
-00005560: 0064 0718 007c 0114 007d 0774 09a0 0a7c  .d...|...}.t...|
-00005570: 077c 011b 0064 0717 00a1 0174 09a0 0a64  .|...d.....t...d
-00005580: 0764 087c 0214 0017 00a1 011b 0064 091b  .d.|.........d..
-00005590: 007d 087c 036a 0b7c 007c 077c 0864 019c  .}.|.j.|.|.|.d..
-000055a0: 0364 0a64 0b8d 027d 036e 847c 0044 005d  .d.d...}.n.|.D.]
-000055b0: 7e7d 0974 04a0 057c 09a1 017d 047c 046a  ~}.t...|...}.|.j
-000055c0: 0664 0364 048d 0164 0519 0064 0619 007d  .d.d...d...d...}
-000055d0: 057c 046a 07a0 08a1 007d 067c 057c 0617  .|.j.....}.|.|..
-000055e0: 007c 051b 0064 0718 007c 0114 007d 0774  .|...d...|...}.t
-000055f0: 09a0 0a7c 077c 011b 0064 0717 00a1 0174  ...|.|...d.....t
-00005600: 09a0 0a64 0764 087c 0214 0017 00a1 011b  ...d.d.|........
-00005610: 0064 091b 007d 087c 036a 0b7c 097c 077c  .d...}.|.j.|.|.|
-00005620: 0864 019c 0364 0a64 0b8d 027d 0371 9a7c  .d...d.d...}.q.|
-00005630: 0353 0029 0c4e 2903 727c 0000 007a 1652  .S.).N).r|...z.R
-00005640: 6574 6f72 6e6f 2063 6f6d 2044 6976 6964  etorno com Divid
-00005650: 656e 646f 737a 1a54 656d 706f 2070 6172  endosz.Tempo par
-00005660: 6120 4174 696e 6769 7220 5265 746f 726e  a Atingir Retorn
-00005670: 6f72 c900 0000 723a 0000 0072 3c00 0000  or....r:...r<...
-00005680: 7248 0000 0072 0100 0000 7254 0000 0072  rH...r....rT...r
-00005690: c800 0000 e90c 0000 0054 2901 5a0c 6967  .........T).Z.ig
-000056a0: 6e6f 7265 5f69 6e64 6578 290c 7243 0000  nore_index).rC..
-000056b0: 0072 4400 0000 7282 0000 0072 8300 0000  .rD...r....r....
-000056c0: 722a 0000 0072 2b00 0000 7240 0000 0072  r*...r+...r@...r
-000056d0: 2900 0000 7231 0000 0072 6700 0000 7268  )...r1...rg...rh
-000056e0: 0000 0072 9900 0000 290a 72db 0000 0072  ...r....).r....r
-000056f0: e500 0000 5a0d 7461 7861 5f64 6573 636f  ....Z.taxa_desco
-00005700: 6e74 6f72 8700 0000 727b 0000 005a 0570  ntor....r{...Z.p
-00005710: 7265 636f 5a0a 6469 7669 6465 6e64 6f73  recoZ.dividendos
-00005720: 72c5 0000 005a 0574 656d 706f 72ce 0000  r....Z.tempor...
-00005730: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00005740: da13 7265 746f 726e 6f73 5f64 6976 6964  ..retornos_divid
-00005750: 656e 646f 73d3 0300 0073 2000 0000 0001  endos....s .....
-00005760: 1002 0a01 0a01 1401 0a01 1401 2801 1802  ............(...
-00005770: 0801 0a01 1401 0a01 1401 2801 1802 72e7  ..........(...r.
-00005780: 0000 0029 0172 3a00 0000 2901 7201 0000  ...).r:...).r...
-00005790: 0029 0172 0100 0000 2901 72e4 0000 0029  .).r....).r....)
-000057a0: 4e5a 0879 6669 6e61 6e63 6572 2a00 0000  NZ.yfinancer*...
-000057b0: 5a0b 7363 6970 792e 7374 6174 7372 0200  Z.scipy.statsr..
-000057c0: 0000 5a0e 7363 6970 792e 6f70 7469 6d69  ..Z.scipy.optimi
-000057d0: 7a65 7203 0000 005a 1473 6b6c 6561 726e  zer....Z.sklearn
-000057e0: 2e6c 696e 6561 725f 6d6f 6465 6c72 0400  .linear_modelr..
-000057f0: 0000 5a08 7365 6c65 6e69 756d 7205 0000  ..Z.seleniumr...
-00005800: 005a 1e73 656c 656e 6975 6d2e 7765 6264  .Z.selenium.webd
-00005810: 7269 7665 722e 636f 6d6d 6f6e 2e6b 6579  river.common.key
-00005820: 7372 0600 0000 5a21 7365 6c65 6e69 756d  sr....Z!selenium
-00005830: 2e77 6562 6472 6976 6572 2e63 6872 6f6d  .webdriver.chrom
-00005840: 652e 6f70 7469 6f6e 7372 0700 0000 5a1c  e.optionsr....Z.
-00005850: 7365 6c65 6e69 756d 2e77 6562 6472 6976  selenium.webdriv
-00005860: 6572 2e63 6f6d 6d6f 6e2e 6279 7208 0000  er.common.byr...
-00005870: 0072 ad00 0000 5a03 6273 3472 0900 0000  .r....Z.bs4r....
-00005880: 5a07 6661 7374 6170 6972 0a00 0000 720b  Z.fastapir....r.
-00005890: 0000 0072 0c00 0000 5a11 6661 7374 6170  ...r....Z.fastap
-000058a0: 692e 7265 7370 6f6e 7365 7372 0d00 0000  i.responsesr....
-000058b0: 5a13 6661 7374 6170 692e 7374 6174 6963  Z.fastapi.static
-000058c0: 6669 6c65 7372 0e00 0000 5a12 6661 7374  filesr....Z.fast
-000058d0: 6170 692e 7465 6d70 6c61 7469 6e67 720f  api.templatingr.
-000058e0: 0000 00da 046a 736f 6e5a 0775 7669 636f  .....jsonZ.uvico
-000058f0: 726e da09 4242 4669 6e61 6e63 65da 0262  rn..BBFinance..b
-00005900: 62da 0670 616e 6461 7372 4300 0000 da05  b..pandasrC.....
-00005910: 6e75 6d70 7972 6700 0000 7210 0000 0072  numpyrg...r....r
-00005920: 1100 0000 da06 7479 7069 6e67 7212 0000  ......typingr...
-00005930: 00da 0877 6172 6e69 6e67 73da 0e66 696c  ...warnings..fil
-00005940: 7465 7277 6172 6e69 6e67 735a 0c70 6472  terwarningsZ.pdr
-00005950: 5f6f 7665 7272 6964 6572 e100 0000 5a0c  _overrider....Z.
-00005960: 6f6e 655f 7965 6172 5f61 676f 72e2 0000  one_year_agor...
-00005970: 0072 cc00 0000 72cd 0000 00da 0361 7070  .r....r......app
-00005980: 7221 0000 0072 ae00 0000 7283 0000 0072  r!...r....r....r
-00005990: 2e00 0000 7235 0000 00da 085f 5f6e 616d  ....r5.....__nam
-000059a0: 655f 5fda 0372 756e 72b5 0000 0072 4400  e__..runr....rD.
-000059b0: 0000 7247 0000 005a 0f72 6573 706f 6e73  ..rG...Z.respons
-000059c0: 6548 6973 746f 7279 724d 0000 0072 5f00  eHistoryrM...r_.
-000059d0: 0000 726c 0000 0072 7100 0000 721d 0000  ..rl...rq...r...
-000059e0: 00da 0369 6e74 7279 0000 0072 3e00 0000  ...intry...r>...
-000059f0: 7289 0000 0072 9d00 0000 72b9 0000 0072  r....r....r....r
-00005a00: bc00 0000 72bf 0000 0072 cf00 0000 72dc  ....r....r....r.
-00005a10: 0000 0072 e300 0000 72e7 0000 0072 1f00  ...r....r....r..
-00005a20: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00005a30: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
-00005a40: cc00 0000 0801 0c01 0c01 0c03 0c01 0c01  ................
-00005a50: 0c01 0c02 0801 0c03 1401 0c01 0c01 0c01  ................
-00005a60: 0801 0801 0802 0801 0801 1001 0c02 0801  ................
-00005a70: 0a03 0802 0802 0e03 0a01 0a02 060c 0809  ................
-00005a80: 0c01 1226 0a01 1201 0a05 0c01 1826 0a01  ...&.........&..
-00005a90: 1201 0a05 0c01 1220 0a01 1201 0a05 0c01  ....... ........
-00005aa0: 1238 0a01 1201 0a05 0c01 1618 0a01 1201  .8..............
-00005ab0: 0a05 0c01 1232 0a01 1201 0a05 0c01 1623  .....2.........#
-00005ac0: 0a01 1201 0a05 0c01 2062 0a01 1201 0a05  ........ b......
-00005ad0: 0801 163a 0a01 1201 0a05 0c01 1418 0a01  ...:............
-00005ae0: 1201 0a05 0c01 1642 0a01 1201 0a05 0c01  .......B........
-00005af0: 1a40 0a01 1201 0a05 0c01 167f 0007 0a01  .@..............
-00005b00: 1201 0a03 0c01 143a 0a01 1201 0a05 081d  .......:........
+00000510: 6a33 6453 6401 6417 8d02 6528 6542 6541  j3dSd.d...e(eBeA
+00000520: 6602 1900 6601 6522 6a3a 644d 9c01 6454  f...f.e"j:dM..dT
+00000530: 6455 8405 8301 5a4b 6537 641b 6b02 9005  dU....ZKe7d.k...
+00000540: 7226 651e 6a38 6531 641d 641e 6453 6420  r&e.j8e1d.d.dSd 
+00000550: 8d04 0100 6515 6421 6422 8d01 5a3c 6456  ....e.d!d"..Z<dV
+00000560: 6457 8400 5a4c 645e 6528 6534 6544 6602  dW..ZLd^e(e4eDf.
+00000570: 1900 6528 6542 6541 6602 1900 6459 9c02  ..e(eBeAf...dY..
+00000580: 645a 645b 8405 5a4d 6401 5300 295f e900  dZd[..ZMd.S.)_..
+00000590: 0000 004e 2901 da04 6e6f 726d 2901 da08  ...N)...norm)...
+000005a0: 6d69 6e69 6d69 7a65 2901 da10 4c69 6e65  minimize)...Line
+000005b0: 6172 5265 6772 6573 7369 6f6e 2901 da09  arRegression)...
+000005c0: 7765 6264 7269 7665 7229 01da 044b 6579  webdriver)...Key
+000005d0: 7329 01da 074f 7074 696f 6e73 2901 da02  s)...Options)...
+000005e0: 4279 2901 da0d 4265 6175 7469 6675 6c53  By)...BeautifulS
+000005f0: 6f75 7029 03da 0746 6173 7441 5049 da08  oup)...FastAPI..
+00000600: 5265 7370 6f6e 7365 da07 5265 7175 6573  Response..Reques
+00000610: 7429 01da 0c48 544d 4c52 6573 706f 6e73  t)...HTMLRespons
+00000620: 6529 01da 0b53 7461 7469 6346 696c 6573  e)...StaticFiles
+00000630: 2901 da0f 4a69 6e6a 6132 5465 6d70 6c61  )...Jinja2Templa
+00000640: 7465 7329 02da 0864 6174 6574 696d 65da  tes)...datetime.
+00000650: 0974 696d 6564 656c 7461 2901 da05 556e  .timedelta)...Un
+00000660: 696f 6eda 0669 676e 6f72 65e9 6d01 0000  ion..ignore.m...
+00000670: a901 da04 6461 7973 fa08 2559 2d25 6d2d  ....days..%Y-%m-
+00000680: 2564 6302 0000 0000 0000 0000 0000 0002  %dc.............
+00000690: 0000 0005 0000 0043 0000 0073 5e00 0000  .......C...s^...
+000006a0: 7c00 7c01 1900 6a00 6401 6402 6403 6404  |.|...j.d.d.d.d.
+000006b0: 8d03 7c00 7c01 3c00 7c00 7c01 1900 6a00  ..|.|.<.|.|...j.
+000006c0: 6405 6402 6403 6404 8d03 7c00 7c01 3c00  d.d.d.d...|.|.<.
+000006d0: 7c00 7c01 1900 6a00 6406 6407 6403 6404  |.|...j.d.d.d.d.
+000006e0: 8d03 7c00 7c01 3c00 7c00 7c01 1900 a001  ..|.|.<.|.|.....
+000006f0: 7402 a101 7c00 7c01 3c00 7c00 5300 2908  t...|.|.<.|.S.).
+00000700: 4e7a 035b 2e5d da00 5429 01da 0572 6567  Nz.[.]..T)...reg
+00000710: 6578 7a03 5b25 5d7a 035b 2c5d da01 2e29  exz.[%]z.[,]...)
+00000720: 03da 0772 6570 6c61 6365 da06 6173 7479  ...replace..asty
+00000730: 7065 da05 666c 6f61 7429 02da 0264 665a  pe..float)...dfZ
+00000740: 0a6e 6f6d 6543 6f6c 756e 61a9 0072 1f00  .nomeColuna..r..
+00000750: 0000 fa40 713a 5c52 6973 636f 5c4e 6f76  ...@q:\Risco\Nov
+00000760: 6f20 5269 7363 6f5c 7079 7468 6f6e 7269  o Risco\pythonri
+00000770: 7363 6f5c 4242 4669 6e61 6e63 655c 4242  sco\BBFinance\BB
+00000780: 4669 6e61 6e63 655c 4242 4669 6e61 6e63  Finance\BBFinanc
+00000790: 652e 7079 da14 666f 726d 6174 6156 616c  e.py..formataVal
+000007a0: 6f72 6573 4e75 6d65 726f 3800 0000 730a  oresNumero8...s.
+000007b0: 0000 0000 0118 0118 0118 0112 0272 2100  .............r!.
+000007c0: 0000 7a15 2f73 746f 636b 732f 7b73 796d  ..z./stocks/{sym
+000007d0: 626f 6c7d 2f69 6e66 6f29 015a 0e72 6573  bol}/info).Z.res
+000007e0: 706f 6e73 655f 6d6f 6465 6c29 02da 0673  ponse_model)...s
+000007f0: 796d 626f 6cda 0672 6574 7572 6e63 0100  ymbol..returnc..
+00000800: 0000 0000 0000 0000 0000 0800 0000 0500  ................
+00000810: 0000 4300 0000 7368 0000 0074 00a0 017c  ..C...sh...t...|
+00000820: 00a1 017d 017c 016a 027d 0274 037c 0283  ...}.|.j.}.t.|..
+00000830: 017d 037c 0374 046b 0272 226e 0874 0564  .}.|.t.k.r"n.t.d
+00000840: 0183 0101 007c 016a 0264 0219 007d 047c  .....|.j.d...}.|
+00000850: 016a 0264 0319 007d 057c 016a 067d 067c  .j.d...}.|.j.}.|
+00000860: 066a 0764 0464 0585 0219 00a0 08a1 007d  .j.d.d.........}
+00000870: 067c 007c 047c 057c 0664 069c 047d 077c  .|.|.|.|.d...}.|
+00000880: 0753 0029 0775 bf00 0000 0a20 2020 2023  .S.).u.....    #
+00000890: 2320 5573 6162 696c 6964 6164 6520 0a20  # Usabilidade . 
+000008a0: 2020 202d 2042 7573 6361 2061 7320 7072     - Busca as pr
+000008b0: 696e 6369 7061 6973 2069 6e66 6f72 6d61  incipais informa
+000008c0: c3a7 6f65 7320 736f 6272 6520 6f20 6174  ..oes sobre o at
+000008d0: 6976 6f20 7365 6c65 6369 6f6e 6164 6f20  ivo selecionado 
+000008e0: 636f 6d6f 2050 7265 c3a7 6f20 6520 4469  como Pre..o e Di
+000008f0: 7669 6465 6e64 6f73 200a 0a20 2020 200a  videndos ..    .
+00000900: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
+00000910: 6f73 0a20 2020 202d 2073 796d 626f 6c20  os.    - symbol 
+00000920: 2d3e 204e 6f6d 6520 646f 2041 7469 766f  -> Nome do Ativo
+00000930: 2070 6172 6120 6120 6275 7363 6120 0a0a   para a busca ..
+00000940: 2020 2020 0a20 2020 20fa 0f54 6963 6b65      .    ..Ticke
+00000950: 7220 496e 7661 6c69 646f da12 7265 6775  r Invalido..regu
+00000960: 6c61 724d 6172 6b65 7450 7269 6365 5a08  larMarketPriceZ.
+00000970: 6c6f 6e67 4e61 6d65 e9ff ffff ff4e 2904  longName.....N).
+00000980: 7222 0000 00da 0d63 7572 7265 6e74 5f70  r".....current_p
+00000990: 7269 6365 da0c 636f 6d70 616e 795f 6e61  rice..company_na
+000009a0: 6d65 da09 6469 7669 6465 6e64 7329 09da  me..dividends)..
+000009b0: 0279 66da 0654 6963 6b65 72da 0469 6e66  .yf..Ticker..inf
+000009c0: 6fda 0474 7970 65da 0464 6963 74da 0570  o..type..dict..p
+000009d0: 7269 6e74 7229 0000 00da 0469 6c6f 63da  rintr).....iloc.
+000009e0: 0373 756d 2908 7222 0000 00da 0573 746f  .sum).r".....sto
+000009f0: 636b 722c 0000 00da 0874 6970 6f49 6e66  ckr,.....tipoInf
+00000a00: 6f72 2700 0000 7228 0000 005a 0864 6976  or'...r(...Z.div
+00000a10: 6964 656e 64da 096a 736f 6e5f 6461 7461  idend..json_data
+00000a20: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00000a30: 0867 6574 5f69 6e66 6f41 0000 0073 2000  .get_infoA...s .
+00000a40: 0000 000c 0a01 0601 0801 0801 0202 0802  ................
+00000a50: 0a03 0a03 0601 1203 0201 0201 0201 02fd  ................
+00000a60: 0607 7235 0000 00da 085f 5f6d 6169 6e5f  ..r5.....__main_
+00000a70: 5f7a 086d 6169 6e3a 6170 707a 0931 3237  _z.main:appz.127
+00000a80: 2e30 2e30 2e31 6940 1f00 007a 1473 746f  .0.0.1i@...z.sto
+00000a90: 636b 732f 7b73 796d 626f 6c7d 2f69 6e66  cks/{symbol}/inf
+00000aa0: 6f29 03da 0468 6f73 74da 0470 6f72 74da  o)...host..port.
+00000ab0: 0764 6566 6175 6c74 7a10 6170 706c 6963  .defaultz.applic
+00000ac0: 6174 696f 6e2f 6a73 6f6e 2901 5a0a 6d65  ation/json).Z.me
+00000ad0: 6469 615f 7479 7065 7a18 2f73 746f 636b  dia_typez./stock
+00000ae0: 732f 7b73 796d 626f 6c7d 2f68 6973 746f  s/{symbol}/histo
+00000af0: 7279 da02 3179 2903 7222 0000 00da 0670  ry..1y).r".....p
+00000b00: 6572 696f 6472 2300 0000 6302 0000 0000  eriodr#...c.....
+00000b10: 0000 0000 0000 0008 0000 0003 0000 0043  ...............C
+00000b20: 0000 0073 7000 0000 7400 a001 7c00 a101  ...sp...t...|...
+00000b30: 7d02 7c02 6a02 7d03 7403 7c03 8301 7d04  }.|.j.}.t.|...}.
+00000b40: 7c04 7404 6b02 7222 6e08 7405 6401 8301  |.t.k.r"n.t.d...
+00000b50: 0100 7c02 6a06 7c01 6402 8d01 7d05 7c05  ..|.j.|.d...}.|.
+00000b60: 6a07 7248 6403 7405 6404 8301 6901 5300  j.rHd.t.d...i.S.
+00000b70: 7c05 6a08 6405 6406 8d01 7d06 7409 6a0a  |.j.d.d...}.t.j.
+00000b80: a00b 7c06 a101 6a0c 6407 6408 8d01 7d07  ..|...j.d.d...}.
+00000b90: 7c07 5300 6409 5300 290a 75ff 0000 000a  |.S.d.S.).u.....
+00000ba0: 2020 2020 2323 2055 7361 6269 6c69 6461      ## Usabilida
+00000bb0: 6465 200a 2020 2020 2d20 5573 6164 6120  de .    - Usada 
+00000bc0: 7061 7261 2076 6572 6966 6963 6172 206f  para verificar o
+00000bd0: 2068 6973 74c3 b372 6963 6f20 6461 2061   hist..rico da a
+00000be0: c3a7 616f 2073 656c 6563 696f 6e61 6461  ..ao selecionada
+00000bf0: 2065 2065 6d20 7175 616c 2070 6572 696f   e em qual perio
+00000c00: 646f 200a 0a20 2020 200a 2020 2020 2323  do ..    .    ##
+00000c10: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
+00000c20: 200a 2020 2020 2d20 7379 6d62 6f6c 202d   .    - symbol -
+00000c30: 3e20 4e6f 6d65 2064 6f20 4174 6976 6f20  > Nome do Ativo 
+00000c40: 7061 7261 2061 2062 7573 6361 200a 0a20  para a busca .. 
+00000c50: 2020 202d 2070 6572 696f 6420 2d3e 2044     - period -> D
+00000c60: 6174 6120 656d 2041 4e4f 5320 7061 7261  ata em ANOS para
+00000c70: 2061 2062 7573 6361 2064 6173 2069 6e66   a busca das inf
+00000c80: 6f72 6d61 c3a7 6f65 7320 646f 2041 7469  orma..oes do Ati
+00000c90: 766f 200a 0a20 2020 200a 2020 2020 7224  vo ..    .    r$
+00000ca0: 0000 00a9 0172 3b00 0000 da05 6572 726f  .....r;.....erro
+00000cb0: 727a 0d4e 6f20 6461 7461 2066 6f75 6e64  rz.No data found
+00000cc0: da04 6c69 7374 2901 5a06 6f72 6965 6e74  ..list).Z.orient
+00000cd0: 4629 01da 0464 726f 704e 290d 722a 0000  F)...dropN).r*..
+00000ce0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000cf0: 722e 0000 0072 2f00 0000 da07 6869 7374  r....r/.....hist
+00000d00: 6f72 79da 0565 6d70 7479 da07 746f 5f64  ory..empty..to_d
+00000d10: 6963 74da 0270 64da 0944 6174 6146 7261  ict..pd..DataFra
+00000d20: 6d65 da09 6672 6f6d 5f64 6963 74da 0b72  me..from_dict..r
+00000d30: 6573 6574 5f69 6e64 6578 2908 7222 0000  eset_index).r"..
+00000d40: 0072 3b00 0000 7232 0000 0072 2c00 0000  .r;...r2...r,...
+00000d50: 7233 0000 0072 4000 0000 5a0c 6869 7374  r3...r@...Z.hist
+00000d60: 6f72 795f 6469 6374 5a0a 6869 7374 6f72  ory_dictZ.histor
+00000d70: 795f 6466 721f 0000 0072 1f00 0000 7220  y_dfr....r....r 
+00000d80: 0000 00da 1167 6574 5f73 746f 636b 5f68  .....get_stock_h
+00000d90: 6973 746f 7279 6f00 0000 7318 0000 0000  istoryo...s.....
+00000da0: 0e0a 0106 0108 0108 0102 0208 020c 0206  ................
+00000db0: 010c 020c 0114 0272 4700 0000 7a17 7374  .......rG...z.st
+00000dc0: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 6869  ocks/{symbol}/hi
+00000dd0: 7374 6f72 797a 152f 7374 6f63 6b2f 7b73  storyz./stock/{s
+00000de0: 796d 626f 6c7d 2f74 7265 6e64 6301 0000  ymbol}/trendc...
+00000df0: 0000 0000 0000 0000 0008 0000 0003 0000  ................
+00000e00: 0043 0000 0073 6800 0000 7400 a001 7c00  .C...sh...t...|.
+00000e10: a101 7d01 7c01 6a02 7d02 7403 7c02 8301  ..}.|.j.}.t.|...
+00000e20: 7d03 7c03 7404 6b02 7222 6e08 7405 6401  }.|.t.k.r"n.t.d.
+00000e30: 8301 0100 7c01 6a06 6402 6403 8d01 7d04  ....|.j.d.d...}.
+00000e40: 7c04 6404 1900 7d05 7c05 6a07 6405 1900  |.d...}.|.j.d...
+00000e50: 7c05 6a07 6406 1900 6b04 7256 6407 6e02  |.j.d...k.rVd.n.
+00000e60: 6408 7d06 7c00 7c06 6409 9c02 7d07 7c07  d.}.|.|.d...}.|.
+00000e70: 5300 290a 75b9 0000 000a 2020 2020 2323  S.).u.....    ##
+00000e80: 2055 7361 6269 6c69 6461 6465 200a 2020   Usabilidade .  
+00000e90: 2020 2d20 4964 656e 7469 6669 6361 2061    - Identifica a
+00000ea0: 2074 656e 6465 6e63 6961 2064 6520 7072   tendencia de pr
+00000eb0: 65c3 a76f 2064 6520 756d 6120 61c3 a761  e..o de uma a..a
+00000ec0: 6f2c 2073 6520 6972 6120 7365 7220 6465  o, se ira ser de
+00000ed0: 2041 4c54 4120 6f75 2042 4149 5841 0a20   ALTA ou BAIXA. 
+00000ee0: 2020 200a 2020 2020 2323 2050 6172 c3a2     .    ## Par..
+00000ef0: 6d65 7472 6f73 0a20 2020 200a 2020 2020  metros.    .    
+00000f00: 2d20 7379 6d62 6f6c 202d 3e20 4e6f 6d65  - symbol -> Nome
+00000f10: 2064 6f20 4174 6976 6f20 7061 7261 2061   do Ativo para a
+00000f20: 2062 7573 6361 200a 0a20 2020 200a 2020   busca ..    .  
+00000f30: 2020 7224 0000 005a 0231 6472 3c00 0000    r$...Z.1dr<...
+00000f40: da05 436c 6f73 6572 2600 0000 7201 0000  ..Closer&...r...
+00000f50: 00da 0275 70da 0464 6f77 6e29 0272 2200  ...up..down).r".
+00000f60: 0000 da05 7472 656e 6429 0872 2a00 0000  ....trend).r*...
+00000f70: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+00000f80: 2e00 0000 722f 0000 0072 4000 0000 7230  ....r/...r@...r0
+00000f90: 0000 0029 0872 2200 0000 7232 0000 0072  ...).r"...r2...r
+00000fa0: 2c00 0000 7233 0000 0072 4000 0000 da0c  ,...r3...r@.....
+00000fb0: 636c 6f73 655f 7072 6963 6573 724b 0000  close_pricesrK..
+00000fc0: 0072 3400 0000 721f 0000 0072 1f00 0000  .r4...r....r....
+00000fd0: 7220 0000 00da 0f67 6574 5f73 746f 636b  r .....get_stock
+00000fe0: 5f74 7265 6e64 9d00 0000 731a 0000 0000  _trend....s.....
+00000ff0: 0d0a 0106 0108 0108 0102 0208 020c 0108  ................
+00001000: 011c 0202 0102 ff06 0672 4d00 0000 7a15  .........rM...z.
+00001010: 7374 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f  stocks/{symbol}/
+00001020: 7472 656e 647a 192f 7374 6f63 6b2f 7b73  trendz./stock/{s
+00001030: 796d 626f 6c7d 2f74 6563 686e 6963 616c  ymbol}/technical
+00001040: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
+00001050: 0006 0000 0043 0000 0073 f800 0000 7400  .....C...s....t.
+00001060: a001 7c00 a101 7d01 7c01 6a02 7d02 7403  ..|...}.|.j.}.t.
+00001070: 7c02 8301 7d03 7c03 7404 6b02 7222 6e08  |...}.|.t.k.r"n.
+00001080: 7405 6401 8301 0100 7c01 6a06 6402 6403  t.d.....|.j.d.d.
+00001090: 8d01 7d04 7c04 6404 1900 7d05 7c05 6a07  ..}.|.d...}.|.j.
+000010a0: 6405 6406 8d01 a008 a100 6a09 6407 1900  d.d.......j.d...
+000010b0: 7d06 7c05 6a07 6408 6406 8d01 a008 a100  }.|.j.d.d.......
+000010c0: 6a09 6407 1900 7d07 7c05 a00a a100 7d08  j.d...}.|.....}.
+000010d0: 7c08 a00b 7c08 6409 6b04 6409 a102 7d09  |...|.d.k.d...}.
+000010e0: 7c08 a00b 7c08 6409 6b00 6409 a102 0b00  |...|.d.k.d.....
+000010f0: 7d0a 7c09 6a07 640a 6406 8d01 a008 a100  }.|.j.d.d.......
+00001100: 7d0b 7c0a 6a07 640a 6406 8d01 a008 a100  }.|.j.d.d.......
+00001110: 7d0c 7c0b 7c0c 1b00 7d0d 640b 640b 640c  }.|.|...}.d.d.d.
+00001120: 7c0d 1700 1b00 6a09 6407 1900 1800 7d0e  |.....j.d.....}.
+00001130: 7c0e 640d 6b05 72e0 640e 7d0f 6e04 640f  |.d.k.r.d.}.n.d.
+00001140: 7d0f 7c00 7c06 7c07 7c0e 7c0f 6410 9c05  }.|.|.|.|.|.d...
+00001150: 7d10 7c10 5300 2911 7579 0200 000a 2020  }.|.S.).uy....  
+00001160: 2020 2323 2055 7361 6269 6c69 6461 6465    ## Usabilidade
+00001170: 200a 2020 2020 2d20 63c3 a16c 6375 6c6f   .    - c..lculo
+00001180: 2065 6e76 6f6c 7665 2061 2063 6f6d 7061   envolve a compa
+00001190: 7261 c3a7 c3a3 6f20 6461 206d c3a9 6469  ra....o da m..di
+000011a0: 6120 6465 2067 616e 686f 7320 656d 2075  a de ganhos em u
+000011b0: 6d20 7065 72c3 ad6f 646f 2064 6520 7465  m per..odo de te
+000011c0: 6d70 6f20 636f 6d20 6120 6dc3 a964 6961  mpo com a m..dia
+000011d0: 2064 6520 7065 7264 6173 2065 6d20 756d   de perdas em um
+000011e0: 2070 6572 c3ad 6f64 6f20 6465 2074 656d   per..odo de tem
+000011f0: 706f 2e20 0a0a 2020 2020 0a20 2020 2023  po. ..    .    #
+00001200: 2320 436f 6d6f 2069 6e74 6572 7072 6574  # Como interpret
+00001210: 6172 200a 2020 2020 2d20 5175 616e 646f  ar .    - Quando
+00001220: 206f 2052 5349 2065 7374 c3a1 2061 6369   o RSI est.. aci
+00001230: 6d61 2064 6520 3730 2c20 6f20 6174 6976  ma de 70, o ativ
+00001240: 6f20 c3a9 2063 6f6e 7369 6465 7261 646f  o .. considerado
+00001250: 2073 6f62 7265 636f 6d70 7261 646f 2c20   sobrecomprado, 
+00001260: 6f20 7175 6520 7369 676e 6966 6963 6120  o que significa 
+00001270: 7175 6520 706f 6465 2065 7374 6172 2070  que pode estar p
+00001280: 7265 7374 6573 2061 2073 6f66 7265 7220  restes a sofrer 
+00001290: 756d 6120 636f 7272 65c3 a7c3 a36f 2070  uma corre....o p
+000012a0: 6172 6120 6261 6978 6f2e 200a 2020 2020  ara baixo. .    
+000012b0: 5175 616e 646f 206f 2052 5349 2065 7374  Quando o RSI est
+000012c0: c3a1 2061 6261 6978 6f20 6465 2033 302c  .. abaixo de 30,
+000012d0: 206f 2061 7469 766f 20c3 a920 636f 6e73   o ativo .. cons
+000012e0: 6964 6572 6164 6f20 736f 6272 6576 656e  iderado sobreven
+000012f0: 6469 646f 2c20 6f20 7175 6520 7369 676e  dido, o que sign
+00001300: 6966 6963 6120 7175 6520 706f 6465 2065  ifica que pode e
+00001310: 7374 6172 2070 7265 7374 6573 2061 2073  star prestes a s
+00001320: 7562 6972 206e 6f76 616d 656e 7465 2e20  ubir novamente. 
+00001330: 0a20 0a20 2020 202d 2073 6d61 5f35 3020  . .    - sma_50 
+00001340: 2d3e 204d 6564 6961 206d 6f76 656c 2064  -> Media movel d
+00001350: 6f73 2035 3020 7065 7269 6f64 6f73 0a20  os 50 periodos. 
+00001360: 2020 202d 2073 6d61 5f32 3030 202d 3e20     - sma_200 -> 
+00001370: 6d65 6469 6120 6d6f 7665 6c20 646f 7320  media movel dos 
+00001380: 3230 3020 7065 7269 646f 730a 0a20 2020  200 peridos..   
+00001390: 2023 2320 5061 72c3 a26d 6574 726f 730a   ## Par..metros.
+000013a0: 2020 2020 2d20 7379 6d62 6f6c 202d 3e20      - symbol -> 
+000013b0: 4e6f 6d65 2064 6f20 4174 6976 6f20 7061  Nome do Ativo pa
+000013c0: 7261 2061 2062 7573 6361 200a 0a20 2020  ra a busca ..   
+000013d0: 200a 2020 2020 7224 0000 00da 036d 6178   .    r$.....max
+000013e0: 723c 0000 0072 4800 0000 e932 0000 0029  r<...rH....2...)
+000013f0: 01da 0677 696e 646f 7772 2600 0000 e9c8  ...windowr&.....
+00001400: 0000 0072 0100 0000 e90e 0000 00e9 6400  ...r..........d.
+00001410: 0000 e901 0000 00e9 4600 0000 7a1f 4120  ........F...z.A 
+00001420: 6368 616e 6365 2064 6f20 7072 6563 6f20  chance do preco 
+00001430: 646f 2061 7469 766f 2043 4149 527a 2041  do ativo CAIRz A
+00001440: 2063 6861 6e63 6520 646f 2070 7265 636f   chance do preco
+00001450: 2064 6f20 6174 6976 6f20 5355 4249 5229   do ativo SUBIR)
+00001460: 0572 2200 0000 da06 736d 615f 3530 da07  .r".....sma_50..
+00001470: 736d 615f 3230 30da 0372 7369 5a08 7465  sma_200..rsiZ.te
+00001480: 6e64 656e 6379 290c 722a 0000 0072 2b00  ndency).r*...r+.
+00001490: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+000014a0: 0072 2f00 0000 7240 0000 005a 0772 6f6c  .r/...r@...Z.rol
+000014b0: 6c69 6e67 da04 6d65 616e 7230 0000 00da  ling..meanr0....
+000014c0: 0464 6966 66da 0577 6865 7265 2911 7222  .diff..where).r"
+000014d0: 0000 0072 3200 0000 722c 0000 0072 3300  ...r2...r,...r3.
+000014e0: 0000 7240 0000 0072 4c00 0000 7256 0000  ..r@...rL...rV..
+000014f0: 0072 5700 0000 da05 6465 6c74 615a 0467  .rW.....deltaZ.g
+00001500: 6169 6e5a 046c 6f73 735a 0861 7667 5f67  ainZ.lossZ.avg_g
+00001510: 6169 6e5a 0861 7667 5f6c 6f73 73da 0272  ainZ.avg_loss..r
+00001520: 7372 5800 0000 da06 7374 6174 7573 7234  srX.....statusr4
+00001530: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00001540: 0000 da14 6765 745f 7374 6f63 6b5f 7465  ....get_stock_te
+00001550: 6368 6e69 6361 6c73 c500 0000 7336 0000  chnicals....s6..
+00001560: 0000 120a 0106 0108 0108 0102 0208 020c  ................
+00001570: 0108 0316 0116 0308 0110 0112 0110 0110  ................
+00001580: 0108 0116 0208 0106 0204 0302 0102 0102  ................
+00001590: 0102 0102 fb06 0a72 5f00 0000 7a19 7374  .......r_...z.st
+000015a0: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 7465  ocks/{symbol}/te
+000015b0: 6368 6e69 6361 6c7a 1a73 746f 636b 732f  chnicalz.stocks/
+000015c0: 7b73 796d 626f 6c7d 2f76 6f6c 6174 696c  {symbol}/volatil
+000015d0: 6974 7929 0472 2200 0000 da0a 7374 6172  ity).r".....star
+000015e0: 745f 6461 7465 da08 656e 645f 6461 7465  t_date..end_date
+000015f0: 7223 0000 0063 0300 0000 0000 0000 0000  r#...c..........
+00001600: 0000 0600 0000 0600 0000 4300 0000 7368  ..........C...sh
+00001610: 0000 007a 2874 006a 017c 007c 017c 0264  ...z(t.j.|.|.|.d
+00001620: 018d 037d 037c 036a 0272 2664 0274 0364  ...}.|.j.r&d.t.d
+00001630: 0383 0169 0157 0053 0057 006e 0c01 0001  ...i.W.S.W.n....
+00001640: 0001 0059 006e 0230 0074 04a0 057c 0364  ...Y.n.0.t...|.d
+00001650: 0419 007c 0364 0419 00a0 0664 05a1 011b  ...|.d.....d....
+00001660: 00a1 017d 0474 04a0 0764 067c 04a0 08a1  ...}.t...d.|....
+00001670: 0014 00a1 017d 057c 0553 0029 0775 6e01  .....}.|.S.).un.
+00001680: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
+00001690: 6964 6164 6520 0a20 2020 202d 204d c3a9  idade .    - M..
+000016a0: 746f 646f 2075 7361 646f 2070 6172 6120  todo usado para 
+000016b0: 7665 7269 6669 6361 7220 6120 766f 6c61  verificar a vola
+000016c0: 7469 6c69 6461 6465 2064 6520 756d 2061  tilidade de um a
+000016d0: 7469 766f 2065 6d20 636f 6d70 6172 6163  tivo em comparac
+000016e0: 616f 2061 6f20 6d65 7263 6164 6f20 656d  ao ao mercado em
+000016f0: 2071 7565 2065 7374 6120 200a 0a20 2020   que esta  ..   
+00001700: 200a 2020 2020 2323 2050 6172 c3a2 6d65   .    ## Par..me
+00001710: 7472 6f73 0a20 2020 202d 2073 796d 626f  tros.    - symbo
+00001720: 6c20 2d3e 204e 6f6d 6520 646f 2041 7469  l -> Nome do Ati
+00001730: 766f 2070 6172 6120 6120 6275 7363 6120  vo para a busca 
+00001740: 0a0a 2020 2020 2d20 7374 6172 745f 6461  ..    - start_da
+00001750: 7465 202d 3e20 4461 7461 2064 6520 496e  te -> Data de In
+00001760: 6963 696f 2064 6120 6275 7363 6120 6461  icio da busca da
+00001770: 7320 696e 666f 7320 2870 7265 636f 2c20  s infos (preco, 
+00001780: 766f 6c75 6d65 2c20 6574 6329 2064 6f20  volume, etc) do 
+00001790: 6174 6976 6f20 0a0a 2020 2020 2d20 656e  ativo ..    - en
+000017a0: 645f 6461 7465 202d 3e20 4461 7461 2046  d_date -> Data F
+000017b0: 696e 616c 2070 6172 6120 6120 6275 7363  inal para a busc
+000017c0: 6120 6461 7320 696e 666f 7320 2870 7265  a das infos (pre
+000017d0: 636f 2c20 766f 6c75 6d65 2c20 6574 6329  co, volume, etc)
+000017e0: 2064 6f20 6174 6976 6f20 0a0a 2020 2020   do ativo ..    
+000017f0: a902 da05 7374 6172 74da 0365 6e64 723d  ....start..endr=
+00001800: 0000 007a 384e 616f 2066 6f69 2065 6e63  ...z8Nao foi enc
+00001810: 6f6e 7472 6164 6f20 6f20 6869 7374 6f72  ontrado o histor
+00001820: 6963 6f20 6e65 7373 6520 7065 7269 6f64  ico nesse period
+00001830: 6f2c 2076 6572 6966 6963 6172 2e72 4800  o, verificar.rH.
+00001840: 0000 7254 0000 00e9 fc00 0000 2909 722a  ..rT........).r*
+00001850: 0000 00da 0864 6f77 6e6c 6f61 6472 4100  .....downloadrA.
+00001860: 0000 722f 0000 00da 026e 70da 036c 6f67  ..r/.....np..log
+00001870: da05 7368 6966 74da 0473 7172 74da 0376  ..shift..sqrt..v
+00001880: 6172 2906 7222 0000 0072 6000 0000 7261  ar).r"...r`...ra
+00001890: 0000 005a 0a73 746f 636b 5f64 6174 615a  ...Z.stock_dataZ
+000018a0: 0b6c 6f67 5f72 6574 7572 6e73 5a0a 766f  .log_returnsZ.vo
+000018b0: 6c61 7469 6c69 7479 721f 0000 0072 1f00  latilityr....r..
+000018c0: 0000 7220 0000 00da 0e67 6574 5f76 6f6c  ..r .....get_vol
+000018d0: 6174 696c 6974 7907 0100 0073 1200 0000  atility....s....
+000018e0: 000d 0201 1001 0601 1201 0601 0602 1c01  ................
+000018f0: 1202 726c 0000 007a 1473 746f 636b 732f  ..rl...z.stocks/
+00001900: 7b73 796d 626f 6c7d 2f62 6574 6163 0100  {symbol}/betac..
+00001910: 0000 0000 0000 0000 0000 0f00 0000 0300  ................
+00001920: 0000 4300 0000 73be 0000 0074 00a0 0164  ..C...s....t...d
+00001930: 01a1 017d 0174 00a0 0164 02a1 017d 027c  ...}.t...d...}.|
+00001940: 016a 027d 037c 026a 027d 0474 037c 0383  .j.}.|.j.}.t.|..
+00001950: 017d 057c 0574 046b 0273 427c 0474 046b  .}.|.t.k.sB|.t.k
+00001960: 0272 3a6e 0874 0564 0383 0101 007c 016a  .r:n.t.d.....|.j
+00001970: 0664 0464 058d 017d 067c 026a 0664 0464  .d.d...}.|.j.d.d
+00001980: 058d 017d 077c 0664 0619 00a0 07a1 007d  ...}.|.d.......}
+00001990: 087c 0764 0619 00a0 07a1 007d 097c 08a0  .|.d.......}.|..
+000019a0: 087c 09a1 017d 0a7c 09a0 09a1 007d 0b7c  .|...}.|.....}.|
+000019b0: 0a7c 0b1b 007d 0c7c 0c64 076b 0472 9864  .|...}.|.d.k.r.d
+000019c0: 087d 0d7c 0c64 076b 0072 a464 097d 0d7c  .}.|.d.k.r.d.}.|
+000019d0: 0c64 076b 0272 b064 0a7d 0d7c 0c7c 0d64  .d.k.r.d.}.|.|.d
+000019e0: 0b9c 027d 0e7c 0e53 0029 0c75 9501 0000  ...}.|.S.).u....
+000019f0: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
+00001a00: 6164 6520 0a20 2020 202d 204f 2062 6574  ade .    - O bet
+00001a10: 6120 c3a9 2075 6d61 206d 6564 6964 6120  a .. uma medida 
+00001a20: 6573 7461 74c3 ad73 7469 6361 2071 7565  estat..stica que
+00001a30: 2069 6e64 6963 6120 6120 7265 6c61 c3a7   indica a rela..
+00001a40: c3a3 6f20 656e 7472 6520 6120 766f 6c61  ..o entre a vola
+00001a50: 7469 6c69 6461 6465 2064 6520 756d 6120  tilidade de uma 
+00001a60: 61c3 a7c3 a36f 2065 2061 2076 6f6c 6174  a....o e a volat
+00001a70: 696c 6964 6164 6520 646f 206d 6572 6361  ilidade do merca
+00001a80: 646f 2063 6f6d 6f20 756d 2074 6f64 6f2e  do como um todo.
+00001a90: 0a20 2020 204f 2076 616c 6f72 2064 6f20  .    O valor do 
+00001aa0: 6265 7461 20c3 a920 7574 696c 697a 6164  beta .. utilizad
+00001ab0: 6f20 7061 7261 206d 6564 6972 206f 2072  o para medir o r
+00001ac0: 6973 636f 2064 6520 756d 6120 61c3 a7c3  isco de uma a...
+00001ad0: a36f 2065 6d20 7265 6c61 c3a7 c3a3 6f20  .o em rela....o 
+00001ae0: 616f 206d 6572 6361 646f 2065 6d20 7175  ao mercado em qu
+00001af0: 6520 656c 6120 c3a9 206e 6567 6f63 6961  e ela .. negocia
+00001b00: 6461 2e20 0a0a 2020 2020 0a20 2020 2023  da. ..    .    #
+00001b10: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
+00001b20: 2020 2d20 7379 6d62 6f6c 202d 3e20 4e6f    - symbol -> No
+00001b30: 6d65 2064 6f20 4174 6976 6f20 7061 7261  me do Ativo para
+00001b40: 2061 2062 7573 6361 200a 0a20 2020 202d   a busca ..    -
+00001b50: 206d 6172 6b65 7420 2d3e 2043 6f6d 6f20   market -> Como 
+00001b60: 7061 6472 616f 2c20 4d65 7263 6164 6f3a  padrao, Mercado:
+00001b70: 2049 424f 5645 5350 4120 2f20 4256 5350   IBOVESPA / BVSP
+00001b80: 0a20 2020 20fa 0850 4554 5234 2e53 417a  .    ..PETR4.SAz
+00001b90: 055e 4256 5350 7224 0000 0072 4e00 0000  .^BVSPr$...rN...
+00001ba0: 723c 0000 0072 4800 0000 7254 0000 007a  r<...rH...rT...z
+00001bb0: 2841 6361 6f20 6d61 6973 2056 6f6c 6174  (Acao mais Volat
+00001bc0: 696c 2071 7565 206f 206d 6572 6361 646f  il que o mercado
+00001bd0: 2065 6d20 6765 7261 6c7a 2941 6361 6f20   em geralz)Acao 
+00001be0: 6d65 6e6f 7320 566f 6c61 7469 6c20 7175  menos Volatil qu
+00001bf0: 6520 6f20 6d65 7263 6164 6f20 656d 2067  e o mercado em g
+00001c00: 6572 616c 7a34 4163 616f 2063 6f6d 2061  eralz4Acao com a
+00001c10: 206d 6573 6d61 2056 6f6c 6174 696c 6964   mesma Volatilid
+00001c20: 6164 6520 7175 6520 6f20 6d65 7263 6164  ade que o mercad
+00001c30: 6f20 656d 2067 6572 616c 2902 da04 6265  o em geral)...be
+00001c40: 7461 725e 0000 0029 0a72 2a00 0000 722b  tar^...).r*...r+
+00001c50: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00001c60: 0000 722f 0000 0072 4000 0000 da0a 7063  ..r/...r@.....pc
+00001c70: 745f 6368 616e 6765 da03 636f 7672 6b00  t_change..covrk.
+00001c80: 0000 290f 7222 0000 005a 0561 7373 6574  ..).r"...Z.asset
+00001c90: 5a06 6d61 726b 6574 722c 0000 005a 0a69  Z.marketr,...Z.i
+00001ca0: 6e66 6f4d 6172 6b65 7472 3300 0000 5a0d  nfoMarketr3...Z.
+00001cb0: 6173 7365 745f 6869 7374 6f72 795a 0e6d  asset_historyZ.m
+00001cc0: 6172 6b65 745f 6869 7374 6f72 795a 0d61  arket_historyZ.a
+00001cd0: 7373 6574 5f72 6574 7572 6e73 5a0e 6d61  sset_returnsZ.ma
+00001ce0: 726b 6574 5f72 6574 7572 6e73 7270 0000  rket_returnsrp..
+00001cf0: 0072 6b00 0000 726e 0000 0072 5e00 0000  .rk...rn...r^...
+00001d00: 7234 0000 0072 1f00 0000 721f 0000 0072  r4...r....r....r
+00001d10: 2000 0000 da08 6765 745f 6265 7461 2701   .....get_beta'.
+00001d20: 0000 7332 0000 0000 0e0a 010a 0106 0106  ..s2............
+00001d30: 0108 0110 0102 0208 020c 010c 030c 010c  ................
+00001d40: 030a 0108 0108 0208 0104 0108 0104 0108  ................
+00001d50: 0104 0302 0102 ff06 0572 7100 0000 7a13  .........rq...z.
+00001d60: 7374 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f  stocks/{symbol}/
+00001d70: 5661 5229 0472 2200 0000 da10 636f 6e66  VaR).r".....conf
+00001d80: 6964 656e 6365 5f6c 6576 656c da0f 6c6f  idence_level..lo
+00001d90: 6f6b 6261 636b 5f70 6572 696f 6472 2300  okback_periodr#.
+00001da0: 0000 6303 0000 0000 0000 0000 0000 000b  ..c.............
+00001db0: 0000 0006 0000 0043 0000 0073 9e00 0000  .......C...s....
+00001dc0: 7400 a001 7c00 a101 7d03 7c03 6a02 7d04  t...|...}.|.j.}.
+00001dd0: 7403 7c04 8301 7d05 7c05 7404 6b02 7222  t.|...}.|.t.k.r"
+00001de0: 6e08 7405 6401 8301 0100 7c03 6a06 7c02  n.t.d.....|.j.|.
+00001df0: 9b00 6402 9d02 6403 8d01 6404 1900 7d06  ..d...d...d...}.
+00001e00: 7407 a008 7c06 7c06 a009 6405 a101 1b00  t...|.|...d.....
+00001e10: a101 7d07 7c07 a00a a100 7d08 7c08 740b  ..}.|.....}.|.t.
+00001e20: a00c 6405 7c01 1800 a101 1400 7d09 7405  ..d.|.......}.t.
+00001e30: 6406 740d 7c09 7c06 6407 1900 1400 6408  d.t.|.|.d.....d.
+00001e40: 8302 6901 8301 0100 740d 7c09 7c06 6407  ..i.....t.|.|.d.
+00001e50: 1900 1400 6408 8302 7d0a 7c0a 5300 2909  ....d...}.|.S.).
+00001e60: 75c8 0100 000a 2020 2020 2323 2055 7361  u.....    ## Usa
+00001e70: 6269 6c69 6461 6465 200a 2020 2020 2d20  bilidade .    - 
+00001e80: 4f20 5661 6c75 6520 6174 2052 6973 6b20  O Value at Risk 
+00001e90: 2856 6152 2920 c3a9 2075 6d61 206d 6564  (VaR) .. uma med
+00001ea0: 6964 6120 6465 2072 6973 636f 2071 7565  ida de risco que
+00001eb0: 2069 6e64 6963 6120 6120 7065 7264 6120   indica a perda 
+00001ec0: 6dc3 a178 696d 6120 6573 7065 7261 6461  m..xima esperada
+00001ed0: 2c20 636f 6d20 756d 2064 6574 6572 6d69  , com um determi
+00001ee0: 6e61 646f 206e c3ad 7665 6c20 6465 2063  nado n..vel de c
+00001ef0: 6f6e 6669 616e c3a7 612c 2065 6d20 756d  onfian..a, em um
+00001f00: 2069 6e74 6572 7661 6c6f 2064 6520 7465   intervalo de te
+00001f10: 6d70 6f20 7072 c3a9 2d64 6574 6572 6d69  mpo pr..-determi
+00001f20: 6e61 646f 2e20 0a0a 2020 2020 0a20 2020  nado. ..    .   
+00001f30: 2023 2320 5061 72c3 a26d 6574 726f 730a   ## Par..metros.
+00001f40: 2020 2020 0a20 2020 202d 2073 796d 626f      .    - symbo
+00001f50: 6c20 2d3e 204e 6f6d 6520 646f 2041 7469  l -> Nome do Ati
+00001f60: 766f 2070 6172 6120 6661 7a65 7220 6120  vo para fazer a 
+00001f70: 6275 7363 6120 0a0a 2020 2020 2d20 636f  busca ..    - co
+00001f80: 6e66 6964 656e 6365 5f6c 6576 656c 202d  nfidence_level -
+00001f90: 3e20 4e69 7665 6c20 6465 2063 6f6e 6669  > Nivel de confi
+00001fa0: 616e c3a7 6120 7061 7261 206f 2056 4152  an..a para o VAR
+00001fb0: 2028 3020 6120 3129 2c20 6e6f 726d 616c   (0 a 1), normal
+00001fc0: 6d65 6e74 6520 7573 6164 6f20 656d 2030  mente usado em 0
+00001fd0: 2e39 3520 0a0a 2020 2020 2d20 6c6f 6f6b  .95 ..    - look
+00001fe0: 6261 636b 5f70 6572 696f 6420 2d3e 2050  back_period -> P
+00001ff0: 6572 696f 646f 2045 4d20 4449 4153 2061  eriodo EM DIAS a
+00002000: 2073 6572 2063 6f6e 7369 6465 7261 646f   ser considerado
+00002010: 2070 6172 6120 6f20 63c3 a16c 6375 6c6f   para o c..lculo
+00002020: 2064 6f20 5661 520a 0a20 2020 2072 2400   do VaR..    r$.
+00002030: 0000 da01 6472 3c00 0000 7248 0000 0072  ....dr<...rH...r
+00002040: 5400 0000 5a03 5661 5272 2600 0000 e902  T...Z.VaRr&.....
+00002050: 0000 0029 0e72 2a00 0000 722b 0000 0072  ...).r*...r+...r
+00002060: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
+00002070: 0000 0072 4000 0000 7267 0000 0072 6800  ...r@...rg...rh.
+00002080: 0000 7269 0000 00da 0373 7464 7202 0000  ..ri.....stdr...
+00002090: 005a 0370 7066 da05 726f 756e 6429 0b72  .Z.ppf..round).r
+000020a0: 2200 0000 7272 0000 0072 7300 0000 7232  "...rr...rs...r2
+000020b0: 0000 0072 2c00 0000 7233 0000 005a 0670  ...r,...r3...Z.p
+000020c0: 7269 6365 73da 0772 6574 7572 6e73 5a07  rices..returnsZ.
+000020d0: 7374 645f 6465 7672 6b00 0000 5a03 5661  std_devrk...Z.Va
+000020e0: 7272 1f00 0000 721f 0000 0072 2000 0000  rr....r....r ...
+000020f0: da07 6765 745f 7661 7261 0100 0073 1a00  ..get_vara...s..
+00002100: 0000 000f 0a01 0601 0801 0801 0202 0803  ................
+00002110: 1603 1403 0801 1201 1a01 1201 7279 0000  ............ry..
+00002120: 007a 1c73 746f 636b 732f 7b73 796d 626f  .z.stocks/{symbo
+00002130: 6c7d 2f41 6e6e 7561 6c52 6574 7572 6e29  l}/AnnualReturn)
+00002140: 04da 0773 796d 626f 6c73 7260 0000 0072  ...symbolsr`...r
+00002150: 6100 0000 7223 0000 0063 0300 0000 0000  a...r#...c......
+00002160: 0000 0000 0000 1100 0000 0700 0000 4300  ..............C.
+00002170: 0000 7392 0100 0074 007c 0074 0183 0272  ..s....t.|.t...r
+00002180: c874 0264 017c 009b 009d 0283 0101 0074  .t.d.|.........t
+00002190: 036a 047c 007c 017c 0264 0264 038d 047d  .j.|.|.|.d.d...}
+000021a0: 037a 8674 03a0 057c 00a1 016a 067d 047c  .z.t...|...j.}.|
+000021b0: 0464 0419 007d 057c 0364 0519 007d 067c  .d...}.|.d...}.|
+000021c0: 06a0 07a1 007d 077c 07a0 08a1 0064 0614  .....}.|.....d..
+000021d0: 007d 087c 07a0 09a1 0064 0714 007d 097c  .}.|.....d...}.|
+000021e0: 066a 0a64 0819 0064 0914 007d 0a7c 066a  .j.d...d...}.|.j
+000021f0: 0a64 0a19 0064 0914 007d 0b7c 0b7c 0a18  .d...d...}.|.|..
+00002200: 007c 0a1b 007d 0c74 0b6a 0c7c 007c 057c  .|...}.t.j.|.|.|
+00002210: 087c 097c 0c64 0b9c 0564 0c67 0164 0d8d  .|.|.d...d.g.d..
+00002220: 027d 0d7c 0d57 0053 0001 0001 0001 0074  .}.|.W.S.......t
+00002230: 0264 0e83 0101 0059 006e 0230 006e c674  .d.....Y.n.0.n.t
+00002240: 007c 0074 0d83 0290 0172 8674 0ba0 0ca1  .|.t.....r.t....
+00002250: 007d 0e74 0264 0f7c 009b 009d 0283 0101  .}.t.d.|........
+00002260: 007c 0044 005d 927d 0f74 036a 047c 0f7c  .|.D.].}.t.j.|.|
+00002270: 017c 0264 0264 038d 047d 037c 0364 0519  .|.d.d...}.|.d..
+00002280: 007d 067c 06a0 07a1 007d 077c 07a0 08a1  .}.|.....}.|....
+00002290: 0064 0614 007d 087c 07a0 09a1 0064 0714  .d...}.|.....d..
+000022a0: 007d 097c 066a 0a64 0819 0064 0914 007d  .}.|.j.d...d...}
+000022b0: 0a7c 066a 0a64 0a19 0064 0914 007d 0b7c  .|.j.d...d...}.|
+000022c0: 0b7c 0a18 007c 0a1b 007d 0c74 0b6a 0c7c  .|...|...}.t.j.|
+000022d0: 0f7c 087c 097c 0c64 109c 0474 0e7c 0083  .|.|.|.d...t.|..
+000022e0: 0167 0164 0d8d 027d 1074 0ba0 0f7c 107c  .g.d...}.t...|.|
+000022f0: 0e67 02a1 017d 0e71 ee7c 0e53 0074 0264  .g...}.q.|.S.t.d
+00002300: 1183 0101 0064 1253 0029 1375 9b01 0000  .....d.S.).u....
+00002310: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
+00002320: 6164 650a 2020 2020 2d20 5265 6365 6265  ade.    - Recebe
+00002330: 2075 6d61 206c 6973 7461 2065 2072 6574   uma lista e ret
+00002340: 6f72 6e61 2075 6d20 4461 7461 4672 616d  orna um DataFram
+00002350: 6520 636f 6d20 6173 2069 6e66 6f72 6d61  e com as informa
+00002360: c3a7 c3b5 6573 2064 6f73 2061 7469 766f  ....es dos ativo
+00002370: 7320 6520 616c 6775 6d61 7320 6573 7461  s e algumas esta
+00002380: 74c3 ad73 7469 6361 7320 62c3 a173 6963  t..sticas b..sic
+00002390: 6173 2e20 0a0a 2020 2020 0a20 2020 2023  as. ..    .    #
+000023a0: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
+000023b0: 2020 2d20 7379 6d62 6f6c 7320 2d3e 2052    - symbols -> R
+000023c0: 6563 6562 6520 756d 6120 6c69 7374 6120  ecebe uma lista 
+000023d0: 6f75 2075 6d20 756e 6963 6f20 6174 6976  ou um unico ativ
+000023e0: 6f20 7061 7261 2062 7573 6361 7220 6e61  o para buscar na
+000023f0: 2062 6173 6520 0a0a 2020 2020 2d20 7374   base ..    - st
+00002400: 6172 745f 6461 7465 202d 3e20 4461 7461  art_date -> Data
+00002410: 2064 6520 496e 6963 696f 2064 6120 6275   de Inicio da bu
+00002420: 7363 6120 6461 7320 696e 666f 7320 2870  sca das infos (p
+00002430: 7265 636f 2c20 766f 6c75 6d65 2c20 6574  reco, volume, et
+00002440: 6329 2064 6f20 6174 6976 6f20 0a0a 2020  c) do ativo ..  
+00002450: 2020 2d20 656e 645f 6461 7465 202d 3e20    - end_date -> 
+00002460: 4461 7461 2046 696e 616c 2070 6172 6120  Data Final para 
+00002470: 6120 6275 7363 6120 6461 7320 696e 666f  a busca das info
+00002480: 7320 2870 7265 636f 2c20 766f 6c75 6d65  s (preco, volume
+00002490: 2c20 6574 6329 2064 6f20 6174 6976 6f20  , etc) do ativo 
+000024a0: 0a0a 2020 2020 0a20 2020 2075 1a00 0000  ..    .    u....
+000024b0: 566f 63c3 aa20 6469 6769 746f 7520 756d  Voc.. digitou um
+000024c0: 6120 7374 7269 6e67 3a20 da06 7469 636b  a string: ..tick
+000024d0: 6572 2904 5a07 7469 636b 6572 7372 6300  er).Z.tickersrc.
+000024e0: 0000 7264 0000 005a 0867 726f 7570 5f62  ..rd...Z.group_b
+000024f0: 7972 2500 0000 7248 0000 0072 6500 0000  yr%...rH...re...
+00002500: 675f 75bc 7ebf bf2f 4072 0100 0000 7253  g_u.~../@r....rS
+00002510: 0000 0072 2600 0000 2905 da05 4174 6976  ...r&...)...Ativ
+00002520: 6f75 1000 0000 5072 65c3 a76f 2061 204d  ou....Pre..o a M
+00002530: 6572 6361 646f fa0d 5265 746f 726e 6f20  ercado..Retorno 
+00002540: 616e 7561 6cf5 1400 0000 4465 7376 696f  anual.....Desvio
+00002550: 2070 6164 72c3 a36f 2061 6e75 616c fa0d   padr..o anual..
+00002560: 5265 746f 726e 6f20 746f 7461 6c72 5400  Retorno totalrT.
+00002570: 0000 a901 da05 696e 6465 7875 1000 0000  ......indexu....
+00002580: 5469 636b 6572 2069 6e76 c3a1 6c69 646f  Ticker inv..lido
+00002590: 7519 0000 0056 6f63 c3aa 2064 6967 6974  u....Voc.. digit
+000025a0: 6f75 2075 6d61 206c 6973 7461 3a20 2904  ou uma lista: ).
+000025b0: 727c 0000 0072 7d00 0000 727e 0000 0072  r|...r}...r~...r
+000025c0: 7f00 0000 752f 0000 0054 6970 6f20 696e  ....u/...Tipo in
+000025d0: 76c3 a16c 6964 6f2e 2044 6967 6974 6520  v..lido. Digite 
+000025e0: 756d 6120 7374 7269 6e67 206f 7520 756d  uma string ou um
+000025f0: 6120 6c69 7374 612e 4e29 10da 0a69 7369  a lista.N)...isi
+00002600: 6e73 7461 6e63 65da 0373 7472 722f 0000  nstance..strr/..
+00002610: 0072 2a00 0000 7266 0000 0072 2b00 0000  .r*...rf...r+...
+00002620: 722c 0000 0072 6f00 0000 7259 0000 0072  r,...ro...rY...r
+00002630: 7600 0000 7230 0000 0072 4300 0000 7244  v...r0...rC...rD
+00002640: 0000 0072 3e00 0000 da03 6c65 6eda 0663  ...r>.....len..c
+00002650: 6f6e 6361 7429 1172 7a00 0000 7260 0000  oncat).rz...r`..
+00002660: 0072 6100 0000 da05 6461 646f 73da 0464  .ra.....dados..d
+00002670: 6174 615a 0b76 616c 7565 4d61 726b 6574  ataZ.valueMarket
+00002680: da05 636c 6f73 655a 0e72 6574 6f72 6e6f  ..closeZ.retorno
+00002690: 5f64 6961 7269 6f5a 0d72 6574 6f72 6e6f  _diarioZ.retorno
+000026a0: 5f61 6e75 616c 5a13 6465 7376 696f 5f70  _anualZ.desvio_p
+000026b0: 6164 7261 6f5f 616e 7561 6c5a 0f76 616c  adrao_anualZ.val
+000026c0: 6f72 5f69 6e76 6573 7469 646f 5a0b 7661  or_investidoZ.va
+000026d0: 6c6f 725f 6174 7561 6c5a 0d72 6574 6f72  lor_atualZ.retor
+000026e0: 6e6f 5f74 6f74 616c 5a0c 7661 6c75 6553  no_totalZ.valueS
+000026f0: 796d 626f 6c73 5a07 7661 6c75 6544 465a  ymbolsZ.valueDFZ
+00002700: 0773 696d 626f 6c6f 5a0d 7265 7475 726e  .simboloZ.return
+00002710: 5379 6d62 6f6c 7372 1f00 0000 721f 0000  Symbolsr....r...
+00002720: 0072 2000 0000 da0f 6173 7365 745f 706f  .r .....asset_po
+00002730: 7274 666f 6c69 6f8c 0100 0073 6000 0000  rtfolio....s`...
+00002740: 000e 0a01 0e01 1202 0202 0c01 0803 0803  ................
+00002750: 0803 0c03 0c03 0e03 0e03 0c03 0401 0201  ................
+00002760: 0201 0201 0201 02fb 0406 04fa 0608 0602  ................
+00002770: 0601 1002 0c01 0801 0e01 0801 1203 0803  ................
+00002780: 0803 0c03 0c03 0e03 0e03 0c03 0401 0201  ................
+00002790: 0201 0201 02fc 0405 08fb 0607 1002 0402  ................
+000027a0: 7289 0000 007a 2473 746f 636b 732f 7b73  r....z$stocks/{s
+000027b0: 796d 626f 6c7d 2f4d 6172 6b6f 7769 747a  ymbol}/Markowitz
+000027c0: 416c 6c6f 6361 7469 6f6e 6e29 0472 7a00  Allocationn).rz.
+000027d0: 0000 da09 7374 6172 5f64 6174 6572 6100  ....star_datera.
+000027e0: 0000 7223 0000 0063 0300 0000 0000 0000  ..r#...c........
+000027f0: 0000 0000 1100 0000 0900 0000 4300 0000  ............C...
+00002800: 733a 0100 0074 006a 017c 007c 017c 0264  s:...t.j.|.|.|.d
+00002810: 018d 0364 0219 007d 037c 03a0 02a1 00a0  ...d...}.|......
+00002820: 03a1 007d 047c 04a0 04a1 007d 0574 05a0  ...}.|.....}.t..
+00002830: 0664 0374 077c 0083 011b 0067 0174 077c  .d.t.|.....g.t.|
+00002840: 0083 0114 00a1 017d 0674 05a0 087c 04a0  .......}.t...|..
+00002850: 09a1 007c 0614 00a1 0164 0414 007d 0774  ...|.....d...}.t
+00002860: 05a0 0a74 05a0 0b7c 066a 0c74 05a0 0b7c  ...t...|.j.t...|
+00002870: 057c 06a1 02a1 02a1 0174 05a0 0a64 04a1  .|.......t...d..
+00002880: 0114 007d 0864 0574 05a0 0d7c 05a1 0114  ...}.d.t...|....
+00002890: 007d 0974 056a 0ea0 0f7c 057c 0974 05a0  .}.t.j...|.|.t..
+000028a0: 107c 056a 1164 0619 00a1 0114 0017 00a1  .|.j.d..........
+000028b0: 017d 0a74 05a0 1274 077c 0083 0164 0366  .}.t...t.|...d.f
+000028c0: 02a1 017d 0b74 05a0 0b7c 0a7c 0ba1 0274  ...}.t...|.|...t
+000028d0: 05a0 0b74 05a0 0b7c 0b6a 0c7c 0aa1 027c  ...t...|.j.|...|
+000028e0: 0ba1 021b 007d 0c7c 0ca0 13a1 007d 0c67  .....}.|.....}.g
+000028f0: 007d 0d74 1474 077c 0083 0183 0144 005d  .}.t.t.|.....D.]
+00002900: 2e7d 0e64 077c 007c 0e19 009b 0064 087c  .}.d.|.|.....d.|
+00002910: 0c7c 0e19 0064 0914 0064 0a9b 0464 0b9d  .|...d...d...d..
+00002920: 057d 0f7c 0da0 157c 0fa1 0101 0071 fa7c  .}.|...|.....q.|
+00002930: 077c 087c 0d64 0c9c 037d 107c 1053 0029  .|.|.d...}.|.S.)
+00002940: 0d75 2403 0000 0a20 2020 2023 2320 5573  .u$....    ## Us
+00002950: 6162 696c 6964 6164 6573 200a 2020 2020  abilidades .    
+00002960: 2d20 416c 6f63 61c3 a7c3 a36f 2064 6520  - Aloca....o de 
+00002970: 4d61 726b 6f77 6974 7a20 c3a9 2075 6d61  Markowitz .. uma
+00002980: 2074 c3a9 636e 6963 6120 6465 206f 7469   t..cnica de oti
+00002990: 6d69 7a61 c3a7 c3a3 6f20 6465 2070 6f72  miza....o de por
+000029a0: 7466 c3b3 6c69 6f20 7175 6520 7669 7361  tf..lio que visa
+000029b0: 2065 6e63 6f6e 7472 6172 2061 2063 6f6d   encontrar a com
+000029c0: 6269 6e61 c3a7 c3a3 6f20 6964 6561 6c20  bina....o ideal 
+000029d0: 6465 2061 7469 766f 7320 7061 7261 206d  de ativos para m
+000029e0: 6178 696d 697a 6172 206f 2072 6574 6f72  aximizar o retor
+000029f0: 6e6f 2064 6f20 696e 7665 7374 696d 656e  no do investimen
+00002a00: 746f 2065 6e71 7561 6e74 6f20 6d69 6e69  to enquanto mini
+00002a10: 6d69 7a61 206f 2072 6973 636f 2e20 0a0a  miza o risco. ..
+00002a20: 0a20 2020 2023 2320 4f20 5265 746f 726e  .    ## O Retorn
+00002a30: 6f20 4573 7065 7261 646f 0a20 2020 202d  o Esperado.    -
+00002a40: 2072 6570 7265 7365 6e74 6120 6120 7461   representa a ta
+00002a50: 7861 2064 6520 7265 746f 726e 6f20 6dc3  xa de retorno m.
+00002a60: a964 6961 2071 7565 2073 6520 6573 7065  .dia que se espe
+00002a70: 7261 206f 6274 6572 2064 6f20 706f 7274  ra obter do port
+00002a80: 66c3 b36c 696f 2064 6520 696e 7665 7374  f..lio de invest
+00002a90: 696d 656e 746f 7320 0a0a 2020 2020 2323  imentos ..    ##
+00002aa0: 204f 2052 6973 636f 200a 2020 2020 2d20   O Risco .    - 
+00002ab0: 7265 7072 6573 656e 7461 2061 206d 6564  representa a med
+00002ac0: 6964 6120 6465 2076 6f6c 6174 696c 6964  ida de volatilid
+00002ad0: 6164 6520 646f 2070 6f72 7466 c3b3 6c69  ade do portf..li
+00002ae0: 6f2c 206f 7520 7365 6a61 2c20 0a20 2020  o, ou seja, .   
+00002af0: 2071 7561 6e74 6f20 6d61 6973 2069 6e73   quanto mais ins
+00002b00: 74c3 a176 656c 2066 6f72 206f 2072 6574  t..vel for o ret
+00002b10: 6f72 6e6f 2064 6f73 2061 7469 766f 732c  orno dos ativos,
+00002b20: 206d 6169 6f72 2073 6572 c3a1 206f 2072   maior ser.. o r
+00002b30: 6973 636f 2064 6f20 706f 7274 66c3 b36c  isco do portf..l
+00002b40: 696f 2063 6f6d 6f20 756d 2074 6f64 6f20  io como um todo 
+00002b50: 0a0a 2020 2020 0a20 2020 200a 2020 2020  ..    .    .    
+00002b60: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
+00002b70: 726f 730a 2020 2020 0a20 2020 202d 2073  ros.    .    - s
+00002b80: 796d 626f 6c73 202d 3e20 5265 6365 6265  ymbols -> Recebe
+00002b90: 2075 6d61 206c 6973 7461 2064 6520 6174   uma lista de at
+00002ba0: 6976 6f73 2070 6172 6120 6275 7363 6172  ivos para buscar
+00002bb0: 206e 6120 6261 7365 200a 0a20 2020 202d   na base ..    -
+00002bc0: 2073 7461 7274 5f64 6174 6520 2d3e 2044   start_date -> D
+00002bd0: 6174 6120 6465 2049 6e69 6369 6f20 6461  ata de Inicio da
+00002be0: 2062 7573 6361 2064 6173 2069 6e66 6f73   busca das infos
+00002bf0: 2028 7072 6563 6f2c 2076 6f6c 756d 652c   (preco, volume,
+00002c00: 2065 7463 2920 646f 2061 7469 766f 200a   etc) do ativo .
+00002c10: 0a20 2020 202d 2065 6e64 5f64 6174 6520  .    - end_date 
+00002c20: 2d3e 2044 6174 6120 4669 6e61 6c20 7061  -> Data Final pa
+00002c30: 7261 2061 2062 7573 6361 2064 6173 2069  ra a busca das i
+00002c40: 6e66 6f73 2028 7072 6563 6f2c 2076 6f6c  nfos (preco, vol
+00002c50: 756d 652c 2065 7463 2920 646f 2061 7469  ume, etc) do ati
+00002c60: 766f 200a 0a0a 2020 2020 7262 0000 007a  vo ...    rb...z
+00002c70: 0941 646a 2043 6c6f 7365 7254 0000 0072  .Adj CloserT...r
+00002c80: 6500 0000 679a 9999 9999 99b9 3f72 0100  e...g.......?r..
+00002c90: 0000 7a08 4f20 6174 6976 6f20 7a15 2064  ..z.O ativo z. d
+00002ca0: 6576 6520 7365 7220 616c 6f63 6164 6f20  eve ser alocado 
+00002cb0: 656d 2072 5300 0000 7a03 2e32 667a 0d25  em rS...z..2fz.%
+00002cc0: 2064 6120 6361 7274 6569 7261 2903 fa10   da carteira)...
+00002cd0: 5265 746f 726e 6f20 4573 7065 7261 646f  Retorno Esperado
+00002ce0: fa11 5269 7363 6f20 6461 2043 6172 7465  ..Risco da Carte
+00002cf0: 6972 61fa 1241 6c6f 6361 6361 6f20 4d61  ira..Alocacao Ma
+00002d00: 726b 6f77 6974 7a29 1672 2a00 0000 7266  rkowitz).r*...rf
+00002d10: 0000 0072 6f00 0000 da06 6472 6f70 6e61  ...ro.....dropna
+00002d20: 7270 0000 0072 6700 0000 da05 6172 7261  rp...rg.....arra
+00002d30: 7972 8400 0000 7231 0000 0072 5900 0000  yr....r1...rY...
+00002d40: 726a 0000 00da 0364 6f74 da01 54da 0574  rj.....dot..T..t
+00002d50: 7261 6365 5a06 6c69 6e61 6c67 da03 696e  raceZ.linalg..in
+00002d60: 76da 0365 7965 da05 7368 6170 65da 046f  v..eye..shape..o
+00002d70: 6e65 73da 0766 6c61 7474 656e da05 7261  nes..flatten..ra
+00002d80: 6e67 65da 0661 7070 656e 6429 1172 7a00  nge..append).rz.
+00002d90: 0000 728a 0000 0072 6100 0000 7286 0000  ..r....ra...r...
+00002da0: 005a 0872 6574 6f72 6e6f 735a 126d 6174  .Z.retornosZ.mat
+00002db0: 7269 7a5f 636f 7661 7269 616e 6369 615a  riz_covarianciaZ
+00002dc0: 0570 6573 6f73 da10 7265 746f 726e 6f5f  .pesos..retorno_
+00002dd0: 6573 7065 7261 646f da05 7269 7363 6f5a  esperado..riscoZ
+00002de0: 076c 616d 6264 615f 5a07 636f 765f 696e  .lambda_Z.cov_in
+00002df0: 765a 0976 6574 6f72 5f75 6e73 5a0b 775f  vZ.vetor_unsZ.w_
+00002e00: 6d61 726b 6f77 6974 7a5a 0d6d 6172 6b6f  markowitzZ.marko
+00002e10: 7769 747a 4c69 7374 da01 695a 0574 6178  witzList..iZ.tax
+00002e20: 6173 7234 0000 0072 1f00 0000 721f 0000  asr4...r....r...
+00002e30: 0072 2000 0000 da14 6d61 726b 6f77 6974  .r .....markowit
+00002e40: 7a5f 616c 6c6f 6361 7469 6f6e f601 0000  z_allocation....
+00002e50: 7328 0000 0000 1614 030c 0308 031c 0316  s(..............
+00002e60: 0326 030e 0120 0112 0122 0108 0304 0110  .&... ..."......
+00002e70: 0120 010c 0102 0102 0102 fe06 0672 9d00  . ...........r..
+00002e80: 0000 7a23 7374 6f63 6b73 2f7b 7379 6d62  ..z#stocks/{symb
+00002e90: 6f6c 7d2f 4d61 726b 6f77 6974 7a41 6c6c  ol}/MarkowitzAll
+00002ea0: 6f63 6174 696f 6e7a 0a2f 696e 666f 4675  ocationz./infoFu
+00002eb0: 6e64 7363 0100 0000 0000 0000 0000 0000  ndsc............
+00002ec0: 0700 0000 0400 0000 4300 0000 7372 0000  ........C...sr..
+00002ed0: 0064 017d 0174 00a0 017c 01a1 017d 0274  .d.}.t...|...}.t
+00002ee0: 027c 026a 0364 0283 027d 037c 03a0 0464  .|.j.d...}.|...d
+00002ef0: 03a1 0164 0419 007d 0474 05a0 0674 077c  ...d...}.t...t.|
+00002f00: 0483 01a1 0164 0419 007d 057c 0564 0519  .....d...}.|.d..
+00002f10: 00a0 0864 0664 0784 00a1 017c 0564 053c  ...d.d.....|.d.<
+00002f20: 007c 056a 097c 0564 0519 007c 006b 0219  .|.j.|.d...|.k..
+00002f30: 007d 067c 0667 0064 08a2 0119 007d 067c  .}.|.g.d.....}.|
+00002f40: 0653 0029 0975 ca00 0000 0a20 2020 2023  .S.).u.....    #
+00002f50: 2320 5573 6162 696c 6964 6164 650a 2020  # Usabilidade.  
+00002f60: 2020 2d20 4675 6ec3 a761 6f20 7574 696c    - Fun..ao util
+00002f70: 697a 6164 6120 7061 7261 2061 6471 7569  izada para adqui
+00002f80: 7269 7220 6173 2070 7269 6e63 6970 6169  rir as principai
+00002f90: 7320 6361 7261 6374 6572 6973 7469 6361  s caracteristica
+00002fa0: 7320 6520 696e 666f 726d 61c3 a7c3 b565  s e informa....e
+00002fb0: 7320 646f 2066 756e 646f 2073 656c 6563  s do fundo selec
+00002fc0: 696f 6e61 646f 0a0a 2020 2020 2323 2050  ionado..    ## P
+00002fd0: 6172 c3a2 6d65 7472 6f73 0a0a 2020 2020  ar..metros..    
+00002fe0: 2d20 7379 6d62 6f6c 202d 3e20 4e6f 6d65  - symbol -> Nome
+00002ff0: 2064 6f20 4675 6e64 6f20 7061 7261 2066   do Fundo para f
+00003000: 617a 6572 2061 2062 7573 6361 200a 0a0a  azer a busca ...
+00003010: 2020 2020 fa28 6874 7470 733a 2f2f 7777      .(https://ww
+00003020: 772e 6675 6e64 7365 7870 6c6f 7265 722e  w.fundsexplorer.
+00003030: 636f 6d2e 6272 2f72 616e 6b69 6e67 fa0b  com.br/ranking..
+00003040: 6874 6d6c 2e70 6172 7365 72da 0574 6162  html.parser..tab
+00003050: 6c65 7201 0000 00f5 1000 0000 43c3 b364  ler.........C..d
+00003060: 6967 6f20 646f 2066 756e 646f 6301 0000  igo do fundoc...
+00003070: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003080: 0053 0000 0073 0800 0000 7c00 6401 1700  .S...s....|.d...
+00003090: 5300 a902 4e7a 032e 5341 721f 0000 00a9  S...Nz..SAr.....
+000030a0: 01da 0178 721f 0000 0072 1f00 0000 7220  ...xr....r....r 
+000030b0: 0000 00da 083c 6c61 6d62 6461 3e4a 0200  .....<lambda>J..
+000030c0: 00f3 0000 0000 7a1b 6765 745f 6675 6e64  ......z.get_fund
+000030d0: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
+000030e0: 6461 3ea9 0672 a100 0000 da05 5365 746f  da>..r......Seto
+000030f0: 72f5 0c00 0000 5072 65c3 a76f 2041 7475  r.....Pre..o Atu
+00003100: 616c da09 4469 7669 6465 6e64 6ff5 1100  al..Dividendo...
+00003110: 0000 5661 7269 61c3 a7c3 a36f 2050 7265  ..Varia....o Pre
+00003120: c3a7 6ff5 1000 0000 5265 6e74 6162 2e20  ..o.....Rentab. 
+00003130: 5065 72c3 ad6f 646f 290a da08 7265 7175  Per..odo)...requ
+00003140: 6573 7473 da03 6765 7472 0900 0000 da07  ests..getr......
+00003150: 636f 6e74 656e 74da 0866 696e 645f 616c  content..find_al
+00003160: 6c72 4300 0000 da09 7265 6164 5f68 746d  lrC.....read_htm
+00003170: 6c72 8300 0000 da05 6170 706c 79da 036c  lr......apply..l
+00003180: 6f63 2907 7222 0000 00da 0375 726c da08  oc).r".....url..
+00003190: 7265 7370 6f6e 7365 da04 736f 7570 72a0  response..soupr.
+000031a0: 0000 00da 0766 756e 6473 4446 da08 7661  .....fundsDF..va
+000031b0: 6c75 6573 4649 721f 0000 0072 1f00 0000  luesFIr....r....
+000031c0: 7220 0000 00da 0967 6574 5f66 756e 6473  r .....get_funds
+000031d0: 3802 0000 7312 0000 0000 0d04 010a 010c  8...s...........
+000031e0: 010e 0112 0116 0212 010c 0272 b900 0000  ...........r....
+000031f0: 7a12 2f63 6f6d 7061 7265 5365 746f 7246  z./compareSetorF
+00003200: 756e 6473 2902 da05 7365 746f 7272 2300  unds)...setorr#.
+00003210: 0000 6302 0000 0000 0000 0000 0000 000c  ..c.............
+00003220: 0000 0006 0000 0043 0000 0073 1e01 0000  .......C...s....
+00003230: 6401 7d02 7400 a001 7c02 a101 7d03 7402  d.}.t...|...}.t.
+00003240: 7c03 6a03 6402 8302 7d04 7c04 a004 6403  |.j.d...}.|...d.
+00003250: a101 6404 1900 7d05 7405 a006 7407 7c05  ..d...}.t...t.|.
+00003260: 8301 a101 6404 1900 7d06 7408 7c06 6405  ....d...}.t.|.d.
+00003270: 8302 0100 7c01 6406 1b00 7d01 7c06 6a09  ....|.d...}.|.j.
+00003280: 7c06 6405 1900 6406 1b00 7c01 6b04 1900  |.d...d...|.k...
+00003290: 7d07 7c07 6700 6407 a201 1900 7d07 7c07  }.|.g.d.....}.|.
+000032a0: a00a a100 7d07 7c07 6405 1900 a00b a100  ....}.|.d.......
+000032b0: 7d08 7c00 6408 6b02 72aa 6409 7d00 7c07  }.|.d.k.r.d.}.|.
+000032c0: 6a09 7c07 640a 1900 7c00 6b02 1900 6405  j.|.d...|.k...d.
+000032d0: 1900 a00b a100 7d09 6e42 7c00 640b 6b02  ......}.nB|.d.k.
+000032e0: 72d2 640c 7d00 7c07 6a09 7c07 640a 1900  r.d.}.|.j.|.d...
+000032f0: 7c00 6b02 1900 6405 1900 a00b a100 7d09  |.k...d.......}.
+00003300: 6e1a 7c07 6a09 7c07 640a 1900 7c00 6b02  n.|.j.|.d...|.k.
+00003310: 1900 6405 1900 a00b a100 7d09 7c07 6405  ..d.......}.|.d.
+00003320: 1900 a00c a100 7d0a 7405 a00d 7c08 6701  ......}.t...|.g.
+00003330: 7c09 6701 7c0a 6701 640d 9c03 a101 7d0b  |.g.|.g.d.....}.
+00003340: 7c0b a00e 640e a101 7d0b 7c0b 5300 290f  |...d...}.|.S.).
+00003350: 7506 0300 000a 2020 2020 2323 2055 7361  u.....    ## Usa
+00003360: 6269 6c69 6461 6465 0a20 2020 200a 2020  bilidade.    .  
+00003370: 2020 2d20 4675 6ec3 a761 6f20 7175 6520    - Fun..ao que 
+00003380: 7574 696c 697a 6120 6173 206d 6574 7269  utiliza as metri
+00003390: 6361 7320 6520 6d65 6469 6173 2064 6f73  cas e medias dos
+000033a0: 2066 756e 646f 2063 6f6d 2062 6173 6520   fundo com base 
+000033b0: 6e6f 2073 6575 2053 6574 6f72 2070 6172  no seu Setor par
+000033c0: 6120 756d 6120 616e 616c 6973 6520 6d61  a uma analise ma
+000033d0: 6973 2072 6573 7472 6974 610a 2020 2020  is restrita.    
+000033e0: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
+000033f0: 726f 730a 2020 2020 0a20 2020 202d 2072  ros.    .    - r
+00003400: 656e 7461 6269 6c69 6461 6465 5f6d 696e  entabilidade_min
+00003410: 202d 3e20 5661 6c6f 7220 656d 2025 2070   -> Valor em % p
+00003420: 6172 6120 6275 7363 6172 2061 2072 656e  ara buscar a ren
+00003430: 7461 6269 6c69 6461 6465 206d 696e 696d  tabilidade minim
+00003440: 6120 646f 2066 756e 646f 2065 7363 6f6c  a do fundo escol
+00003450: 6869 646f 0a20 2020 202d 2073 6574 6f72  hido.    - setor
+00003460: 202d 3e20 5365 746f 7265 7320 6465 2066   -> Setores de f
+00003470: 756e 646f 7320 7175 6520 706f 6465 7261  undos que podera
+00003480: 6d20 7365 7220 6573 636f 6c68 6964 6f73  m ser escolhidos
+00003490: 2c20 7365 6775 6520 6120 6c69 7374 613a  , segue a lista:
+000034a0: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
+000034b0: 2020 5469 706f 7353 6574 6f72 6573 3a0a    TiposSetores:.
+000034c0: 2020 2020 2d20 436f 7270 6f72 6174 6976      - Corporativ
+000034d0: 6173 203d 2022 4c61 6a65 7320 436f 7270  as = "Lajes Corp
+000034e0: 6f72 6174 6976 6173 2220 0a20 2020 202d  orativas" .    -
+000034f0: 204d 6f62 696c 6961 7269 6f73 203d 2022   Mobiliarios = "
+00003500: 54c3 ad74 756c 6f73 2065 2056 616c 2e20  T..tulos e Val. 
+00003510: 4d6f 622e 220a 2020 2020 2d20 5368 6f70  Mob.".    - Shop
+00003520: 7069 6e67 7320 3d20 2253 686f 7070 696e  pings = "Shoppin
+00003530: 6773 220a 2020 2020 2d20 48c3 ad62 7269  gs".    - H..bri
+00003540: 646f 203d 2027 48c3 ad62 7269 646f 270a  do = 'H..brido'.
+00003550: 2020 2020 2d20 5265 6e64 6120 3d20 2752      - Renda = 'R
+00003560: 656e 6461 270a 2020 2020 2d20 4c6f 67c3  enda'.    - Log.
+00003570: ad73 7469 6361 203d 2027 4c6f 67c3 ad73  .stica = 'Log..s
+00003580: 7469 6361 270a 2020 2020 2d20 486f 7370  tica'.    - Hosp
+00003590: 6974 616c 203d 2027 486f 7370 6974 616c  ital = 'Hospital
+000035a0: 270a 2020 2020 2d20 5265 7369 6465 6e63  '.    - Residenc
+000035b0: 6961 6c20 3d20 2752 6573 6964 656e 6369  ial = 'Residenci
+000035c0: 616c 270a 2020 2020 2d20 4f75 7472 6f73  al'.    - Outros
+000035d0: 203d 2027 4f75 7472 6f73 270a 0a20 2020   = 'Outros'..   
+000035e0: 2060 6060 0a20 2020 2023 2320 4578 656d   ```.    ## Exem
+000035f0: 706c 6f3a 0a20 2020 200a 2020 2020 6060  plo:.    .    ``
+00003600: 600a 2020 2020 3e3e 3e20 6262 2e63 6f6d  `.    >>> bb.com
+00003610: 7061 7265 5f73 6574 6f72 5f66 756e 6473  pare_setor_funds
+00003620: 2873 6574 6f72 3d27 436f 7270 6f72 6174  (setor='Corporat
+00003630: 6976 6173 272c 2072 656e 7461 6269 6c69  ivas', rentabili
+00003640: 6461 6465 5f6d 696e 203d 2033 290a 2020  dade_min = 3).  
+00003650: 2020 6060 600a 0a20 2020 2072 9e00 0000    ```..    r....
+00003660: 729f 0000 0072 a000 0000 7201 0000 0072  r....r....r....r
+00003670: ac00 0000 7253 0000 0072 a700 0000 5a0c  ....rS...r....Z.
+00003680: 436f 7270 6f72 6174 6976 6173 7a12 4c61  Corporativasz.La
+00003690: 6a65 7320 436f 7270 6f72 6174 6976 6173  jes Corporativas
+000036a0: 72a8 0000 005a 0b4d 6f62 696c 6961 7269  r....Z.Mobiliari
+000036b0: 6f73 7514 0000 0054 c3ad 7475 6c6f 7320  osu....T..tulos 
+000036c0: 6520 5661 6c2e 204d 6f62 2e29 0375 2a00  e Val. Mob.).u*.
+000036d0: 0000 5265 6e74 6162 696c 6964 6164 6520  ..Rentabilidade 
+000036e0: 4dc3 a964 6961 2064 6f73 2046 4949 7320  M..dia dos FIIs 
+000036f0: 5365 6c65 6369 6f6e 6164 6f73 751f 0000  Selecionadosu...
+00003700: 0052 656e 7461 6269 6c69 6461 6465 204d  .Rentabilidade M
+00003710: c3a9 6469 6120 646f 204d 6572 6361 646f  ..dia do Mercado
+00003720: 7537 0000 0044 6573 7669 6f20 5061 6472  u7...Desvio Padr
+00003730: c3a3 6f20 6461 7320 5265 6e74 6162 696c  ..o das Rentabil
+00003740: 6964 6164 6573 2064 6f73 2046 4949 7320  idades dos FIIs 
+00003750: 5365 6c65 6369 6f6e 6164 6f73 7a20 4f20  Selecionadosz O 
+00003760: 7365 746f 722f 7661 6c6f 7220 6e61 6f20  setor/valor nao 
+00003770: 666f 6920 656e 636f 6e74 7261 646f 290f  foi encontrado).
+00003780: 72ad 0000 0072 ae00 0000 7209 0000 0072  r....r....r....r
+00003790: af00 0000 72b0 0000 0072 4300 0000 72b1  ....r....rC...r.
+000037a0: 0000 0072 8300 0000 7221 0000 0072 b300  ...r....r!...r..
+000037b0: 0000 728e 0000 0072 5900 0000 7276 0000  ..r....rY...rv..
+000037c0: 0072 4400 0000 5a06 6669 6c6c 6e61 290c  .rD...Z.fillna).
+000037d0: 72ba 0000 005a 1172 656e 7461 6269 6c69  r....Z.rentabili
+000037e0: 6461 6465 5f6d 696e 72b4 0000 0072 b500  dade_minr....r..
+000037f0: 0000 72b6 0000 0072 a000 0000 72b7 0000  ..r....r....r...
+00003800: 0072 b800 0000 5a13 7265 6e74 6162 696c  .r....Z.rentabil
+00003810: 6964 6164 655f 6d65 6469 615a 1572 656e  idade_mediaZ.ren
+00003820: 7461 6269 6c69 6461 6465 5f6d 6572 6361  tabilidade_merca
+00003830: 646f da0d 6465 7376 696f 5f70 6164 7261  do..desvio_padra
+00003840: 6f5a 0a72 6573 756c 7461 646f 7372 1f00  oZ.resultadosr..
+00003850: 0000 721f 0000 0072 2000 0000 da13 636f  ..r....r .....co
+00003860: 6d70 6172 655f 7365 746f 725f 6675 6e64  mpare_setor_fund
+00003870: 7358 0200 0073 3400 0000 0022 0401 0a01  sX...s4...."....
+00003880: 0c01 0e01 1202 0a01 0801 1601 0c01 0801  ................
+00003890: 0c01 0801 0401 1c01 0801 0401 1c02 1a02  ................
+000038a0: 0c02 0401 0401 0401 04fd 0806 0a02 72bc  ..............r.
+000038b0: 0000 007a 0d2f 636f 6d70 6172 6546 756e  ...z./compareFun
+000038c0: 6473 2901 7223 0000 0063 0300 0000 0000  ds).r#...c......
+000038d0: 0000 0000 0000 1200 0000 0400 0000 4300  ..............C.
+000038e0: 0000 734a 0100 007c 0172 bc7c 0264 016b  ..sJ...|.r.|.d.k
+000038f0: 0372 bc64 027d 0374 00a0 017c 03a1 017d  .r.d.}.t...|...}
+00003900: 0474 027c 046a 0364 0383 027d 057c 05a0  .t.|.j.d...}.|..
+00003910: 0464 04a1 0164 0519 007d 0674 05a0 0674  .d...d...}.t...t
+00003920: 077c 0683 01a1 0164 0519 007d 077c 0764  .|.....d...}.|.d
+00003930: 0619 00a0 0864 0764 0884 00a1 017c 0764  .....d.d.....|.d
+00003940: 063c 007c 0767 0064 09a2 0119 007d 077c  .<.|.g.d.....}.|
+00003950: 076a 0964 0667 0164 0a8d 017d 077c 076a  .j.d.g.d...}.|.j
+00003960: 0a7c 0764 0619 007c 016b 0219 007d 087c  .|.d...|.k...}.|
+00003970: 076a 0a7c 0764 0619 007c 026b 0219 007d  .j.|.d...|.k...}
+00003980: 0974 05a0 0b7c 087c 0967 02a1 017d 0a7c  .t...|.|.g...}.|
+00003990: 0a6a 0c72 b874 0d64 0b83 0101 006e 047c  .j.r.t.d.....n.|
+000039a0: 0a53 007c 0064 0175 0072 ca67 007d 006e  .S.|.d.u.r.g.}.n
+000039b0: 7c64 0c7d 0b64 0d7d 0c7c 0044 005d 3a7d  |d.}.d.}.|.D.]:}
+000039c0: 0d74 0ea0 0f7c 0da1 017d 0e7c 0e6a 1064  .t...|...}.|.j.d
+000039d0: 0e64 0f8d 017d 0f7c 0f64 1019 00a0 11a1  .d...}.|.d......
+000039e0: 00a0 12a1 007d 107c 107c 0b6b 0472 d67c  .....}.|.|.k.r.|
+000039f0: 107d 0b7c 0d7d 0c71 d674 056a 137c 0c7c  .}.|.}.q.t.j.|.|
+00003a00: 0b64 1114 0064 129c 0274 147c 0083 0167  .d...d...t.|...g
+00003a10: 0164 138d 027d 117c 116a 0c90 0172 4274  .d...}.|.j...rBt
+00003a20: 0d64 1483 0101 006e 047c 1153 0064 0153  .d.....n.|.S.d.S
+00003a30: 0029 1575 2403 0000 0a20 2020 2023 2320  .).u$....    ## 
+00003a40: 5573 6162 696c 6964 6164 650a 2020 2020  Usabilidade.    
+00003a50: 0a20 2020 202d 2046 756e c3a7 616f 2071  .    - Fun..ao q
+00003a60: 7565 2072 6561 6c69 7a61 2061 2063 6f6d  ue realiza a com
+00003a70: 7061 7261 c3a7 616f 2065 6e74 7265 2064  para..ao entre d
+00003a80: 6f69 7320 6675 6e64 6f73 2c20 7365 6a61  ois fundos, seja
+00003a90: 2066 6569 7461 2061 2072 6571 7569 7369   feita a requisi
+00003aa0: c3a7 616f 2064 6f73 2066 756e 646f 7320  ..ao dos fundos 
+00003ab0: 7669 6120 6c69 7374 6120 6f75 2075 6e69  via lista ou uni
+00003ac0: 636f 7320 0a20 2020 202d 2052 6571 7569  cos .    - Requi
+00003ad0: 7369 c3a7 616f 204c 6973 7461 733a 2052  si..ao Listas: R
+00003ae0: 6574 6f72 6e61 206f 2066 756e 646f 2063  etorna o fundo c
+00003af0: 6f6d 206d 6169 6f72 2070 6f72 6365 6e74  om maior porcent
+00003b00: 6167 656d 2064 6520 7269 7363 6f20 2861  agem de risco (a
+00003b10: 2076 6172 6961 c3a7 c3a3 6f20 7065 7263   varia....o perc
+00003b20: 656e 7475 616c 2064 6f73 2070 7265 c3a7  entual dos pre..
+00003b30: 6f73 2064 6f73 2061 7469 766f 732c 2063  os dos ativos, c
+00003b40: 616c 6375 6c6f 2072 6561 6c69 7a61 646f  alculo realizado
+00003b50: 2063 6f6d 2062 6173 6520 6e6f 2064 6573   com base no des
+00003b60: 7669 6f20 7061 6472 c3a3 6f29 0a20 2020  vio padr..o).   
+00003b70: 202d 2052 6571 7569 7369 c3a7 616f 2055   - Requisi..ao U
+00003b80: 6e69 6361 3a20 5265 746f 726e 6120 756d  nica: Retorna um
+00003b90: 2044 6174 6166 7261 6d65 2063 6f6d 2061   Dataframe com a
+00003ba0: 7320 7072 696e 6369 7061 6973 2069 6e66  s principais inf
+00003bb0: 6f72 6d61 c3a7 6f65 7320 646f 7320 6675  orma..oes dos fu
+00003bc0: 6e64 6f73 2c20 6166 696d 2064 6520 756d  ndos, afim de um
+00003bd0: 6120 636f 6d70 6172 61c3 a761 6f20 656e  a compara..ao en
+00003be0: 7472 6520 7365 7573 2076 616c 6f72 6573  tre seus valores
+00003bf0: 200a 0a20 2020 200a 2020 2020 2323 2050   ..    .    ## P
+00003c00: 6172 c3a2 6d65 7472 6f73 0a20 2020 200a  ar..metros.    .
+00003c10: 2020 2020 2d20 6c69 7374 6675 6e64 202d      - listfund -
+00003c20: 3e20 4c69 7374 6120 646f 7320 6675 6e64  > Lista dos fund
+00003c30: 6f73 2070 6172 6120 616e 616c 6973 6520  os para analise 
+00003c40: 6465 2072 6973 636f 0a20 2020 202d 2066  de risco.    - f
+00003c50: 756e 645f 3120 2d3e 2050 7269 6d65 6972  und_1 -> Primeir
+00003c60: 6f20 6675 6e64 6f20 7061 7261 2061 6e61  o fundo para ana
+00003c70: 6c69 7365 2075 6e69 6361 0a20 2020 202d  lise unica.    -
+00003c80: 2066 756e 645f 3220 2d3e 2053 6567 756e   fund_2 -> Segun
+00003c90: 646f 2066 756e 646f 2070 6172 6120 616e  do fundo para an
+00003ca0: 616c 6973 6520 756e 6963 610a 2020 2020  alise unica.    
+00003cb0: 0a20 2020 2023 2320 4578 656d 706c 6f73  .    ## Exemplos
+00003cc0: 3a0a 2020 2020 0a20 2020 2060 6060 0a20  :.    .    ```. 
+00003cd0: 2020 203e 3e3e 2062 622e 636f 6d70 6172     >>> bb.compar
+00003ce0: 655f 6675 6e64 7328 6c69 7374 6675 6e64  e_funds(listfund
+00003cf0: 3d20 6c69 7374 2920 0a20 2020 2020 2020  = list) .       
+00003d00: 2020 2020 2020 2020 2020 2020 206f 750a               ou.
+00003d10: 2020 2020 3e3e 3e20 6262 2e63 6f6d 7061      >>> bb.compa
+00003d20: 7265 5f66 756e 6473 2866 756e 645f 313d  re_funds(fund_1=
+00003d30: 2027 6675 6e64 3127 2c20 6675 6e64 5f32   'fund1', fund_2
+00003d40: 3d20 2766 756e 6432 2729 0a20 2020 2060  = 'fund2').    `
+00003d50: 6060 0a20 2020 200a 2020 2020 4e72 9e00  ``.    .    Nr..
+00003d60: 0000 729f 0000 0072 a000 0000 7201 0000  ..r....r....r...
+00003d70: 0072 a100 0000 6301 0000 0000 0000 0000  .r....c.........
+00003d80: 0000 0001 0000 0002 0000 0053 0000 0073  ...........S...s
+00003d90: 0800 0000 7c00 6401 1700 5300 72a2 0000  ....|.d...S.r...
+00003da0: 0072 1f00 0000 72a3 0000 0072 1f00 0000  .r....r....r....
+00003db0: 721f 0000 0072 2000 0000 72a5 0000 00c1  r....r ...r.....
+00003dc0: 0200 0072 a600 0000 7a1f 636f 6d70 6172  ...r....z.compar
+00003dd0: 655f 6675 6e64 732e 3c6c 6f63 616c 733e  e_funds.<locals>
+00003de0: 2e3c 6c61 6d62 6461 3e29 0872 a100 0000  .<lambda>).r....
+00003df0: 72a8 0000 0072 a900 0000 72aa 0000 0072  r....r....r....r
+00003e00: ab00 0000 72ac 0000 007a 0e44 6976 6964  ....r....z.Divid
+00003e10: 656e 6420 5969 656c 647a 1144 5920 2833  end Yieldz.DY (3
+00003e20: 4d29 2041 6375 6d75 6c61 646f 2901 5a06  M) Acumulado).Z.
+00003e30: 7375 6273 6574 753e 0000 004e 616f 2066  subsetu>...Nao f
+00003e40: 6f72 616d 2061 7072 6573 656e 7461 646f  oram apresentado
+00003e50: 2064 6164 6f73 2064 6f73 2066 756e 646f   dados dos fundo
+00003e60: 7320 7061 7261 2076 6572 6966 6963 61c3  s para verifica.
+00003e70: a761 6f20 756e 6963 6172 2600 0000 7218  .ao unicar&...r.
+00003e80: 0000 0072 4e00 0000 723c 0000 0072 4800  ...rN...r<...rH.
+00003e90: 0000 7253 0000 0029 025a 0446 756e 647a  ..rS...).Z.Fundz
+00003ea0: 0c4d 6178 2072 6973 6b20 2825 2972 8000  .Max risk (%)r..
+00003eb0: 0000 7542 0000 004e 616f 2066 6f72 616d  ..uB...Nao foram
+00003ec0: 2061 7072 6573 656e 7461 646f 2064 6164   apresentado dad
+00003ed0: 6f73 2064 6f73 2066 756e 646f 7320 7061  os dos fundos pa
+00003ee0: 7261 2076 6572 6966 6963 61c3 a761 6f20  ra verifica..ao 
+00003ef0: 6dc3 ba6c 7469 706c 6129 1572 ad00 0000  m..ltipla).r....
+00003f00: 72ae 0000 0072 0900 0000 72af 0000 0072  r....r....r....r
+00003f10: b000 0000 7243 0000 0072 b100 0000 7283  ....rC...r....r.
+00003f20: 0000 0072 b200 0000 da0f 6472 6f70 5f64  ...r......drop_d
+00003f30: 7570 6c69 6361 7465 7372 b300 0000 7285  uplicatesr....r.
+00003f40: 0000 0072 4100 0000 722f 0000 0072 2a00  ...rA...r/...r*.
+00003f50: 0000 722b 0000 0072 4000 0000 726f 0000  ..r+...r@...ro..
+00003f60: 0072 7600 0000 7244 0000 0072 8400 0000  .rv...rD...r....
+00003f70: 2912 5a08 6c69 7374 6675 6e64 5a06 6675  ).Z.listfundZ.fu
+00003f80: 6e64 5f31 5a06 6675 6e64 5f32 72b4 0000  nd_1Z.fund_2r...
+00003f90: 0072 b500 0000 72b6 0000 0072 a000 0000  .r....r....r....
+00003fa0: 72b7 0000 005a 0566 756e 6431 5a05 6675  r....Z.fund1Z.fu
+00003fb0: 6e64 32da 0475 6e69 745a 096d 6178 5f72  nd2..unitZ.max_r
+00003fc0: 6973 636f 5a10 7469 636b 6572 5f6d 6178  iscoZ.ticker_max
+00003fd0: 5f72 6973 636f 727b 0000 005a 0566 756e  _riscor{...Z.fun
+00003fe0: 646f 721e 0000 0072 bb00 0000 5a09 7661  dor....r....Z.va
+00003ff0: 6c75 6572 6973 6b72 1f00 0000 721f 0000  lueriskr....r...
+00004000: 0072 2000 0000 da0d 636f 6d70 6172 655f  .r .....compare_
+00004010: 6675 6e64 73a2 0200 0073 4400 0000 0019  funds....sD.....
+00004020: 0c01 0401 0a01 0c01 0e01 1201 1601 0c01  ................
+00004030: 0e02 1201 1202 0e01 0601 0a02 0402 0801  ................
+00004040: 0602 0401 0401 0801 0a01 0c01 1001 0801  ................
+00004050: 0401 0602 0601 06ff 0401 08ff 0603 0801  ................
+00004060: 0a02 72bf 0000 007a 0b2f 6265 7374 4173  ..r....z./bestAs
+00004070: 7365 7473 6301 0000 0000 0000 0000 0000  setsc...........
+00004080: 0019 0000 0005 0000 0043 0000 0073 fa02  .........C...s..
+00004090: 0000 6401 7d01 7400 a001 7c01 a101 7d02  ..d.}.t...|...}.
+000040a0: 7c02 6a02 6402 6b03 7224 7403 6403 8301  |.j.d.k.r$t.d...
+000040b0: 0100 9002 6ed2 7404 7c02 6a05 6404 8302  ....n.t.|.j.d...
+000040c0: 7d03 7c03 a006 6405 a101 6406 1900 7d04  }.|...d...d...}.
+000040d0: 7407 6a08 7409 7c04 8301 6407 6408 6409  t.j.t.|...d.d.d.
+000040e0: 8d03 6406 1900 7d05 7c05 640a 1900 a00a  ..d...}.|.d.....
+000040f0: 640b 640c 8400 a101 7c05 640a 3c00 7403  d.d.....|.d.<.t.
+00004100: 640d 8301 0100 740b 6a0c 7c05 640a 1900  d.....t.j.|.d...
+00004110: a00d a100 640e 640f 8d02 6410 1900 7d06  ....d.d...d...}.
+00004120: 6411 6412 8400 7d07 6413 6414 8400 7d08  d.d...}.d.d...}.
+00004130: 6900 7d09 6900 7d0a 7c06 6a0e 4400 5d24  i.}.i.}.|.j.D.]$
+00004140: 7d0b 7c06 7c0b 1900 7d0c 7c07 7c0c 8301  }.|.|...}.|.|...
+00004150: 7c09 7c0b 3c00 7c08 7c0c 8301 7c0a 7c0b  |.|.<.|.|...|.|.
+00004160: 3c00 71ac 7c00 6415 6b02 9001 7288 6700  <.q.|.d.k...r.g.
+00004170: 7d0d 7c06 6a0e 4400 5d26 7d0b 7c09 7c0b  }.|.j.D.]&}.|.|.
+00004180: 1900 6416 6b04 72e6 7c0a 7c0b 1900 6417  ..d.k.r.|.|...d.
+00004190: 6b04 72e6 7c0d a00f 7c0b a101 0100 71e6  k.r.|...|.....q.
+000041a0: 7407 6a10 7c0d 6418 6701 6419 8d02 7d0e  t.j.|.d.g.d...}.
+000041b0: 7403 641a 8301 0100 7411 7c0d 7412 7413  t.d.....t.|.t.t.
+000041c0: 641b 8d03 7d0f 7c0f 6701 7d0f 7407 a010  d...}.|.g.}.t...
+000041d0: 7c0f a101 7d10 7c10 a014 641c a101 7d10  |...}.|...d...}.
+000041e0: 7c10 641d 1900 a015 a100 a016 a100 7c10  |.d...........|.
+000041f0: 641d 3c00 7c10 641e 1900 a015 a100 a016  d.<.|.d.........
+00004200: a100 7c10 641e 3c00 7c10 6a17 9001 7280  ..|.d.<.|.j...r.
+00004210: 6e04 7c10 5300 9001 6e6e 7c00 641f 6b02  n.|.S...nn|.d.k.
+00004220: 9002 7242 6700 7d11 7c06 6a0e 4400 5d2c  ..rBg.}.|.j.D.],
+00004230: 7d0b 7c09 7c0b 1900 6420 6b04 9001 729c  }.|.|...d k...r.
+00004240: 7c0a 7c0b 1900 6421 6b00 9001 729c 7c11  |.|...d!k...r.|.
+00004250: a00f 7c0b a101 0100 9001 719c 7407 6a10  ..|.......q.t.j.
+00004260: 7c11 6422 6701 6419 8d02 7d12 7403 641a  |.d"g.d...}.t.d.
+00004270: 8301 0100 7411 7c11 7412 7413 641b 8d03  ....t.|.t.t.d...
+00004280: 7d13 7c13 6701 7d13 7407 a010 7c13 a101  }.|.g.}.t...|...
+00004290: 7d14 7c14 a014 641c a101 7d14 7c14 641d  }.|...d...}.|.d.
+000042a0: 1900 a015 a100 a016 a100 7c14 641d 3c00  ..........|.d.<.
+000042b0: 7c14 641e 1900 a015 a100 a016 a100 7c14  |.d...........|.
+000042c0: 641e 3c00 7c14 6a17 9002 723c 6e04 7c14  d.<.|.j...r<n.|.
+000042d0: 5300 6eb4 7c00 6423 6b02 9002 72ee 6700  S.n.|.d#k...r.g.
+000042e0: 7d15 7c06 6a0e 4400 5d1e 7d0b 7c0a 7c0b  }.|.j.D.].}.|.|.
+000042f0: 1900 6417 6b00 9002 7256 7c15 a00f 7c0b  ..d.k...rV|...|.
+00004300: a101 0100 9002 7156 7407 6a10 7c15 6424  ......qVt.j.|.d$
+00004310: 6701 6419 8d02 7d16 7403 641a 8301 0100  g.d...}.t.d.....
+00004320: 7411 7c15 7412 7413 641b 8d03 7d17 7c17  t.|.t.t.d...}.|.
+00004330: 6701 7d17 7407 a010 7c17 a101 7d18 7c18  g.}.t...|...}.|.
+00004340: a014 641c a101 7d18 7c18 641d 1900 a015  ..d...}.|.d.....
+00004350: a100 a016 a100 7c18 641d 3c00 7c18 641e  ......|.d.<.|.d.
+00004360: 1900 a015 a100 a016 a100 7c18 641e 3c00  ..........|.d.<.
+00004370: 7c18 6a17 9002 72e8 6e04 7c18 5300 6e08  |.j...r.n.|.S.n.
+00004380: 7403 6425 8301 0100 6426 5300 2927 750c  t.d%....d&S.)'u.
+00004390: 0200 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
+000043a0: 6c69 6461 6465 0a20 2020 202d 2046 756e  lidade.    - Fun
+000043b0: c3a7 c3a3 6f20 7175 6520 616e 616c 6973  ....o que analis
+000043c0: 6120 6f73 2070 7269 6e63 6970 6169 7320  a os principais 
+000043d0: 6174 6976 6f73 206c 6973 7461 646f 7320  ativos listados 
+000043e0: 6e6f 206d 6572 6361 646f 2071 7565 2063  no mercado que c
+000043f0: 6f6d 2062 6173 6520 6e6f 2070 6572 6669  om base no perfi
+00004400: 6c20 6573 636f 6c68 6964 6f20 6d6f 7374  l escolhido most
+00004410: 7261 2071 7561 6973 2070 6f64 656d 2073  ra quais podem s
+00004420: 6572 2073 7561 7320 6573 636f 6c68 6173  er suas escolhas
+00004430: 2065 2071 7561 6e74 6f73 2070 6f72 6365   e quantos porce
+00004440: 6e74 6f20 7365 2064 6576 6520 7465 7220  nto se deve ter 
+00004450: 6e61 2063 6172 7465 6972 610a 2020 2020  na carteira.    
+00004460: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
+00004470: 726f 730a 2020 2020 0a20 2020 202d 2070  ros.    .    - p
+00004480: 6572 6669 6c20 2d3e 2050 6572 6669 7320  erfil -> Perfis 
+00004490: 7175 6520 706f 6465 6d20 7365 7220 6573  que podem ser es
+000044a0: 636f 6c68 6964 6f73 2070 6172 6120 7265  colhidos para re
+000044b0: 616c 697a 6172 2061 2061 6ec3 a16c 6973  alizar a an..lis
+000044c0: 652c 2073 6567 7565 2061 206c 6973 7461  e, segue a lista
+000044d0: 3a20 0a0a 2020 2020 0a20 2020 2060 6060  : ..    .    ```
+000044e0: 0a20 2020 2054 6970 6f50 6572 6669 733a  .    TipoPerfis:
+000044f0: 0a20 2020 202a 2041 6772 6573 7369 766f  .    * Agressivo
+00004500: 0a20 2020 202a 204d 6f64 6572 6164 6f0a  .    * Moderado.
+00004510: 2020 2020 2a20 436f 6e73 6572 7661 646f      * Conservado
+00004520: 720a 2020 2020 0a20 2020 2060 6060 0a20  r.    .    ```. 
+00004530: 2020 200a 2020 2020 2323 2045 7865 6d70     .    ## Exemp
+00004540: 6c6f 0a20 2020 200a 2020 2020 6060 600a  lo.    .    ```.
+00004550: 2020 2020 0a20 2020 203e 3e3e 2061 6c6f      .    >>> alo
+00004560: 6361 7469 6f6e 203d 2062 6573 745f 6173  cation = best_as
+00004570: 7365 7473 2870 6572 6669 6c3d 2741 6772  sets(perfil='Agr
+00004580: 6573 7369 766f 2729 0a20 2020 200a 2020  essivo').    .  
+00004590: 2020 6060 600a 2020 2020 0a20 2020 207a    ```.    .    z
+000045a0: 2d68 7474 7073 3a2f 2f77 7777 2e64 6164  -https://www.dad
+000045b0: 6f73 6465 6d65 7263 6164 6f2e 636f 6d2e  osdemercado.com.
+000045c0: 6272 2f62 6f6c 7361 2f61 636f 6573 7251  br/bolsa/acoesrQ
+000045d0: 0000 007a 3141 6365 7373 6f20 6e65 6761  ...z1Acesso nega
+000045e0: 646f 2061 2062 6173 652c 2074 656e 7465  do a base, tente
+000045f0: 206e 6f76 616d 656e 7465 206d 6169 7320   novamente mais 
+00004600: 7461 7264 652e 729f 0000 0072 a000 0000  tarde.r....r....
+00004610: 7201 0000 00fa 012c 721a 0000 0029 02da  r......,r....)..
+00004620: 0764 6563 696d 616c 5a09 7468 6f75 7361  .decimalZ.thousa
+00004630: 6e64 73f5 0700 0000 43c3 b364 6967 6f63  nds.....C..digoc
+00004640: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004650: 0200 0000 5300 0000 7308 0000 007c 0064  ....S...s....|.d
+00004660: 0117 0053 0072 a200 0000 721f 0000 0072  ...S.r....r....r
+00004670: a300 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+00004680: 0000 0072 a500 0000 1003 0000 72a6 0000  ...r........r...
+00004690: 007a 1d62 6573 745f 6173 7365 7473 2e3c  .z.best_assets.<
+000046a0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000046b0: 7a13 4275 7363 616e 646f 2061 7469 766f  z.Buscando ativo
+000046c0: 732e 2e2e 2e72 3a00 0000 723c 0000 0072  s....r:...r<...r
+000046d0: 4800 0000 6301 0000 0000 0000 0000 0000  H...c...........
+000046e0: 0003 0000 0002 0000 0053 0000 0073 1400  .........S...s..
+000046f0: 0000 7c00 a000 a100 7d01 7c01 a001 a100  ..|.....}.|.....
+00004700: 7d02 7c02 5300 a901 4e29 0272 6f00 0000  }.|.S...N).ro...
+00004710: 7259 0000 0029 03da 0670 7265 636f 73da  rY...)...precos.
+00004720: 0772 6574 6f72 6e6f 5a0d 7265 746f 726e  .retornoZ.retorn
+00004730: 6f5f 6d65 6469 6f72 1f00 0000 721f 0000  o_medior....r...
+00004740: 0072 2000 0000 da10 6361 6c63 756c 6172  .r .....calcular
+00004750: 5f72 6574 6f72 6e6f 1503 0000 7306 0000  _retorno....s...
+00004760: 0000 0108 0108 017a 2562 6573 745f 6173  .......z%best_as
+00004770: 7365 7473 2e3c 6c6f 6361 6c73 3e2e 6361  sets.<locals>.ca
+00004780: 6c63 756c 6172 5f72 6574 6f72 6e6f 6301  lcular_retornoc.
+00004790: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+000047a0: 0000 0053 0000 0073 1400 0000 7c00 a000  ...S...s....|...
+000047b0: a100 7d01 7c01 a001 a100 7d02 7c02 5300  ..}.|.....}.|.S.
+000047c0: 72c3 0000 0029 0272 6f00 0000 7276 0000  r....).ro...rv..
+000047d0: 0029 0372 c400 0000 72c5 0000 0072 9b00  .).r....r....r..
+000047e0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+000047f0: 00da 0e63 616c 6375 6c61 725f 7269 7363  ...calcular_risc
+00004800: 6f1b 0300 0073 0600 0000 0001 0801 0801  o....s..........
+00004810: 7a23 6265 7374 5f61 7373 6574 732e 3c6c  z#best_assets.<l
+00004820: 6f63 616c 733e 2e63 616c 6375 6c61 725f  ocals>.calcular_
+00004830: 7269 7363 6f5a 0941 6772 6573 7369 766f  riscoZ.Agressivo
+00004840: 672d 431c ebe2 361a 3fe7 7b14 ae47 e17a  g-C...6.?.{..G.z
+00004850: 843f 7a12 4174 6976 6f73 2050 2f41 6772  .?z.Ativos P/Agr
+00004860: 6573 7369 766f a901 da07 636f 6c75 6d6e  essivo....column
+00004870: 737a 3f52 6561 6c69 7a61 6e64 6f20 6361  sz?Realizando ca
+00004880: 6c63 756c 6f73 2070 6172 6120 6120 7375  lculos para a su
+00004890: 6120 6361 7274 6569 7261 2063 6f6d 2062  a carteira com b
+000048a0: 6173 6520 6e6f 2073 6575 2070 6572 6669  ase no seu perfi
+000048b0: 6c2e 2902 728a 0000 0072 6100 0000 728d  l.).r....ra...r.
+000048c0: 0000 0072 8b00 0000 728c 0000 005a 084d  ...r....r....Z.M
+000048d0: 6f64 6572 6164 6f67 6132 5530 2aa9 333f  oderadoga2U0*.3?
+000048e0: 67b8 1e85 eb51 b89e 3f7a 1141 7469 766f  g....Q..?z.Ativo
+000048f0: 7320 502f 4d6f 6465 7261 646f 5a0b 436f  s P/ModeradoZ.Co
+00004900: 6e73 6572 7661 646f 727a 1441 7469 766f  nservadorz.Ativo
+00004910: 7320 502f 436f 6e73 6572 7661 646f 7275  s P/Conservadoru
+00004920: 5a00 0000 5065 7266 696c 206e c3a3 6f20  Z...Perfil n..o 
+00004930: 7265 636f 6e68 6563 6964 6f2c 206f 7320  reconhecido, os 
+00004940: 7065 7266 6973 2064 6973 706f 6e69 7665  perfis disponive
+00004950: 6973 2065 7374 616f 2070 7265 7365 6e74  is estao present
+00004960: 6573 206e 6120 6578 706c 6963 61c3 a7c3  es na explica...
+00004970: a36f 2064 6120 6675 6ec3 a7c3 a36f 4e29  .o da fun....oN)
+00004980: 1872 ad00 0000 72ae 0000 005a 0b73 7461  .r....r....Z.sta
+00004990: 7475 735f 636f 6465 722f 0000 0072 0900  tus_coder/...r..
+000049a0: 0000 72af 0000 0072 b000 0000 7243 0000  ..r....r....rC..
+000049b0: 0072 b100 0000 7283 0000 0072 b200 0000  .r....r....r....
+000049c0: 722a 0000 0072 6600 0000 da06 746f 6c69  r*...rf.....toli
+000049d0: 7374 72ca 0000 0072 9900 0000 7244 0000  str....r....rD..
+000049e0: 0072 9d00 0000 da04 6f6e 6559 da09 6375  .r......oneY..cu
+000049f0: 7272 656e 746c 795a 0765 7870 6c6f 6465  rrentlyZ.explode
+00004a00: 72bd 0000 0072 8e00 0000 7241 0000 0029  r....r....rA...)
+00004a10: 195a 0670 6572 6669 6c72 b400 0000 72b5  .Z.perfilr....r.
+00004a20: 0000 0072 b600 0000 72a0 0000 0072 b700  ...r....r....r..
+00004a30: 0000 72c4 0000 0072 c600 0000 72c7 0000  ..r....r....r...
+00004a40: 0072 c500 0000 729b 0000 00da 0561 7469  .r....r......ati
+00004a50: 766f 5a0c 7072 6563 6f73 5f61 7469 766f  voZ.precos_ativo
+00004a60: 5a09 6167 7265 7373 6976 6f5a 0b44 6641  Z.agressivoZ.DfA
+00004a70: 6772 6573 7369 766f 5a13 616c 6f63 6174  gressivoZ.alocat
+00004a80: 696f 6e5f 4167 7265 7373 6976 655a 1764  ion_AgressiveZ.d
+00004a90: 6174 6141 6c6f 6361 7469 6f6e 5f41 6772  ataAlocation_Agr
+00004aa0: 6573 7369 7665 5a08 6d6f 6465 7261 646f  essiveZ.moderado
+00004ab0: 5a0a 4466 4d6f 6465 7261 646f 5a12 616c  Z.DfModeradoZ.al
+00004ac0: 6f63 6174 696f 6e5f 4d6f 6465 7261 6465  ocation_Moderade
+00004ad0: 5a16 6461 7461 416c 6f63 6174 696f 6e5f  Z.dataAlocation_
+00004ae0: 4d6f 6465 7261 6465 5a0b 636f 6e73 6572  ModeradeZ.conser
+00004af0: 7661 646f 725a 0d44 6643 6f6e 7365 7276  vadorZ.DfConserv
+00004b00: 6164 6f72 5a16 616c 6f63 6174 696f 6e5f  adorZ.alocation_
+00004b10: 436f 6e73 6572 7661 7469 7665 5a1a 6461  ConservativeZ.da
+00004b20: 7461 416c 6f63 6174 696f 6e5f 436f 6e73  taAlocation_Cons
+00004b30: 6572 7661 7469 7665 721f 0000 0072 1f00  ervativer....r..
+00004b40: 0000 7220 0000 00da 0b62 6573 745f 6173  ..r .....best_as
+00004b50: 7365 7473 ea02 0000 7386 0000 0000 1e04  sets....s.......
+00004b60: 010a 010a 010c 020c 010e 0118 0116 0108  ................
+00004b70: 011a 0308 0608 0604 0104 010a 0108 010c  ................
+00004b80: 010e 030a 0104 010a 0118 010c 0210 0108  ................
+00004b90: 010e 0106 010a 010a 0414 0114 0208 0102  ................
+00004ba0: 0208 020a 0204 010a 011c 010e 0210 0108  ................
+00004bb0: 010e 0106 010a 010a 0414 0114 0208 0102  ................
+00004bc0: 0206 020a 0204 010a 010e 010e 0110 0208  ................
+00004bd0: 010e 0106 010a 010a 0314 0114 0208 0102  ................
+00004be0: 0206 0272 cf00 0000 7a11 2f62 6573 7441  ...r....z./bestA
+00004bf0: 7373 6574 7356 616c 7565 7363 0100 0000  ssetsValuesc....
+00004c00: 0000 0000 0000 0000 0900 0000 0500 0000  ................
+00004c10: 0300 0000 736c 0100 0074 00a0 0164 01a1  ....sl...t...d..
+00004c20: 017d 017c 0164 0219 00a0 0264 0364 0484  .}.|.d.....d.d..
+00004c30: 00a1 017c 0164 023c 0074 036a 047c 0164  ...|.d.<.t.j.|.d
+00004c40: 0219 00a0 05a1 0064 0564 068d 0264 0719  .......d.d...d..
+00004c50: 007d 027c 026a 0664 0864 098d 017d 027c  .}.|.j.d.d...}.|
+00004c60: 02a0 07a1 00a0 08a1 0064 0a14 0089 007c  .........d.....|
+00004c70: 02a0 07a1 00a0 09a1 0074 0aa0 0b64 0aa1  .........t...d..
+00004c80: 0114 007d 0374 00a0 0c88 007c 0364 0b9c  ...}.t.....|.d..
+00004c90: 02a1 017d 047c 0464 0c19 007c 0464 0d19  ...}.|.d...|.d..
+00004ca0: 001b 007c 0464 0e3c 007c 046a 0d64 0e64  ...|.d.<.|.j.d.d
+00004cb0: 0f64 108d 02a0 0e64 11a1 017d 047c 0464  .d.....d...}.|.d
+00004cc0: 0e19 007c 0464 0e19 00a0 0fa1 001b 007c  ...|.d.........|
+00004cd0: 0464 123c 007c 0464 1219 0088 0114 007c  .d.<.|.d.......|
+00004ce0: 0464 133c 007c 04a0 10a1 007d 047c 046a  .d.<.|.....}.|.j
+00004cf0: 1164 1464 1564 169c 0264 178d 017d 047c  .d.d.d...d...}.|
+00004d00: 0464 1419 0044 005d 407d 0574 036a 047c  .d...D.]@}.t.j.|
+00004d10: 0564 0564 068d 027d 067c 0664 0719 006a  .d.d...}.|.d...j
+00004d20: 1264 1819 007c 0664 0719 006a 1264 1919  .d...|.d...j.d..
+00004d30: 0018 007c 0664 0719 006a 1264 1919 001b  ...|.d...j.d....
+00004d40: 0088 007c 053c 0071 ee87 0087 0166 0264  ...|.<.q.....f.d
+00004d50: 1a64 1b84 087c 0464 1419 0044 0083 017d  .d...|.d...D...}
+00004d60: 077c 07a0 13a1 007d 0874 147c 0883 017d  .|.....}.t.|...}
+00004d70: 087c 087c 0464 1c3c 007c 0467 0064 1da2  .|.|.d.<.|.g.d..
+00004d80: 0119 0053 0029 1e75 1a02 0000 0a20 2020  ...S.).u.....   
+00004d90: 2023 2320 5573 6162 696c 6964 6164 650a   ## Usabilidade.
+00004da0: 2020 2020 2d20 4675 6ec3 a7c3 a36f 2071      - Fun....o q
+00004db0: 7565 2061 6e61 6c69 7361 206f 7320 6174  ue analisa os at
+00004dc0: 6976 6f73 2064 6f20 4942 4f56 4553 5041  ivos do IBOVESPA
+00004dd0: 2071 7565 2063 6f6d 2062 6173 6520 6e6f   que com base no
+00004de0: 2076 616c 6f72 2064 6520 696e 7665 7374   valor de invest
+00004df0: 696d 656e 746f 2065 7363 6f6c 6869 646f  imento escolhido
+00004e00: 206d 6f73 7472 6120 7175 6169 7320 706f   mostra quais po
+00004e10: 6465 6d20 7365 7220 7375 6173 2065 7363  dem ser suas esc
+00004e20: 6f6c 6861 732c 206f 2071 7561 6e74 6f20  olhas, o quanto 
+00004e30: 6972 6120 7465 7220 7175 6520 696e 7665  ira ter que inve
+00004e40: 7374 6972 2070 6172 6120 6361 6461 2061  stir para cada a
+00004e50: 7469 766f 2065 206f 2072 6574 6f72 6e6f  tivo e o retorno
+00004e60: 2061 7072 6f78 696d 6164 6f20 7061 7261   aproximado para
+00004e70: 2063 6164 6120 756d 2064 656c 6573 200a   cada um deles .
+00004e80: 0a20 2020 202d 2055 7361 6d6f 7320 636f  .    - Usamos co
+00004e90: 6d6f 206d 6574 6f64 6f20 6465 2063 c3a1  mo metodo de c..
+00004ea0: 6c63 756c 6f20 6f20 6120 6d65 6469 6461  lculo o a medida
+00004eb0: 2053 6861 7270 6520 7175 6520 6e61 6461   Sharpe que nada
+00004ec0: 206d 6169 7320 c3a9 2071 7565 2075 6d61   mais .. que uma
+00004ed0: 2020 6d65 6469 6461 2064 6520 6465 7365    medida de dese
+00004ee0: 6d70 656e 686f 2064 6520 696e 7665 7374  mpenho de invest
+00004ef0: 696d 656e 746f 7320 7175 6520 6c65 7661  imentos que leva
+00004f00: 2065 6d20 636f 6e73 6964 6572 61c3 a7c3   em considera...
+00004f10: a36f 206f 2072 6574 6f72 6e6f 206f 6274  .o o retorno obt
+00004f20: 6964 6f20 7065 6c6f 2069 6e76 6573 7469  ido pelo investi
+00004f30: 6d65 6e74 6f20 656d 2072 656c 61c3 a7c3  mento em rela...
+00004f40: a36f 2061 6f20 7269 7363 6f20 6173 7375  .o ao risco assu
+00004f50: 6d69 646f 0a20 2020 2023 2320 5061 72c3  mido.    ## Par.
+00004f60: a26d 6574 726f 730a 2020 2020 0a20 2020  .metros.    .   
+00004f70: 202d 2076 616c 6f72 202d 3e20 5661 6c6f   - valor -> Valo
+00004f80: 7220 646f 2069 6e76 6573 7469 6d65 6e74  r do investiment
+00004f90: 6f2c 2070 6f72 2070 6164 72c3 a36f 2030  o, por padr..o 0
+00004fa0: 0a0a 2020 2020 7a3e 513a 5c52 6973 636f  ..    z>Q:\Risco
+00004fb0: 5c4e 6f76 6f20 5269 7363 6f5c 7079 7468  \Novo Risco\pyth
+00004fc0: 6f6e 7269 7363 6f5c 4242 4669 6e61 6e63  onrisco\BBFinanc
+00004fd0: 655c 4461 7461 5c41 7469 766f 7349 626f  e\Data\AtivosIbo
+00004fe0: 762e 786c 7378 72c2 0000 0063 0100 0000  v.xlsxr....c....
+00004ff0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00005000: 5300 0000 7308 0000 007c 0064 0117 0053  S...s....|.d...S
+00005010: 0072 a200 0000 721f 0000 0072 a300 0000  .r....r....r....
+00005020: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00005030: a500 0000 8503 0000 72a6 0000 007a 2362  ........r....z#b
+00005040: 6573 745f 6173 7365 7473 5f76 616c 7565  est_assets_value
+00005050: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00005060: 613e 723a 0000 0072 3c00 0000 7248 0000  a>r:...r<...rH..
+00005070: 0072 5400 0000 2901 5a04 6178 6973 7265  .rT...).Z.axisre
+00005080: 0000 0029 0272 9a00 0000 729b 0000 0072  ...).r....r....r
+00005090: 9a00 0000 729b 0000 005a 0673 6861 7270  ....r....Z.sharp
+000050a0: 6546 2901 5a09 6173 6365 6e64 696e 67e9  eF).Z.ascending.
+000050b0: 0600 0000 5a08 616c 6f63 6163 616f da05  ....Z.alocacao..
+000050c0: 7661 6c6f 72da 0641 7469 766f 73fa 1351  valor..Ativos..Q
+000050d0: 7464 204e 6563 6573 7361 7269 6120 2852  td Necessaria (R
+000050e0: 2429 2902 7281 0000 0072 d100 0000 72c9  $)).r....r....r.
+000050f0: 0000 0072 2600 0000 7201 0000 0063 0100  ...r&...r....c..
+00005100: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00005110: 0000 1300 0000 731a 0000 0069 007c 005d  ......s....i.|.]
+00005120: 127d 017c 0188 007c 0119 0088 0114 0093  .}.|...|........
+00005130: 0271 0453 0072 1f00 0000 721f 0000 0029  .q.S.r....r....)
+00005140: 02da 022e 3072 ce00 0000 a902 729a 0000  ....0r......r...
+00005150: 0072 d100 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00005160: da0a 3c64 6963 7463 6f6d 703e a803 0000  ..<dictcomp>....
+00005170: 72a6 0000 007a 2562 6573 745f 6173 7365  r....z%best_asse
+00005180: 7473 5f76 616c 7565 2e3c 6c6f 6361 6c73  ts_value.<locals
+00005190: 3e2e 3c64 6963 7463 6f6d 703e fa0e 5265  >.<dictcomp>..Re
+000051a0: 746f 726e 6f20 4170 726f 782e 2903 72d2  torno Aprox.).r.
+000051b0: 0000 0072 d300 0000 72d7 0000 0029 1572  ...r....r....).r
+000051c0: 4300 0000 5a0a 7265 6164 5f65 7863 656c  C...Z.read_excel
+000051d0: 72b2 0000 0072 2a00 0000 7266 0000 0072  r....r*...rf...r
+000051e0: cb00 0000 728e 0000 0072 6f00 0000 7259  ....r....ro...rY
+000051f0: 0000 0072 7600 0000 7267 0000 0072 6a00  ...rv...rg...rj.
+00005200: 0000 7244 0000 005a 0b73 6f72 745f 7661  ..rD...Z.sort_va
+00005210: 6c75 6573 da04 6865 6164 7231 0000 0072  lues..headr1...r
+00005220: 4600 0000 da06 7265 6e61 6d65 7230 0000  F.....renamer0..
+00005230: 00da 0676 616c 7565 7372 3e00 0000 2909  ...valuesr>...).
+00005240: 72d1 0000 00da 0661 7469 766f 7372 c400  r......ativosr..
+00005250: 0000 729b 0000 005a 0961 7469 766f 735f  ..r....Z.ativos_
+00005260: 6466 72ce 0000 0072 8700 0000 5a11 7265  dfr....r....Z.re
+00005270: 746f 726e 6f5f 706f 725f 6174 6976 6f5a  torno_por_ativoZ
+00005280: 0c4c 6973 7461 5265 746f 726e 6f72 1f00  .ListaRetornor..
+00005290: 0000 72d5 0000 0072 2000 0000 da11 6265  ..r....r .....be
+000052a0: 7374 5f61 7373 6574 735f 7661 6c75 6576  st_assets_valuev
+000052b0: 0300 0073 2a00 0000 000e 0a01 1603 1a03  ...s*...........
+000052c0: 0c03 1001 1603 1003 1403 1403 1803 1001  ................
+000052d0: 0802 1202 0c01 0e01 3003 1801 0801 0802  ........0.......
+000052e0: 0803 72dc 0000 0063 0100 0000 0000 0000  ..r....c........
+000052f0: 0000 0000 0800 0000 0900 0000 4300 0000  ............C...
+00005300: 73d8 0000 0074 006a 0164 0164 0264 038d  s....t.j.d.d.d..
+00005310: 027d 017c 01a0 02a1 007d 0174 03a0 047c  .}.|.....}.t...|
+00005320: 0164 0419 00a0 0574 06a1 016a 06a0 0764  .d.....t...j...d
+00005330: 0564 06a1 02a1 017d 027c 0164 0719 007d  .d.....}.|.d...}
+00005340: 0374 0883 007d 047c 04a0 097c 026a 0aa0  .t...}.|...|.j..
+00005350: 0b64 0864 09a1 027c 03a1 0201 0074 036a  .d.d...|.....t.j
+00005360: 0ca0 0da1 00a0 0e64 0aa1 017d 0574 036a  .......d...}.t.j
+00005370: 0ca0 0da1 0074 036a 0f64 0b64 0c8d 0117  .....t.j.d.d....
+00005380: 00a0 0e64 0aa1 017d 067c 04a0 1074 03a0  ...d...}.|...t..
+00005390: 047c 06a0 0764 0564 06a1 0267 01a1 01a0  .|...d.d...g....
+000053a0: 0b64 0864 09a1 02a1 017c 04a0 1074 03a0  .d.d.....|...t..
+000053b0: 047c 05a0 0764 0564 06a1 0267 01a1 01a0  .|...d.d...g....
+000053c0: 0b64 0864 09a1 02a1 011b 0064 0918 007d  .d.d.......d...}
+000053d0: 077c 0764 0d19 0064 0814 0053 0029 0e4e  .|.d...d...S.).N
+000053e0: 726d 0000 0072 3a00 0000 723c 0000 00da  rm...r:...r<....
+000053f0: 0444 6174 65fa 012d 7218 0000 0072 4800  .Date..-r....rH.
+00005400: 0000 7226 0000 0072 5400 0000 7217 0000  ..r&...rT...r...
+00005410: 0072 1400 0000 7215 0000 0072 0100 0000  .r....r....r....
+00005420: 2911 722a 0000 0072 6600 0000 7246 0000  ).r*...rf...rF..
+00005430: 0072 4300 0000 5a0a 746f 5f6e 756d 6572  .rC...Z.to_numer
+00005440: 6963 721c 0000 0072 8300 0000 721b 0000  icr....r....r...
+00005450: 0072 0400 0000 5a03 6669 7472 da00 0000  .r....Z.fitr....
+00005460: da07 7265 7368 6170 65da 0954 696d 6573  ..reshape..Times
+00005470: 7461 6d70 da05 746f 6461 79da 0873 7472  tamp..today..str
+00005480: 6674 696d 655a 0a44 6174 654f 6666 7365  ftimeZ.DateOffse
+00005490: 745a 0770 7265 6469 6374 2908 72ce 0000  tZ.predict).r...
+000054a0: 005a 1064 6164 6f73 5f68 6973 746f 7269  .Z.dados_histori
+000054b0: 636f 735a 0564 6174 6173 72c4 0000 005a  cosZ.datasr....Z
+000054c0: 066d 6f64 656c 6f5a 0a64 6174 615f 6174  .modeloZ.data_at
+000054d0: 7561 6c5a 0b64 6174 615f 6675 7475 7261  ualZ.data_futura
+000054e0: 5a0c 7461 7861 5f72 6574 6f72 6e6f 721f  Z.taxa_retornor.
+000054f0: 0000 0072 1f00 0000 7220 0000 00da 1370  ...r....r .....p
+00005500: 7265 7665 725f 7461 7861 5f72 6574 6f72  rever_taxa_retor
+00005510: 6e6f b803 0000 731c 0000 0000 020e 0108  no....s.........
+00005520: 061e 0108 0306 0316 0310 011c 0120 0120  ............. . 
+00005530: ff02 0102 ff04 0372 e300 0000 e771 3d0a  .......r.....q=.
+00005540: d7a3 70cd 3f29 0272 db00 0000 da0c 696e  ..p.?).r......in
+00005550: 7665 7374 696d 656e 746f 6303 0000 0000  vestimentoc.....
+00005560: 0000 0000 0000 000a 0000 0007 0000 0043  ...............C
+00005570: 0000 0073 1e01 0000 7400 6a01 6700 6401  ...s....t.j.g.d.
+00005580: a201 6402 8d01 7d03 7402 7c00 7403 8302  ..d...}.t.|.t...
+00005590: 7296 7404 a005 7c00 a101 7d04 7c04 6a06  r.t...|...}.|.j.
+000055a0: 6403 6404 8d01 6405 1900 6406 1900 7d05  d.d...d...d...}.
+000055b0: 7c04 6a07 a008 a100 7d06 7c05 7c06 1700  |.j.....}.|.|...
+000055c0: 7c05 1b00 6407 1800 7c01 1400 7d07 7409  |...d...|...}.t.
+000055d0: a00a 7c07 7c01 1b00 6407 1700 a101 7409  ..|.|...d.....t.
+000055e0: a00a 6407 6408 7c02 1400 1700 a101 1b00  ..d.d.|.........
+000055f0: 6409 1b00 7d08 7c03 6a0b 7c00 7c07 7c08  d...}.|.j.|.|.|.
+00005600: 6401 9c03 640a 640b 8d02 7d03 6e84 7c00  d...d.d...}.n.|.
+00005610: 4400 5d7e 7d09 7404 a005 7c09 a101 7d04  D.]~}.t...|...}.
+00005620: 7c04 6a06 6403 6404 8d01 6405 1900 6406  |.j.d.d...d...d.
+00005630: 1900 7d05 7c04 6a07 a008 a100 7d06 7c05  ..}.|.j.....}.|.
+00005640: 7c06 1700 7c05 1b00 6407 1800 7c01 1400  |...|...d...|...
+00005650: 7d07 7409 a00a 7c07 7c01 1b00 6407 1700  }.t...|.|...d...
+00005660: a101 7409 a00a 6407 6408 7c02 1400 1700  ..t...d.d.|.....
+00005670: a101 1b00 6409 1b00 7d08 7c03 6a0b 7c09  ....d...}.|.j.|.
+00005680: 7c07 7c08 6401 9c03 640a 640b 8d02 7d03  |.|.d...d.d...}.
+00005690: 719a 7c03 5300 290c 4e29 0372 7c00 0000  q.|.S.).N).r|...
+000056a0: 7a16 5265 746f 726e 6f20 636f 6d20 4469  z.Retorno com Di
+000056b0: 7669 6465 6e64 6f73 7a1a 5465 6d70 6f20  videndosz.Tempo 
+000056c0: 7061 7261 2041 7469 6e67 6972 2052 6574  para Atingir Ret
+000056d0: 6f72 6e6f 72c9 0000 0072 3a00 0000 723c  ornor....r:...r<
+000056e0: 0000 0072 4800 0000 7201 0000 0072 5400  ...rH...r....rT.
+000056f0: 0000 72c8 0000 00e9 0c00 0000 5429 015a  ..r.........T).Z
+00005700: 0c69 676e 6f72 655f 696e 6465 7829 0c72  .ignore_index).r
+00005710: 4300 0000 7244 0000 0072 8200 0000 7283  C...rD...r....r.
+00005720: 0000 0072 2a00 0000 722b 0000 0072 4000  ...r*...r+...r@.
+00005730: 0000 7229 0000 0072 3100 0000 7267 0000  ..r)...r1...rg..
+00005740: 0072 6800 0000 7299 0000 0029 0a72 db00  .rh...r....).r..
+00005750: 0000 72e5 0000 005a 0d74 6178 615f 6465  ..r....Z.taxa_de
+00005760: 7363 6f6e 746f 7287 0000 0072 7b00 0000  scontor....r{...
+00005770: 5a05 7072 6563 6f5a 0a64 6976 6964 656e  Z.precoZ.dividen
+00005780: 646f 7372 c500 0000 5a05 7465 6d70 6f72  dosr....Z.tempor
+00005790: ce00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+000057a0: 0000 00da 1372 6574 6f72 6e6f 735f 6469  .....retornos_di
+000057b0: 7669 6465 6e64 6f73 d503 0000 7320 0000  videndos....s ..
+000057c0: 0000 0110 020a 010a 0114 010a 0114 0128  ...............(
+000057d0: 0118 0208 010a 0114 010a 0114 0128 0118  .............(..
+000057e0: 0272 e700 0000 2901 723a 0000 0029 0172  .r....).r:...).r
+000057f0: 0100 0000 2901 72e4 0000 0029 4e5a 0879  ....).r....)NZ.y
+00005800: 6669 6e61 6e63 6572 2a00 0000 5a0b 7363  financer*...Z.sc
+00005810: 6970 792e 7374 6174 7372 0200 0000 5a0e  ipy.statsr....Z.
+00005820: 7363 6970 792e 6f70 7469 6d69 7a65 7203  scipy.optimizer.
+00005830: 0000 005a 1473 6b6c 6561 726e 2e6c 696e  ...Z.sklearn.lin
+00005840: 6561 725f 6d6f 6465 6c72 0400 0000 5a08  ear_modelr....Z.
+00005850: 7365 6c65 6e69 756d 7205 0000 005a 1e73  seleniumr....Z.s
+00005860: 656c 656e 6975 6d2e 7765 6264 7269 7665  elenium.webdrive
+00005870: 722e 636f 6d6d 6f6e 2e6b 6579 7372 0600  r.common.keysr..
+00005880: 0000 5a21 7365 6c65 6e69 756d 2e77 6562  ..Z!selenium.web
+00005890: 6472 6976 6572 2e63 6872 6f6d 652e 6f70  driver.chrome.op
+000058a0: 7469 6f6e 7372 0700 0000 5a1c 7365 6c65  tionsr....Z.sele
+000058b0: 6e69 756d 2e77 6562 6472 6976 6572 2e63  nium.webdriver.c
+000058c0: 6f6d 6d6f 6e2e 6279 7208 0000 0072 ad00  ommon.byr....r..
+000058d0: 0000 5a03 6273 3472 0900 0000 5a07 6661  ..Z.bs4r....Z.fa
+000058e0: 7374 6170 6972 0a00 0000 720b 0000 0072  stapir....r....r
+000058f0: 0c00 0000 5a11 6661 7374 6170 692e 7265  ....Z.fastapi.re
+00005900: 7370 6f6e 7365 7372 0d00 0000 5a13 6661  sponsesr....Z.fa
+00005910: 7374 6170 692e 7374 6174 6963 6669 6c65  stapi.staticfile
+00005920: 7372 0e00 0000 5a12 6661 7374 6170 692e  sr....Z.fastapi.
+00005930: 7465 6d70 6c61 7469 6e67 720f 0000 00da  templatingr.....
+00005940: 046a 736f 6e5a 0775 7669 636f 726e da09  .jsonZ.uvicorn..
+00005950: 4242 4669 6e61 6e63 65da 0262 62da 0670  BBFinance..bb..p
+00005960: 616e 6461 7372 4300 0000 da05 6e75 6d70  andasrC.....nump
+00005970: 7972 6700 0000 7210 0000 0072 1100 0000  yrg...r....r....
+00005980: da06 7479 7069 6e67 7212 0000 00da 0877  ..typingr......w
+00005990: 6172 6e69 6e67 73da 0e66 696c 7465 7277  arnings..filterw
+000059a0: 6172 6e69 6e67 735a 0c70 6472 5f6f 7665  arningsZ.pdr_ove
+000059b0: 7272 6964 6572 e100 0000 5a0c 6f6e 655f  rrider....Z.one_
+000059c0: 7965 6172 5f61 676f 72e2 0000 0072 cc00  year_agor....r..
+000059d0: 0000 72cd 0000 00da 0361 7070 7221 0000  ..r......appr!..
+000059e0: 0072 ae00 0000 7283 0000 0072 2e00 0000  .r....r....r....
+000059f0: 7235 0000 00da 085f 5f6e 616d 655f 5fda  r5.....__name__.
+00005a00: 0372 756e 72b5 0000 0072 4400 0000 7247  .runr....rD...rG
+00005a10: 0000 005a 0f72 6573 706f 6e73 6548 6973  ...Z.responseHis
+00005a20: 746f 7279 724d 0000 0072 5f00 0000 726c  toryrM...r_...rl
+00005a30: 0000 0072 7100 0000 721d 0000 00da 0369  ...rq...r......i
+00005a40: 6e74 7279 0000 0072 3e00 0000 7289 0000  ntry...r>...r...
+00005a50: 0072 9d00 0000 72b9 0000 0072 bc00 0000  .r....r....r....
+00005a60: 72bf 0000 0072 cf00 0000 72dc 0000 0072  r....r....r....r
+00005a70: e300 0000 72e7 0000 0072 1f00 0000 721f  ....r....r....r.
+00005a80: 0000 0072 1f00 0000 7220 0000 00da 083c  ...r....r .....<
+00005a90: 6d6f 6475 6c65 3e02 0000 0073 cc00 0000  module>....s....
+00005aa0: 0801 0c01 0c01 0c03 0c01 0c01 0c01 0c02  ................
+00005ab0: 0801 0c03 1401 0c01 0c01 0c01 0801 0801  ................
+00005ac0: 0802 0801 0801 1001 0c02 0801 0a03 0802  ................
+00005ad0: 0802 0e03 0a01 0a02 060c 0809 0c01 1226  ...............&
+00005ae0: 0a01 1201 0a05 0c01 1826 0a01 1201 0a05  .........&......
+00005af0: 0c01 1220 0a01 1201 0a05 0c01 123a 0a01  ... .........:..
+00005b00: 1201 0a05 0c01 1618 0a01 1201 0a05 0c01  ................
+00005b10: 1232 0a01 1201 0a05 0c01 1623 0a01 1201  .2.........#....
+00005b20: 0a05 0c01 2062 0a01 1201 0a05 0801 163a  .... b.........:
+00005b30: 0a01 1201 0a05 0c01 1418 0a01 1201 0a05  ................
+00005b40: 0c01 1642 0a01 1201 0a05 0c01 1a40 0a01  ...B.........@..
+00005b50: 1201 0a05 0c01 167f 0007 0a01 1201 0a03  ................
+00005b60: 0c01 1e3a 0a01 1201 0a05 081d            ...:........
```

### Comparing `BBFinance-1.4.7/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.4.8/BBFinance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 BBFinance.egg-info/dependency_links.txt
 BBFinance.egg-info/requires.txt
 BBFinance.egg-info/top_level.txt
 BBFinance/__pycache__/BBFinance.cpython-311.pyc
 BBFinance/__pycache__/BBFinance.cpython-39.pyc
 BBFinance/__pycache__/__init__.cpython-311.pyc
 BBFinance/__pycache__/__init__.cpython-39.pyc
-Data/AtivosIbov.xlsx
 __pycache__/__init__.cpython-39.pyc
-__pycache__/main.cpython-39.pyc
+__pycache__/main.cpython-39.pyc
+docs/CNAME
```

### Comparing `BBFinance-1.4.7/LICENSE.txt` & `BBFinance-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/__pycache__/main.cpython-39.pyc` & `BBFinance-1.4.8/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/requirements.txt` & `BBFinance-1.4.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.7/setup.py` & `BBFinance-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4.7',
+    version='1.4.8',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
-    license='MIT',
+    license='GPLv3',
     packages=['BBFinance'],
     long_description= long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'yfinance==0.2.14',
         'selenium>=3.141.0',
         'pandas-datareader>=0.10.0',
         'json5>=0.9.6',
-        'numpy>=1.23.4',
+        'numpy>=1.21.6',
         'uvicorn>=0.21.1',
         'fastapi>=0.95.0',
         'scipy>=1.10.1',
         'requests>=2.28.2',
         'bs4>=0.0.1',
         'beautifulsoup4>=4.11.2',
         'pydantic>=1.10.7',
```

