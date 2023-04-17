# Comparing `tmp/piedomains-0.0.8.tar.gz` & `tmp/piedomains-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piedomains-0.0.8.tar", last modified: Sun Jan 29 17:00:37 2023, max compression
+gzip compressed data, was "piedomains-0.0.9.tar", last modified: Sat Feb  4 15:47:12 2023, max compression
```

## Comparing `piedomains-0.0.8.tar` & `piedomains-0.0.9.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.482570 piedomains-0.0.8/
--rw-r--r--   0 rchint1    (501) staff       (20)     1105 2022-05-03 21:52:04.000000 piedomains-0.0.8/LICENSE
--rw-r--r--   0 rchint1    (501) staff       (20)     5216 2023-01-29 17:00:37.482767 piedomains-0.0.8/PKG-INFO
--rw-r--r--   0 rchint1    (501) staff       (20)     4295 2023-01-29 16:51:29.000000 piedomains-0.0.8/README.rst
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.212317 piedomains-0.0.8/piedomains/
--rw-r--r--   0 rchint1    (501) staff       (20)       66 2022-05-03 20:55:09.000000 piedomains-0.0.8/piedomains/__init__.py
--rw-r--r--   0 rchint1    (501) staff       (20)     1087 2022-05-03 20:43:19.000000 piedomains-0.0.8/piedomains/base.py
--rw-r--r--   0 rchint1    (501) staff       (20)      530 2022-05-03 20:54:35.000000 piedomains-0.0.8/piedomains/domain.py
--rw-r--r--   0 rchint1    (501) staff       (20)       98 2022-04-30 14:27:41.000000 piedomains-0.0.8/piedomains/logging.py
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.162515 piedomains-0.0.8/piedomains/model/
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.163070 piedomains-0.0.8/piedomains/model/calibrate/
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.326628 piedomains-0.0.8/piedomains/model/calibrate/text/
--rw-------   0 rchint1    (501) staff       (20)     2023 2023-01-27 23:23:13.000000 piedomains-0.0.8/piedomains/model/calibrate/text/adv.sav
--rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:14.000000 piedomains-0.0.8/piedomains/model/calibrate/text/aggressive.sav
--rw-------   0 rchint1    (501) staff       (20)     1575 2023-01-27 23:23:14.000000 piedomains-0.0.8/piedomains/model/calibrate/text/alcohol.sav
--rw-------   0 rchint1    (501) staff       (20)      863 2023-01-27 23:23:14.000000 piedomains-0.0.8/piedomains/model/calibrate/text/anonvpn.sav
--rw-------   0 rchint1    (501) staff       (20)     2271 2023-01-27 23:23:15.000000 piedomains-0.0.8/piedomains/model/calibrate/text/automobile.sav
--rw-------   0 rchint1    (501) staff       (20)      807 2023-01-27 23:23:15.000000 piedomains-0.0.8/piedomains/model/calibrate/text/costtraps.sav
--rw-------   0 rchint1    (501) staff       (20)     1991 2023-01-27 23:23:15.000000 piedomains-0.0.8/piedomains/model/calibrate/text/dating.sav
--rw-------   0 rchint1    (501) staff       (20)     1823 2023-01-27 23:23:16.000000 piedomains-0.0.8/piedomains/model/calibrate/text/downloads.sav
--rw-------   0 rchint1    (501) staff       (20)     1895 2023-01-27 23:23:16.000000 piedomains-0.0.8/piedomains/model/calibrate/text/drugs.sav
--rw-------   0 rchint1    (501) staff       (20)      711 2023-01-27 23:23:16.000000 piedomains-0.0.8/piedomains/model/calibrate/text/dynamic.sav
--rw-------   0 rchint1    (501) staff       (20)     2759 2023-01-27 23:23:17.000000 piedomains-0.0.8/piedomains/model/calibrate/text/education.sav
--rw-------   0 rchint1    (501) staff       (20)     2695 2023-01-27 23:23:17.000000 piedomains-0.0.8/piedomains/model/calibrate/text/finance.sav
--rw-------   0 rchint1    (501) staff       (20)     1511 2023-01-27 23:23:17.000000 piedomains-0.0.8/piedomains/model/calibrate/text/fortunetelling.sav
--rw-------   0 rchint1    (501) staff       (20)     2631 2023-01-27 23:23:18.000000 piedomains-0.0.8/piedomains/model/calibrate/text/forum.sav
--rw-------   0 rchint1    (501) staff       (20)     2631 2023-01-27 23:23:18.000000 piedomains-0.0.8/piedomains/model/calibrate/text/gamble.sav
--rw-------   0 rchint1    (501) staff       (20)     1671 2023-01-27 23:23:18.000000 piedomains-0.0.8/piedomains/model/calibrate/text/government.sav
--rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:19.000000 piedomains-0.0.8/piedomains/model/calibrate/text/hacking.sav
--rw-------   0 rchint1    (501) staff       (20)     3399 2023-01-27 23:23:19.000000 piedomains-0.0.8/piedomains/model/calibrate/text/hobby.sav
--rw-------   0 rchint1    (501) staff       (20)     1127 2023-01-27 23:23:19.000000 piedomains-0.0.8/piedomains/model/calibrate/text/homestyle.sav
--rw-------   0 rchint1    (501) staff       (20)     1863 2023-01-27 23:23:20.000000 piedomains-0.0.8/piedomains/model/calibrate/text/hospitals.sav
--rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:20.000000 piedomains-0.0.8/piedomains/model/calibrate/text/imagehosting.sav
--rw-------   0 rchint1    (501) staff       (20)     1447 2023-01-27 23:23:20.000000 piedomains-0.0.8/piedomains/model/calibrate/text/isp.sav
--rw-------   0 rchint1    (501) staff       (20)     2119 2023-01-27 23:23:21.000000 piedomains-0.0.8/piedomains/model/calibrate/text/jobsearch.sav
--rw-------   0 rchint1    (501) staff       (20)     1095 2023-01-27 23:23:21.000000 piedomains-0.0.8/piedomains/model/calibrate/text/library.sav
--rw-------   0 rchint1    (501) staff       (20)     1255 2023-01-27 23:23:22.000000 piedomains-0.0.8/piedomains/model/calibrate/text/military.sav
--rw-------   0 rchint1    (501) staff       (20)     1727 2023-01-27 23:23:22.000000 piedomains-0.0.8/piedomains/model/calibrate/text/models.sav
--rw-------   0 rchint1    (501) staff       (20)     2247 2023-01-27 23:23:22.000000 piedomains-0.0.8/piedomains/model/calibrate/text/movies.sav
--rw-------   0 rchint1    (501) staff       (20)     2791 2023-01-27 23:23:23.000000 piedomains-0.0.8/piedomains/model/calibrate/text/music.sav
--rw-------   0 rchint1    (501) staff       (20)     3495 2023-01-27 23:23:23.000000 piedomains-0.0.8/piedomains/model/calibrate/text/news.sav
--rw-------   0 rchint1    (501) staff       (20)     1087 2023-01-27 23:23:23.000000 piedomains-0.0.8/piedomains/model/calibrate/text/podcasts.sav
--rw-------   0 rchint1    (501) staff       (20)     2087 2023-01-27 23:23:24.000000 piedomains-0.0.8/piedomains/model/calibrate/text/politics.sav
--rw-------   0 rchint1    (501) staff       (20)     4999 2023-01-27 23:23:24.000000 piedomains-0.0.8/piedomains/model/calibrate/text/porn.sav
--rw-------   0 rchint1    (501) staff       (20)     2535 2023-01-27 23:23:24.000000 piedomains-0.0.8/piedomains/model/calibrate/text/radiotv.sav
--rw-------   0 rchint1    (501) staff       (20)     4799 2023-01-27 23:23:25.000000 piedomains-0.0.8/piedomains/model/calibrate/text/recreation.sav
--rw-------   0 rchint1    (501) staff       (20)     2343 2023-01-27 23:23:25.000000 piedomains-0.0.8/piedomains/model/calibrate/text/redirector.sav
--rw-------   0 rchint1    (501) staff       (20)     2279 2023-01-27 23:23:25.000000 piedomains-0.0.8/piedomains/model/calibrate/text/religion.sav
--rw-------   0 rchint1    (501) staff       (20)      863 2023-01-27 23:23:25.000000 piedomains-0.0.8/piedomains/model/calibrate/text/remotecontrol.sav
--rw-------   0 rchint1    (501) staff       (20)     1223 2023-01-27 23:23:26.000000 piedomains-0.0.8/piedomains/model/calibrate/text/ringtones.sav
--rw-------   0 rchint1    (501) staff       (20)     1735 2023-01-27 23:23:26.000000 piedomains-0.0.8/piedomains/model/calibrate/text/science.sav
--rw-------   0 rchint1    (501) staff       (20)     1479 2023-01-27 23:23:26.000000 piedomains-0.0.8/piedomains/model/calibrate/text/searchengines.sav
--rw-------   0 rchint1    (501) staff       (20)     1351 2023-01-27 23:23:27.000000 piedomains-0.0.8/piedomains/model/calibrate/text/sex.sav
--rw-------   0 rchint1    (501) staff       (20)     5479 2023-01-27 23:23:27.000000 piedomains-0.0.8/piedomains/model/calibrate/text/shopping.sav
--rw-------   0 rchint1    (501) staff       (20)     1439 2023-01-27 23:23:27.000000 piedomains-0.0.8/piedomains/model/calibrate/text/socialnet.sav
--rw-------   0 rchint1    (501) staff       (20)     2215 2023-01-27 23:23:28.000000 piedomains-0.0.8/piedomains/model/calibrate/text/spyware.sav
--rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:28.000000 piedomains-0.0.8/piedomains/model/calibrate/text/tracker.sav
--rw-------   0 rchint1    (501) staff       (20)      839 2023-01-27 23:23:28.000000 piedomains-0.0.8/piedomains/model/calibrate/text/updatesites.sav
--rw-------   0 rchint1    (501) staff       (20)     1375 2023-01-27 23:23:29.000000 piedomains-0.0.8/piedomains/model/calibrate/text/urlshortener.sav
--rw-------   0 rchint1    (501) staff       (20)     1095 2023-01-27 23:23:29.000000 piedomains-0.0.8/piedomains/model/calibrate/text/violence.sav
--rw-------   0 rchint1    (501) staff       (20)     1375 2023-01-27 23:23:29.000000 piedomains-0.0.8/piedomains/model/calibrate/text/warez.sav
--rw-------   0 rchint1    (501) staff       (20)     1511 2023-01-27 23:23:30.000000 piedomains-0.0.8/piedomains/model/calibrate/text/weapons.sav
--rw-------   0 rchint1    (501) staff       (20)     1671 2023-01-27 23:23:30.000000 piedomains-0.0.8/piedomains/model/calibrate/text/webmail.sav
--rw-------   0 rchint1    (501) staff       (20)      967 2023-01-27 23:23:30.000000 piedomains-0.0.8/piedomains/model/calibrate/text/webphone.sav
--rw-------   0 rchint1    (501) staff       (20)     1927 2023-01-27 23:23:31.000000 piedomains-0.0.8/piedomains/model/calibrate/text/webradio.sav
--rw-------   0 rchint1    (501) staff       (20)     1255 2023-01-27 23:23:31.000000 piedomains-0.0.8/piedomains/model/calibrate/text/webtv.sav
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.468848 piedomains-0.0.8/piedomains/notebooks/
--rw-r--r--   0 rchint1    (501) staff       (20)     2217 2022-04-30 13:42:53.000000 piedomains-0.0.8/piedomains/notebooks/01_get_shallalist.ipynb
--rwxr-xr-x   0 rchint1    (501) staff       (20)     5728 2022-04-30 13:42:53.000000 piedomains-0.0.8/piedomains/notebooks/01_scrape_webpages.ipynb
--rw-r--r--   0 rchint1    (501) staff       (20)     3590 2022-04-30 13:42:53.000000 piedomains-0.0.8/piedomains/notebooks/01a_scrape_stratified_random_sample.ipynb
--rw-r--r--   0 rchint1    (501) staff       (20)     4951 2022-10-28 19:01:46.000000 piedomains-0.0.8/piedomains/notebooks/01b_scraper_webpages_all.ipynb
--rw-r--r--   0 rchint1    (501) staff       (20)    22826 2022-10-28 19:01:46.000000 piedomains-0.0.8/piedomains/notebooks/01c_upload_to_dataverse.ipynb
--rwxr-xr-x   0 rchint1    (501) staff       (20)    14386 2022-04-30 13:42:53.000000 piedomains-0.0.8/piedomains/notebooks/02_parse_html_data.ipynb
--rwxr-xr-x   0 rchint1    (501) staff       (20)   178111 2022-10-28 22:57:19.000000 piedomains-0.0.8/piedomains/notebooks/03_data_clean_up.ipynb
--rwxr-xr-x   0 rchint1    (501) staff       (20)   465526 2022-10-28 22:56:48.000000 piedomains-0.0.8/piedomains/notebooks/04_train_model.ipynb
--rw-------   0 rchint1    (501) staff       (20)   126099 2023-01-27 23:22:13.000000 piedomains-0.0.8/piedomains/notebooks/05_text_calibrate_isotonic.ipynb
--rw-------   0 rchint1    (501) staff       (20)  3055216 2023-01-29 16:57:25.000000 piedomains-0.0.8/piedomains/notebooks/06_preprocessing_images.ipynb
--rw-------   0 rchint1    (501) staff       (20)   586681 2023-01-29 16:57:53.000000 piedomains-0.0.8/piedomains/notebooks/07_train_images.ipynb
--rw-r--r--   0 rchint1    (501) staff       (20)    39074 2022-10-28 19:01:46.000000 piedomains-0.0.8/piedomains/notebooks/archive-upload-screenshot-to-dataverse.ipynb
--rw-r--r--   0 rchint1    (501) staff       (20)     8281 2023-01-29 16:51:11.000000 piedomains-0.0.8/piedomains/pydomain.py
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.481673 piedomains-0.0.8/piedomains/tests/
--rw-r--r--   0 rchint1    (501) staff       (20)      342 2022-05-03 21:02:34.000000 piedomains-0.0.8/piedomains/tests/__init__.py
--rw-r--r--   0 rchint1    (501) staff       (20)      853 2022-05-04 14:11:27.000000 piedomains-0.0.8/piedomains/tests/test_010_pred_domain.py
--rw-r--r--   0 rchint1    (501) staff       (20)     1411 2023-01-29 00:45:48.000000 piedomains-0.0.8/piedomains/utils.py
-drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-01-29 17:00:37.220802 piedomains-0.0.8/piedomains.egg-info/
--rw-r--r--   0 rchint1    (501) staff       (20)     5216 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/PKG-INFO
--rw-r--r--   0 rchint1    (501) staff       (20)     3458 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/SOURCES.txt
--rw-r--r--   0 rchint1    (501) staff       (20)        1 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/dependency_links.txt
--rw-r--r--   0 rchint1    (501) staff       (20)       54 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/entry_points.txt
--rw-r--r--   0 rchint1    (501) staff       (20)      132 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/requires.txt
--rw-r--r--   0 rchint1    (501) staff       (20)       11 2023-01-29 17:00:37.000000 piedomains-0.0.8/piedomains.egg-info/top_level.txt
--rw-r--r--   0 rchint1    (501) staff       (20)       88 2023-01-29 17:00:37.486595 piedomains-0.0.8/setup.cfg
--rw-r--r--   0 rchint1    (501) staff       (20)     5136 2023-01-29 16:58:17.000000 piedomains-0.0.8/setup.py
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:12.424000 piedomains-0.0.9/
+-rw-r--r--   0 rchint1    (501) staff       (20)     1105 2022-05-03 21:52:04.000000 piedomains-0.0.9/LICENSE
+-rw-r--r--   0 rchint1    (501) staff       (20)     7934 2023-02-04 15:47:12.424194 piedomains-0.0.9/PKG-INFO
+-rw-r--r--   0 rchint1    (501) staff       (20)     7013 2023-02-04 15:38:22.000000 piedomains-0.0.9/README.rst
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:10.894014 piedomains-0.0.9/piedomains/
+-rw-r--r--   0 rchint1    (501) staff       (20)      127 2023-02-04 14:24:11.000000 piedomains-0.0.9/piedomains/__init__.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     1175 2023-02-03 21:31:37.000000 piedomains-0.0.9/piedomains/base.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     1127 2023-02-04 14:24:04.000000 piedomains-0.0.9/piedomains/constants.py
+-rw-r--r--   0 rchint1    (501) staff       (20)      705 2023-02-03 21:58:58.000000 piedomains-0.0.9/piedomains/domain.py
+-rw-r--r--   0 rchint1    (501) staff       (20)      116 2023-02-03 21:31:21.000000 piedomains-0.0.9/piedomains/logging.py
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:10.789110 piedomains-0.0.9/piedomains/model/
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:10.789697 piedomains-0.0.9/piedomains/model/calibrate/
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:11.796651 piedomains-0.0.9/piedomains/model/calibrate/text/
+-rw-------   0 rchint1    (501) staff       (20)     2023 2023-01-27 23:23:13.000000 piedomains-0.0.9/piedomains/model/calibrate/text/adv.sav
+-rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:14.000000 piedomains-0.0.9/piedomains/model/calibrate/text/aggressive.sav
+-rw-------   0 rchint1    (501) staff       (20)     1575 2023-01-27 23:23:14.000000 piedomains-0.0.9/piedomains/model/calibrate/text/alcohol.sav
+-rw-------   0 rchint1    (501) staff       (20)      863 2023-01-27 23:23:14.000000 piedomains-0.0.9/piedomains/model/calibrate/text/anonvpn.sav
+-rw-------   0 rchint1    (501) staff       (20)     2271 2023-01-27 23:23:15.000000 piedomains-0.0.9/piedomains/model/calibrate/text/automobile.sav
+-rw-------   0 rchint1    (501) staff       (20)      807 2023-01-27 23:23:15.000000 piedomains-0.0.9/piedomains/model/calibrate/text/costtraps.sav
+-rw-------   0 rchint1    (501) staff       (20)     1991 2023-01-27 23:23:15.000000 piedomains-0.0.9/piedomains/model/calibrate/text/dating.sav
+-rw-------   0 rchint1    (501) staff       (20)     1823 2023-01-27 23:23:16.000000 piedomains-0.0.9/piedomains/model/calibrate/text/downloads.sav
+-rw-------   0 rchint1    (501) staff       (20)     1895 2023-01-27 23:23:16.000000 piedomains-0.0.9/piedomains/model/calibrate/text/drugs.sav
+-rw-------   0 rchint1    (501) staff       (20)      711 2023-01-27 23:23:16.000000 piedomains-0.0.9/piedomains/model/calibrate/text/dynamic.sav
+-rw-------   0 rchint1    (501) staff       (20)     2759 2023-01-27 23:23:17.000000 piedomains-0.0.9/piedomains/model/calibrate/text/education.sav
+-rw-------   0 rchint1    (501) staff       (20)     2695 2023-01-27 23:23:17.000000 piedomains-0.0.9/piedomains/model/calibrate/text/finance.sav
+-rw-------   0 rchint1    (501) staff       (20)     1511 2023-01-27 23:23:17.000000 piedomains-0.0.9/piedomains/model/calibrate/text/fortunetelling.sav
+-rw-------   0 rchint1    (501) staff       (20)     2631 2023-01-27 23:23:18.000000 piedomains-0.0.9/piedomains/model/calibrate/text/forum.sav
+-rw-------   0 rchint1    (501) staff       (20)     2631 2023-01-27 23:23:18.000000 piedomains-0.0.9/piedomains/model/calibrate/text/gamble.sav
+-rw-------   0 rchint1    (501) staff       (20)     1671 2023-01-27 23:23:18.000000 piedomains-0.0.9/piedomains/model/calibrate/text/government.sav
+-rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:19.000000 piedomains-0.0.9/piedomains/model/calibrate/text/hacking.sav
+-rw-------   0 rchint1    (501) staff       (20)     3399 2023-01-27 23:23:19.000000 piedomains-0.0.9/piedomains/model/calibrate/text/hobby.sav
+-rw-------   0 rchint1    (501) staff       (20)     1127 2023-01-27 23:23:19.000000 piedomains-0.0.9/piedomains/model/calibrate/text/homestyle.sav
+-rw-------   0 rchint1    (501) staff       (20)     1863 2023-01-27 23:23:20.000000 piedomains-0.0.9/piedomains/model/calibrate/text/hospitals.sav
+-rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:20.000000 piedomains-0.0.9/piedomains/model/calibrate/text/imagehosting.sav
+-rw-------   0 rchint1    (501) staff       (20)     1447 2023-01-27 23:23:20.000000 piedomains-0.0.9/piedomains/model/calibrate/text/isp.sav
+-rw-------   0 rchint1    (501) staff       (20)     2119 2023-01-27 23:23:21.000000 piedomains-0.0.9/piedomains/model/calibrate/text/jobsearch.sav
+-rw-------   0 rchint1    (501) staff       (20)     1095 2023-01-27 23:23:21.000000 piedomains-0.0.9/piedomains/model/calibrate/text/library.sav
+-rw-------   0 rchint1    (501) staff       (20)     1255 2023-01-27 23:23:22.000000 piedomains-0.0.9/piedomains/model/calibrate/text/military.sav
+-rw-------   0 rchint1    (501) staff       (20)     1727 2023-01-27 23:23:22.000000 piedomains-0.0.9/piedomains/model/calibrate/text/models.sav
+-rw-------   0 rchint1    (501) staff       (20)     2247 2023-01-27 23:23:22.000000 piedomains-0.0.9/piedomains/model/calibrate/text/movies.sav
+-rw-------   0 rchint1    (501) staff       (20)     2791 2023-01-27 23:23:23.000000 piedomains-0.0.9/piedomains/model/calibrate/text/music.sav
+-rw-------   0 rchint1    (501) staff       (20)     3495 2023-01-27 23:23:23.000000 piedomains-0.0.9/piedomains/model/calibrate/text/news.sav
+-rw-------   0 rchint1    (501) staff       (20)     1087 2023-01-27 23:23:23.000000 piedomains-0.0.9/piedomains/model/calibrate/text/podcasts.sav
+-rw-------   0 rchint1    (501) staff       (20)     2087 2023-01-27 23:23:24.000000 piedomains-0.0.9/piedomains/model/calibrate/text/politics.sav
+-rw-------   0 rchint1    (501) staff       (20)     4999 2023-01-27 23:23:24.000000 piedomains-0.0.9/piedomains/model/calibrate/text/porn.sav
+-rw-------   0 rchint1    (501) staff       (20)     2535 2023-01-27 23:23:24.000000 piedomains-0.0.9/piedomains/model/calibrate/text/radiotv.sav
+-rw-------   0 rchint1    (501) staff       (20)     4799 2023-01-27 23:23:25.000000 piedomains-0.0.9/piedomains/model/calibrate/text/recreation.sav
+-rw-------   0 rchint1    (501) staff       (20)     2343 2023-01-27 23:23:25.000000 piedomains-0.0.9/piedomains/model/calibrate/text/redirector.sav
+-rw-------   0 rchint1    (501) staff       (20)     2279 2023-01-27 23:23:25.000000 piedomains-0.0.9/piedomains/model/calibrate/text/religion.sav
+-rw-------   0 rchint1    (501) staff       (20)      863 2023-01-27 23:23:25.000000 piedomains-0.0.9/piedomains/model/calibrate/text/remotecontrol.sav
+-rw-------   0 rchint1    (501) staff       (20)     1223 2023-01-27 23:23:26.000000 piedomains-0.0.9/piedomains/model/calibrate/text/ringtones.sav
+-rw-------   0 rchint1    (501) staff       (20)     1735 2023-01-27 23:23:26.000000 piedomains-0.0.9/piedomains/model/calibrate/text/science.sav
+-rw-------   0 rchint1    (501) staff       (20)     1479 2023-01-27 23:23:26.000000 piedomains-0.0.9/piedomains/model/calibrate/text/searchengines.sav
+-rw-------   0 rchint1    (501) staff       (20)     1351 2023-01-27 23:23:27.000000 piedomains-0.0.9/piedomains/model/calibrate/text/sex.sav
+-rw-------   0 rchint1    (501) staff       (20)     5479 2023-01-27 23:23:27.000000 piedomains-0.0.9/piedomains/model/calibrate/text/shopping.sav
+-rw-------   0 rchint1    (501) staff       (20)     1439 2023-01-27 23:23:27.000000 piedomains-0.0.9/piedomains/model/calibrate/text/socialnet.sav
+-rw-------   0 rchint1    (501) staff       (20)     2215 2023-01-27 23:23:28.000000 piedomains-0.0.9/piedomains/model/calibrate/text/spyware.sav
+-rw-------   0 rchint1    (501) staff       (20)     1287 2023-01-27 23:23:28.000000 piedomains-0.0.9/piedomains/model/calibrate/text/tracker.sav
+-rw-------   0 rchint1    (501) staff       (20)      839 2023-01-27 23:23:28.000000 piedomains-0.0.9/piedomains/model/calibrate/text/updatesites.sav
+-rw-------   0 rchint1    (501) staff       (20)     1375 2023-01-27 23:23:29.000000 piedomains-0.0.9/piedomains/model/calibrate/text/urlshortener.sav
+-rw-------   0 rchint1    (501) staff       (20)     1095 2023-01-27 23:23:29.000000 piedomains-0.0.9/piedomains/model/calibrate/text/violence.sav
+-rw-------   0 rchint1    (501) staff       (20)     1375 2023-01-27 23:23:29.000000 piedomains-0.0.9/piedomains/model/calibrate/text/warez.sav
+-rw-------   0 rchint1    (501) staff       (20)     1511 2023-01-27 23:23:30.000000 piedomains-0.0.9/piedomains/model/calibrate/text/weapons.sav
+-rw-------   0 rchint1    (501) staff       (20)     1671 2023-01-27 23:23:30.000000 piedomains-0.0.9/piedomains/model/calibrate/text/webmail.sav
+-rw-------   0 rchint1    (501) staff       (20)      967 2023-01-27 23:23:30.000000 piedomains-0.0.9/piedomains/model/calibrate/text/webphone.sav
+-rw-------   0 rchint1    (501) staff       (20)     1927 2023-01-27 23:23:31.000000 piedomains-0.0.9/piedomains/model/calibrate/text/webradio.sav
+-rw-------   0 rchint1    (501) staff       (20)     1255 2023-01-27 23:23:31.000000 piedomains-0.0.9/piedomains/model/calibrate/text/webtv.sav
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:12.380805 piedomains-0.0.9/piedomains/notebooks/
+-rw-r--r--   0 rchint1    (501) staff       (20)     2217 2022-04-30 13:42:53.000000 piedomains-0.0.9/piedomains/notebooks/01_get_shallalist.ipynb
+-rwxr-xr-x   0 rchint1    (501) staff       (20)     5728 2022-04-30 13:42:53.000000 piedomains-0.0.9/piedomains/notebooks/01_scrape_webpages.ipynb
+-rw-r--r--   0 rchint1    (501) staff       (20)     3590 2022-04-30 13:42:53.000000 piedomains-0.0.9/piedomains/notebooks/01a_scrape_stratified_random_sample.ipynb
+-rw-r--r--   0 rchint1    (501) staff       (20)     4951 2022-10-28 19:01:46.000000 piedomains-0.0.9/piedomains/notebooks/01b_scraper_webpages_all.ipynb
+-rw-r--r--   0 rchint1    (501) staff       (20)    22826 2022-10-28 19:01:46.000000 piedomains-0.0.9/piedomains/notebooks/01c_upload_to_dataverse.ipynb
+-rwxr-xr-x   0 rchint1    (501) staff       (20)    14386 2022-04-30 13:42:53.000000 piedomains-0.0.9/piedomains/notebooks/02_parse_html_data.ipynb
+-rwxr-xr-x   0 rchint1    (501) staff       (20)   178111 2022-10-28 22:57:19.000000 piedomains-0.0.9/piedomains/notebooks/03_data_clean_up.ipynb
+-rwxr-xr-x   0 rchint1    (501) staff       (20)   465526 2022-10-28 22:56:48.000000 piedomains-0.0.9/piedomains/notebooks/04_train_model.ipynb
+-rw-------   0 rchint1    (501) staff       (20)   126099 2023-01-27 23:22:13.000000 piedomains-0.0.9/piedomains/notebooks/05_text_calibrate_isotonic.ipynb
+-rw-------   0 rchint1    (501) staff       (20)  3055216 2023-01-29 16:57:25.000000 piedomains-0.0.9/piedomains/notebooks/06_preprocessing_images.ipynb
+-rw-------   0 rchint1    (501) staff       (20)   586681 2023-01-29 16:57:53.000000 piedomains-0.0.9/piedomains/notebooks/07_train_images.ipynb
+-rw-r--r--   0 rchint1    (501) staff       (20)    39074 2022-10-28 19:01:46.000000 piedomains-0.0.9/piedomains/notebooks/archive-upload-screenshot-to-dataverse.ipynb
+-rw-r--r--   0 rchint1    (501) staff       (20)    14093 2023-02-04 15:27:37.000000 piedomains-0.0.9/piedomains/piedomain.py
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:12.422994 piedomains-0.0.9/piedomains/tests/
+-rw-r--r--   0 rchint1    (501) staff       (20)      343 2023-02-04 14:24:58.000000 piedomains-0.0.9/piedomains/tests/__init__.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     1186 2023-02-04 15:13:33.000000 piedomains-0.0.9/piedomains/tests/test_001_pred_domain_text.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     1434 2023-02-04 15:16:56.000000 piedomains-0.0.9/piedomains/tests/test_002_pred_domain_images.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     2023 2023-02-04 15:20:11.000000 piedomains-0.0.9/piedomains/tests/test_003_pred_domain_combined.py
+-rw-r--r--   0 rchint1    (501) staff       (20)     1451 2023-02-03 21:30:54.000000 piedomains-0.0.9/piedomains/utils.py
+drwxr-xr-x   0 rchint1    (501) staff       (20)        0 2023-02-04 15:47:10.920128 piedomains-0.0.9/piedomains.egg-info/
+-rw-r--r--   0 rchint1    (501) staff       (20)     7934 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/PKG-INFO
+-rw-r--r--   0 rchint1    (501) staff       (20)     3586 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/SOURCES.txt
+-rw-r--r--   0 rchint1    (501) staff       (20)        1 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/dependency_links.txt
+-rw-r--r--   0 rchint1    (501) staff       (20)       52 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/entry_points.txt
+-rw-r--r--   0 rchint1    (501) staff       (20)      132 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/requires.txt
+-rw-r--r--   0 rchint1    (501) staff       (20)       11 2023-02-04 15:47:10.000000 piedomains-0.0.9/piedomains.egg-info/top_level.txt
+-rw-r--r--   0 rchint1    (501) staff       (20)       88 2023-02-04 15:47:12.426528 piedomains-0.0.9/setup.cfg
+-rw-r--r--   0 rchint1    (501) staff       (20)     5135 2023-02-04 15:45:26.000000 piedomains-0.0.9/setup.py
```

### Comparing `piedomains-0.0.8/LICENSE` & `piedomains-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/base.py` & `piedomains-0.0.9/piedomains/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import os
 from pkg_resources import resource_filename
 from .utils import download_file, REPO_BASE_URL
 from .logging import get_logger
 
 logger = get_logger()
 
