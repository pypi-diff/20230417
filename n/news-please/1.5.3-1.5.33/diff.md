# Comparing `tmp/news-please-1.5.3.tar.gz` & `tmp/news-please-1.5.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/news-please-1.5.3.tar", last modified: Thu Apr 30 08:23:04 2020, max compression
+gzip compressed data, was "news-please-1.5.33.tar", last modified: Mon Apr 17 14:54:23 2023, max compression
```

## Comparing `news-please-1.5.3.tar` & `news-please-1.5.33.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/
--rw-r--r--   0 felix      (501) staff       (20)    11356 2017-02-24 09:14:32.000000 news-please-1.5.3/LICENSE.txt
--rw-r--r--   0 felix      (501) staff       (20)      182 2017-02-24 19:19:10.000000 news-please-1.5.3/MANIFEST.in
--rw-r--r--   0 felix      (501) staff       (20)     1680 2020-04-30 08:23:04.000000 news-please-1.5.3/PKG-INFO
--rw-r--r--   0 felix      (501) staff       (20)    13982 2020-04-09 06:19:20.000000 news-please-1.5.3/README.md
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/
--rw-r--r--   0 felix      (501) staff       (20)     1680 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/PKG-INFO
--rw-r--r--   0 felix      (501) staff       (20)     2645 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/SOURCES.txt
--rw-r--r--   0 felix      (501) staff       (20)        1 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/dependency_links.txt
--rw-r--r--   0 felix      (501) staff       (20)      112 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/entry_points.txt
--rw-r--r--   0 felix      (501) staff       (20)        1 2020-01-14 20:52:16.000000 news-please-1.5.3/news_please.egg-info/not-zip-safe
--rw-r--r--   0 felix      (501) staff       (20)      392 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/requires.txt
--rw-r--r--   0 felix      (501) staff       (20)       11 2020-04-30 08:23:03.000000 news-please-1.5.3/news_please.egg-info/top_level.txt
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/
--rw-r--r--   0 felix      (501) staff       (20)     1627 2020-03-20 10:24:18.000000 news-please-1.5.3/newsplease/NewsArticle.py
--rw-r--r--   0 felix      (501) staff       (20)     5128 2020-04-30 08:21:24.000000 news-please-1.5.3/newsplease/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)    24157 2020-04-06 18:43:18.000000 news-please-1.5.3/newsplease/__main__.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/config/
--rw-r--r--   0 felix      (501) staff       (20)    14455 2020-04-06 18:43:18.000000 news-please-1.5.3/newsplease/config/config.cfg
--rw-r--r--   0 felix      (501) staff       (20)    14505 2020-04-06 18:43:18.000000 news-please-1.5.3/newsplease/config/config_lib.cfg
--rw-r--r--   0 felix      (501) staff       (20)     2127 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/config/sitelist.hjson
--rw-r--r--   0 felix      (501) staff       (20)     9095 2020-04-30 08:21:24.000000 news-please-1.5.3/newsplease/config.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/crawler/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/crawler/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)    14409 2020-04-30 08:21:24.000000 news-please-1.5.3/newsplease/crawler/commoncrawl_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)    14647 2019-08-06 08:29:21.000000 news-please-1.5.3/newsplease/crawler/commoncrawl_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     1450 2017-05-18 12:22:17.000000 news-please-1.5.3/newsplease/crawler/items.py
--rw-r--r--   0 felix      (501) staff       (20)     1779 2018-05-29 10:49:21.000000 news-please-1.5.3/newsplease/crawler/simple_crawler.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/crawler/spiders/
--rw-r--r--   0 felix      (501) staff       (20)      161 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/crawler/spiders/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     1242 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/crawler/spiders/download_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)     3426 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/crawler/spiders/gdelt_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)     1889 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/crawler/spiders/recursive_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)     2133 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/crawler/spiders/recursive_sitemap_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)     3327 2020-01-14 20:51:50.000000 news-please-1.5.3/newsplease/crawler/spiders/rss_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)     2037 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/crawler/spiders/sitemap_crawler.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/examples/
--rw-r--r--   0 felix      (501) staff       (20)        0 2019-07-15 13:05:32.000000 news-please-1.5.3/newsplease/examples/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     7878 2020-04-30 08:21:24.000000 news-please-1.5.3/newsplease/examples/commoncrawl.py
--rw-r--r--   0 felix      (501) staff       (20)      707 2017-05-21 10:40:30.000000 news-please-1.5.3/newsplease/examples/downloadfromfile.py
--rw-r--r--   0 felix      (501) staff       (20)      534 2017-07-05 09:49:18.000000 news-please-1.5.3/newsplease/examples/downloadfromurl.py
--rw-r--r--   0 felix      (501) staff       (20)     1177 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/helper.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:03.000000 news-please-1.5.3/newsplease/helper_classes/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/helper_classes/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     4819 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/helper_classes/heuristics.py
--rw-r--r--   0 felix      (501) staff       (20)     4803 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/helper_classes/parse_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)    11872 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/helper_classes/savepath_parser.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/newsplease/helper_classes/sub_classes/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/helper_classes/sub_classes/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     9811 2018-07-31 09:48:34.000000 news-please-1.5.3/newsplease/helper_classes/sub_classes/heuristics_manager.py
--rw-r--r--   0 felix      (501) staff       (20)     6551 2020-01-14 20:51:50.000000 news-please-1.5.3/newsplease/helper_classes/url_extractor.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/newsplease/pipeline/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/pipeline/__init__.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/newsplease/pipeline/extractor/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/pipeline/extractor/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)      362 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/article_candidate.py
--rw-r--r--   0 felix      (501) staff       (20)     2599 2019-11-13 10:07:04.000000 news-please-1.5.3/newsplease/pipeline/extractor/article_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     3798 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/pipeline/extractor/cleaner.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     1960 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer.py
--rw-r--r--   0 felix      (501) staff       (20)     1934 2019-11-13 09:45:59.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_Language.py
--rw-r--r--   0 felix      (501) staff       (20)     1349 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_author.py
--rw-r--r--   0 felix      (501) staff       (20)     1274 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_date.py
--rw-r--r--   0 felix      (501) staff       (20)     1411 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_description.py
--rw-r--r--   0 felix      (501) staff       (20)     3329 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_text.py
--rw-r--r--   0 felix      (501) staff       (20)     3056 2018-07-31 09:48:34.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_title.py
--rw-r--r--   0 felix      (501) staff       (20)     1973 2019-04-02 13:02:07.000000 news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_topimage.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2020-04-30 08:23:04.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/
--rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     2011 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/abstract_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     8442 2020-04-30 08:21:24.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/date_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     2533 2019-11-13 09:32:27.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/lang_detect_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     1671 2017-06-01 09:33:29.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/newspaper_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)     1306 2017-05-31 11:47:46.000000 news-please-1.5.3/newsplease/pipeline/extractor/extractors/readability_extractor.py
--rw-r--r--   0 felix      (501) staff       (20)    32601 2020-04-06 18:43:18.000000 news-please-1.5.3/newsplease/pipeline/pipelines.py
--rw-r--r--   0 felix      (501) staff       (20)    10652 2020-01-14 20:51:50.000000 news-please-1.5.3/newsplease/single_crawler.py
--rw-r--r--   0 felix      (501) staff       (20)      346 2020-04-08 17:39:28.000000 news-please-1.5.3/requirements.txt
--rw-r--r--   0 felix      (501) staff       (20)       38 2020-04-30 08:23:04.000000 news-please-1.5.3/setup.cfg
--rw-r--r--   0 felix      (501) staff       (20)     2912 2020-04-30 08:21:24.000000 news-please-1.5.3/setup.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.926318 news-please-1.5.33/
+-rw-r--r--   0 felix      (501) staff       (20)    11356 2017-02-24 09:14:32.000000 news-please-1.5.33/LICENSE.txt
+-rw-r--r--   0 felix      (501) staff       (20)      182 2017-02-24 19:19:10.000000 news-please-1.5.33/MANIFEST.in
+-rw-r--r--   0 felix      (501) staff       (20)     1677 2023-04-17 14:54:23.926136 news-please-1.5.33/PKG-INFO
+-rw-r--r--   0 felix      (501) staff       (20)    14757 2023-04-17 13:36:28.000000 news-please-1.5.33/README.md
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.918199 news-please-1.5.33/news_please.egg-info/
+-rw-r--r--   0 felix      (501) staff       (20)     1677 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/PKG-INFO
+-rw-r--r--   0 felix      (501) staff       (20)     2800 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/SOURCES.txt
+-rw-r--r--   0 felix      (501) staff       (20)        1 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/dependency_links.txt
+-rw-r--r--   0 felix      (501) staff       (20)      111 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/entry_points.txt
+-rw-r--r--   0 felix      (501) staff       (20)        1 2023-04-17 14:46:13.000000 news-please-1.5.33/news_please.egg-info/not-zip-safe
+-rw-r--r--   0 felix      (501) staff       (20)      397 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/requires.txt
+-rw-r--r--   0 felix      (501) staff       (20)       11 2023-04-17 14:54:23.000000 news-please-1.5.33/news_please.egg-info/top_level.txt
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.919003 news-please-1.5.33/newsplease/
+-rw-r--r--   0 felix      (501) staff       (20)     1627 2020-03-20 10:24:18.000000 news-please-1.5.33/newsplease/NewsArticle.py
+-rw-r--r--   0 felix      (501) staff       (20)     5679 2023-04-17 14:35:20.000000 news-please-1.5.33/newsplease/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)    24157 2020-04-06 18:43:18.000000 news-please-1.5.33/newsplease/__main__.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.919400 news-please-1.5.33/newsplease/config/
+-rw-r--r--   0 felix      (501) staff       (20)    14641 2023-02-21 16:22:32.000000 news-please-1.5.33/newsplease/config/config.cfg
+-rw-r--r--   0 felix      (501) staff       (20)    14640 2023-02-21 16:22:32.000000 news-please-1.5.33/newsplease/config/config_lib.cfg
+-rw-r--r--   0 felix      (501) staff       (20)     2127 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/config/sitelist.hjson
+-rw-r--r--   0 felix      (501) staff       (20)     9098 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/config.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.920176 news-please-1.5.33/newsplease/crawler/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/crawler/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)    18927 2023-02-21 16:22:32.000000 news-please-1.5.33/newsplease/crawler/commoncrawl_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)    15901 2023-02-21 16:22:32.000000 news-please-1.5.33/newsplease/crawler/commoncrawl_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)     1450 2017-05-18 12:22:17.000000 news-please-1.5.33/newsplease/crawler/items.py
+-rw-r--r--   0 felix      (501) staff       (20)     1612 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/crawler/response_decoder.py
+-rw-r--r--   0 felix      (501) staff       (20)     3455 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/crawler/simple_crawler.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.921107 news-please-1.5.33/newsplease/crawler/spiders/
+-rw-r--r--   0 felix      (501) staff       (20)      161 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/crawler/spiders/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     1242 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/crawler/spiders/download_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)     3426 2019-04-02 13:02:07.000000 news-please-1.5.33/newsplease/crawler/spiders/gdelt_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)     1889 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/crawler/spiders/recursive_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)     2133 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/crawler/spiders/recursive_sitemap_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)     3327 2020-01-14 20:51:50.000000 news-please-1.5.33/newsplease/crawler/spiders/rss_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)     2037 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/crawler/spiders/sitemap_crawler.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.921613 news-please-1.5.33/newsplease/examples/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2019-07-15 13:05:32.000000 news-please-1.5.33/newsplease/examples/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     9059 2023-02-21 16:22:32.000000 news-please-1.5.33/newsplease/examples/commoncrawl.py
+-rw-r--r--   0 felix      (501) staff       (20)      707 2017-05-21 10:40:30.000000 news-please-1.5.33/newsplease/examples/downloadfromfile.py
+-rw-r--r--   0 felix      (501) staff       (20)      534 2017-07-05 09:49:18.000000 news-please-1.5.33/newsplease/examples/downloadfromurl.py
+-rw-r--r--   0 felix      (501) staff       (20)     1262 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/helper.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.922373 news-please-1.5.33/newsplease/helper_classes/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/helper_classes/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)      702 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/helper_classes/class_loader.py
+-rw-r--r--   0 felix      (501) staff       (20)     4819 2019-04-02 13:02:07.000000 news-please-1.5.33/newsplease/helper_classes/heuristics.py
+-rw-r--r--   0 felix      (501) staff       (20)     4847 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/helper_classes/parse_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)    11872 2019-04-02 13:02:07.000000 news-please-1.5.33/newsplease/helper_classes/savepath_parser.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.922620 news-please-1.5.33/newsplease/helper_classes/sub_classes/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/helper_classes/sub_classes/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     9811 2018-07-31 09:48:34.000000 news-please-1.5.33/newsplease/helper_classes/sub_classes/heuristics_manager.py
+-rw-r--r--   0 felix      (501) staff       (20)     6551 2020-01-14 20:51:50.000000 news-please-1.5.33/newsplease/helper_classes/url_extractor.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.922871 news-please-1.5.33/newsplease/pipeline/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/pipeline/__init__.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.923668 news-please-1.5.33/newsplease/pipeline/extractor/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/pipeline/extractor/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)      362 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/article_candidate.py
+-rw-r--r--   0 felix      (501) staff       (20)     2909 2023-04-17 14:06:11.000000 news-please-1.5.33/newsplease/pipeline/extractor/article_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)     3909 2021-02-02 13:02:35.000000 news-please-1.5.33/newsplease/pipeline/extractor/cleaner.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.924970 news-please-1.5.33/newsplease/pipeline/extractor/comparer/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     1960 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer.py
+-rw-r--r--   0 felix      (501) staff       (20)     1934 2019-11-13 09:45:59.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_Language.py
+-rw-r--r--   0 felix      (501) staff       (20)     1349 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_author.py
+-rw-r--r--   0 felix      (501) staff       (20)     1274 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_date.py
+-rw-r--r--   0 felix      (501) staff       (20)     1411 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_description.py
+-rw-r--r--   0 felix      (501) staff       (20)     3329 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_text.py
+-rw-r--r--   0 felix      (501) staff       (20)     3056 2018-07-31 09:48:34.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_title.py
+-rw-r--r--   0 felix      (501) staff       (20)     1973 2019-04-02 13:02:07.000000 news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_topimage.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2023-04-17 14:54:23.925925 news-please-1.5.33/newsplease/pipeline/extractor/extractors/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2017-02-24 09:14:32.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     2011 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/abstract_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)     8442 2020-04-30 08:21:24.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/date_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)     2905 2021-02-07 14:02:12.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/lang_detect_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)     1897 2023-04-17 14:31:57.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/newspaper_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)      178 2021-02-24 07:44:54.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/newspaper_extractor_no_images.py
+-rw-r--r--   0 felix      (501) staff       (20)     1306 2017-05-31 11:47:46.000000 news-please-1.5.33/newsplease/pipeline/extractor/extractors/readability_extractor.py
+-rw-r--r--   0 felix      (501) staff       (20)    32549 2021-02-05 15:07:01.000000 news-please-1.5.33/newsplease/pipeline/pipelines.py
+-rw-r--r--   0 felix      (501) staff       (20)    11221 2020-10-23 13:14:07.000000 news-please-1.5.33/newsplease/single_crawler.py
+-rw-r--r--   0 felix      (501) staff       (20)      370 2023-02-21 16:22:32.000000 news-please-1.5.33/requirements.txt
+-rw-r--r--   0 felix      (501) staff       (20)       38 2023-04-17 14:54:23.926364 news-please-1.5.33/setup.cfg
+-rw-r--r--   0 felix      (501) staff       (20)     2930 2023-04-17 14:34:46.000000 news-please-1.5.33/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `news-please-1.5.3/LICENSE.txt` & `news-please-1.5.33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/PKG-INFO` & `news-please-1.5.33/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: news-please
-Version: 1.5.3
+Version: 1.5.33
 Summary: news-please is an open source easy-to-use news extractor that just works.
 Home-page: https://github.com/fhamborg/news-please
+Download-URL: https://github.com/fhamborg/news-please
 Author: Felix Hamborg
 Author-email: felix.hamborg@uni-konstanz.de
 License: Apache License 2.0
-Download-URL: https://github.com/fhamborg/news-please
-Description: news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website. Furthermore, its API allows developers to access the exctraction functionality within their software. news-please also implements a workflow optimized for the news archive provided by commoncrawl.org, allowing users to efficiently crawl and extract news articles including various filter options.
 Keywords: news crawler news scraper news extractor crawler extractor scraper information retrieval
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE.txt
+
+news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website. Furthermore, its API allows developers to access the exctraction functionality within their software. news-please also implements a workflow optimized for the news archive provided by commoncrawl.org, allowing users to efficiently crawl and extract news articles including various filter options.
```

