# Comparing `tmp/home-assistant-intents-2023.4.17.tar.gz` & `tmp/home-assistant-intents-2023.4.17.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.4.17.tar", last modified: Mon Apr 17 16:05:10 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.4.17.post1.tar", last modified: Mon Apr 17 16:27:24 2023, max compression
```

## Comparing `home-assistant-intents-2023.4.17.tar` & `home-assistant-intents-2023.4.17.post1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.17/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.17/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.17/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      938 2023-04-17 16:04:21.000000 home-assistant-intents-2023.4.17/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.016872 home-assistant-intents-2023.4.17/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12939 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21003 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    25271 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68839 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-17 16:05:10.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-04-17 15:42:03.000000 home-assistant-intents-2023.4.17/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.738942 home-assistant-intents-2023.4.17.post1/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.17.post1/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.17.post1/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      909 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.17.post1/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:08:03.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12939 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21003 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    25271 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68839 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      909 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      992 2023-04-17 16:27:17.000000 home-assistant-intents-2023.4.17.post1/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-17 16:27:24.738942 home-assistant-intents-2023.4.17.post1/setup.cfg
```

### Comparing `home-assistant-intents-2023.4.17/LICENSE.md` & `home-assistant-intents-2023.4.17.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/PKG-INFO` & `home-assistant-intents-2023.4.17.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.4.17
+Version: 2023.4.17.post1
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """API for home_assistant_intents package."""
+import importlib.resources
 import json
 import os
 import typing
 from pathlib import Path
-from typing import Any, Callable, Dict, List, IO, Optional
-
-import importlib.resources
+from typing import IO, Any, Callable, Dict, List, Optional
 
-from .languages import DOMAINS_AND_LANGUAGES
+from .domains import DOMAINS_AND_LANGUAGES
 
 _PACKAGE = "home_assistant_intents"
 _DIR = Path(typing.cast(os.PathLike, importlib.resources.files(_PACKAGE)))
 _DATA_DIR = _DIR / "data"
 
 
 def get_intents(
```

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents/domains.py` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents/domains.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.4.17
+Version: 2023.4.17.post1
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17/pyproject.toml` & `home-assistant-intents-2023.4.17.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.4.17"
+version     = "2023.4.17-1"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