+"""
+Base class for all models
+"""
+
 
 class Base(object):
     MODELFN = None
 
+    """
+    Load model data from the server
+    """
+
     @classmethod
     def load_model_data(cls, file_name, latest=False):
         model_path = None
         if cls.MODELFN:
             print(f"model fn {cls.MODELFN}")
             model_fn = resource_filename(__name__, cls.MODELFN)
             print(model_fn)
```

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/adv.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/adv.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/aggressive.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/aggressive.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/alcohol.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/alcohol.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/anonvpn.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/anonvpn.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/automobile.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/automobile.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/costtraps.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/costtraps.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/dating.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/dating.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/downloads.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/downloads.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/drugs.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/drugs.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/dynamic.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/dynamic.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/education.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/education.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/finance.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/finance.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/fortunetelling.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/fortunetelling.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/forum.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/forum.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/gamble.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/gamble.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/government.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/government.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/hacking.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/hacking.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/hobby.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/hobby.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/homestyle.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/homestyle.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/hospitals.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/hospitals.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/imagehosting.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/imagehosting.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/isp.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/isp.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/jobsearch.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/jobsearch.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/library.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/library.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/military.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/military.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/models.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/models.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/movies.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/movies.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/music.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/music.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/news.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/news.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/podcasts.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/podcasts.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/politics.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/politics.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/porn.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/porn.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/radiotv.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/radiotv.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/recreation.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/recreation.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/redirector.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/redirector.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/religion.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/religion.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/remotecontrol.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/remotecontrol.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/ringtones.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/ringtones.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/science.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/science.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/searchengines.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/searchengines.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/sex.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/sex.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/shopping.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/shopping.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/socialnet.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/socialnet.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/spyware.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/spyware.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/tracker.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/tracker.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/updatesites.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/updatesites.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/urlshortener.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/urlshortener.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/violence.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/violence.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/warez.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/warez.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/weapons.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/weapons.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/webmail.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/webmail.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/webphone.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/webphone.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/webradio.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/webradio.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/model/calibrate/text/webtv.sav` & `piedomains-0.0.9/piedomains/model/calibrate/text/webtv.sav`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/01_get_shallalist.ipynb` & `piedomains-0.0.9/piedomains/notebooks/01_get_shallalist.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/01_scrape_webpages.ipynb` & `piedomains-0.0.9/piedomains/notebooks/01_scrape_webpages.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/01a_scrape_stratified_random_sample.ipynb` & `piedomains-0.0.9/piedomains/notebooks/01a_scrape_stratified_random_sample.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/01b_scraper_webpages_all.ipynb` & `piedomains-0.0.9/piedomains/notebooks/01b_scraper_webpages_all.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/01c_upload_to_dataverse.ipynb` & `piedomains-0.0.9/piedomains/notebooks/01c_upload_to_dataverse.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/02_parse_html_data.ipynb` & `piedomains-0.0.9/piedomains/notebooks/02_parse_html_data.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/03_data_clean_up.ipynb` & `piedomains-0.0.9/piedomains/notebooks/03_data_clean_up.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/04_train_model.ipynb` & `piedomains-0.0.9/piedomains/notebooks/04_train_model.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/05_text_calibrate_isotonic.ipynb` & `piedomains-0.0.9/piedomains/notebooks/05_text_calibrate_isotonic.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/06_preprocessing_images.ipynb` & `piedomains-0.0.9/piedomains/notebooks/06_preprocessing_images.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/07_train_images.ipynb` & `piedomains-0.0.9/piedomains/notebooks/07_train_images.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/notebooks/archive-upload-screenshot-to-dataverse.ipynb` & `piedomains-0.0.9/piedomains/notebooks/archive-upload-screenshot-to-dataverse.ipynb`

 * *Files identical despite different names*

### Comparing `piedomains-0.0.8/piedomains/utils.py` & `piedomains-0.0.9/piedomains/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import tarfile
 import requests
 
 
 REPO_BASE_URL = os.environ.get("PIEDOMAINS_MODEL_URL") or "https://dataverse.harvard.edu/api/access/datafile/6908064"
 
 