### Comparing `news-please-1.5.3/README.md` & `news-please-1.5.33/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # **news-please** #
 
 [![PyPI version](https://img.shields.io/pypi/v/news-please.svg)](https://pypi.org/project/news-please/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4120316.svg)](http://dx.doi.org/10.5281/zenodo.4120316)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url)
 
 <img align="right" height="128px" width="128px" src="https://raw.githubusercontent.com/fhamborg/news-please/master/misc/logo/logo-256.png" />
 
-news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website to crawl it completely. news-please combines the power of multiple state-of-the-art libraries and tools, such as [scrapy](https://scrapy.org/), [Newspaper](https://github.com/codelucas/newspaper), and [readability](https://github.com/buriy/python-readability). news-please also features a library mode, which allows Python developers to use the crawling and extraction functionality within their own program. Moreover, news-please allows to conveniently [crawl and extract articles](/newsplease/examples/commoncrawl.py) from commoncrawl.org.
+news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can recursively follow internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website to crawl it completely. news-please combines the power of multiple state-of-the-art libraries and tools, such as [scrapy](https://scrapy.org/), [Newspaper](https://github.com/codelucas/newspaper), and [readability](https://github.com/buriy/python-readability). news-please also features a library mode, which allows Python developers to use the crawling and extraction functionality within their own program. Moreover, news-please allows to conveniently [crawl and extract articles](/newsplease/examples/commoncrawl.py) from the (very) large news archive at commoncrawl.org.
 
-If you like news-please and would like to [contribute](#Contribution-and-custom-features) to it, please have a look at our list of [issues that need help](https://github.com/fhamborg/news-please/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22). Of course, we are always looking forward to [pull requests](#contribution-and-custom-features) containing bug fixes, improvements, or your own ideas.
+If you want to [contribute](#contributions) to news-please, please have a look at our list of [issues that need help](https://github.com/fhamborg/news-please/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) or look [here](#contributions-and-custom-features).
 
 ## Announcements
+03/23/2021: If you're interested in sentiment classification in news articles, check out our large-scale dataset for target-dependent sentiment classification. We also publish an easy-to-use neural model that achieves state-of-the-art performance. Visit the project [here](https://github.com/fhamborg/NewsMTSC).
+
 06/01/2018: If you're interested in news analysis, you might also want to check out our new project, [Giveme5W1H](https://github.com/fhamborg/Giveme5W1H) - a tool that extracts phrases answering the journalistic five W and one H questions to describe an article's main event, i.e., who did what, when, where, why, and how.
 
 ## Extracted information
-news-please extracts the following attributes from news articles. Also, have a look at an [examplary json file](https://github.com/fhamborg/news-please/blob/master/newsplease/examples/sample.json) extracted by news-please.
+news-please extracts the following attributes from news articles. An examplary json file as extracted by news-please can be found [here](https://github.com/fhamborg/news-please/blob/master/newsplease/examples/sample.json).
 * headline
 * lead paragraph
 * main text
 * main image
 * name(s) of author(s)
 * publication date
 * language
@@ -40,27 +43,27 @@
 * crawl and extract information given a list of article URLs
 * to use news-please within your own Python code
 
 #### News archive from commoncrawl.org
 * commoncrawl.org provides an extensive, free-to-use archive of news articles from small and major publishers world wide
 * news-please enables users to conveniently download and extract articles from commoncrawl.org
 * you can optionally define filter criteria, such as news publisher(s) or the date period, within which articles need to be published
-* clone the news-please repository, [install the awscli tool](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html), adapt the config section in [newsplease/examples/commoncrawl.py](/newsplease/examples/commoncrawl.py), and execute `python3 -m newsplease.examples.commoncrawl`
+* clone the news-please repository, adapt the config section in [newsplease/examples/commoncrawl.py](/newsplease/examples/commoncrawl.py), and execute `python3 -m newsplease.examples.commoncrawl`
 
 ## Getting started
 It's super easy, we promise!
 
 ### Installation
 news-please runs on Python 3.5+.
 ```
 $ pip3 install news-please
 ```
 
 ### Use within your own code (as a library)
-You can access the core functionality of news-please, i.e. extraction of semi-structured information from one or more news articles, in your own code by using news-please in library mode. If you want to use news-please's full website extraction (given only the root URL) or continuous crawling mode (using RSS), you'll need to use the CLI mode.
+You can access the core functionality of news-please, i.e. extraction of semi-structured information from one or more news articles, in your own code by using news-please in library mode. If you want to use news-please's full website extraction (given only the root URL) or continuous crawling mode (using RSS), you'll need to use the CLI mode, which is described later.
 ```python
 from newsplease import NewsPlease
 article = NewsPlease.from_url('https://www.nytimes.com/2017/02/23/us/politics/cpac-stephen-bannon-reince-priebus.html?hp')
 print(article.title)
 ```
 A sample of an extracted article can be found [here (as a JSON file)](https://github.com/fhamborg/news-please/blob/master/newsplease/examples/sample.json).
 
@@ -73,19 +76,28 @@
 NewsPlease.from_file(path)
 ```
 or if you have raw HTML data (you can also provide the original URL to increase the accuracy of extracting the publishing date)
 ```python
 NewsPlease.from_html(html, url=None)
 ```
 or if you have a [WARC file](https://github.com/webrecorder/warcio) (also check out our [commoncrawl workflow](https://github.com/fhamborg/news-please/blob/master/newsplease/examples/commoncrawl.py), which provides convenient methods to filter commoncrawl's archive for specific news outlets and dates)
-```
+```python
 NewsPlease.from_warc(warc_record)
 ```
 In library mode, news-please will attempt to download and extract information from each URL. The previously described functions are blocking, i.e., will return once news-please has attempted all URLs. The resulting list contains all successfully extracted articles.
 
+Finally, you can process the extracted information contained in the article object(s). For example, to export into a JSON format, you may use:
+
+```python
+import json
+
+with open("article.json", "w") as file:
+    json.dump(article.get_serializable_dict(), file)
+```
+
 ### Run the crawler (via the CLI)
 
 ```
 $ news-please
 ```
 
 news-please will then start crawling a few examples pages. To terminate the process press `CTRL+C`. news-please will then shut down within 5-60 seconds. You can also press `CTRL+C` twice, which will immediately kill the process (not recommended, though).
@@ -144,22 +156,22 @@
 
 If you plan to use news-please and its export to PostgreSQL in a production environment, we recommend to uninstall the `psycopg2-binary` package and install `psycopg2`. We use the former since it does not require a C compiler in order to be installed. See [here](https://pypi.org/project/psycopg2-binary/), for more information on differences between `psycopg2` and `psycopg2-binary` and how to setup a production environment.
 
 
 ### What's next?
 We have collected a bunch of useful information for both [users](https://github.com/fhamborg/news-please/wiki/user-guide)  and [developers](https://github.com/fhamborg/news-please/wiki/developer-guide). As a user, you will most likely only deal with two files: [`sitelist.hjson`](https://github.com/fhamborg/news-please/wiki/user-guide#sitelisthjson) (to define sites to be crawled) and [`config.cfg`](https://github.com/fhamborg/news-please/wiki/configuration) (probably only rarely, in case you want to tweak the configuration).
 
-## Wiki and support (also, how to open an issue)
+## Support (also, how to open an issue)
 You can find more information on usage and development in our [wiki](https://github.com/fhamborg/news-please/wiki)! Before contacting us, please check out the wiki. If you still have questions on how to use news-please, please create a new [issue](https://github.com/fhamborg/news-please/issues) on GitHub. Please understand that we are not able to provide individual support via email. We think that help is more valuable if it is shared publicly so that more people can benefit from it.
 
 ### Issues
 For bug reports, we ask you to use the Bug report template. Make sure you're using the latest version of news-please, since we cannot give support for older versions. Unfortunately, we cannot give support for issues or questions sent by email.
 
 ### Donation
-Your donations are greatly appreciated! They will free me up to work on this project more, to take on tasks such as adding new features, bug-fix support, and addressing further concerns with the library.
+Your donations are greatly appreciated! They will free us up to work on this project more, to take on tasks such as adding new features, bug-fix support, and addressing further concerns with the library. 
 
 * [GitHub Sponsors](https://github.com/sponsors/fhamborg)
 * [PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url)
 
 ## Acknowledgements
 This project would not have been possible without the contributions of the following students (ordered alphabetically):
 
@@ -182,27 +194,31 @@
 ```
 @InProceedings{Hamborg2017,
   author     = {Hamborg, Felix and Meuschke, Norman and Breitinger, Corinna and Gipp, Bela},
   title      = {news-please: A Generic News Crawler and Extractor},
   year       = {2017},
   booktitle  = {Proceedings of the 15th International Symposium of Information Science},
   location   = {Berlin},
-  editor     = {Gaede, Maria and Trkulja, Violeta and Petra, Vivien},
+  doi        = {10.5281/zenodo.4120316},
   pages      = {218--223},
   month      = {March}
 }
 ```
 You can find more information on this and other news projects on our [website](https://felix.hamborg.eu/).
 
-## Contributions and custom features
-Do you want to contribute? Great, we are always happy for any support on this project! We are particularly looking for pull requests that fix bugs (issues are found under the [issues tab](https://github.com/fhamborg/news-please/issues)), but welcome also pull requests that contribute your own ideas. If you plan to submit a pull request adding new functionality, we suggest to open an issue first in order to briefly discuss with us how it should be implemented to best fit into news-please's architecture.
+## Contributions
+Do you want to contribute? Great, we are always happy for any support on this project! We are particularly looking for pull requests that fix [bugs](https://github.com/fhamborg/news-please/issues). We also welcome pull requests that contribute your own ideas. 
+
+By contributing to this project, you agree that your contributions will be licensed under the project's [license](#license).
 
-Please note that we usually do not have enough resources to implement features requested by users - instead we recommend to implement them yourself, and send a pull request.
+### Pull requests
+We love contributions by our users! If you plan to submit a pull request, please open an issue first and desribe the issue you want to fix or what you want to improve and how! This way, we can discuss whether your idea could be added to news-please in the first place and, if so, how it could best be implemented in order to fit into architecture and coding style. In the issue, please state that you're planning to implement the described features. 
 
-By contributing to this project, you agree that your contributions will be licensed under the project's license (see below).
+### Custom features
+Unfortunately, we do not have resources to implement features requested by users. Instead, we recommend that you implement features you need and if you'd like open a pull request here so that the community can benefit from your improvements, too.
 
 ## License
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use news-please except in compliance with the License. A copy of the License is included in the project, see the file [LICENSE.txt](LICENSE.txt).
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License. The news-please logo is courtesy of [Mario Hamborg](https://mario.hamborg.eu/).
 
-Copyright 2016-2020 The news-please team
+Copyright 2016-2023 The news-please team
```

### Comparing `news-please-1.5.3/news_please.egg-info/PKG-INFO` & `news-please-1.5.33/news_please.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: news-please
-Version: 1.5.3
+Version: 1.5.33
 Summary: news-please is an open source easy-to-use news extractor that just works.
 Home-page: https://github.com/fhamborg/news-please
+Download-URL: https://github.com/fhamborg/news-please
 Author: Felix Hamborg
 Author-email: felix.hamborg@uni-konstanz.de
 License: Apache License 2.0
-Download-URL: https://github.com/fhamborg/news-please
-Description: news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website. Furthermore, its API allows developers to access the exctraction functionality within their software. news-please also implements a workflow optimized for the news archive provided by commoncrawl.org, allowing users to efficiently crawl and extract news articles including various filter options.
 Keywords: news crawler news scraper news extractor crawler extractor scraper information retrieval
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE.txt
+
+news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website. Furthermore, its API allows developers to access the exctraction functionality within their software. news-please also implements a workflow optimized for the news archive provided by commoncrawl.org, allowing users to efficiently crawl and extract news articles including various filter options.
```

### Comparing `news-please-1.5.3/news_please.egg-info/SOURCES.txt` & `news-please-1.5.33/news_please.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 newsplease/config/config.cfg
 newsplease/config/config_lib.cfg
 newsplease/config/sitelist.hjson
 newsplease/crawler/__init__.py
 newsplease/crawler/commoncrawl_crawler.py
 newsplease/crawler/commoncrawl_extractor.py
 newsplease/crawler/items.py
+newsplease/crawler/response_decoder.py
 newsplease/crawler/simple_crawler.py
 newsplease/crawler/spiders/__init__.py
 newsplease/crawler/spiders/download_crawler.py
 newsplease/crawler/spiders/gdelt_crawler.py
 newsplease/crawler/spiders/recursive_crawler.py
 newsplease/crawler/spiders/recursive_sitemap_crawler.py
 newsplease/crawler/spiders/rss_crawler.py
 newsplease/crawler/spiders/sitemap_crawler.py
 newsplease/examples/__init__.py
 newsplease/examples/commoncrawl.py
 newsplease/examples/downloadfromfile.py
 newsplease/examples/downloadfromurl.py
 newsplease/helper_classes/__init__.py
+newsplease/helper_classes/class_loader.py
 newsplease/helper_classes/heuristics.py
 newsplease/helper_classes/parse_crawler.py
 newsplease/helper_classes/savepath_parser.py
 newsplease/helper_classes/url_extractor.py
 newsplease/helper_classes/sub_classes/__init__.py
 newsplease/helper_classes/sub_classes/heuristics_manager.py
 newsplease/pipeline/__init__.py
@@ -58,8 +60,9 @@
 newsplease/pipeline/extractor/comparer/comparer_title.py
 newsplease/pipeline/extractor/comparer/comparer_topimage.py
 newsplease/pipeline/extractor/extractors/__init__.py
 newsplease/pipeline/extractor/extractors/abstract_extractor.py
 newsplease/pipeline/extractor/extractors/date_extractor.py
 newsplease/pipeline/extractor/extractors/lang_detect_extractor.py
 newsplease/pipeline/extractor/extractors/newspaper_extractor.py
+newsplease/pipeline/extractor/extractors/newspaper_extractor_no_images.py
 newsplease/pipeline/extractor/extractors/readability_extractor.py
```

### Comparing `news-please-1.5.3/newsplease/NewsArticle.py` & `news-please-1.5.33/newsplease/NewsArticle.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/__init__.py` & `news-please-1.5.33/newsplease/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,75 +11,99 @@
 from newsplease.pipeline.extractor import article_extractor
 from newsplease.crawler.items import NewscrawlerItem
 from dotmap import DotMap
 from newsplease.pipeline.pipelines import ExtractedInformationStorage
 from newsplease.crawler.simple_crawler import SimpleCrawler
 
 
+class EmptyResponseError(ValueError):
+    pass
+
+
 class NewsPlease:
     """
     Access news-please functionality via this interface
     """
 
     @staticmethod
-    def from_warc(warc_record):
+    def from_warc(warc_record, decode_errors="replace", fetch_images=True):
         """
         Extracts relevant information from a WARC record. This function does not invoke scrapy but only uses the article
         extractor.
         :return:
         """
         raw_stream = warc_record.raw_stream.read()
         encoding = None
         try:
-            encoding = warc_record.http_headers.get_header('Content-Type').split(';')[1].split('=')[1]
+            encoding = (
+                warc_record.http_headers.get_header("Content-Type")
+                .split(";")[1]
+                .split("=")[1]
+            )
         except:
             pass
         if not encoding:
             encoding = EncodingDetector.find_declared_encoding(raw_stream, is_html=True)
         if not encoding:
             # assume utf-8
-            encoding = 'utf-8'
+            encoding = "utf-8"
 
-        html = raw_stream.decode(encoding)
-        url = warc_record.rec_headers.get_header('WARC-Target-URI')
-        download_date = warc_record.rec_headers.get_header('WARC-Date')
-        article = NewsPlease.from_html(html, url=url, download_date=download_date)
+        try:
+            html = raw_stream.decode(encoding, errors=decode_errors)
+        except LookupError:
+            # non-existent encoding: fallback to utf-9
+            html = raw_stream.decode("utf-8", errors=decode_errors)
+        if not html:
+            raise EmptyResponseError()
+        url = warc_record.rec_headers.get_header("WARC-Target-URI")
+        download_date = warc_record.rec_headers.get_header("WARC-Date")
+        article = NewsPlease.from_html(
+            html, url=url, download_date=download_date, fetch_images=fetch_images
+        )
         return article
 
     @staticmethod
-    def from_html(html, url=None, download_date=None):
+    def from_html(html, url=None, download_date=None, fetch_images=True):
         """
         Extracts relevant information from an HTML page given as a string. This function does not invoke scrapy but only
         uses the article extractor. If you have the original URL make sure to provide it as this helps NewsPlease
         to extract the publishing date and title.
         :param html:
         :param url:
         :return:
         """
         extractor = article_extractor.Extractor(
-            ['newspaper_extractor', 'readability_extractor', 'date_extractor', 'lang_detect_extractor'])
+            (
+                ["newspaper_extractor"]
+                if fetch_images
+                else [("newspaper_extractor_no_images", "NewspaperExtractorNoImages")]
+            )
+            + ["readability_extractor", "date_extractor", "lang_detect_extractor"]
+        )
 
-        title_encoded = ''.encode()
+        title_encoded = "".encode()
         if not url:
-            url = ''
+            url = ""
 
         # if an url was given, we can use that as the filename
-        filename = urllib.parse.quote_plus(url) + '.json'
+        filename = urllib.parse.quote_plus(url) + ".json"
 
         item = NewscrawlerItem()
-        item['spider_response'] = DotMap()
-        item['spider_response'].body = html
-        item['url'] = url
-        item['source_domain'] = urllib.parse.urlparse(url).hostname.encode() if url != '' else ''.encode()
-        item['html_title'] = title_encoded
-        item['rss_title'] = title_encoded
-        item['local_path'] = None
-        item['filename'] = filename
-        item['download_date'] = download_date
-        item['modified_date'] = None
+        item["spider_response"] = DotMap()
+        item["spider_response"].body = html
+        item["url"] = url
+        item["source_domain"] = (
+            urllib.parse.urlparse(url).hostname.encode() if url != "" else "".encode()
+        )
+        item["html_title"] = title_encoded
+        item["rss_title"] = title_encoded
+        item["local_path"] = None
+        item["filename"] = filename
+        item["download_date"] = download_date
+        item["modified_date"] = None
         item = extractor.extract(item)
 
         tmp_article = ExtractedInformationStorage.extract_relevant_info(item)
         final_article = ExtractedInformationStorage.convert_to_class(tmp_article)
         return final_article
 
     @staticmethod
@@ -102,24 +126,23 @@
         """
         Crawls articles from the urls and extracts relevant information.
         :param urls:
         :param timeout: in seconds, if None, the urllib default is used
         :return: A dict containing given URLs as keys, and extracted information as corresponding values.
         """
         results = {}
-        download_date = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        download_date = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
         if len(urls) == 0:
-            # Nested blocks of code should not be left empty.
-            # When a block contains a comment, this block is not considered to be empty
             pass
         elif len(urls) == 1:
             url = urls[0]
             html = SimpleCrawler.fetch_url(url, timeout=timeout)
-            results[url] = NewsPlease.from_html(html, url, download_date)
+            if html:
+                results[url] = NewsPlease.from_html(html, url, download_date)
         else:
             results = SimpleCrawler.fetch_urls(urls)
             for url in results:
                 results[url] = NewsPlease.from_html(results[url], url, download_date)
 
         return results
```

### Comparing `news-please-1.5.3/newsplease/__main__.py` & `news-please-1.5.33/newsplease/__main__.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/config/config.cfg` & `news-please-1.5.33/newsplease/config/config.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 # -------------
 
 # urls which end on any of the following file extensions are ignored for recursive crawling
 # default: "(pdf)|(docx?)|(xlsx?)|(pptx?)|(epub)|(jpe?g)|(png)|(bmp)|(gif)|(tiff)|(webp)|(avi)|(mpe?g)|(mov)|(qt)|(webm)|(ogg)|(midi)|(mid)|(mp3)|(wav)|(zip)|(rar)|(exe)|(apk)|(css)"
 ignore_file_extensions = "(pdf)|(docx?)|(xlsx?)|(pptx?)|(epub)|(jpe?g)|(png)|(bmp)|(gif)|(tiff)|(webp)|(avi)|(mpe?g)|(mov)|(qt)|(webm)|(ogg)|(midi)|(mid)|(mp3)|(wav)|(zip)|(rar)|(exe)|(apk)|(css)"
 
 # urls which match the following regex are ignored for recursive crawling
-# default: ""
-ignore_regex = ""
+# default: "(mail[tT]o)|([jJ]avascript)|(tel)|(fax)"
+ignore_regex = "(mail[tT]o)|([jJ]avascript)|(tel)|(fax)"
 
 # Crawl the sitemaps of subdomains (if sitemap is enabled)
 # If True, any SitemapCrawler will try to crawl on the sitemap of the given domain including subdomains instead of a domain's main sitemap.
 # e.g. if True, a SitemapCrawler to be started on https://blog.zeit.de will try to crawl on the sitemap listed in http://blog.zeit.de/robots.txt. If not found, it will fall back to the False setting.
 #      if False, a SitemapCrawler to be started on https://blog.zeit.de will try to crawl on the sitemap listed in http://zeit.de/robots.txt
 # default: True
 sitemap_allow_subdomains = True
@@ -318,15 +318,17 @@
 # User-agent activation
 # default: 'news-please (+http://www.example.com/)'
 USER_AGENT = 'news-please (+http://www.example.com/)'
 
 # Pipeline activation
 # Syntax: '<relative location>.<Pipeline name>': <Order of execution from 0-1000>
 # default: {'newsplease.pipeline.pipelines.ArticleMasterExtractor':100, 'newsplease.crawler.pipeline.HtmlFileStorage':200, 'newsplease.pipeline.pipelines.JsonFileStorage': 300}
-# Further options: 'newsplease.pipeline.pipelines.ElasticsearchStorage': 350
+# Further options: 'newsplease.pipeline.pipelines.ElasticsearchStorage': 350, 'newsplease.pipeline.pipelines.DateFilter': 150,
 ITEM_PIPELINES = {'newsplease.pipeline.pipelines.ArticleMasterExtractor':100,
                   'newsplease.pipeline.pipelines.HtmlFileStorage':200,
                   'newsplease.pipeline.pipelines.JsonFileStorage':300
                   }
 
+ITEM_CLASS = 'newsplease.crawler.items.NewscrawlerItem'
+
 [Pandas]
-file_name = "PandasStorage"
+file_name = "PandasStorage"
```

### Comparing `news-please-1.5.3/newsplease/config/config_lib.cfg` & `news-please-1.5.33/newsplease/config/config_lib.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 # -------------
 
 # urls which end on any of the following file extensions are ignored for recursive crawling
 # default: "(pdf)|(docx?)|(xlsx?)|(pptx?)|(epub)|(jpe?g)|(png)|(bmp)|(gif)|(tiff)|(webp)|(avi)|(mpe?g)|(mov)|(qt)|(webm)|(ogg)|(midi)|(mid)|(mp3)|(wav)|(zip)|(rar)|(exe)|(apk)|(css)"
 ignore_file_extensions = "(pdf)|(docx?)|(xlsx?)|(pptx?)|(epub)|(jpe?g)|(png)|(bmp)|(gif)|(tiff)|(webp)|(avi)|(mpe?g)|(mov)|(qt)|(webm)|(ogg)|(midi)|(mid)|(mp3)|(wav)|(zip)|(rar)|(exe)|(apk)|(css)"
 
 # urls which match the following regex are ignored for recursive crawling
-# default: ""
-ignore_regex = ""
+# default: "(mail[tT]o)|([jJ]avascript)|(tel)|(fax)"
+ignore_regex = "(mail[tT]o)|([jJ]avascript)|(tel)|(fax)"
 
 # Crawl the sitemaps of subdomains (if sitemap is enabled)
 # If True, any SitemapCrawler will try to crawl on the sitemap of the given domain including subdomains instead of a domain's main sitemap.
 # e.g. if True, a SitemapCrawler to be started on https://blog.zeit.de will try to crawl on the sitemap listed in http://blog.zeit.de/robots.txt. If not found, it will fall back to the False setting.
 #      if False, a SitemapCrawler to be started on https://blog.zeit.de will try to crawl on the sitemap listed in http://zeit.de/robots.txt
 # default: True
 sitemap_allow_subdomains = True
@@ -328,7 +328,9 @@
 # Pipeline activation
 # Syntax: '<relative location>.<Pipeline name>': <Order of execution from 0-1000>
 # default: {'newsplease.pipeline.pipelines.ArticleMasterExtractor':100, 'newsplease.crawler.pipeline.HtmlFileStorage':200, 'newsplease.pipeline.pipelines.JsonFileStorage': 300}
 # Further options: 'newsplease.pipeline.pipelines.ElasticsearchStorage': 350
 ITEM_PIPELINES = {'newsplease.pipeline.pipelines.ArticleMasterExtractor':100,
                   'newsplease.pipeline.pipelines.InMemoryStorage':200
                   }
+
+ITEM_CLASS = 'newsplease.crawler.items.NewscrawlerItem'
```

### Comparing `news-please-1.5.3/newsplease/config/sitelist.hjson` & `news-please-1.5.33/newsplease/config/sitelist.hjson`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/config.py` & `news-please-1.5.33/newsplease/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                         self.__config[section][option] = literal_eval(opt)
                     except (SyntaxError, ValueError):
                         self.__config[section][option] = opt
                         self.log_output.append(
                             {"level": "debug",
                              "msg": "Option not literal_eval-parsable"
                                     " (maybe string): [{0}] {1}"
-                                 .format(section, option)})
+                                    .format(section, option)})
 
                     if self.__config[section][option] == -1:
                         self.log_output.append(
                             {"level": "debug",
                              "msg": "Skipping: [%s] %s" % (section, option)}
                         )
                 except ConfigParser.NoOptionError as exc:
@@ -151,19 +151,19 @@
         handled here
         """
 
         configure_logging(self.get_scrapy_options())
 
         # Now, after log-level is correctly set, lets log them.
         for msg in self.log_output:
-            if msg["level"] is "error":
+            if msg["level"] == "error":
                 self.log.error(msg["msg"])
-            elif msg["level"] is "info":
+            elif msg["level"] == "info":
                 self.log.info(msg["msg"])
-            elif msg["level"] is "debug":
+            elif msg["level"] == "debug":
                 self.log.debug(msg["msg"])
 
     def config(self):
         """
         Get the whole config as a dict.
 
         :returns: The whole config as dict[section][option] (all lowercase)
```

### Comparing `news-please-1.5.3/newsplease/crawler/commoncrawl_crawler.py` & `news-please-1.5.33/newsplease/crawler/commoncrawl_crawler.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 """
 Provides functionality to crawl and extract news articles from commoncrawl.org. Filter criteria, such as publish date
 and host list, can be defined. Currently, all WARC files will be downloaded to the path WORKINGDIR/cc_download_warc, if
 not otherwise specified.
 """
 import logging
 import os
-import subprocess
 import time
 from functools import partial
 from multiprocessing import Pool
 import datetime
+import gzip
+from urllib.parse import urlparse
 
+import boto3
+import botocore
 from dateutil import parser
+import requests
 from scrapy.utils.log import configure_logging
 
 from ..crawler.commoncrawl_extractor import CommonCrawlExtractor
 
 __author__ = "Felix Hamborg"
 __copyright__ = "Copyright 2017"
 __credits__ = ["Sebastian Nagel"]
 
 # commoncrawl.org
-__cc_base_url = 'https://commoncrawl.s3.amazonaws.com/'
+__cc_base_url = 'https://data.commoncrawl.org/'
+__cc_bucket = 'commoncrawl'
 
 # log file of fully extracted WARC files
 __log_pathname_fully_extracted_warcs = None
 
 # logging
 logging.basicConfig(level=logging.INFO)
 __logger = logging.getLogger(__name__)
@@ -38,36 +43,40 @@
 __counter_article_discarded = 0
 __counter_article_error = 0
 __counter_article_total = 0
 __counter_warc_skipped = 0
 __counter_warc_processed = 0
 __start_time = time.time()
 
+# When Common Crawl started.
+__common_crawl_start_date = datetime.datetime(2016, 8, 26)
 
 def __setup(local_download_dir_warc, log_level):
     """
     Setup
     :return:
     """
-    if not os.path.exists(local_download_dir_warc):
-        os.makedirs(local_download_dir_warc)
+    os.makedirs(local_download_dir_warc, exist_ok=True)
 
     global __log_pathname_fully_extracted_warcs
     __log_pathname_fully_extracted_warcs = os.path.join(local_download_dir_warc, 'fullyextractedwarcs.list')
 
-    # make loggers quite
+    # make loggers quiet
     configure_logging({"LOG_LEVEL": "ERROR"})
     logging.getLogger('requests').setLevel(logging.CRITICAL)
     logging.getLogger('readability').setLevel(logging.CRITICAL)
     logging.getLogger('PIL').setLevel(logging.CRITICAL)
     logging.getLogger('newspaper').setLevel(logging.CRITICAL)
     logging.getLogger('newsplease').setLevel(logging.CRITICAL)
     logging.getLogger('urllib3').setLevel(logging.CRITICAL)
     logging.getLogger('jieba').setLevel(logging.CRITICAL)
 
+    boto3.set_stream_logger('botocore', log_level)
+    boto3.set_stream_logger('boto3', log_level)
+
     # set own logger
     logging.basicConfig(level=log_level)
     __logger = logging.getLogger(__name__)
     __logger.setLevel(log_level)
 
 
 def __get_publishing_date(warc_record, article):
@@ -86,67 +95,148 @@
     """
     Creates a download url given the name
     :param name:
     :return:
     """
     return __cc_base_url + name
 
-def __iterate_by_month(start_date, end_date, month_step=1):
+
+def __iterate_by_month(start_date=None, end_date=None, month_step=1):
+    if start_date is None:
+        # The starting month of Common Crawl.
+        start_date = __common_crawl_start_date
+    if end_date is None:
+        # Until now.
+        end_date = datetime.datetime.today()
     current_date = start_date
-    while current_date < end_date:
-        yield current_date
+    yield current_date
+    while True:
         carry, new_month = divmod(current_date.month - 1 + month_step, 12)
         new_month += 1
         current_date = current_date.replace(year=current_date.year + carry,
                                             month=new_month)
+        yield current_date
+        if current_date > end_date:
+            break
 
 
-def __get_remote_index(warc_files_start_date):
+def __extract_date_from_warc_filename(path):
+    fn = os.path.basename(path)
+    # Assume the filename pattern is CC-NEWS-20160911145202-00018.warc.gz
+    fn = fn.replace('CC-NEWS-', '')
+    dt = fn.split('-')[0]
+
+    try:
+        return datetime.datetime.strptime(dt, '%Y%m%d%H%M%S')
+    except:
+        # return date clearly outside the range
+        return datetime.datetime(1900, 1, 1)
+
+
+def __date_within_period(date, start_date=None, end_date=None):
+    if start_date is None:
+        # The starting month of Common Crawl.
+        start_date = __common_crawl_start_date
+    if end_date is None:
+        # Until now.
+        end_date = datetime.datetime.today()
+    return start_date <= date < end_date
+
+
+def __get_remote_index(warc_files_start_date=None, warc_files_end_date=None):
     """
     Gets the index of news crawl files from commoncrawl.org and returns an array of names
+    :param warc_files_start_date: only list .warc files with greater or equal date in
+    their filename
+    :param warc_files_end_date: only list .warc files with smaller date in their filename
     :return:
     """
-    # cleanup
-    subprocess.getoutput("rm tmpaws.txt")
-    # get the remote info
-
-    cmd = ''
-    if warc_files_start_date:
-        warc_dates = __iterate_by_month(warc_files_start_date, datetime.datetime.today())
+
+    s3_client = boto3.client('s3')
+    # Verify access to commoncrawl bucket
+    try:
+        s3_client.head_bucket(Bucket=__cc_bucket)
+    except (botocore.exceptions.ClientError, botocore.exceptions.NoCredentialsError):
+        __logger.info('Failed to read %s bucket, using monthly WARC file listings', __cc_bucket)
+        s3_client = None
+
+    objects = []
+
+    if s3_client:
+        def s3_list_objects(bucket, prefix):
+            response = s3_client.list_objects(Bucket=bucket, Prefix=prefix)
+            if 'Contents' not in response:
+                return []
+            return [x['Key'] for x in response['Contents']]
+
+        if warc_files_start_date or warc_files_end_date:
+            # The news files are grouped per year and month in separate folders
+            warc_dates = __iterate_by_month(start_date=warc_files_start_date, end_date=warc_files_end_date)
+            for date in warc_dates:
+                year = date.strftime('%Y')
+                month = date.strftime('%m')
+                prefix = 'crawl-data/CC-NEWS/%s/%s/' % (year, month)
+                __logger.debug('Listing objects on S3 bucket %s and prefix %s', __cc_bucket, prefix)
+                objects += s3_list_objects(__cc_bucket, prefix)
+        else:
+            objects = s3_list_objects(__cc_bucket, 'crawl-data/CC-NEWS/')
+
+    else:
+        # The news files are grouped per year and month in separate folders
+        warc_dates = __iterate_by_month(start_date=warc_files_start_date, end_date=warc_files_end_date)
         for date in warc_dates:
             year = date.strftime('%Y')
             month = date.strftime('%m')
-            cmd += "aws s3 ls --recursive s3://commoncrawl/crawl-data/CC-NEWS/%s/%s/ --no-sign-request >> .tmpaws.txt && " %(year, month)
-
-        cmd += "awk '{ print $4 }' .tmpaws.txt && " \
-              "rm .tmpaws.txt"
-    else:
-        cmd = "aws s3 ls --recursive s3://commoncrawl/crawl-data/CC-NEWS/ --no-sign-request > .tmpaws.txt && " \
-          "awk '{ print $4 }' .tmpaws.txt && " \
-          "rm .tmpaws.txt"
-    __logger.info('executing: %s', cmd)
-    stdout_data = subprocess.getoutput(cmd)
-
-    lines = stdout_data.splitlines()
-    return lines
+            url = '%scrawl-data/CC-NEWS/%s/%s/warc.paths.gz' % (__cc_base_url, year, month)
+            __logger.debug('Fetching WARC paths listing %s', url)
+            response = requests.get(url)
+            if response:
+                objects += gzip.decompress(response.content).decode('ascii').strip().split('\n')
+            else:
+                __logger.info('Failed to fetch WARC file list %s: %s', url, response)
 
+    if warc_files_start_date or warc_files_end_date:
+        # Now filter further on day of month, hour, minute
+        objects = [
+            p for p in objects if __date_within_period(
+                __extract_date_from_warc_filename(p),
+                start_date=warc_files_start_date,
+                end_date=warc_files_end_date,
+            )
+        ]
+
+    __logger.info('Found %i WARC files', len(objects))
+
+    return objects
+
+def __get_url_path(url_or_path):
+    if url_or_path.startswith('http:') or url_or_path.startswith('https:'):
+        try:
+            url = urlparse(url_or_path)
+            return url.path.lstrip('/') # trim leading slash
+        except:
+            pass
+    return url_or_path
 
-def __get_list_of_fully_extracted_warc_urls():
+def __get_list_of_fully_extracted_warc_paths():
     """
     Reads in the log file that contains a list of all previously, fully extracted WARC urls
     :return:
     """
     if not os.path.isfile(__log_pathname_fully_extracted_warcs):
         return []
 
     with open(__log_pathname_fully_extracted_warcs) as log_file:
         list_warcs = log_file.readlines()
     # remove break lines
     list_warcs = [x.strip() for x in list_warcs]
 
+    # (back-ward compatibility) if it's a URL keep only the path
+    list_warcs = [__get_url_path(x) for x in list_warcs]
+
     return list_warcs
 
 
 def __callback_on_warc_completed(warc_path, counter_article_passed, counter_article_discarded, counter_article_error,
                                  counter_article_total):
     """
     Internal callback on completion of one WARC file. Calculating some statistics on processing speed.
@@ -178,143 +268,161 @@
     remaining_warcs = __number_of_warc_files_on_cc - (__counter_warc_processed + __counter_warc_skipped)
 
     __logger.info("warc processing statistics")
     __logger.info("warc files skipped = %i, processed = %i, remaining = %i, total = %i", __counter_warc_skipped,
                   __counter_warc_processed, remaining_warcs, __number_of_warc_files_on_cc)
     __logger.info("global [s/article] = %f", sec_per_article)
     __logger.info("global [h/warc] = %.3f", h_per_warc)
-    __logger.info("estimated remaining time [h] = %f", remaining_warcs / h_per_warc)
+    __logger.info("estimated remaining time [h] = %f", remaining_warcs * h_per_warc)
 
     # invoke the external callback
     __extern_callback_on_warc_completed(warc_path, __counter_article_passed, __counter_article_discarded,
                                         __counter_article_error, __counter_article_total, __counter_warc_processed)
 
 
-def __start_commoncrawl_extractor(warc_download_url, callback_on_article_extracted=None,
+def __start_commoncrawl_extractor(warc_path, callback_on_article_extracted=None,
                                   callback_on_warc_completed=None, valid_hosts=None,
-                                  start_date=None, end_date=None, 
+                                  start_date=None, end_date=None,
                                   strict_date=True, reuse_previously_downloaded_files=True,
                                   local_download_dir_warc=None,
                                   continue_after_error=True, show_download_progress=False,
                                   log_level=logging.ERROR,
                                   delete_warc_after_extraction=True,
                                   continue_process=True,
-                                  log_pathname_fully_extracted_warcs=None):
+                                  log_pathname_fully_extracted_warcs=None,
+                                  extractor_cls=CommonCrawlExtractor,
+                                  fetch_images=False):
     """
     Starts a single CommonCrawlExtractor
-    :param warc_download_url:
+    :param warc_path: path to the WARC file on s3://commoncrawl/ resp. https://data.commoncrawl.org/
     :param callback_on_article_extracted:
     :param callback_on_warc_completed:
     :param valid_hosts:
     :param start_date:
     :param end_date:
     :param strict_date:
     :param reuse_previously_downloaded_files:
     :param local_download_dir_warc:
     :param continue_after_error:
     :param show_download_progress:
     :param log_level:
+    :param extractor_cls: A subclass of CommonCrawlExtractor, which can be used
+        to add custom filtering by overriding .filter_record(...)
     :return:
     """
-    commoncrawl_extractor = CommonCrawlExtractor()
-    commoncrawl_extractor.extract_from_commoncrawl(warc_download_url, callback_on_article_extracted,
+    commoncrawl_extractor = extractor_cls()
+    commoncrawl_extractor.extract_from_commoncrawl(warc_path, callback_on_article_extracted,
                                                    callback_on_warc_completed=callback_on_warc_completed,
                                                    valid_hosts=valid_hosts,
                                                    start_date=start_date, end_date=end_date,
                                                    strict_date=strict_date,
                                                    reuse_previously_downloaded_files=reuse_previously_downloaded_files,
                                                    local_download_dir_warc=local_download_dir_warc,
                                                    continue_after_error=continue_after_error,
                                                    show_download_progress=show_download_progress,
                                                    log_level=log_level,
                                                    delete_warc_after_extraction=delete_warc_after_extraction,
-                                                   log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs)
+                                                   log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs,
+                                                   fetch_images=fetch_images)
 
 
 def crawl_from_commoncrawl(callback_on_article_extracted, callback_on_warc_completed=None, valid_hosts=None,
-                           start_date=None, end_date=None, warc_files_start_date=None, strict_date=True, 
-                           reuse_previously_downloaded_files=True, local_download_dir_warc=None, 
+                           start_date=None, end_date=None, warc_files_start_date=None, warc_files_end_date=None, strict_date=True,
+                           reuse_previously_downloaded_files=True, local_download_dir_warc=None,
                            continue_after_error=True, show_download_progress=False,
                            number_of_extraction_processes=4, log_level=logging.ERROR,
-                           delete_warc_after_extraction=True, continue_process=True):
+                           delete_warc_after_extraction=True, continue_process=True,
+                           extractor_cls=CommonCrawlExtractor, fetch_images=False,
+                           dry_run=False):
     """
     Crawl and extract articles form the news crawl provided by commoncrawl.org. For each article that was extracted
     successfully the callback function callback_on_article_extracted is invoked where the first parameter is the
     article object.
     :param continue_process:
     :param delete_warc_after_extraction:
     :param number_of_extraction_processes:
     :param callback_on_article_extracted:
     :param valid_hosts:
     :param start_date:
     :param end_date:
+    :param warc_files_start_date
+    :param warc_files_end_date
     :param strict_date:
     :param reuse_previously_downloaded_files:
     :param local_download_dir_warc:
     :param continue_after_error:
     :param show_download_progress:
     :param log_level:
+    :param extractor_cls:
+    :param dry_run: if True just list the WARC files to be processed but do not actually process them
     :return:
     """
     __setup(local_download_dir_warc, log_level)
 
     global __extern_callback_on_warc_completed
     __extern_callback_on_warc_completed = callback_on_warc_completed
 
-    cc_news_crawl_names = __get_remote_index(warc_files_start_date)
+    cc_news_crawl_names = __get_remote_index(warc_files_start_date, warc_files_end_date)
     global __number_of_warc_files_on_cc
     __number_of_warc_files_on_cc = len(cc_news_crawl_names)
     __logger.info('found %i files at commoncrawl.org', __number_of_warc_files_on_cc)
 
     # multiprocessing (iterate the list of crawl_names, and for each: download and process it)
     __logger.info('creating extraction process pool with %i processes', number_of_extraction_processes)
-    warc_download_urls = []
-    fully_extracted_warc_urls = __get_list_of_fully_extracted_warc_urls()
-    for name in cc_news_crawl_names:
-        warc_download_url = __get_download_url(name)
+    warc_paths = []
+    fully_extracted_warc_paths = __get_list_of_fully_extracted_warc_paths()
+    for warc_path in cc_news_crawl_names:
         if continue_process:
             # check if the current WARC has already been fully extracted (assuming that the filter criteria have not
             # been changed!)
-            if warc_download_url in fully_extracted_warc_urls:
-                __logger.info('skipping WARC because fully extracted: %s' % warc_download_url)
+            if warc_path in fully_extracted_warc_paths:
+                __logger.info('skipping WARC because fully extracted: %s', warc_path)
                 global __counter_warc_skipped
                 __counter_warc_skipped += 1
                 pass
             else:
-                warc_download_urls.append(warc_download_url)
+                warc_paths.append(warc_path)
 
         else:
             # if not continue process, then always add
-            warc_download_urls.append(warc_download_url)
+            warc_paths.append(warc_path)
+
+    if dry_run:
+        for warc_path in warc_paths:
+            __logger.info('(Dry run) Selected WARC file for processing: %s', warc_path)
 
     # run the crawler in the current, single process if number of extraction processes is set to 1
-    if number_of_extraction_processes > 1:
+    elif number_of_extraction_processes > 1:
         with Pool(number_of_extraction_processes) as extraction_process_pool:
             extraction_process_pool.map(partial(__start_commoncrawl_extractor,
                                                 callback_on_article_extracted=callback_on_article_extracted,
                                                 callback_on_warc_completed=__callback_on_warc_completed,
                                                 valid_hosts=valid_hosts,
                                                 start_date=start_date, end_date=end_date,
                                                 strict_date=strict_date,
                                                 reuse_previously_downloaded_files=reuse_previously_downloaded_files,
                                                 local_download_dir_warc=local_download_dir_warc,
                                                 continue_after_error=continue_after_error,
                                                 show_download_progress=show_download_progress,
                                                 log_level=log_level,
                                                 delete_warc_after_extraction=delete_warc_after_extraction,
-                                                log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs),
-                                        warc_download_urls)
+                                                log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs,
+                                                extractor_cls=extractor_cls,
+                                                fetch_images=fetch_images),
+                                        warc_paths)
     else:
-        for warc_download_url in warc_download_urls:
-            __start_commoncrawl_extractor(warc_download_url,
+        for warc_path in warc_paths:
+            __start_commoncrawl_extractor(warc_path,
                                           callback_on_article_extracted=callback_on_article_extracted,
                                           callback_on_warc_completed=__callback_on_warc_completed,
                                           valid_hosts=valid_hosts,
                                           start_date=start_date, end_date=end_date,
                                           strict_date=strict_date,
                                           reuse_previously_downloaded_files=reuse_previously_downloaded_files,
                                           local_download_dir_warc=local_download_dir_warc,
                                           continue_after_error=continue_after_error,
                                           show_download_progress=show_download_progress,
                                           log_level=log_level,
                                           delete_warc_after_extraction=delete_warc_after_extraction,
-                                          log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs)
+                                          log_pathname_fully_extracted_warcs=__log_pathname_fully_extracted_warcs,
+                                          extractor_cls=extractor_cls,
+                                          fetch_images=fetch_images)
```

### Comparing `news-please-1.5.3/newsplease/crawler/commoncrawl_extractor.py` & `news-please-1.5.33/newsplease/crawler/commoncrawl_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 """
 Provides functionality to crawl and extract news articles from a single WARC file from commoncrawl.org. Filter criteria, such as publish date
 and host list, can be defined. Currently, the WARC file will be downloaded to the path WORKINGDIR/cc_download_warc, if
 not otherwise specified.
 """
 import logging
 import os
-import subprocess
 import sys
 import time
 
 from ago import human
+import boto3
+import botocore
 from dateutil import parser
 from hurry.filesize import size
 from scrapy.utils.log import configure_logging
 from six.moves import urllib
 from warcio.archiveiterator import ArchiveIterator
 
-from .. import NewsPlease
+from .. import NewsPlease, EmptyResponseError
+from . import commoncrawl_crawler
 
 __author__ = "Felix Hamborg"
 __copyright__ = "Copyright 2017"
 __credits__ = ["Sebastian Nagel"]
 
 
 class CommonCrawlExtractor:
     # remote url where we can download the warc file
-    __warc_download_url = None
+    __warc_path = None
     # download dir for warc files
     __local_download_dir_warc = './cc_download_warc/'
     # hosts (if None or empty list, any host is OK)
     __filter_valid_hosts = []  # example: ['elrancaguino.cl']
     # start date (if None, any date is OK as start date), as datetime
     __filter_start_date = None
     # end date (if None, any date is OK as end date)
@@ -38,21 +40,26 @@
     # if date filtering is string, e.g., if we could not detect the date of an article, we will discard the article
     __filter_strict_date = True
     # if True, the script checks whether a file has been downloaded already and uses that file instead of downloading
     # again. Note that there is no check whether the file has been downloaded completely or is valid!
     __reuse_previously_downloaded_files = True
     # continue after error
     __continue_after_error = False
+    # ignore unicode errors
+    __ignore_unicode_errors = False
+    # fetch images
+    __fetch_images = False
     # log level
     __log_level = logging.INFO
     __delete_warc_after_extraction = True
     __log_pathname_fully_extracted_warcs = None
 
     # commoncrawl.org
-    __cc_base_url = 'https://commoncrawl.s3.amazonaws.com/'
+    __cc_base_url = 'https://data.commoncrawl.org/'
+    __cc_bucket = 'commoncrawl'
     __cc_news_crawl_names = None
 
     # event handler called when an article was extracted successfully and passed all filter criteria
     __callback_on_article_extracted = None
     # event handler called when a warc file is fully processed
     __callback_on_warc_completed = None
     # if the download progress is shown
@@ -63,41 +70,45 @@
     __logger = logging.getLogger(__name__)
 
     def __setup(self):
         """
         Setup
         :return:
         """
-        if not os.path.exists(self.__local_download_dir_warc):
-            os.makedirs(self.__local_download_dir_warc)
+        os.makedirs(self.__local_download_dir_warc, exist_ok=True)
 
-        # make loggers quite
+        # make loggers quiet
         configure_logging({"LOG_LEVEL": "ERROR"})
         logging.getLogger('requests').setLevel(logging.CRITICAL)
         logging.getLogger('readability').setLevel(logging.CRITICAL)
         logging.getLogger('PIL').setLevel(logging.CRITICAL)
         logging.getLogger('newspaper').setLevel(logging.CRITICAL)
         logging.getLogger('newsplease').setLevel(logging.CRITICAL)
         logging.getLogger('urllib3').setLevel(logging.CRITICAL)
 
+        boto3.set_stream_logger('botocore', self.__log_level)
+        boto3.set_stream_logger('boto3', self.__log_level)
+        boto3.set_stream_logger('s3transfer', self.__log_level)
+
         # set own logger
         logging.basicConfig(level=self.__log_level)
         self.__logger = logging.getLogger(__name__)
         self.__logger.setLevel(self.__log_level)
 
-    def __register_fully_extracted_warc_file(self, warc_url):
+    def __register_fully_extracted_warc_file(self, warc_path):
         """
         Saves the URL warc_url in the log file for fully extracted WARC URLs
         :param warc_url:
         :return:
         """
-        with open(self.__log_pathname_fully_extracted_warcs, 'a') as log_file:
-            log_file.write(warc_url + '\n')
+        if self.__log_pathname_fully_extracted_warcs is not None:
+            with open(self.__log_pathname_fully_extracted_warcs, 'a') as log_file:
+                log_file.write(warc_path + '\n')
 
-    def __filter_record(self, warc_record, article=None):
+    def filter_record(self, warc_record, article=None):
         """
         Returns true if a record passes all tests: hosts, publishing date
         :param warc_record:
         :return: A tuple of (True or False) and an article (might be None)
         """
         # filter by host
         if self.__filter_valid_hosts:
@@ -112,15 +123,15 @@
                     break
             else:
                 return False, article
 
         # filter by date
         if self.__filter_start_date or self.__filter_end_date:
             if not article:
-                article = NewsPlease.from_warc(warc_record)
+                article = self._from_warc(warc_record)
 
             publishing_date = self.__get_publishing_date(warc_record, article)
             if not publishing_date:
                 if self.__filter_strict_date:
                     return False, article
             else:  # here we for sure have a date
                 # is article published too early?
@@ -138,39 +149,20 @@
         :return:
         """
         if hasattr(article, 'date_publish'):
             return parser.parse(article.date_publish) if isinstance(article.date_publish, str) else article.date_publish
         else:
             return None
 
-    def __get_download_url(self, name):
-        """
-        Creates a download url given the name
-        :param name:
-        :return:
-        """
-        return self.__cc_base_url + name
-
     def __get_remote_index(self):
         """
         Gets the index of news crawl files from commoncrawl.org and returns an array of names
         :return:
         """
-        # cleanup
-        subprocess.getoutput("rm tmpaws.txt")
-        # get the remote info
-        cmd = "aws s3 ls --recursive s3://commoncrawl/crawl-data/CC-NEWS/ --no-sign-request > tmpaws.txt && " \
-              "awk '{ print $4 }' tmpaws.txt && " \
-              "rm tmpaws.txt"
-        self.__logger.info('executing: %s', cmd)
-        stdout_data = subprocess.getoutput(cmd)
-        print(stdout_data)
-
-        lines = stdout_data.splitlines()
-        return lines
+        return commoncrawl_crawler.__get_remote_index()
 
     def __on_download_progress_update(self, blocknum, blocksize, totalsize):
         """
         Prints some download progress information
         :param blocknum:
         :param blocksize:
         :param totalsize:
@@ -184,38 +176,47 @@
             s = "\r%s / %s" % (size(readsofar), size(totalsize))
             sys.stdout.write(s)
             if readsofar >= totalsize:  # near the end
                 sys.stderr.write("\r")
         else:  # total size is unknown
             sys.stdout.write("\rread %s" % (size(readsofar)))
 
-    def __download(self, url):
+    def __download(self, path):
         """
         Download and save a file locally.
         :param url: Where to download from
         :return: File path name of the downloaded file
         """
-        local_filename = urllib.parse.quote_plus(url)
+        local_filename = urllib.parse.quote_plus(path)
         local_filepath = os.path.join(self.__local_download_dir_warc, local_filename)
 
         if os.path.isfile(local_filepath) and self.__reuse_previously_downloaded_files:
             self.__logger.info("found local file %s, not downloading again due to configuration", local_filepath)
             return local_filepath
         else:
             # cleanup
             try:
                 os.remove(local_filepath)
             except OSError:
                 pass
 
             # download
-            self.__logger.info('downloading %s (local: %s)', url, local_filepath)
-            urllib.request.urlretrieve(url, local_filepath, reporthook=self.__on_download_progress_update)
-            self.__logger.info('download completed, local file: %s', local_filepath)
-            return local_filepath
+            if self.__s3_client:
+                with open(local_filepath, 'wb') as file_obj:
+                    self.__s3_client.download_fileobj(self.__cc_bucket, path, file_obj)
+                return local_filepath
+            else:
+                url = self.__cc_base_url + path
+                self.__logger.info('downloading %s (local: %s)', url, local_filepath)
+                urllib.request.urlretrieve(url, local_filepath, reporthook=self.__on_download_progress_update)
+                self.__logger.info('download completed, local file: %s', local_filepath)
+                return local_filepath
+
+    def _from_warc(self, record):
+        return NewsPlease.from_warc(record, decode_errors="replace" if self.__ignore_unicode_errors else "strict", fetch_images=self.__fetch_images)
 
     def __process_warc_gz_file(self, path_name):
         """
         Iterates all transactions in one WARC file and for each transaction tries to extract an article object.
         Afterwards, each article is checked against the filter criteria and if all are passed, the function
         on_valid_article_extracted is invoked with the article object.
         :param path_name:
@@ -230,18 +231,25 @@
         with open(path_name, 'rb') as stream:
             for record in ArchiveIterator(stream):
                 try:
                     if record.rec_type == 'response':
                         counter_article_total += 1
 
                         # if the article passes filter tests, we notify the user
-                        filter_pass, article = self.__filter_record(record)
+                        try:
+                            filter_pass, article = self.filter_record(record)
+                        except (UnicodeDecodeError, EmptyResponseError):
+                            filter_pass = False
+                        if filter_pass:
+                            try:
+                                if not article:
+                                    article = self._from_warc(record)
+                            except (UnicodeDecodeError, EmptyResponseError):
+                                filter_pass = False
                         if filter_pass:
-                            if not article:
-                                article = NewsPlease.from_warc(record)
                             counter_article_passed += 1
 
                             self.__logger.info('article pass (%s; %s; %s)', article.source_domain, article.date_publish,
                                                article.title)
                             self.__callback_on_article_extracted(article)
                         else:
                             counter_article_discarded += 1
@@ -261,78 +269,91 @@
                             self.__logger.info('pass = %i, discard = %i, error = %i, total = %i',
                                                counter_article_passed,
                                                counter_article_discarded, counter_article_error, counter_article_total)
                             self.__logger.info('extraction from current WARC file started %s; %f s/article',
                                                human(start_time), secs_per_article)
                 except:
                     if self.__continue_after_error:
-                        self.__logger.error('Unexpected error: %s', sys.exc_info()[0])
+                        self.__logger.error('Unexpected error: %s (%s)', *sys.exc_info()[0:2])
+                        self.__logger.error(sys.exc_info()[2], exc_info=True)
                         counter_article_error += 1
                         pass
                     else:
                         raise
 
         # cleanup
         if self.__delete_warc_after_extraction:
             os.remove(path_name)
 
-        self.__register_fully_extracted_warc_file(self.__warc_download_url)
-        self.__callback_on_warc_completed(self.__warc_download_url, counter_article_passed, counter_article_discarded,
+        self.__register_fully_extracted_warc_file(self.__warc_path)
+        self.__callback_on_warc_completed(self.__warc_path, counter_article_passed, counter_article_discarded,
                                           counter_article_error, counter_article_total)
 
     def __run(self):
         """
         Main execution method, which consists of: get an up-to-date list of WARC files, and for each of them: download
         and extract articles. Each article is checked against a filter. Finally, for each valid article the method
         on_valid_article_extracted will be invoked after the extraction of the article has completed.
         :return:
         """
         self.__setup()
 
-        local_path_name = self.__download(self.__warc_download_url)
+        local_path_name = self.__download(self.__warc_path)
         self.__process_warc_gz_file(local_path_name)
 
-    def extract_from_commoncrawl(self, warc_download_url, callback_on_article_extracted,
+    def extract_from_commoncrawl(self, warc_path, callback_on_article_extracted,
                                  callback_on_warc_completed=None,
                                  valid_hosts=None,
                                  start_date=None, end_date=None,
                                  strict_date=True, reuse_previously_downloaded_files=True, local_download_dir_warc=None,
-                                 continue_after_error=True, show_download_progress=False,
-                                 log_level=logging.ERROR, delete_warc_after_extraction=True,
-                                 log_pathname_fully_extracted_warcs=None):
+                                 continue_after_error=True, ignore_unicode_errors=False,
+                                 show_download_progress=False, log_level=logging.ERROR, delete_warc_after_extraction=True,
+                                 log_pathname_fully_extracted_warcs=None, fetch_images=False):
         """
         Crawl and extract articles form the news crawl provided by commoncrawl.org. For each article that was extracted
         successfully the callback function callback_on_article_extracted is invoked where the first parameter is the
         article object.
         :param log_pathname_fully_extracted_warcs:
         :param delete_warc_after_extraction:
-        :param warc_download_url:
+        :param warc_path:
         :param callback_on_article_extracted:
         :param callback_on_warc_completed:
         :param valid_hosts:
         :param start_date:
         :param end_date:
         :param strict_date:
         :param reuse_previously_downloaded_files:
         :param local_download_dir_warc:
         :param continue_after_error:
         :param show_download_progress:
         :param log_level:
         :return:
         """
-        self.__warc_download_url = warc_download_url
+        self.__warc_path = warc_path
         self.__filter_valid_hosts = valid_hosts
         self.__filter_start_date = start_date
         self.__filter_end_date = end_date
         self.__filter_strict_date = strict_date
         if local_download_dir_warc:
             self.__local_download_dir_warc = local_download_dir_warc
         self.__reuse_previously_downloaded_files = reuse_previously_downloaded_files
         self.__continue_after_error = continue_after_error
+        self.__ignore_unicode_errors = ignore_unicode_errors
+        self.__fetch_images = fetch_images
         self.__callback_on_article_extracted = callback_on_article_extracted
         self.__callback_on_warc_completed = callback_on_warc_completed
         self.__show_download_progress = show_download_progress
         self.__log_level = log_level
         self.__delete_warc_after_extraction = delete_warc_after_extraction
         self.__log_pathname_fully_extracted_warcs = log_pathname_fully_extracted_warcs
 
+        self.__s3_client = None
+        try:
+            s3_client = boto3.client('s3')
+            # Verify access to commoncrawl bucket
+            s3_client.head_bucket(Bucket=self.__cc_bucket)
+            self.__s3_client = s3_client
+        except (botocore.exceptions.ClientError, botocore.exceptions.NoCredentialsError):
+            self.__logger.info('Failed to read %s bucket, using monthly WARC file listings', self.__cc_bucket)
+
+
         self.__run()
```

### Comparing `news-please-1.5.3/newsplease/crawler/items.py` & `news-please-1.5.33/newsplease/crawler/items.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/download_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/download_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/gdelt_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/gdelt_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/recursive_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/recursive_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/recursive_sitemap_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/recursive_sitemap_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/rss_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/rss_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/crawler/spiders/sitemap_crawler.py` & `news-please-1.5.33/newsplease/crawler/spiders/sitemap_crawler.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/examples/commoncrawl.py` & `news-please-1.5.33/newsplease/examples/commoncrawl.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 """
 This scripts downloads WARC files from commoncrawl.org's news crawl and extracts articles from these files. You can
 define filter criteria that need to be met (see YOUR CONFIG section), otherwise an article is discarded. Currently, the
 script stores the extracted articles in JSON files, but this behaviour can be adapted to your needs in the method
 on_valid_article_extracted. To speed up the crawling and extraction process, the script supports multiprocessing. You can
 control the number of processes with the parameter my_number_of_extraction_processes.
 
-You can also crawl and extract articles programmatically, i.e., from within your own code, by using the class
-CommonCrawlCrawler provided in newsplease.crawler.commoncrawl_crawler.py
-
-In case the script crashes and contains a log message in the beginning that states that only 1 file on AWS storage
-was found, make sure that awscli was correctly installed. You can check that by running aws --version from a terminal.
-If aws is not installed, you can (on Ubuntu) also install it using sudo apt-get install awscli.
+You can also crawl and extract articles programmatically, i.e., from within
+your own code, by using the class CommonCrawlCrawler or the function
+commoncrawl_crawler.crawl_from_commoncrawl(...) provided in
+newsplease.crawler.commoncrawl_crawler.py. In this case there is also the
+possibility of passing in a your own subclass of CommonCrawlExtractor as
+extractor_cls=... . One use case here is that your subclass can customise
+filtering by overriding `.filter_record(...)`.
 
 This script uses relative imports to ensure that the latest, local version of news-please is used, instead of the one
 that might have been installed with pip. Hence, you must run this script following this workflow.
 git clone https://github.com/fhamborg/news-please.git
 cd news-please
 python3 -m newsplease.examples.commoncrawl
+
+Note that by default the script does not extract main images since they are not contained
+WARC files. You can enable extraction of main images by setting `my_fetch_images=True`
 """
 import hashlib
 import json
 import logging
 import os
 import sys
 import datetime
@@ -41,16 +45,22 @@
 my_local_download_dir_article = './cc_download_articles/'
 # hosts (if None or empty list, any host is OK)
 my_filter_valid_hosts = []  # example: ['elrancaguino.cl']
 # start date (if None, any date is OK as start date), as datetime
 my_filter_start_date = None  # datetime.datetime(2016, 1, 1)
 # end date (if None, any date is OK as end date), as datetime
 my_filter_end_date = None  # datetime.datetime(2016, 12, 31)
-# if date filtering is strict and news-please could not detect the date of an article, the article will be discarded
+# Only .warc files published within [my_warc_files_start_date, my_warc_files_end_date) will be downloaded.
+# Note that the date a warc file has been published does not imply it contains only news
+# articles from that date. Instead, you must assume that the warc file can contain articles
+# from ANY time before the warc file was published, e.g., a warc file published in August 2020
+# may contain news articles from December 2016.
 my_warc_files_start_date = None # example: datetime.datetime(2020, 3, 1)
+my_warc_files_end_date = None # example: datetime.datetime(2020, 3, 2)
+# if date filtering is strict and news-please could not detect the date of an article, the article will be discarded
 my_filter_strict_date = True
 # if True, the script checks whether a file has been downloaded already and uses that file instead of downloading
 # again. Note that there is no check whether the file has been downloaded completely or is valid!
 my_reuse_previously_downloaded_files = True
 # continue after error
 my_continue_after_error = True
 # show the progress of downloading the WARC files
@@ -62,43 +72,47 @@
 # number of extraction processes
 my_number_of_extraction_processes = 1
 # if True, the WARC file will be deleted after all articles have been extracted from it
 my_delete_warc_after_extraction = True
 # if True, will continue extraction from the latest fully downloaded but not fully extracted WARC files and then
 # crawling new WARC files. This assumes that the filter criteria have not been changed since the previous run!
 my_continue_process = True
+# if True, will crawl and extract main image of each article. Note that the WARC files
+# do not contain any images, so that news-please will crawl the current image from
+# the articles online webpage, if this option is enabled.
+my_fetch_images = False
+# if True, just list the WARC files to be processed, but do not actually download and process them
+my_dry_run=False
 ############ END YOUR CONFIG #########
 
 
 # logging
 logging.basicConfig(level=my_log_level)
 __logger = logging.getLogger(__name__)
 
 
 def __setup__():
     """
     Setup
     :return:
     """
-    if not os.path.exists(my_local_download_dir_article):
-        os.makedirs(my_local_download_dir_article)
+    os.makedirs(my_local_download_dir_article, exist_ok=True)
 
 
 def __get_pretty_filepath(path, article):
     """
     Pretty might be an euphemism, but this function tries to avoid too long filenames, while keeping some structure.
     :param path:
     :param name:
     :return:
     """
     short_filename = hashlib.sha256(article.filename.encode()).hexdigest()
     sub_dir = article.source_domain
     final_path = os.path.join(path, sub_dir)
-    if not os.path.exists(final_path):
-        os.makedirs(final_path)
+    os.makedirs(final_path, exist_ok=True)
     return os.path.join(final_path, short_filename + '.json')
 
 
 def on_valid_article_extracted(article):
     """
     This function will be invoked for each article that was extracted successfully from the archived data and that
     satisfies the filter criteria.
@@ -129,44 +143,47 @@
     """
     pass
 
 
 def main():
     global my_local_download_dir_warc
     global my_local_download_dir_article
-    delete_warc_after_extraction = False
+    global my_delete_warc_after_extraction
     global my_number_of_extraction_processes
 
     if len(sys.argv) >= 2:
         my_local_download_dir_warc = sys.argv[1]
     if len(sys.argv) >= 3:
         my_local_download_dir_article = sys.argv[2]
     if len(sys.argv) >= 4:
-        delete_warc_after_extraction = sys.argv[3] == "delete"
+        my_delete_warc_after_extraction = sys.argv[3] == "delete"
     if len(sys.argv) >= 5:
         my_number_of_extraction_processes = int(sys.argv[4])
 
     print("my_local_download_dir_warc=" + my_local_download_dir_warc)
     print("my_local_download_dir_article=" + my_local_download_dir_article)
-    print("delete_warc_after_extraction=" + str(delete_warc_after_extraction))
+    print("my_delete_warc_after_extraction=" + str(my_delete_warc_after_extraction))
     print("my_number_of_extraction_processes=" + str(my_number_of_extraction_processes))
 
     __setup__()
     commoncrawl_crawler.crawl_from_commoncrawl(on_valid_article_extracted,
                                                callback_on_warc_completed=callback_on_warc_completed,
                                                valid_hosts=my_filter_valid_hosts,
                                                start_date=my_filter_start_date,
                                                end_date=my_filter_end_date,
                                                warc_files_start_date=my_warc_files_start_date,
+                                               warc_files_end_date=my_warc_files_end_date,
                                                strict_date=my_filter_strict_date,
                                                reuse_previously_downloaded_files=my_reuse_previously_downloaded_files,
                                                local_download_dir_warc=my_local_download_dir_warc,
                                                continue_after_error=my_continue_after_error,
                                                show_download_progress=my_show_download_progress,
                                                number_of_extraction_processes=my_number_of_extraction_processes,
                                                log_level=my_log_level,
-                                               delete_warc_after_extraction=delete_warc_after_extraction,
-                                               continue_process=True)
+                                               delete_warc_after_extraction=my_delete_warc_after_extraction,
+                                               continue_process=True,
+                                               fetch_images=my_fetch_images,
+                                               dry_run=my_dry_run)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `news-please-1.5.3/newsplease/examples/downloadfromfile.py` & `news-please-1.5.33/newsplease/examples/downloadfromfile.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/examples/downloadfromurl.py` & `news-please-1.5.33/newsplease/examples/downloadfromurl.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/helper.py` & `news-please-1.5.33/newsplease/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,18 @@
             self,
             cfg_heuristics,
             cfg_savepath,
             relative_to_path,
             format_relative_path,
             sites_object,
             crawler_class,
+            crawler_item_class,
             working_path
     ):
         if not isinstance(sites_object[0]["url"], list):
             self.heuristics = Heuristics(
                 cfg_heuristics, sites_object, crawler_class)
         self.url_extractor = UrlExtractor()
         self.savepath_parser = SavepathParser(
             cfg_savepath, relative_to_path, format_relative_path, self, working_path)
+        self.crawler_item_class = crawler_item_class
         self.parse_crawler = ParseCrawler(self)
```

### Comparing `news-please-1.5.3/newsplease/helper_classes/heuristics.py` & `news-please-1.5.33/newsplease/helper_classes/heuristics.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/helper_classes/parse_crawler.py` & `news-please-1.5.33/newsplease/helper_classes/parse_crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 import logging
 import re
 import time
 
 import scrapy
 
-from ..crawler.items import NewscrawlerItem
-
 # to improve performance, regex statements are compiled only once per module
 re_html = re.compile('text/html')
 
 
 class ParseCrawler(object):
     """
     Helper class for the crawler's parse methods.
@@ -53,15 +51,16 @@
     ):
         timestamp = time.strftime('%Y-%m-%d %H:%M:%S',
                                   time.gmtime(time.time()))
 
         relative_local_path = self.helper.savepath_parser \
             .get_savepath(response.url)
 
-        article = NewscrawlerItem()
+        # Instantiate the crawler item class defined in the configuration
+        article = self.helper.crawler_item_class()
         article['local_path'] = self.helper.savepath_parser \
             .get_formatted_relative_path(relative_local_path)
         article['filename'] = self.helper.savepath_parser.get_filename(article['local_path'])
         article['abs_local_path'] = self.helper.savepath_parser \
             .get_abs_path(relative_local_path)
         article['modified_date'] = timestamp
         article['download_date'] = timestamp
```

### Comparing `news-please-1.5.3/newsplease/helper_classes/savepath_parser.py` & `news-please-1.5.33/newsplease/helper_classes/savepath_parser.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/helper_classes/sub_classes/heuristics_manager.py` & `news-please-1.5.33/newsplease/helper_classes/sub_classes/heuristics_manager.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/helper_classes/url_extractor.py` & `news-please-1.5.33/newsplease/helper_classes/url_extractor.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/article_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/article_extractor.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,32 +14,42 @@
 
     def __init__(self, extractor_list):
         """
         Initializes all the extractors, comparers and the cleaner.
 
         :param extractor_list: List of strings containing all extractors to be initialized.
         """
+        def proc_instance(instance):
+            if instance is not None:
+                self.log.info('Extractor initialized: %s', extractor)
+                self.extractor_list.append(instance)
+            else:
+                self.log.error("Misconfiguration: An unknown Extractor was found and"
+                               " will be ignored: %s", extractor)
+
         self.log = logging.getLogger(__name__)
         self.extractor_list = []
         for extractor in extractor_list:
 
-            module = importlib.import_module(__package__ + '.extractors.' + extractor)
+            if isinstance(extractor, tuple):
+                extractor_module = extractor[0]
+            else:
+                extractor_module = extractor
+
+            module = importlib.import_module(__package__ + '.extractors.' + extractor_module)
+
+            if isinstance(extractor, tuple):
+                proc_instance(getattr(module, extractor[1], None)())
+            else:
+                # check module for subclasses of AbstractExtractor
+                for member in inspect.getmembers(module, inspect.isclass):
+                    if issubclass(member[1], AbstractExtractor) and member[0] != 'AbstractExtractor':
 
-            # check module for subclasses of AbstractExtractor
-            for member in inspect.getmembers(module, inspect.isclass):
-                if issubclass(member[1], AbstractExtractor) and member[0] != 'AbstractExtractor':
-
-                    # instantiate extractor
-                    instance = getattr(module, member[0], None)()
-                    if instance is not None:
-                        self.log.info('Extractor initialized: %s', extractor)
-                        self.extractor_list.append(instance)
-                    else:
-                        self.log.error("Misconfiguration: An unknown Extractor was found and"
-                                       " will be ignored: %s", extractor)
+                        # instantiate extractor
+                        proc_instance(getattr(module, member[0], None)())
 
         self.cleaner = Cleaner()
         self.comparer = Comparer()
 
     def extract(self, item):
         """Runs the HTML-response trough a list of initialized extractors, a cleaner and compares the results.
```

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/cleaner.py` & `news-please-1.5.33/newsplease/pipeline/extractor/cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         """Removes html-tags from extracted data.
 
         :param arg: A string, the string which shall be cleaned
         :return: A string, the cleaned string
         """
 
         if len(arg) > 0:
-            raw = html.fromstring(arg)
+            try:
+                raw = html.fromstring(arg)
+            except ValueError:
+                raw = html.fromstring(arg.encode("utf-8"))
             return raw.text_content().strip()
 
         return arg
 
     def delete_whitespaces(self, arg):
         """Removes newlines, tabs and whitespaces at the beginning, the end and if there is more than one.
```

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_Language.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_Language.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_author.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_author.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_date.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_date.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_description.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_description.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_text.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_text.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_title.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_title.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/comparer/comparer_topimage.py` & `news-please-1.5.33/newsplease/pipeline/extractor/comparer/comparer_topimage.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/extractors/abstract_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/extractors/abstract_extractor.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/extractors/date_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/extractors/date_extractor.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/extractors/lang_detect_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/extractors/lang_detect_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,18 @@
         self.langcode_pattern = re.compile(r'\b[a-zA-Z]{2}(?=([-_]|\b))')
 
     def _language(self, item):
         """Returns the language of the extracted article by analyzing metatags and inspecting the visible text
         with langdetect"""
 
         response = item['spider_response'].body
-        root = html.fromstring(response)
+        try:
+            root = html.fromstring(response)
+        except ValueError:
+            root = html.fromstring(response.encode("utf-8"))
 
         # Check for lang-attributes
         lang = root.get('lang')
 
         if lang is None:
             lang = root.get('xml:lang')
 
@@ -44,16 +47,22 @@
                 lang = meta[0].get('content')
 
         # Look for <article> elements and inspect the one with the largest payload with langdetect
         if lang is None:
             article_list = []
             for article in root.xpath('//article'):
                 article_list.append(re.sub(r'\s+', ' ', article.text_content().strip()))
-                if len(article_list) > 0:
-                    lang = detect(max(article_list))
+                longest_articles = sorted(article_list, key=lambda article: len(article), reverse=True)
+                for article in longest_articles:
+                    try:
+                        lang = detect(article)
+                    except LangDetectException:
+                        continue
+                    else:
+                        break
 
         # Analyze the whole body with langdetect
         if lang is None:
             try:
                 lang = detect(root.text_content().strip())
             except LangDetectException:
                 pass
```

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/extractors/newspaper_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/extractors/newspaper_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,39 @@
     a subclass of ExtractorsInterface
     """
 
     def __init__(self):
         self.log = logging.getLogger(__name__)
         self.name = "newspaper"
 
+    def _article_kwargs(self):
+        return {}
+
     def extract(self, item):
         """Creates an instance of Article without a Download and returns an ArticleCandidate with the results of
         parsing the HTML-Code.
 
         :param item: A NewscrawlerItem to parse.
         :return: ArticleCandidate containing the recovered article data.
         """
         article_candidate = ArticleCandidate()
         article_candidate.extractor = self._name()
 
-        article = Article('')
-        article.set_html(item['spider_response'].body)
+        article = Article('', **self._article_kwargs())
+        # old version of newspaper2k
+        # article.set_html(item['spider_response'].body)
+        # new version
+        article.download(input_html=item['spider_response'].body, title=item['html_title'].decode())
         article.parse()
         article_candidate.title = article.title
         article_candidate.description = article.meta_description
         article_candidate.text = article.text
         article_candidate.topimage = article.top_image
         article_candidate.author = article.authors
-        if article.publish_date is not None:
+        if article.publish_date:
             try:
                 article_candidate.publish_date = article.publish_date.strftime('%Y-%m-%d %H:%M:%S')
             except ValueError as exception:
                 self.log.debug('%s: Newspaper failed to extract the date in the supported format,'
                               'Publishing date set to None' % item['url'])
         article_candidate.language = article.meta_lang
```

### Comparing `news-please-1.5.3/newsplease/pipeline/extractor/extractors/readability_extractor.py` & `news-please-1.5.33/newsplease/pipeline/extractor/extractors/readability_extractor.py`

 * *Files identical despite different names*

### Comparing `news-please-1.5.3/newsplease/pipeline/pipelines.py` & `news-please-1.5.33/newsplease/pipeline/pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,16 +520,15 @@
     # Save the html and filename to the local storage folder
     def process_item(self, item, spider):
         # Add a log entry confirming the save
         self.log.info("Saving HTML to %s", item['abs_local_path'])
 
         # Ensure path exists
         dir_ = os.path.dirname(item['abs_local_path'])
-        if not os.path.exists(dir_):
-            os.makedirs(dir_)
+        os.makedirs(dir_, exist_ok=True)
 
         # Write raw html to local file system
         with open(item['abs_local_path'], 'wb') as file_:
             file_.write(item['spider_response'].body)
 
         return item
 
@@ -546,16 +545,15 @@
         file_path = item['abs_local_path'] + '.json'
 
         # Add a log entry confirming the save
         self.log.info("Saving JSON to %s", file_path)
 
         # Ensure path exists
         dir_ = os.path.dirname(item['abs_local_path'])
-        if not os.path.exists(dir_):
-            os.makedirs(dir_)
+        os.makedirs(dir_, exist_ok=True)
 
         # Write JSON to local file system
         with open(file_path, 'w') as file_:
             json.dump(ExtractedInformationStorage.extract_relevant_info(item), file_, ensure_ascii=False)
 
         return item
```

### Comparing `news-please-1.5.3/newsplease/single_crawler.py` & `news-please-1.5.33/newsplease/single_crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 cur_path = os.path.dirname(os.path.realpath(__file__))
 par_path = os.path.dirname(cur_path)
 sys.path.append(cur_path)
 sys.path.append(par_path)
 from newsplease.config import CrawlerConfig
 from newsplease.config import JsonConfig
 from newsplease.helper import Helper
+from newsplease.helper_classes.class_loader import ClassLoader
+from newsplease.crawler.items import NewscrawlerItem
 
 try:
     from _thread import start_new_thread
 except ImportError:
     from thread import start_new_thread
 from twisted.internet.error import ReactorAlreadyRunning
 
@@ -118,20 +120,29 @@
 
         if not self.cfg.section('Files')['relative_to_start_processes_file']:
             relative_to_path = os.path.dirname(self.cfg_file_path)
         else:
             # absolute dir this script is in
             relative_to_path = os.path.dirname(__file__)
 
+        news_item_class_name = self.cfg.section("Scrapy").get("item_class", None)
+        if not news_item_class_name:
+            news_item_class = NewscrawlerItem
+        else:
+            news_item_class = ClassLoader.from_string(news_item_class_name)
+            if not issubclass(news_item_class, NewscrawlerItem):
+                raise ImportError("ITEM_CLASS must be a subclass of NewscrawlerItem")
+
         self.helper = Helper(self.cfg.section('Heuristics'),
                              self.cfg.section("Files")["local_data_directory"],
                              relative_to_path,
                              self.cfg.section('Files')['format_relative_path'],
                              sites,
                              crawler_class,
+                             news_item_class,
                              self.cfg.get_working_path())
 
         self.__scrapy_options = self.cfg.get_scrapy_options()
 
         self.update_jobdir(site)
 
         # make sure the crawler does not resume crawling
```

### Comparing `news-please-1.5.3/setup.py` & `news-please-1.5.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='news-please',
-      version='1.5.03',
+      version='1.5.33',
       description="news-please is an open source easy-to-use news extractor that just works.",
       long_description="""\
 news-please is an open source, easy-to-use news crawler that extracts structured information from almost any news website. It can follow recursively internal hyperlinks and read RSS feeds to fetch both most recent and also old, archived articles. You only need to provide the root URL of the news website. Furthermore, its API allows developers to access the exctraction functionality within their software. news-please also implements a workflow optimized for the news archive provided by commoncrawl.org, allowing users to efficiently crawl and extract news articles including various filter options.""",
       classifiers=[
           'Development Status :: 4 - Beta',
           'Environment :: Console',
           'Intended Audience :: Developers',
@@ -44,17 +44,18 @@
           'dotmap>=1.2.17',
           'readability-lxml>=0.6.2',
           'PyDispatcher>=2.0.5',
           'warcio>=1.3.3',
           'ago>=0.0.9',
           'six>=1.10.0',
           'lxml>=3.3.5',
-          'awscli>=1.11.117',
           'hurry.filesize>=0.9',
-          'bs4'
+          'bs4',
+          'cchardet>=2.1.7',
+          'boto3'
       ],
       extras_require={
           ':sys_platform == "win32"': [
               'pywin32>=220'
           ]
       },
       entry_points={
```