+"""
+Download file from the server
+"""
+
+
 def download_file(url, target, file_name):
     status = True
     try:
         # download the file
         r = requests.get(url, allow_redirects=True)
         open(f"{target}/{file_name}", "wb").write(r.content)
         # untar
```

### Comparing `piedomains-0.0.8/piedomains.egg-info/SOURCES.txt` & `piedomains-0.0.9/piedomains.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 piedomains/__init__.py
 piedomains/base.py
+piedomains/constants.py
 piedomains/domain.py
 piedomains/logging.py
-piedomains/pydomain.py
+piedomains/piedomain.py
 piedomains/utils.py
 piedomains.egg-info/PKG-INFO
 piedomains.egg-info/SOURCES.txt
 piedomains.egg-info/dependency_links.txt
 piedomains.egg-info/entry_points.txt
 piedomains.egg-info/requires.txt
 piedomains.egg-info/top_level.txt
@@ -77,8 +78,10 @@
 piedomains/notebooks/03_data_clean_up.ipynb
 piedomains/notebooks/04_train_model.ipynb
 piedomains/notebooks/05_text_calibrate_isotonic.ipynb
 piedomains/notebooks/06_preprocessing_images.ipynb
 piedomains/notebooks/07_train_images.ipynb
 piedomains/notebooks/archive-upload-screenshot-to-dataverse.ipynb
 piedomains/tests/__init__.py
-piedomains/tests/test_010_pred_domain.py
+piedomains/tests/test_001_pred_domain_text.py
+piedomains/tests/test_002_pred_domain_images.py
+piedomains/tests/test_003_pred_domain_combined.py
```

### Comparing `piedomains-0.0.8/setup.py` & `piedomains-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if args:
             args = shlex.split(self.tox_args)
         tox.cmdline(args=args)
 
 
 setup(
     name="piedomains",
-    version="0.0.8",
+    version="0.0.9",
     description="Predict categories based domain names and it's content",
     long_description_content_type="text/x-rst",
     long_description=long_description,
     # The project's main homepage.
     url="https://github.com/themains/piedomains",
     # Author details
     author="Rajashekar Chintalapati and Gaurav Sood",
@@ -132,16 +132,16 @@
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files # noqa
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points={
-        "console_scripts": ["classify_domains=newpydomain:main"],
+        "console_scripts": ["classify_domains=piedomain:main"],
     },
     cmdclass={
         "develop": PostDevelopCommand,
         "install": PostInstallCommand,
         "test": Tox,
     },
     tests_require=["tox"],
-)
+)
```

