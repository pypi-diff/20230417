# Comparing `tmp/home-assistant-intents-2023.3.29.tar.gz` & `tmp/home-assistant-intents-2023.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.3.29.tar", last modified: Wed Mar 29 15:46:13 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.4.17.tar", last modified: Mon Apr 17 16:05:10 2023, max compression
```

## Comparing `home-assistant-intents-2023.3.29.tar` & `home-assistant-intents-2023.4.17.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.273285 home-assistant-intents-2023.3.29/
--rw-r--r--   0 paulus     (501) staff       (20)    18657 2023-02-15 03:53:50.000000 home-assistant-intents-2023.3.29/LICENSE.md
--rw-r--r--   0 paulus     (501) staff       (20)       72 2023-02-15 03:53:50.000000 home-assistant-intents-2023.3.29/MANIFEST.in
--rw-r--r--   0 paulus     (501) staff       (20)      903 2023-03-29 15:46:13.273142 home-assistant-intents-2023.3.29/PKG-INFO
--rw-r--r--   0 paulus     (501) staff       (20)      190 2023-02-15 03:53:50.000000 home-assistant-intents-2023.3.29/README.md
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.258585 home-assistant-intents-2023.3.29/home_assistant_intents/
--rw-r--r--   0 paulus     (501) staff       (20)      688 2023-02-15 03:53:50.000000 home-assistant-intents-2023.3.29/home_assistant_intents/__init__.py
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.257300 home-assistant-intents-2023.3.29/home_assistant_intents/data/
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.266883 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 paulus     (501) staff       (20)     4877 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 paulus     (501) staff       (20)    16176 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 paulus     (501) staff       (20)     1903 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 paulus     (501) staff       (20)    12544 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 paulus     (501) staff       (20)    19903 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 paulus     (501) staff       (20)     7033 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 paulus     (501) staff       (20)    19633 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 paulus     (501) staff       (20)    23946 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 paulus     (501) staff       (20)     8325 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 paulus     (501) staff       (20)    56696 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 paulus     (501) staff       (20)    14729 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 paulus     (501) staff       (20)     2885 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 paulus     (501) staff       (20)    40173 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 paulus     (501) staff       (20)     6747 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 paulus     (501) staff       (20)    17198 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 paulus     (501) staff       (20)     5245 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 paulus     (501) staff       (20)     1373 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 paulus     (501) staff       (20)    16181 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 paulus     (501) staff       (20)     1525 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 paulus     (501) staff       (20)    18547 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 paulus     (501) staff       (20)     7330 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 paulus     (501) staff       (20)     3603 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 paulus     (501) staff       (20)     2214 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 paulus     (501) staff       (20)    14790 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 paulus     (501) staff       (20)     3331 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 paulus     (501) staff       (20)     1197 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 paulus     (501) staff       (20)    11801 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 paulus     (501) staff       (20)    11322 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 paulus     (501) staff       (20)     8002 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 paulus     (501) staff       (20)    11714 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 paulus     (501) staff       (20)     1367 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 paulus     (501) staff       (20)     4824 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 paulus     (501) staff       (20)    16333 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 paulus     (501) staff       (20)    68839 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 paulus     (501) staff       (20)    28352 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 paulus     (501) staff       (20)     7860 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 paulus     (501) staff       (20)    13050 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 paulus     (501) staff       (20)    51451 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 paulus     (501) staff       (20)    14961 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 paulus     (501) staff       (20)    11029 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 paulus     (501) staff       (20)     3079 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 paulus     (501) staff       (20)     4312 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 paulus     (501) staff       (20)    11472 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 paulus     (501) staff       (20)     1197 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 paulus     (501) staff       (20)     1296 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 paulus     (501) staff       (20)     5477 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 paulus     (501) staff       (20)    14445 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 paulus     (501) staff       (20)    14341 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 paulus     (501) staff       (20)    12024 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 paulus     (501) staff       (20)    16782 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 paulus     (501) staff       (20)    13464 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 paulus     (501) staff       (20)    37672 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.272931 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/
--rw-r--r--   0 paulus     (501) staff       (20)      180 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 paulus     (501) staff       (20)     4257 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 paulus     (501) staff       (20)      725 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 paulus     (501) staff       (20)     3620 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 paulus     (501) staff       (20)     1479 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/da.json
--rw-r--r--   0 paulus     (501) staff       (20)     1696 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 paulus     (501) staff       (20)     1918 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/de.json
--rw-r--r--   0 paulus     (501) staff       (20)     1526 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/el.json
--rw-r--r--   0 paulus     (501) staff       (20)     3236 2023-03-29 15:46:08.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/en.json
--rw-r--r--   0 paulus     (501) staff       (20)     1608 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/es.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 paulus     (501) staff       (20)     5421 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 paulus     (501) staff       (20)     1876 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 paulus     (501) staff       (20)     1389 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 paulus     (501) staff       (20)     1350 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 paulus     (501) staff       (20)     1223 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/he.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 paulus     (501) staff       (20)     2274 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 paulus     (501) staff       (20)     1723 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 paulus     (501) staff       (20)     1258 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/id.json
--rw-r--r--   0 paulus     (501) staff       (20)      422 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/is.json
--rw-r--r--   0 paulus     (501) staff       (20)     1774 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/it.json
--rw-r--r--   0 paulus     (501) staff       (20)      598 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 paulus     (501) staff       (20)     2574 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 paulus     (501) staff       (20)     2145 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 paulus     (501) staff       (20)     2062 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 paulus     (501) staff       (20)     2720 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 paulus     (501) staff       (20)     1368 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 paulus     (501) staff       (20)     2174 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 paulus     (501) staff       (20)     2594 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 paulus     (501) staff       (20)     1163 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 paulus     (501) staff       (20)      419 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 paulus     (501) staff       (20)     1950 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 paulus     (501) staff       (20)     3315 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 paulus     (501) staff       (20)     1857 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 paulus     (501) staff       (20)     1548 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 paulus     (501) staff       (20)     1554 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 paulus     (501) staff       (20)     2563 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/te.json
--rw-r--r--   0 paulus     (501) staff       (20)      416 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 paulus     (501) staff       (20)     1681 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 paulus     (501) staff       (20)     1405 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 paulus     (501) staff       (20)     1510 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 paulus     (501) staff       (20)     2172 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 paulus     (501) staff       (20)     2008 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 paulus     (501) staff       (20)     2126 2023-03-29 15:46:09.000000 home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-tw.json
-drwxr-xr-x   0 paulus     (501) staff       (20)        0 2023-03-29 15:46:13.259321 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/
--rw-r--r--   0 paulus     (501) staff       (20)      903 2023-03-29 15:46:12.000000 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 paulus     (501) staff       (20)     5127 2023-03-29 15:46:13.000000 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 paulus     (501) staff       (20)        1 2023-03-29 15:46:13.000000 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 paulus     (501) staff       (20)       23 2023-03-29 15:46:13.000000 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 paulus     (501) staff       (20)        1 2023-03-29 15:45:04.000000 home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 paulus     (501) staff       (20)      990 2023-03-29 15:40:56.000000 home-assistant-intents-2023.3.29/pyproject.toml
--rw-r--r--   0 paulus     (501) staff       (20)       38 2023-03-29 15:46:13.273327 home-assistant-intents-2023.3.29/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.17/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.17/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.17/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      938 2023-04-17 16:04:21.000000 home-assistant-intents-2023.4.17/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.016872 home-assistant-intents-2023.4.17/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12939 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21003 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    25271 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68839 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-17 16:05:05.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-17 16:05:06.000000 home-assistant-intents-2023.4.17/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:05:10.020872 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-17 16:05:10.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-17 16:05:09.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-04-17 15:42:03.000000 home-assistant-intents-2023.4.17/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-17 16:05:10.024872 home-assistant-intents-2023.4.17/setup.cfg
```

### Comparing `home-assistant-intents-2023.3.29/LICENSE.md` & `home-assistant-intents-2023.4.17/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/PKG-INFO` & `home-assistant-intents-2023.4.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.3.29
+Version: 2023.4.17
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.612866512345679%*

 * *Differences: {"'expansion_rules'": '{\'name\': "([le | la | les] {name} | [l\']{name})", \'area\': "([le | la ] '*

 * *                      '{area} | [l\']{area})", \'brightness\': \'{brightness:brightness}[%| '*

 * *                      "pourcent]', 'temperature': '{temperature}[°| degrés] [{temperature_unit}]', "*

 * *                      "'regle': '(règle | met | ajuste | change)', 'allume': '(allume | active | "*

 * *                      "démarre | ouvre)', 'eteins': '(éteint | éteins | désactive | stoppe | "*

 * *                       […]*

```diff
@@ -1,205 +1,271 @@
 {
     "expansion_rules": {
-        "area": "[\u0627\u0644] {area}",
-        "brightness": "{brightness}[% | \u0628\u0627\u0644\u0645\u0627\u0626\u0629]",
-        "close": "(\u0627\u063a\u0644\u0642 | \u0627\u0642\u0641\u0644 | \u0627\u062e\u0641\u0636)",
-        "name": "[\u0627\u0644] {name}",
-        "open": "(\u0627\u0641\u062a\u062d | \u0627\u0631\u0641\u0639)",
-        "temp": "\u062f\u0631\u062c\u0629 [\u0627\u0644]\u062d\u0631\u0627\u0631\u0629",
-        "temperature": "{temperature}[\u00b0| \u062f\u0631\u062c\u0629] [{temperature_unit}]",
-        "turn": "( \u0627\u0641\u062a\u062d | \u0634\u063a\u0644 | \u063a\u064a\u0631 | \u0627\u0636\u0628\u0637 )",
-        "what_is": "( \u0645\u0627 \u0647\u0648 | \u0645\u0627 \u0647\u0649 | \u0645\u0627\u0630\u0627 \u064a\u0643\u0648\u0646 | \u0645\u0627\u0630\u0627 \u062a\u0643\u0648\u0646 )",
-        "window": "(\u0646\u0627\u0641\u0630\u0629 | \u0646\u0648\u0627\u0641\u0630 | \u0645\u0638\u0644\u0629 | \u0645\u0638\u0644\u0627\u062a | \u0633\u062a\u0627\u0631\u0629 | \u0633\u062a\u0627\u0626\u0631)"
+        "allume": "(allume | active | d\u00e9marre | ouvre)",
+        "area": "([le | la ] {area} | [l']{area})",
+        "brightness": "{brightness:brightness}[%| pourcent]",
+        "dans": "(dans | du | de)",
+        "eteins": "(\u00e9teint | \u00e9teins | d\u00e9sactive | stoppe | arr\u00eate | coupe | ferme )",
+        "lumiere": "(la lumi\u00e8re | la lampe | l'ampoule)",
+        "lumieres": "[les] (lumi\u00e8res | lampes | ampoules)",
+        "name": "([le | la | les] {name} | [l']{name})",
+        "regle": "(r\u00e8gle | met | ajuste | change)",
+        "temperature": "{temperature}[\u00b0| degr\u00e9s] [{temperature_unit}]",
+        "ventilateur": "(le ventilateur | l'\u00e9changeur d'air | la fan)",
+        "ventilateurs": "(les ventilateurs | les fans)"
     },
-    "intents": {},
-    "language": "ar",
+    "intents": {
+        "HassTurnOff": {
+            "data": [
+                {
+                    "sentences": [
+                        "<eteins> ([tous] | [toutes] ) <ventilateurs> <dans> [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<eteins> <ventilateur> [<dans>] [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<eteins> <name> [dans|du|de] <area>",
+                        "<eteins> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "(ferme | baisse) <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "(ferme | baisse) <name> <dans> <area>"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<eteins> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "(ferme | baisse) [la] porte du garage"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "(ferme | baisse) [les] (stores | toiles| rideaux) <dans> <area>"
+                    ],
+                    "slots": {
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
+                    }
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
+                {
+                    "sentences": [
+                        "<allume> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "ouvre [la] porte du garage"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "ouvre [les] (stores | rideaux | toiles) <dans> <area>"
+                    ],
+                    "slots": {
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<allume> ([tous] | [toutes] ) (<ventilateur> | <ventilateurs>) [<dans>] [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<allume> (<ventilateur> | <ventilateurs>) [<dans>] [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<allume> <name>",
+                        "<allume> <name> [dans|du|de] <area>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "ouvre <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "ouvre <name> <dans> <area>"
+                    ]
+                }
+            ]
+        }
+    },
+    "language": "fr-CA",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
-        "brightness_level": {
-            "values": [
-                {
-                    "in": "( \u0639\u0627\u0644\u064a| \u0642\u0635\u0648\u0649 )",
-                    "out": 100
-                },
-                {
-                    "in": "\u0645\u0646\u062e\u0641\u0636",
-                    "out": 1
-                }
-            ]
-        },
         "color": {
             "values": [
                 {
-                    "in": "\u0627\u0628\u064a\u0636",
+                    "in": "(blanc|blanche)",
                     "out": "white"
                 },
                 {
-                    "in": "\u0627\u0633\u0648\u062f",
+                    "in": "(noir | noire)",
                     "out": "black"
                 },
                 {
-                    "in": "\u0627\u062d\u0645\u0631",
+                    "in": "rouge",
                     "out": "red"
                 },
                 {
-                    "in": "\u0628\u0631\u062a\u0642\u0627\u0644\u064a",
+                    "in": "orange",
                     "out": "orange"
                 },
                 {
-                    "in": "\u0627\u0635\u0641\u0631",
+                    "in": "jaune",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u0627\u062e\u0636\u0631",
+                    "in": "(vert | verte)",
                     "out": "green"
                 },
                 {
-                    "in": "\u0627\u0632\u0631\u0642",
+                    "in": "(bleu | bleue)",
                     "out": "blue"
                 },
                 {
-                    "in": "\u0628\u0646\u0641\u0633\u062c\u064a",
+                    "in": "(violet | violette)",
                     "out": "purple"
                 },
                 {
-                    "in": "\u0628\u0646\u064a",
+                    "in": "brun",
                     "out": "brown"
-                }
-            ]
-        },
-        "cover_classes": {
-            "values": [
-                {
-                    "in": "( \u0645\u0638\u0644\u0627\u062a | \u0645\u0638\u0644\u0629 )",
-                    "out": "awning"
-                },
-                {
-                    "in": "( \u0633\u062a\u0627\u0626\u0631 | \u0633\u062a\u0627\u0631\u0629 )",
-                    "out": "curtain"
-                },
-                {
-                    "in": "( \u0628\u0627\u0628 | \u0627\u0628\u0648\u0627\u0628 )",
-                    "out": "door"
-                },
-                {
-                    "in": "( \u0628\u0627\u0628 | \u0627\u0628\u0648\u0627\u0628 ) \u0627\u0644\u062c\u0631\u0627\u062c",
-                    "out": "garage"
-                },
-                {
-                    "in": "( \u0628\u0648\u0627\u0628\u0629 | \u0628\u0648\u0627\u0628\u0627\u062a )",
-                    "out": "gate"
-                },
-                {
-                    "in": "( \u0634\u0628\u0627\u0643 | \u0634\u0628\u0627\u0628\u064a\u0643 | \u0646\u0627\u0641\u0630\u0629 | \u0646\u0648\u0627\u0641\u0630 )",
-                    "out": "window"
-                }
-            ]
-        },
-        "cover_states": {
-            "values": [
-                {
-                    "in": "\u0645\u0641\u062a\u0648\u062d",
-                    "out": "open"
-                },
-                {
-                    "in": "( \u0645\u063a\u0644\u0642 | \u0645\u0642\u0641\u0648\u0644 )",
-                    "out": "closed"
-                },
-                {
-                    "in": "\u064a\u0641\u062a\u062d",
-                    "out": "opening"
-                },
-                {
-                    "in": "\u064a\u063a\u0644\u0642",
-                    "out": "closing"
-                }
-            ]
-        },
-        "on_off_domains": {
-            "values": [
-                {
-                    "in": "( \u0646\u0648\u0631 | \u0644\u0645\u0628\u0629 | \u0644\u0645\u0628\u0627\u062a | \u0623\u0646\u0648\u0627\u0631 )",
-                    "out": "light"
-                },
-                {
-                    "in": "( \u0645\u0631\u0648\u062d\u0629 | \u0645\u0631\u0627\u0648\u062d )",
-                    "out": "fan"
-                },
-                {
-                    "in": "( \u0645\u0641\u062a\u0627\u062d | \u0645\u0641\u0627\u062a\u064a\u062d )",
-                    "out": "switch"
-                }
-            ]
-        },
-        "on_off_states": {
-            "values": [
-                {
-                    "in": "\u0634\u063a\u0644",
-                    "out": "on"
                 },
                 {
-                    "in": "\u0623\u0637\u0641\u064a",
-                    "out": "off"
+                    "in": "rose",
+                    "out": "pink"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "\u0645\u0626\u0648\u064a\u0629",
+                "celsius",
                 {
                     "in": "c",
                     "out": "celsius"
                 },
-                "\u0641\u0647\u0631\u0646\u0647\u0627\u064a\u062a",
+                "fahrenheit",
                 {
                     "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u062d\u062f\u062b \u062e\u0637\u0623 \u0627\u062b\u0646\u0627\u0621 \u0645\u0639\u0627\u0644\u062c\u0629 \u0627\u0644\u0646\u0635",
-            "no_area": "\u0644\u0627 \u062a\u0648\u062c\u062f \u0645\u0646\u0637\u0642\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ area }}",
-            "no_device_class": "\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }} \u0644\u0627 \u062a\u062d\u062a\u0648\u0649 \u0639\u0644\u0649 \u0641\u0626\u0629 \u0627\u0644\u0623\u062c\u0647\u0632\u0629 {{ device_class }}",
-            "no_domain": "\u0627\u0644\u0646\u0637\u0627\u0642 {{ domain }} \u063a\u064a\u0631 \u0645\u0648\u062c\u0648\u062f \u0628\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }}",
-            "no_entity": "\u0644\u0627 \u064a\u0648\u062c\u062f \u062c\u0647\u0627\u0632 \u0627\u0648 \u062e\u0627\u0635\u064a\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ entity }}",
-            "no_intent": "\u0639\u0641\u0648\u0627, \u0644\u0645 \u0627\u0641\u0647\u0645 \u0647\u0630\u0627"
+            "handle_error": "Une erreur s'est produite pendant le traitement",
+            "no_area": "Aucune zone appel\u00e9e {{ area }}",
+            "no_device_class": "{{ area }} ne contient pas de {{ device_class }}",
+            "no_domain": "{{ area }} ne contient pas de {{ domain }}",
+            "no_entity": "Aucun appareil ou entit\u00e9 appel\u00e9 {{ entity }}",
+            "no_intent": "D\u00e9sol\u00e9, je n'ai pas compris"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "TODO: Closed",
-                "cover_device_class": "TODO: Closed {{ slots.device_class }}",
-                "default": "TODO: Turned off {{ state.domain }}",
-                "fans_area": "TODO: Turned off fans",
-                "lights_area": "TODO: Turned off lights"
+                "cover": "{{ slots.name }} ferm\u00e9",
+                "cover_area": "Ouvrants de {{ slots.area }} ferm\u00e9s",
+                "cover_device_class": "{{ slots.device_class }} ferm\u00e9",
+                "default": "{{ slots.name }} \u00e9teint",
+                "fans_area": "ventilateurs de {{ slots.area }} \u00e9teints",
+                "lights_area": "Lumi\u00e8res de {{ slots.area }} \u00e9teintes"
             },
             "HassTurnOn": {
-                "cover": "TODO: Opened",
-                "cover_device_class": "TODO: Opened {{ slots.device_class }}",
-                "default": "TODO: Turned on {{ state.domain }}",
-                "fans_area": "TODO: Turned on fans",
-                "lights_area": "TODO: Turned on lights"
+                "cover": "{{ slots.name }} ouvert",
+                "cover_area": "Ouvrants de {{ slots.area }} ouverts",
+                "cover_device_class": "{{ slots.device_class }} ouvert",
+                "default": "{{ slots.name }} allum\u00e9",
+                "fans_area": "Ventilateurs de {{ slots.area }} activ\u00e9",
+                "lights_area": "Lumi\u00e8res de {{ slots.area }} allum\u00e9es"
             }
         }
     },
     "skip_words": [
-        "(\u0645\u0646 \u0641\u0636\u0644\u0643 | \u0644\u0648 \u0633\u0645\u062d\u062a)",
-        "(\u0647\u0644 \u064a\u0645\u0643\u0646\u0643 | \u062a\u0642\u062f\u0631)"
+        "s'il te pla\u00eet",
+        "merci",
+        "peux-tu",
+        "s'il vous pla\u00eet",
+        "Heille"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ru.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7438019344124669%*

 * *Differences: {"'expansion_rules'": "{'area': '[в|во|на] {area}', 'brightness': '{brightness}[%| "*

 * *                      "процент[ов|а]]', 'temp': '(температур(а|у)|градус[ов|а])', 'temperature': "*

 * *                      "'{temperature}[°|градус[ов|а]] [{temperature_unit}]', 'turn_on': "*

 * *                      "'(запусти|включи)[ть]', 'turn_off': '(выключи|отключи)[ть]', 'set': "*

 * *                      "'(сдела(й|ть)|установи[ть]|постав(ь|ить)|поменя(й|ть)|измени[ть]|выстав(ь|ить)|переключи[ть]|переве(сти|ди)|увелич(ь|ить)| […]*

```diff
@@ -1,487 +1,455 @@
 {
     "expansion_rules": {
-        "all": "\u0432\u0441\u0438\u0447\u043a\u0438[\u0442\u0435]|\u0432\u0441\u044f\u043a(\u043e|\u0430)|\u0432\u0441\u0435\u043a\u0438",
-        "area": "[\u0432|\u043d\u0430|\u0432\u044a\u0432] {area}",
-        "brightness": "{brightness}[%| \u043f\u0440\u043e\u0446\u0435\u043d\u0442[\u0430]]",
-        "close": "\u0437\u0430\u0442\u0432\u043e\u0440\u0438|\u0441\u043c\u044a\u043a\u043d\u0438|\u0441\u043f\u0443\u0441\u043d\u0438|\u0437\u0430\u043a\u0440\u0438\u0439|\u0441\u0432\u0430\u043b\u0438",
-        "covers": "\u0449\u043e\u0440(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u0437\u0430\u0432\u0435\u0441(a|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043f\u0435\u0440\u0434\u0435[\u0442\u043e|\u0442\u0430|\u0442\u0430\u0442\u0430]|\u043a\u0435\u043f\u0435\u043d\u0446\u0438[\u0442\u0435]|\u043a\u0430\u043f\u0430(\u043a|\u043a\u0430|\u043a\u044a\u0442|\u0446\u0438|\u0446\u0438\u0442\u0435)",
-        "fans": "\u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440[\u0430|\u044a\u0442|\u0438|\u0438\u0442\u0435]",
-        "lights": "\u043b\u0430\u043c\u043f(\u0430|\u0430\u0442\u0430|\u0438|\u0438\u0442\u0435)|\u043e\u0441\u0432\u0435\u0442\u043b\u0435\u043d\u0438\u0435[\u0442\u043e]|\u043a\u0440\u0443\u0448\u043a(\u0430|\u0430\u0442\u0430|\u0438|\u0438\u0442\u0435)",
-        "lights_brightness": "[\u043d\u0430] [\u044f\u0440\u043a\u043e\u0441\u0442[\u0442\u0430]] [\u043d\u0430] [\u0441\u0432\u0435\u0442\u0435\u043d\u0435[\u0442\u043e]] [\u043d\u0430] [\u0441\u0432\u0435\u0442\u043b\u0438\u043d\u0430[\u0442\u0430]] [\u043e\u0441\u0432\u0435\u0442\u0435\u043d\u043e\u0441\u0442[\u0442\u0430]]",
-        "max": "max|\u043c\u0430\u043a\u0441\u0438\u043c\u0430\u043b\u043d\u0430[\u0442\u0430]|\u043c\u0430\u043a\u0441|\u043a\u0440\u0430\u0439|\u043d\u0430\u0439[-]\u0432\u0438\u0441\u043e\u043a\u0430[\u0442\u0430]",
-        "min": "\u043c\u0438\u043d\u0438\u043c\u0430\u043b\u043d\u0430|\u043c\u0438\u043d\u0438\u043c\u0443\u043c|\u043d\u0430\u0439[-]\u043d\u0438\u0441\u043a\u0430",
+        "area": "[\u0432|\u0432\u043e|\u043d\u0430] {area}",
+        "brightness": "{brightness}[%| \u043f\u0440\u043e\u0446\u0435\u043d\u0442[\u043e\u0432|\u0430]]",
+        "close": "(\u0437\u0430\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043f\u0440\u0438\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043e\u043f\u0443\u0441\u0442\u0438[\u0442\u044c])",
         "name": "{name}",
-        "open": "\u043e\u0442\u0432\u043e\u0440\u0438|\u0432\u0434\u0438\u0433\u043d\u0438|\u043e\u0442\u043a\u0440\u0438\u0439",
-        "set": "\u043d\u0430\u043f\u0440\u0430\u0432\u0438|\u0441\u043b\u043e\u0436\u0438|\u043f\u043e\u0441\u0442\u0430\u0432\u0438|\u0441\u043c\u0435\u043d\u0438|\u043f\u0440\u043e\u043c\u0435\u043d\u0438|\u043d\u0430\u0441\u0442\u0440\u043e\u0439|\u0437\u0430\u0434\u0430\u0439|\u043d\u0430\u0433\u043b\u0430\u0441\u0438|\u0442\u0443\u0440\u0438|\u043d\u0430\u0432\u0438\u0439",
-        "temp": "\u0442\u0435\u043c\u043f\u0435\u0440\u0430\u0442\u0443\u0440(\u0430|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u0433\u0440\u0430\u0434\u0443\u0441[\u0430|\u0438|\u0442\u0435|\u044a\u0442]|\u0442\u0435\u0440\u043c\u043e\u0441\u0442\u0430\u0442[\u0430|\u044a\u0442|\u0438\u0442\u0435]",
-        "temperature": "{temperature}[\u00b0| \u0433\u0440\u0430\u0434\u0443\u0441\u0430] [{temperature_unit}]",
-        "turn_off": "\u0441\u043f\u0440\u0438|\u0438\u0437\u043a\u043b\u044e\u0447\u0438|\u0438\u0437\u0433\u0430\u0441\u0438|\u0443\u0433\u0430\u0441\u0438|\u0437\u0430\u0433\u0430\u0441\u0438",
-        "turn_on": "\u043f\u0443\u0441\u043d\u0438|\u0432\u043a\u043b\u044e\u0447\u0438|\u0441\u0432\u0435\u0442\u043d\u0438|\u0437\u0430\u043f\u0430\u043b\u0438",
-        "what_is": "\u043a\u0430\u043a\u0432\u043e [\u0435]|\u043a\u0430\u043a\u0432\u0430 [\u0435]|\u043a\u0430\u043a\u0432\u0438 [\u0441\u0430]|\u043a\u0430\u043a\u044a\u0432 [\u0435]|\u043a\u043e\u043b\u043a\u043e [\u0435]|\u043a\u043e\u043b\u043a\u043e [\u0441\u0430]"
+        "open": "(\u043e\u0442\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043f\u043e\u0434\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c))",
+        "set": "(\u0441\u0434\u0435\u043b\u0430(\u0439|\u0442\u044c)|\u0443\u0441\u0442\u0430\u043d\u043e\u0432\u0438[\u0442\u044c]|\u043f\u043e\u0441\u0442\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043f\u043e\u043c\u0435\u043d\u044f(\u0439|\u0442\u044c)|\u0438\u0437\u043c\u0435\u043d\u0438[\u0442\u044c]|\u0432\u044b\u0441\u0442\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043f\u0435\u0440\u0435\u043a\u043b\u044e\u0447\u0438[\u0442\u044c]|\u043f\u0435\u0440\u0435\u0432\u0435(\u0441\u0442\u0438|\u0434\u0438)|\u0443\u0432\u0435\u043b\u0438\u0447(\u044c|\u0438\u0442\u044c)|\u0443\u043c\u0435\u043d\u044c\u0448(\u0438|\u0438\u0442\u044c)|\u043f\u043e\u0434\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c)|\u043e\u043f\u0443\u0441\u0442\u0438[\u0442\u044c]|\u043f\u0440\u0438\u0431\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043e\u0442\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c)|\u043f\u043e\u0432\u044b\u0441(\u044c|\u0438\u0442\u044c)|\u043f\u043e\u043d\u0438\u0437(\u044c|\u0438\u0442\u044c))",
+        "temp": "(\u0442\u0435\u043c\u043f\u0435\u0440\u0430\u0442\u0443\u0440(\u0430|\u0443)|\u0433\u0440\u0430\u0434\u0443\u0441[\u043e\u0432|\u0430])",
+        "temperature": "{temperature}[\u00b0|\u0433\u0440\u0430\u0434\u0443\u0441[\u043e\u0432|\u0430]] [{temperature_unit}]",
+        "turn_off": "(\u0432\u044b\u043a\u043b\u044e\u0447\u0438|\u043e\u0442\u043a\u043b\u044e\u0447\u0438)[\u0442\u044c]",
+        "turn_on": "(\u0437\u0430\u043f\u0443\u0441\u0442\u0438|\u0432\u043a\u043b\u044e\u0447\u0438)[\u0442\u044c]"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
                     "response": "one",
                     "sentences": [
-                        "\u043a\u0430\u043a(\u044a\u0432|\u0432\u0430|\u0432\u043e|\u0432\u0438) (\u0435|\u0441\u0430) [\u0441\u044a\u0441\u0442\u043e\u044f\u043d\u0438\u0435\u0442\u043e \u043d\u0430] <name> [<area>]"
+                        "\u0427\u0442\u043e \u0441[\u043e] <name> [<area>]",
+                        "\u041a\u0430\u043a(\u043e\u0435|\u043e\u0432\u043e|\u0430\u044f|\u043e\u0439) [\u0441\u043e\u0441\u0442\u043e\u044f\u043d\u0438\u0435] [\u0443] <name> [<area>]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "{on_off_states:state} \u043b\u0438 \u0435 [\u0441\u044a\u0441\u0442\u043e\u044f\u043d\u0438\u0435\u0442\u043e \u043d\u0430] <name> [<area>]"
+                        "<name> [<area>] {on_off_states:state}",
+                        "{on_off_states:state} [\u043b\u0438] <name> [<area>]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "\u0438\u043c\u0430 \u043b\u0438 {on_off_domains:domain} {on_off_states:state} [<area>]",
-                        "\u0438\u043c\u0430 \u043b\u0438 {on_off_states:state} {on_off_domains:domain} [<area>]"
+                        "[\u0415\u0441\u0442\u044c] [\u043b\u0438] [\u043a\u0430\u043a(\u043e\u0439|\u043e\u0435|\u0438\u0435)-\u043d\u0438\u0431\u0443\u0434\u044c] {on_off_states:state} {on_off_domains:domain} [<area>]",
+                        "[\u0415\u0441\u0442\u044c] [\u043b\u0438] [<area>] [\u043a\u0430\u043a(\u043e\u0439|\u043e\u0435|\u0438\u0435)-\u043d\u0438\u0431\u0443\u0434\u044c] {on_off_states:state} {on_off_domains:domain}"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "{on_off_states:state} \u043b\u0438 \u0441\u0430 \u0432\u0441\u0438\u0447\u043a\u0438[\u0442\u0435] {on_off_domains:domain} [<area>]",
-                        "\u0432\u0441\u0438\u0447\u043a\u0438 {on_off_domains:domain} \u043b\u0438 \u0441\u0430 {on_off_states:state} [<area>]"
+                        "(\u0412\u0441\u0435|\u0432\u0435\u0441\u044c) [\u043b\u0438] {on_off_domains:domain} {on_off_states:state} [<area>]",
+                        "{on_off_states:state} [\u043b\u0438] (\u0432\u0441\u0435|\u0432\u0435\u0441\u044c) {on_off_domains:domain} [<area>]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(\u043a\u043e(\u0438|\u044f|\u0435|\u0439)|\u043a\u0430\u043a(\u044a\u0432|\u0432\u0430|\u0432\u043e|\u0432\u0438)) {on_off_domains:domain} (\u0435|\u0441\u0430) {on_off_states:state} [<area>]"
+                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {on_off_domains:domain} {on_off_states:state} [<area>]",
+                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {on_off_domains:domain} [<area>] {on_off_states:state}"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "\u043a\u043e\u043b\u043a\u043e {on_off_domains:domain} \u0441\u0430 {on_off_states:state} [<area>]"
+                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_domains:domain} {on_off_states:state} [<area>]",
+                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_domains:domain} [<area>] {on_off_states:state}",
+                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_states:state} {on_off_domains:domain} [<area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "{cover_states:state} \u043b\u0438 \u0435 <name> [<area>]"
+                        "{cover_states:state} [\u043b\u0438] <name> [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "\u0418\u043c\u0430 \u043b\u0438 [\u043d\u044f\u043a\u043e(\u0439|\u0438|\u044f|\u0435)|\u043d\u044f\u043a\u0430\u043a(\u044a\u0432|\u0432\u0430|\u0432\u043e|\u0432\u0438)] {cover_states:state} {cover_classes:device_class} [<area>]",
-                        "\u0418\u043c\u0430 \u043b\u0438 [\u043d\u044f\u043a\u043e(\u0439|\u0438|\u044f|\u0435)|\u043d\u044f\u043a\u0430\u043a(\u044a\u0432|\u0432\u0430|\u0432\u043e|\u0432\u0438)] {cover_classes:device_class} [\u043a\u043e(\u0439\u0442\u043e|\u0438\u0442\u043e|\u044f\u0442\u043e|\u0435\u0442\u043e) \u0441\u0430|e] {cover_states:state} [<area>]"
+                        "\u0415\u0441\u0442\u044c [\u043b\u0438] {cover_states:state} {cover_classes:device_class} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "\u0412\u0441\u0438\u0447\u043a\u0438[\u0442\u0435] {cover_classes:device_class} \u043b\u0438 \u0441\u0430 {cover_states:state} [<area>]"
+                        "\u0412\u0441\u0435 [\u043b\u0438] {cover_classes:device_class} [<area>] {cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(\u043a\u043e\u0438|\u043a\u043e\u0439|\u043a\u043e\u044f|\u043a\u043e\u0435) {cover_classes:device_class} (\u0435|\u0441\u0430) {cover_states:state} [<area>]"
+                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {cover_classes:device_class} {cover_states:state} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "\u041a\u043e\u043b\u043a\u043e {cover_classes:device_class} [\u0441\u0430|\u0441\u0435] {cover_states:state} [<area>]",
-                        "\u041a\u043e\u043b\u043a\u043e \u0441\u0430 {cover_states:state} {cover_classes:device_class} [<area>]"
+                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {cover_classes:device_class} {cover_states:state} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "lights_area",
+                    "response": "fans_area",
                     "sentences": [
-                        "<turn_off> [<all>] <lights> <area>",
-                        "<turn_off> [<all>] <area> <lights>"
+                        "<turn_off> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b] <area>",
+                        "<turn_off> <area> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
+                    "sentences": [
+                        "<turn_off> <name>"
+                    ]
+                },
+                {
                     "response": "cover",
                     "sentences": [
-                        "<close> <name>"
+                        "<close> <name>",
+                        "<close> <name> <area>"
                     ]
                 },
                 {
+                    "response": "lights_area",
+                    "sentences": [
+                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442",
+                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
+                        "<turn_off> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442",
+                        "<turn_off> <area> <name>",
+                        "<turn_off> <name> <area>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<close> [\u0432\u0440\u0430\u0442\u0430\u0442\u0430] [\u043d\u0430] \u0433\u0430\u0440\u0430\u0436\u0430",
-                        "<close> \u0433\u0430\u0440\u0430\u0436\u043d\u0430\u0442\u0430 \u0432\u0440\u0430\u0442\u0430"
+                        "<close> [\u0434\u0432\u0435\u0440\u044c] \u0433\u0430\u0440\u0430\u0436\u0430",
+                        "<close> \u0433\u0430\u0440\u0430\u0436\u043d\u0443\u044e \u0434\u0432\u0435\u0440\u044c"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<close> [<all>] <covers> <area>",
-                        "<close>  <area> [<all>] <covers>"
+                        "<close> (\u0448\u0442\u043e\u0440(\u044b|\u0443)|\u0437\u0430\u043d\u0430\u0432\u0435\u0441\u043a(\u0438|\u0443)|\u0436\u0430\u043b\u044e\u0437\u0438|\u043e\u043a\u043d(\u043e|\u0430)) <area>"
                     ],
                     "slots": {
-                        "area": "bedroom",
                         "device_class": [
+                            "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_off> [<all>] <fans> <area>",
-                        "<turn_off> [<all>] <area> <fans>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> <name>"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "light",
-                    "sentences": [
-                        "<turn_off> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> <name> <area>",
-                        "<close> <area> <name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "lights_area",
                     "sentences": [
-                        "<turn_on> <name>"
-                    ]
+                        "<turn_on> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
+                        "<turn_on> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "light",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<turn_on> <name>"
-                    ]
+                        "<open> [\u0434\u0432\u0435\u0440\u044c] \u0433\u0430\u0440\u0430\u0436[\u0430]",
+                        "<open> \u0433\u0430\u0440\u0430\u0436\u043d\u0443\u044e \u0434\u0432\u0435\u0440\u044c"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<open> <name>  <area>",
-                        "<open> <area> <name>"
-                    ]
+                        "<open> (\u0448\u0442\u043e\u0440(\u044b|\u0443)|\u0437\u0430\u043d\u0430\u0432\u0435\u0441\u043a(\u0438|\u0443)|\u0436\u0430\u043b\u044e\u0437\u0438) <area>"
+                    ],
+                    "slots": {
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
+                    }
                 },
                 {
                     "response": "fans_area",
                     "sentences": [
-                        "<turn_on> [<all>] <fans> <area>",
-                        "<turn_on> [<all>] <area> <fans>"
+                        "<turn_on> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b] <area>",
+                        "<turn_on> <area> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "lights_area",
                     "sentences": [
-                        "<turn_on> [<all>] <lights> <area>",
-                        "<turn_on> [<all>] <area> <lights>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
+                        "<turn_on> <name>"
+                    ]
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
                     "response": "cover",
                     "sentences": [
                         "<open> <name>"
                     ]
                 },
                 {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<open> [\u0432\u0440\u0430\u0442\u0430\u0442\u0430] [\u043d\u0430] \u0433\u0430\u0440\u0430\u0436\u0430",
-                        "<open> \u0433\u0430\u0440\u0430\u0436\u043d\u0430\u0442\u0430 \u0432\u0440\u0430\u0442\u0430"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
                     "response": "cover_area",
                     "sentences": [
-                        "<open> [<all>] <covers> <area>",
-                        "<open> <area> [<all>] <covers>"
-                    ],
-                    "slots": {
-                        "area": "bedroom",
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
+                        "<open> <name> <area>"
+                    ]
                 }
             ]
         }
     },
-    "language": "bg",
+    "language": "ru",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "\u0431\u044f\u043b[\u043e|\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430]|\u0431\u0435\u043b(\u0438|\u0438\u044f|\u0438\u044f\u0442|\u0438\u0442\u0435)",
+                    "in": "\u0431\u0435\u043b\u044b\u0439|\u0431\u0435\u043b\u043e\u0433\u043e|\u0431\u0435\u043b\u044b\u043c",
                     "out": "white"
                 },
                 {
-                    "in": "\u0447\u0435\u0440\u0435\u043d|\u0447\u0435\u0440\u043d(\u043e|\u043d\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430|\u0438|\u0438\u044f\u0442|\u0438\u0442\u0435)",
+                    "in": "\u0447\u0435\u0440\u043d\u044b\u0439|\u0447\u0435\u0440\u043d\u043e\u0433\u043e|\u0447\u0451\u0440\u043d\u044b\u0439|\u0447\u0451\u0440\u043d\u043e\u0433\u043e|\u0447\u0435\u0440\u043d\u044b\u043c|\u0447\u0451\u0440\u043d\u044b\u043c",
                     "out": "black"
                 },
                 {
-                    "in": "\u0447\u0435\u0440\u0432\u0435\u043d[\u043e|\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430|\u0438|\u0438\u044f|\u0438\u044f\u0442]",
+                    "in": "\u043a\u0440\u0430\u0441\u043d\u044b\u0439|\u043a\u0440\u0430\u0441\u043d\u043e\u0433\u043e|\u043a\u0440\u0430\u0441\u043d\u044b\u043c",
                     "out": "red"
                 },
                 {
-                    "in": "\u043e\u0440\u0430\u043d\u0436\u0435\u0432[\u043e|\u0430|\u043e\u0442\u043e|\u0432\u0430\u0442\u0430|\u0438|\u0438\u044f|\u0438\u044f\u0442]",
+                    "in": "\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u044b\u0439|\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u043e\u0433\u043e|\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u044b\u043c",
                     "out": "orange"
                 },
                 {
-                    "in": "\u0436\u044a\u043b\u0442[\u043e|\u0430|\u043e\u0442\u043e|\u0438|\u0438\u044f|\u0438\u044f\u0442|\u0430\u0442\u0430]",
+                    "in": "\u0436\u0435\u043b\u0442\u044b\u0439|\u0436\u0435\u043b\u0442\u043e\u0433\u043e|\u0436\u0451\u043b\u0442\u044b\u0439|\u0436\u0451\u043b\u0442\u043e\u0433\u043e|\u0436\u0435\u043b\u0442\u044b\u043c|\u0436\u0451\u043b\u0442\u044b\u043c",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u0437\u0435\u043b\u0435\u043d[\u043e|\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430|\u0438|\u0438\u044f|\u0438\u044f\u0442]",
+                    "in": "\u0437\u0435\u043b\u0435\u043d\u044b\u0439|\u0437\u0435\u043b\u0451\u043d\u044b\u0439|\u0437\u0435\u043b\u0435\u043d\u043e\u0433\u043e|\u0437\u0435\u043b\u0451\u043d\u043e\u0433\u043e|\u0437\u0435\u043b\u0435\u043d\u044b\u043c|\u0437\u0435\u043b\u0451\u043d\u044b\u043c",
                     "out": "green"
                 },
                 {
-                    "in": "\u0441\u0438\u043d[\u044c\u043e|\u044f|\u044c\u043e\u0442\u043e|\u044f\u0442\u0430|\u0438\u044f\u0442|\u0438|\u0438\u0442\u0435]",
+                    "in": "\u0441\u0438\u043d\u0438\u0439|\u0441\u0438\u043d\u0435\u0433\u043e|\u0441\u0438\u043d\u0438\u043c",
                     "out": "blue"
                 },
                 {
-                    "in": "\u043b\u0438\u043b\u0430\u0432[\u043e|\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430|\u0438|\u0438\u044f|\u0438\u044f\u0442|\u0438\u0442\u0435]",
+                    "in": "\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u044b\u0439|\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u043e\u0433\u043e|\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u044b\u043c",
                     "out": "purple"
                 },
                 {
-                    "in": "\u043a\u0430\u0444\u044f\u0432[\u043e|\u0430|\u043e\u0442\u043e|\u0430\u0442\u0430|\u0438|\u0438\u044f|\u0438\u044f\u0442|\u0438\u0442\u0435]",
+                    "in": "\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u044b\u0439|\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u043e\u0433\u043e|\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u044b\u043c",
                     "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "\u0442\u0435\u043d\u0442(a|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)",
+                    "in": "\u043d\u0430\u0432\u0435\u0441[\u0430|\u044b|\u043e\u043c|\u0430\u043c\u0438]",
                     "out": "awning"
                 },
                 {
-                    "in": "\u0449\u043e\u0440(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)",
+                    "in": "\u0436\u0430\u043b\u044e\u0437\u0438",
                     "out": "blind"
                 },
                 {
-                    "in": "\u043f\u0435\u0440\u0434\u0435[\u0442\u0430|\u0442\u043e|\u0442\u0430\u0442\u0430]|\u0437\u0430\u0432\u0435\u0441(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)",
+                    "in": "\u0448\u0442\u043e\u0440[\u0430|\u044b|\u043e\u043c|\u0430\u043c\u0438]",
                     "out": "curtain"
                 },
                 {
-                    "in": "\u0432\u0440\u0430\u0442(\u0430|\u0438|\u0442\u0430|\u0438\u0442\u0435)",
+                    "in": "\u0434\u0432\u0435\u0440(\u044c[\u044e]|\u043c\u0438)",
                     "out": "door"
                 },
                 {
-                    "in": "\u0433\u0430\u0440\u0430\u0436[\u0430|\u0438|\u044a\u0442|\u0438\u0442\u0435]|(\u0433\u0430\u0440\u0430\u0436(\u043d\u0430|\u043d\u0430\u0442\u0430|\u043d\u0438|\u043d\u0438\u0442\u0435) \u0432\u0440\u0430\u0442(\u0430|\u0438))",
+                    "in": "\u0433\u0430\u0440\u0430\u0436\u043d(\u0430\u044f|\u0443\u044e|\u043e\u0439|\u044b\u043c\u0438) \u0434\u0432\u0435\u0440(\u044c[\u044e]|\u043c\u0438)",
                     "out": "garage"
                 },
                 {
-                    "in": "\u043f\u043e\u0440\u0442(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)",
+                    "in": "gate[s]",
                     "out": "gate"
                 },
                 {
-                    "in": "\u0441\u0435\u043d\u043d\u0438(\u043a|\u0446\u0438|\u043a\u0430|\u043a\u044a\u0442|\u0446\u0438\u0442\u0435)",
+                    "in": "shade[s]",
                     "out": "shade"
                 },
                 {
-                    "in": "\u043a\u0435\u043f\u0435\u043d\u0446\u0438[\u0442\u0435]|\u043a\u0430\u043f\u0430(\u043a|\u043a\u0430|\u043a\u044a\u0442|\u0446\u0438|\u0446\u0438\u0442\u0435)",
+                    "in": "\u0441\u0442\u0430\u0432\u043d(\u044f[\u043c\u0438]|\u0438)",
                     "out": "shutter"
                 },
                 {
-                    "in": "\u043f\u0440\u043e\u0437\u043e\u0440(\u0435\u0446|\u0446\u0438|\u0435\u0446\u0430|\u0446\u0438\u0442\u0435|\u0435\u0446\u044a\u0442)",
+                    "in": "\u043e\u043a\u043d(\u043e[\u043c]|\u0430[\u043c\u0438])",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "\u043e\u0442\u0432\u043e\u0440\u0435\u043d[\u0430|\u0438|\u043e|\u0438\u0442\u0435]|\u0432\u0434\u0438\u0433\u043d\u0430\u0442[\u0430|\u043e|\u0438|\u0438\u0442\u0435]|\u043e\u0442\u043a\u0440\u0438\u0442[\u0430|\u043e|\u0438|\u0438\u0442\u0435]",
-                    "out": "open"
+                    "in": "\u043e\u0442\u043a\u0440\u044b\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043d\u0435[ ]\u0437\u0430\u0434\u0435\u0440\u043d\u0443\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043f\u043e\u0434\u043d\u044f\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]",
+                    "out": "\u043e\u0442\u043a\u0440\u044b\u0442\u0430"
                 },
                 {
-                    "in": "\u0437\u0430\u0442\u0432\u043e\u0440\u0435\u043d[\u0430|\u0438|\u043e|\u0438\u0442\u0435]|\u0441\u043c\u044a\u043a\u043d\u0430\u0442[\u0430|\u043e|\u0438|\u0438\u0442\u0435]|\u0441\u043f\u0443\u0441\u043d\u0430\u0442[\u0430|\u043e|\u0438|\u0438\u0442\u0435]|\u0437\u0430\u043a\u0440\u0438\u0442[\u0430|\u043e|\u0438|\u0438\u0442\u0435]|\u0441\u0432\u0430\u043b\u0435\u043d[\u0430|\u043e|\u0438|\u0438\u0442\u0435]",
-                    "out": "closed"
+                    "in": "\u0437\u0430\u043a\u0440\u044b\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u0437\u0430\u0434\u0435\u0440\u043d\u0443\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043e\u043f\u0443\u0449\u0435\u043d[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]",
+                    "out": "\u0437\u0430\u043a\u0440\u044b\u0442\u0430"
                 },
                 {
-                    "in": "\u043e\u0442\u0432\u0430\u0440\u044f[\u0442]|\u0432\u0434\u0438\u0433\u0430[\u0442]|\u043e\u0442\u043a\u0440\u0438\u0432\u0430[\u0442]",
-                    "out": "opening"
+                    "in": "\u043e\u0442\u043a\u0440\u044b\u0432\u0430(\u0435|\u044e)\u0442\u0441\u044f|\u043f\u043e\u0434\u043d\u0438\u043c\u0430(\u0435|\u044e)\u0442\u0441\u044f",
+                    "out": "\u043e\u0442\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f"
                 },
                 {
-                    "in": "\u0437\u0430\u0442\u0432\u0430\u0440\u044f[\u0442]|\u0441\u043c\u044a\u043a\u0432\u0430[\u0442]|\u0441\u043f\u0443\u0441\u043a\u0430[\u0442]|\u0437\u0430\u043a\u0440\u0438\u0432\u0430[\u0442]|\u0441\u0432\u0430\u043b\u044f[\u0442]",
-                    "out": "closing"
+                    "in": "\u0437\u0430\u043a\u0440\u044b\u0432\u0430(\u0435|\u044e)\u0442\u0441\u044f|\u043e\u043f\u0443\u0441\u043a\u0430(\u0435|\u044e)\u0442\u0441\u044f",
+                    "out": "\u0437\u0430\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "\u0441\u0432\u0442\u043b\u0438\u043d(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043b\u0430\u043c\u043f(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043a\u0440\u0443\u0448\u043a(\u0430|\u0438|\u0430\u0442\u0430|\u0438\u0442\u0435)|\u043e\u0441\u0432\u0435\u0442\u043b\u0435\u043d(\u0438\u044f|\u0438\u0435|\u0438\u0435\u0442\u043e|\u0438\u044f\u0442\u0430)",
+                    "in": "(\u0441\u0432\u0435\u0442[\u0430]|\u043e\u0441\u0432\u0435\u0449\u0435\u043d\u0438\u0435|\u043b\u0430\u043c\u043f[\u0430|\u044b|\u043e\u0439|\u0430\u043c\u0438|\u0443]|\u0441\u0432\u0435\u0442\u0438\u043b\u044c\u043d\u0438\u043a(\u0430|\u0443|\u043e\u043c|\u0438|\u0430\u043c\u0438))",
                     "out": "light"
                 },
                 {
-                    "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440[\u0438|\u0430|\u044a\u0442|\u0438\u0442\u0435]",
+                    "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]",
                     "out": "fan"
                 },
                 {
-                    "in": "\u043a\u043b\u044e\u0447[\u043e\u0432\u0435|\u043e\u0432\u0435\u0442\u0435]",
+                    "in": "\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b(\u0438|\u044c|\u0435\u0439|\u0435\u043c|\u044f\u043c\u0438)",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "\u0432\u043a\u043b\u044e\u0447\u0435\u043d[\u0430|\u043e|\u0438|\u0438\u044f\u0442|\u0438\u0442\u0435|\u043e\u0442\u043e|\u0430\u0442\u0430]",
-                    "out": "on"
+                    "in": "\u0432\u043a\u043b\u044e\u0447\u0435\u043d[\u043d][\u0430|\u044b[\u0435]|\u043e[\u0439]]",
+                    "out": "\u0432\u043a\u043b\u044e\u0447\u0435\u043d"
                 },
                 {
-                    "in": "\u0438\u0437\u043a\u043b\u044e\u0447\u0435\u043d[\u0430|\u043e|\u0438|\u0438\u044f\u0442|\u0438\u0442\u0435|\u043e\u0442\u043e|\u0430\u0442\u0430]",
-                    "out": "off"
+                    "in": "\u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d[\u043d][\u0430|\u044b[\u0435]|\u043e[\u0439]]",
+                    "out": "\u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 {
-                    "in": "c|[\u043f\u043e|\u0432] \u0446\u0435\u043b\u0437\u0438\u0439",
+                    "in": "c|\u0446\u0435\u043b\u044c\u0441\u0438\u044f|\u043f\u043e \u0446\u0435\u043b\u044c\u0441\u0438\u044e",
                     "out": "celsius"
                 },
                 {
-                    "in": "f|[\u043f\u043e|\u0432\u044a\u0432] \u0444\u0430\u0440\u0435\u043d\u0445\u0430\u0439\u0442",
+                    "in": "f|\u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0430|\u043f\u043e \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0443",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u0412\u044a\u0437\u043d\u0438\u043a\u043d\u0430 \u043d\u0435\u043e\u0447\u0430\u043a\u0432\u0430\u043d\u0430 \u0433\u0440\u0435\u0448\u043a\u0430 \u043f\u0440\u0438 \u0438\u0437\u043f\u044a\u043b\u043d\u0435\u043d\u0438\u0435 \u043d\u0430 \u043a\u043e\u043c\u0430\u043d\u0434\u0430\u0442\u0430",
-            "no_area": "\u041d\u044f\u043c\u0430 \u043e\u0431\u043b\u0430\u0441\u0442 \u0441 \u0438\u043c\u0435 {{ area }}",
-            "no_device_class": "\u0412 \u043e\u0431\u043b\u0430\u0441\u0442\u0442\u0430 {{ area }} \u043d\u044f\u043c\u0430 {{ device_class }}",
-            "no_domain": "\u0412 \u043e\u0431\u043b\u0430\u0441\u0442\u0442\u0430 {{ area }} \u043d\u044f\u043c\u0430 {{ domain }}",
-            "no_entity": "\u041d\u044f\u043c\u0430 \u0443\u0441\u0442\u0440\u043e\u0439\u0441\u0442\u0432\u043e \u0438\u043b\u0438 \u043e\u0431\u0435\u043a\u0442 \u0441 \u0438\u043c\u0435 {{ entity }}",
-            "no_intent": "\u0421\u044a\u0436\u0430\u043b\u044f\u0432\u0430\u043c, \u043d\u0435 \u043c\u043e\u0436\u0430\u0445 \u0434\u0430 \u0440\u0430\u0437\u0431\u0435\u0440\u0430 \u0442\u043e\u0432\u0430"
+            "handle_error": "\u0412\u043e \u0432\u0440\u0435\u043c\u044f \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0438 \u043d\u0430\u043c\u0435\u0440\u0435\u043d\u0438\u044f \u043f\u0440\u043e\u0438\u0437\u043e\u0448\u043b\u0430 \u043d\u0435\u043f\u0440\u0435\u0434\u0432\u0438\u0434\u0435\u043d\u043d\u0430\u044f \u043e\u0448\u0438\u0431\u043a\u0430",
+            "no_area": "\u041d\u0435\u0442 \u0437\u043e\u043d\u044b, \u043d\u0430\u0437\u0432\u0430\u043d\u043d\u043e\u0439 {{ area }}",
+            "no_device_class": "\u0412 \u0437\u043e\u043d\u0435 {{ area }} \u043d\u0435\u0442 \u0443\u0441\u0442\u0440\u043e\u0439\u0441\u0442\u0432 {{ device_class }}",
+            "no_domain": "\u0412 \u0437\u043e\u043d\u0435 {{ area }} \u043d\u0435\u0442 \u043e\u0431\u044a\u0435\u043a\u0442\u043e\u0432 {{ domain }}",
+            "no_entity": "\u041d\u0435\u0442 \u0443\u0441\u0442\u0440\u043e\u0439\u0441\u0442\u0432\u0430 \u0438\u043b\u0438 \u0441\u0443\u0449\u043d\u043e\u0441\u0442\u0438, \u043d\u0430\u0437\u0432\u0430\u043d\u043d\u043e\u0439 {{ entity }}",
+            "no_intent": "\u041f\u0440\u043e\u0448\u0443 \u043f\u0440\u043e\u0449\u0435\u043d\u0438\u044f, \u043e\u0431\u0440\u0430\u0449\u0435\u043d\u0438\u0435 \u043d\u0435 \u0440\u0430\u0441\u043f\u043e\u0437\u043d\u0430\u043d\u043e"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  \u0414\u0430\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u041d\u0435, {{ no_match[:3] | join(\", \") }} \u0438 \u043e\u0449\u0435 {{ (no_match | length - 3) }} \u043d\u0435 \u0441\u0430\n  {%- else -%}\n    \u041d\u0435,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor %} \u043d\u0435 \u0435\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0414\u0430, {{ match[:3] | join(\", \") }} \u0438 \u043e\u0449\u0435 {{ (match | length - 3) }} \u0434\u0440\u0443\u0433\u0438\n  {%- else -%}\n    \u0414\u0430,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u041d\u0435\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  \u0414\u0430\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    {{ no_match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (no_match | length - 3) }} \u2014 \u043d\u0435\u0442\n  {%- else -%}\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }} \u2014 \u043d\u0435\u0442\n    {%- endfor %}\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0414\u0430, {{ match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (match | length - 3) }}\n  {%- else -%}\n    \u0414\u0430,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u041d\u0435\u0442\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "{{ slots.name | capitalize }} \u0435 {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  \u0414\u0430\n{% else %}\n  \u041d\u0435, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  \u041d\u0438\u043a\u043e\u0438\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0438 \u043e\u0449\u0435 {{ (match | length - 3) }} \u0434\u0440\u0443\u0433\u0438\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+                "one": "{{ slots.name | capitalize }} {{ state.state_with_unit }}\n",
+                "one_yesno": "{% if query.matched %}\n  \u0414\u0430\n{% else %}\n  \u041d\u0435\u0442, {{ state.state_with_unit }}\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u041d\u0438 \u043e\u0434\u043d\u043e\u0433\u043e\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.name }}",
-                "cover_area": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.area }}",
-                "cover_device_class": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.device_class }}",
-                "default": "\u0418\u0437\u043a\u043b\u044e\u0447\u0438\u0445 {{ slots.name }}",
-                "fans_area": "\u0418\u0437\u043a\u043b\u044e\u0447\u0438\u0445 \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0438\u0442\u0435 \u0432 {{ slots.area }}",
-                "light": "\u0418\u0437\u0433\u0430\u0441\u0438\u0445 {{ slots.name }}",
-                "lights_area": "\u0418\u0437\u0433\u0430\u0441\u0438\u0445 \u043b\u0430\u043c\u043f\u0438\u0442\u0435 \u0432 {{ slots.area }}"
+                "cover": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.name }}",
+                "cover_area": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.area }}",
+                "cover_device_class": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.device_class }}",
+                "default": "{{ slots.name }} \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d",
+                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432 {{ slots.area }}",
+                "lights_area": "\u0412\u044b\u043a\u043b\u044e\u0447\u0435\u043d \u0441\u0432\u0435\u0442 \u0432 {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "\u041e\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.name }}",
-                "cover_area": "\u041e\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.area }}",
-                "cover_device_class": "\u041e\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.device_class }}",
-                "default": "\u0412\u043a\u043b\u044e\u0447\u0438\u0445 {{ slots.name }}",
-                "fans_area": "\u0412\u043a\u043b\u044e\u0447\u0438\u0445 \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0430 \u0432 {{ slots.area }}",
-                "light": "\u0421\u0432\u0435\u0442\u043d\u0430\u0445 {{ slots.name }}",
-                "lights_area": "\u0421\u0432\u0435\u0442\u043d\u0430\u0445 \u043b\u0430\u043c\u043f\u0438\u0442\u0435 \u0432 {{ slots.area }}"
+                "cover": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.name }}",
+                "cover_area": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.area }}",
+                "cover_device_class": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.device_class }}",
+                "default": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d {{ slots.name }}",
+                "fans_area": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432 {{ slots.area }}",
+                "lights_area": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d \u0441\u0432\u0435\u0442 \u0432 {{ slots.area }}"
             }
         }
     },
     "skip_words": [
-        "\u0438\u0437\u0432\u0438\u043d\u044f\u0432\u0430\u0439",
-        "\u043c\u043e\u0436\u0435\u0448 \u043b\u0438",
-        "\u043c\u043e\u0436\u0435 \u043b\u0438",
-        "\u043a\u0430\u0436\u0438 \u043c\u0438",
-        "\u043c\u043e\u043b\u044f"
+        "\u043f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430",
+        "\u043c\u043e\u0436\u0435\u0448\u044c",
+        "\u0441\u043a\u0430(\u0436\u0438|\u0437\u0430\u0442\u044c)",
+        "\u043f\u0440\u043e\u0448\u0443",
+        "\u0443\u0437\u043d\u0430(\u0439|\u0442\u044c)"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/bn.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,26 +1,26 @@
 {
     "language": "bn",
     "intents": {
-        "HassTurnOn": {
+        "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "\u099a\u09be\u09b2\u09c1 \u0995\u09b0\u09c1\u09a8 <name>",
-                        " <name> \u099a\u09be\u09b2\u09c1 \u0995\u09b0\u09c1\u09a8"
+                        "\u09ac\u09a8\u09cd\u09a7 \u0995\u09b0\u09c1\u09a8 <name>",
+                        "<name> \u09ac\u09a8\u09cd\u09a7 \u0995\u09b0\u09c1\u09a8"
                     ]
                 }
             ]
         },
-        "HassTurnOff": {
+        "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "\u09ac\u09a8\u09cd\u09a7 \u0995\u09b0\u09c1\u09a8 <name>",
-                        "<name> \u09ac\u09a8\u09cd\u09a7 \u0995\u09b0\u09c1\u09a8"
+                        "\u099a\u09be\u09b2\u09c1 \u0995\u09b0\u09c1\u09a8 <name>",
+                        " <name> \u099a\u09be\u09b2\u09c1 \u0995\u09b0\u09c1\u09a8"
                     ]
                 }
             ]
         }
     },
     "responses": {
         "errors": {
@@ -28,29 +28,29 @@
             "no_area": "\u201c{{ area }} \u098f\u09b0 \u0995\u09cd\u09b7\u09c7\u09a4\u09cd\u09b0 \u0986\u0997\u09c7 \u0989\u09a0\u09be\u09a8\u09cb \u09b9\u09af\u09bc\u09a8\u09bf \u201d",
             "no_domain": "\u201c{{ area }} \u098f\u09b0\u09ae\u09a7\u09cd\u09af\u09c7  {{ domain }} \u09a8\u09c7\u0987\u201d",
             "no_device_class": "\u201c{{ area }} \u098f\u09b0\u09ae\u09a7\u09cd\u09af\u09c7  {{ device_class }} \u09a8\u09c7\u0987",
             "no_entity": "\u201c\u098f\u0987 \u09a8\u09be\u09ae\u09c7 \u0995\u09cb\u09a8 \u09ae\u09c7\u09b6\u09bf\u09a8 \u09ac\u09be  {{ entity }} \u09a8\u09be\u09ae\u09c7  \u0995\u09bf\u099b\u09c1 \u09a8\u09c7\u0987\u201d",
             "handle_error": "\u201c\u0995\u09be\u099c\u099f\u09bf \u09b6\u09c7\u09b7 \u0995\u09b0\u09be\u09b0 \u0986\u0997\u09c7 \u0985\u09aa\u09cd\u09b0\u09a4\u09cd\u09af\u09be\u09b6\u09bf\u09a4 \u098f\u0995\u099f\u09bf \u09ad\u09c1\u09b2\u09b8\u0982\u0998\u099f\u09bf\u09a4 \u09b9\u09af\u09bc\u09c7\u099b\u09c7\u201d"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {
         "name": "{name}"
     },
     "skip_words": []
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ca.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9914529914529915%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(5, OrderedDict([('sentences', ['<engega> el[s] "*

 * *              "ventilador[s] <area> [en marxa]']), ('slots', OrderedDict([('domain', 'fan')]))])), "*

 * *              "(6, OrderedDict([('sentences', ['<engega> tots els ventiladors [<area>]']), "*

 * *              "('slots', OrderedDict([('domain', 'fan'), ('name', 'all')]))])), (7, "*

 * *              "OrderedDict([('sentences', ['<engega> <name> [en marxa]']), ('excludes_context', "*

 * *              "OrderedDict([('domai […]*

```diff
@@ -67,14 +67,42 @@
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "<apaga> el[s] ventilador[s] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<apaga> tots els ventiladors [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<apaga> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<tanca> <name> [<area>]"
+                    ]
+                },
+                {
+                    "sentences": [
                         "(<apaga>|<tanca>) tots els llums [<area>]",
                         "(<apaga>|<tanca>) totes les llums [<area>]",
                         "(<apaga>|<tanca>) (els|les) llums [<area>]"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
@@ -116,82 +144,20 @@
                     "sentences": [
                         "<tanca> [(la|les)] cortin(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<apaga> el[s] ventilador[s] <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<apaga> tots els ventiladors [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<apaga> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<tanca> <name> [<area>]"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "lock"
-                        ]
-                    },
-                    "sentences": [
-                        "<engega> <name> [en marxa]"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<obre> <name> [<area>]"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<engega> el[s] ventilador[s] <area> [en marxa]"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<engega> tots els ventiladors [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "sentences": [
                         "<engega> tots els llums [<area>]",
                         "<engega> totes les llums [<area>]",
                         "<engega> [els|les] llums [<area>]"
                     ],
                     "slots": {
                         "domain": "light",
@@ -234,14 +200,48 @@
                     "sentences": [
                         "<obre> [(la|les)] cortin(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<engega> el[s] ventilador[s] <area> [en marxa]"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<engega> tots els ventiladors [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "lock"
+                        ]
+                    },
+                    "sentences": [
+                        "<engega> <name> [en marxa]"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<obre> <name> [<area>]"
+                    ]
                 }
             ]
         }
     },
     "language": "ca",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/cs.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907021604938272%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {5: {'sentences': ['(<otevrit>|<roztahnout>) "*

 * *              "(rolet(u|y)|žaluzi(i|e)|závěs[y]) <area>']}, insert: [(3, "*

 * *              "OrderedDict([('sentences', ['<otevrit> {name} [<area>]']), ('requires_context', "*

 * *              "OrderedDict([('domain', 'cover')])), ('response', 'cover')])), (4, "*

 * *              "OrderedDict([('sentences', ['<roztahnout> {name} [<area>]']), ('requires_context', "*

 * *              "OrderedDict([('device_class', ['blind', 'curtain', 'shu […]*

```diff
@@ -77,14 +77,48 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<vypnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky) <area>",
+                        "<area> <vypnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fan",
+                    "sentences": [
+                        "<vypnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k) <area>",
+                        "<area> <vypnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k)"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "fan",
+                            "light"
+                        ]
+                    },
+                    "sentences": [
+                        "<vypnout> {name}",
+                        "{name} <vypnout>"
+                    ]
+                },
+                {
                     "response": "light",
                     "sentences": [
                         "(<vypnout>|<zhasnout>) [sv\u011btlo] {name}",
                         "{name} (<vypnout>|<zhasnout>) [sv\u011btlo]"
                     ],
                     "slots": {
                         "domain": "light"
@@ -109,100 +143,55 @@
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
                     "sentences": [
-                        "(<zavrit>|<zatahnout>) (rolety|\u017ealuzie|z\u00e1v\u011bsy) <area>"
-                    ],
-                    "slots": {
+                        "<zavrit> {name} [<area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
-                    }
-                },
-                {
-                    "response": "fans_area",
+                    },
+                    "response": "cover",
                     "sentences": [
-                        "<vypnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky) <area>",
-                        "<area> <vypnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
+                        "<zatahnout> {name} [<area>]"
+                    ]
                 },
                 {
-                    "response": "fan",
+                    "response": "cover_area",
                     "sentences": [
-                        "<vypnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k) <area>",
-                        "<area> <vypnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k)"
+                        "(<zavrit>|<zatahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]) <area>"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "fan",
-                            "light"
-                        ]
-                    },
-                    "sentences": [
-                        "<vypnout> {name}",
-                        "{name} <vypnout>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "fan",
-                            "light"
-                        ]
-                    },
-                    "sentences": [
-                        "<zapnout> {name}",
-                        "{name} <zapnout>"
-                    ]
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<zapnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky) <area>",
-                        "<area> <zapnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fan",
-                    "sentences": [
-                        "<zapnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k) <area>",
-                        "<area> <zapnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k)"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
                     "response": "light",
                     "sentences": [
                         "(<zapnout>|<rozsvitit>) [sv\u011btlo] {name}",
                         "{name} (<zapnout>|<rozsvitit>) [sv\u011btlo]"
                     ],
                     "slots": {
                         "domain": "light"
@@ -227,26 +216,83 @@
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
+                    "sentences": [
+                        "<otevrit> {name} [<area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
+                    },
+                    "response": "cover",
+                    "sentences": [
+                        "<roztahnout> {name} [<area>]"
+                    ]
+                },
+                {
                     "response": "cover_area",
                     "sentences": [
-                        "(<otevrit>|<roztahnout>) (rolety|\u017ealuzie|z\u00e1v\u011bsy) <area>"
+                        "(<otevrit>|<roztahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]) <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<zapnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky) <area>",
+                        "<area> <zapnout> [v\u0161echny] [stropn\u00ed] (ventil\u00e1tory|v\u011btr\u00e1ky)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fan",
+                    "sentences": [
+                        "<zapnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k) <area>",
+                        "<area> <zapnout> [stropn\u00ed] (ventil\u00e1tor|v\u011btr\u00e1k)"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "fan",
+                            "light"
+                        ]
+                    },
+                    "sentences": [
+                        "<zapnout> {name}",
+                        "{name} <zapnout>"
+                    ]
                 }
             ]
         }
     },
     "language": "cs",
     "lists": {
         "brightness": {
@@ -775,25 +821,25 @@
                 "one": "{{ slots.name | capitalize }} je {{ state.state_with_unit }}\n",
                 "one_cover": "{% set present_continuous = ('je', 'j\u00ed', 'r\u00e1') %}\n{% set present_simple = ('no', 'n\u00e1', 'n\u00e9') %}\n\n{{ slots.name | capitalize }} {{ 'se' if state.state_with_unit.endswith(present_continuous) else 'je' }} {{ state.state_with_unit }}\n",
                 "one_light": "Sv\u011btlo {{ slots.name | capitalize }} je {{ state.state_with_unit }}\n",
                 "one_yesno": "{% set present_continuous = ('je', 'j\u00ed', 'r\u00e1') %}\n{% set present_simple = ('no', 'n\u00e1', 'n\u00e9') %}\n\n{% if query.matched %}\n  Ano, {{ slots.name }} {{ 'se' if state.state_with_unit.endswith(present_continuous) else 'je' }} {{ state.state_with_unit }}\n{% else %}\n  Ne, {{ slots.name }} {{ 'se' if state.state_with_unit.endswith(present_continuous) else 'je' }} {{ state.state_with_unit }}\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  \u017e\u00e1dn\u00e9\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} a {{ (match | length - 3) }} dal\u0161\u00ed\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} a {% endif -%}\n      {{ name }} {{ 'je' if match | length == 1 else 'jsou'}} {{ state.state_with_unit }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "{{ slots.name }} zav\u0159eno",
+                "cover": "{{ slots.name | capitalize }} zav\u0159eno",
                 "cover_area": "St\u00edn\u011bn\u00ed v {{ slots.area }} zav\u0159eno",
                 "default": "{{ slots.name }} vypnuto",
                 "fan": "V\u011btr\u00e1k {{ slots.name }} vypnut",
                 "fans_area": "V\u011btr\u00e1ky v {{ slots.area }} byly vypnuty",
                 "garage": "Gar\u00e1\u017eov\u00e1 vrata zav\u0159ena",
                 "light": "Sv\u011btlo {{ slots.name }} bylo zhasnuto",
                 "lights_area": "Sv\u011btla v {{ slots.area }} byla zhasnuta"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} otev\u0159eno",
+                "cover": "{{ slots.name | capitalize }} otev\u0159eno",
                 "cover_area": "St\u00edn\u011bn\u00ed v {{ slots.area }} otev\u0159eno",
                 "default": "{{ slots.name }} byl zapnut",
                 "fan": "V\u011btr\u00e1k {{ slots.name }} byl zapnut",
                 "fans_area": "V\u011btr\u00e1ky v {{ slots.area }} byly zapnuty",
                 "garage": "Gar\u00e1\u017eov\u00e1 vrata otev\u0159ena",
                 "light": "Sv\u011btlo {{ slots.name }} bylo rozsv\u00edceno",
                 "lights_area": "Sv\u011btla v {{ slots.area }} byla rozsv\u00edcena"
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lv.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7172652450430229%*

 * *Differences: {"'expansion_rules'": "{replace: OrderedDict([('name', '{name}'), ('area', '{area}'), ('ieslēgt', "*

 * *                      "'(palaid | ieslēgt | ieslēdz | ieslēdziet)'), ('izslēgt', '(atslēgt | "*

 * *                      "atslēdz | izslēgt | izslēdz | izslēdziet)'), ('set', '(uzstādi | "*

 * *                      "ieliec[iet] | [(iz|pa)]maini[et] | uzseto)'), ('close', '(aizver[iet] | "*

 * *                      "nolaist)'), ('open', '(atver | pacel)'), ('brightness', '{brightness}[%| "*

 * *                      "procent(i […]*

```diff
@@ -1,283 +1,297 @@
 {
     "expansion_rules": {
-        "al": "(alle | alt)",
-        "bl\u00e6ser": "bl\u00e6ser[(e|en|ne)]",
-        "garaged\u00f8r": "garaged\u00f8r[(en|e|ene)]",
-        "gardin": "gardin[(et|er|erne)]",
-        "i_p\u00e5": "(i | p\u00e5)",
-        "koldt_varmt": "(kold[t] | varm[t])",
-        "luk": "luk [for]",
-        "lys": "lys[(ene|et)]",
-        "lysstyrke": "{brightness}[%| procent]",
-        "navn": "{name}[(en|et|n|t)]",
-        "omr\u00e5de": "{area}[(en|et|n|t)]",
-        "persienne": "persienne[(n|r|rne)]",
-        "rullegardin": "rullegardin[(et|er|erne)]",
-        "skodde": "skodde[(n|r|rne)]",
-        "sluk": "sluk [for]",
-        "temperatur": "{temperature}[\u00b0| grader] [{temperature_unit}]",
-        "t\u00e6nd": "t\u00e6nd [for]",
-        "\u00e5bn": "\u00e5bn [for]"
+        "area": "{area}",
+        "brightness": "{brightness}[%| procent(i|iem|u|us)]",
+        "close": "(aizver[iet] | nolaist)",
+        "iesl\u0113gt": "(palaid | iesl\u0113gt | iesl\u0113dz | iesl\u0113dziet)",
+        "izsl\u0113gt": "(atsl\u0113gt | atsl\u0113dz | izsl\u0113gt | izsl\u0113dz | izsl\u0113dziet)",
+        "name": "{name}",
+        "open": "(atver | pacel)",
+        "set": "(uzst\u0101di | ieliec[iet] | [(iz|pa)]maini[et] | uzseto)",
+        "temperature": "{temperature}[\u00b0| gr\u0101d(s|u|i|iem)] [p\u0113c] [{temperature_unit}]"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<sluk> [<al>] <lys> <i_p\u00e5> <omr\u00e5de>",
-                        "<sluk> [<al>] <omr\u00e5de> <lys>"
+                        "<izsl\u0113gt> [visus] ventilatoru[s] <area>",
+                        "<izsl\u0113gt> <area> [visus] ventilatoru[s]",
+                        "<izsl\u0113gt> visus <area> ventilatoru[s]"
                     ],
                     "slots": {
-                        "domain": "light",
+                        "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<luk> <persienne> <i_p\u00e5> <omr\u00e5de>",
-                        "<luk> <rullegardin> <i_p\u00e5> <omr\u00e5de>",
-                        "rul <rullegardin> ned <i_p\u00e5> <omr\u00e5de>"
-                    ],
-                    "slots": {
-                        "device_class": "blind",
-                        "domain": "cover"
-                    }
+                        "<izsl\u0113gt> <name>",
+                        "<izsl\u0113gt> <area> <name>",
+                        "<izsl\u0113gt> <name> <area>"
+                    ]
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover",
                     "sentences": [
-                        "<luk> <gardin> <i_p\u00e5> <omr\u00e5de>",
-                        "tr\u00e6k <gardin> for <i_p\u00e5> <omr\u00e5de>"
+                        "<close> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<close> <name> <area>"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<izsl\u0113gt> [visas] (gaismas | lampas) <area>",
+                        "<izsl\u0113gt> [visas] <area> (gaismas | lampas)",
+                        "<izsl\u0113gt> <area> visas (gaismas | lampas)",
+                        "<izsl\u0113gt> [visu] (gaismu | apgaismojumu) <area>",
+                        "<izsl\u0113gt> [visu] <area> (gaismu | apgaismojumu)",
+                        "<izsl\u0113gt> <area> visu (gaismu | apgaismojumu)"
                     ],
                     "slots": {
-                        "device_class": "curtain",
-                        "domain": "cover"
+                        "domain": "light",
+                        "name": "all"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<luk> <garaged\u00f8r>"
+                        "<close> [vis(as|us)] gar\u0101\u017e[(a|as|u)] durvis"
                     ],
                     "slots": {
+                        "area": "all",
                         "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "cover",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover_area",
                     "sentences": [
-                        "<luk> <skodde> <i_p\u00e5> <omr\u00e5de>"
+                        "<close> [visas] gar\u0101\u017e[(a|as|u)] [durvis] <area>",
+                        "<close> <area> [visas] gar\u0101\u017e[(a|as|u)] [durvis]"
                     ],
                     "slots": {
-                        "device_class": "shutter",
-                        "domain": "cover"
+                        "device_class": "garage",
+                        "domain": "cover",
+                        "name": "all"
                     }
                 },
                 {
+                    "response": "cover_area",
                     "sentences": [
-                        "<sluk> [<al>] <bl\u00e6ser> <i_p\u00e5> <omr\u00e5de>",
-                        "<sluk> [<al>] <omr\u00e5de> <bl\u00e6ser>"
+                        "<close> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas) <area>",
+                        "<close> <area> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas)"
                     ],
                     "slots": {
-                        "domain": "fan",
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover",
                         "name": "all"
                     }
-                },
-                {
-                    "sentences": [
-                        "<sluk> <navn>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<luk> <navn>",
-                        "<luk> <navn> <i_p\u00e5> <omr\u00e5de>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<t\u00e6nd> <navn>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<\u00e5bn> <navn>",
-                        "<\u00e5bn> <navn> <i_p\u00e5> <omr\u00e5de>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<t\u00e6nd> [<al>] <bl\u00e6ser> <i_p\u00e5> <omr\u00e5de>",
-                        "<t\u00e6nd> [<al>] <omr\u00e5de> <bl\u00e6ser>"
+                        "<iesl\u0113gt> [visas] (gaismas | lampas) <area>",
+                        "<iesl\u0113gt> [visas] <area> (gaismas | lampas)",
+                        "<iesl\u0113gt> <area> visas (gaismas | lampas)",
+                        "<iesl\u0113gt> [visu] (gaismu | apgaismojumu) <area>",
+                        "<iesl\u0113gt> [visu] <area> (gaismu | apgaismojumu)",
+                        "<iesl\u0113gt> <area> visu (gaismu | apgaismojumu)"
                     ],
                     "slots": {
-                        "domain": "fan",
+                        "domain": "light",
                         "name": "all"
                     }
                 },
                 {
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<t\u00e6nd> [<al>] <lys> <i_p\u00e5> <omr\u00e5de>",
-                        "<t\u00e6nd> [<al>] <omr\u00e5de> <lys>"
+                        "<open> [vis(as|us)] gar\u0101\u017e[(a|\u0101|as|i|u)] (durvis | v\u0101rtus)"
                     ],
                     "slots": {
-                        "domain": "light",
+                        "area": "all",
+                        "device_class": "garage",
+                        "domain": "cover",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover_area",
                     "sentences": [
-                        "<\u00e5bn> <persienne> <i_p\u00e5> <omr\u00e5de>",
-                        "<\u00e5bn> <rullegardin> <i_p\u00e5> <omr\u00e5de>",
-                        "rul <rullegardin> op <i_p\u00e5> <omr\u00e5de>"
+                        "<open> [visas] gar\u0101\u017e[(a|\u0101|as|i|u)] [durvis | v\u0101rtus] <area>",
+                        "<open> <area> [visas] gar\u0101\u017e[(a|\u0101|as|i|u)] [durvis | v\u0101rtus]"
                     ],
                     "slots": {
-                        "device_class": "blind",
-                        "domain": "cover"
+                        "device_class": "garage",
+                        "domain": "cover",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover_area",
                     "sentences": [
-                        "<\u00e5bn> <gardin> <i_p\u00e5> <omr\u00e5de>",
-                        "tr\u00e6k <gardin> fra <i_p\u00e5> <omr\u00e5de>"
+                        "<open> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas) <area>",
+                        "<open> <area> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas)"
                     ],
                     "slots": {
-                        "device_class": "curtain",
-                        "domain": "cover"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u00e5bn> <garaged\u00f8r>"
+                        "<iesl\u0113gt> [visus] ventilatoru[s] <area>",
+                        "<iesl\u0113gt> <area> [visus] ventilatoru[s]",
+                        "<iesl\u0113gt> [visus] <area> ventilatoru[s]"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u00e5bn> <skodde> <i_p\u00e5> <omr\u00e5de>"
-                    ],
-                    "slots": {
-                        "device_class": "shutter",
-                        "domain": "cover"
-                    }
+                        "<iesl\u0113gt> <name>",
+                        "<iesl\u0113gt> <area> <name>",
+                        "<iesl\u0113gt> <name> <area>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<open> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<open> <name> <area>"
+                    ]
                 }
             ]
         }
     },
-    "language": "da",
+    "language": "lv",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "hvid",
+                    "in": "balt(s|a|\u0101|o)",
                     "out": "white"
                 },
                 {
-                    "in": "sort",
+                    "in": "meln(s|a|\u0101|o)",
                     "out": "black"
                 },
                 {
-                    "in": "r\u00f8d",
+                    "in": "sarkan(s|a|\u0101|o)",
                     "out": "red"
                 },
                 {
-                    "in": "orange",
+                    "in": "oran\u017e(s|a|\u0101|o)",
                     "out": "orange"
                 },
                 {
-                    "in": "gul",
+                    "in": "dzelten(s|a|\u0101|o)",
                     "out": "yellow"
                 },
                 {
-                    "in": "gr\u00f8n",
+                    "in": "za\u013c(\u0161|a|\u0101|o)",
                     "out": "green"
                 },
                 {
-                    "in": "bl\u00e5",
+                    "in": "zil(s|a|\u0101|o)",
                     "out": "blue"
                 },
                 {
-                    "in": "lilla",
+                    "in": "violet(s|a|\u0101|o)",
                     "out": "purple"
                 },
                 {
-                    "in": "brun",
+                    "in": "br\u016bn(s|a|\u0101|o)",
                     "out": "brown"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "celsius",
                 {
-                    "in": "c",
+                    "in": "c | celsija | p\u0113c celsija",
                     "out": "celsius"
                 },
-                "fahrenheit",
                 {
-                    "in": "f",
+                    "in": "f | f\u0101renheita | p\u0113c f\u0101renheita",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Der opstod en uventet fejl under h\u00e5ndtering af hensigten",
-            "no_area": "Omr\u00e5det med navnet {{ area }} findes ikke",
-            "no_device_class": "{{ device_class }} findes ikke i omr\u00e5det {{ area }}",
-            "no_domain": "{{ domain }} findes ikke i omr\u00e5det {{ area }}",
-            "no_entity": "{{ entity }} findes ikke",
-            "no_intent": "Undskyld, det forstod jeg ikke"
+            "handle_error": "Apstr\u0101d\u0101jot nol\u016bku, rad\u0101s neparedz\u0113ta k\u013c\u016bda",
+            "no_area": "Nav zonas ar nosaukumu {{ area }}",
+            "no_device_class": "Zon\u0101 {{ area }} nav {{ device_class }}",
+            "no_domain": "Zon\u0101 {{ area }} nav {{ domain }}",
+            "no_entity": "Nav ier\u012bces vai ent\u012btijas ar nosaukumu {{ entity }}",
+            "no_intent": "Atvainojiet, es nevar\u0113ju to saprast"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "Lukkede {{ slots.name }}",
-                "cover_area": "Lukkede {{ slots.area}}",
-                "cover_device_class": "Lukkede {{ slots.device_class }}",
-                "default": "Slukkede {{ slots.name }}",
-                "fans_area": "Slukkede bl\u00e6sere i {{ slots.name }}",
-                "lights_area": "Slukkede lys i {{ slots.name }}"
+                "cover": "Closed {{ slots.name }}",
+                "cover_area": "Closed {{ slots.area }}",
+                "cover_device_class": "Closed {{ slots.device_class }}",
+                "default": "Turned off {{ slots.name }}",
+                "fans_area": "Turned off fans in {{ slots.area }}",
+                "lights_area": "Turned off lights in {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "\u00c5bnede {{ slots.name }}",
-                "cover_area": "\u00c5bnede {{ slots.area }}",
-                "cover_device_class": "\u00c5bnede {{ slots.device_class }}",
-                "default": "T\u00e6ndte {{ slots.name }}",
-                "fans_area": "T\u00e6ndte bl\u00e6sere i {{ slots.area }}",
-                "lights_area": "T\u00e6ndte lys i {{ slots.area }}"
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}",
+                "cover_device_class": "Opened {{ slots.device_class }}",
+                "default": "Turned on {{ slots.name }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "lights_area": "Turned on lights in {{ slots.area }}"
             }
         }
     },
-    "skip_words": []
+    "skip_words": [
+        "l\u016bdzu",
+        "paldies",
+        "[vai] vari",
+        "ir",
+        "\u0101r\u0101",
+        "va\u013c\u0101"
+    ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883596380471381%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(12, OrderedDict([('sentences', ['Isch <name> "*

 * *              "{lock_states:state} [<area>]']), ('response', 'one_yesno'), ('requires_context', "*

 * *              "OrderedDict([('domain', 'lock')])), ('slots', OrderedDict([('domain', "*

 * *              "'lock')]))])), (13, OrderedDict([('sentences', ['Isch (e|es|ei) "*

 * *              "(Tür[e]|Tor|Schloss) {lock_states:state} [<area>]', 'Isch [<area>] (e|es|ei) "*

 * *              "(Tür[e]|Tor|Schloss) {lock_states:stat […]*

```diff
@@ -14,67 +14,14 @@
         "temp": "{temperature} [Grad] [{temperature_unit}]",
         "what_is": "(was isch|wasch)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "Isch <name> {lock_states:state} [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "Isch (e|es|ei) (T\u00fcr[e]|Tor|Schloss) {lock_states:state} [<area>]",
-                        "Isch [<area>] (e|es|ei) (T\u00fcr[e]|Tor|Schloss) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "Sy aui (T\u00fcre|Tor|Schl\u00f6sser) {lock_states:state} [<area>]",
-                        "Sy aui (T\u00fcre|Tor|Schl\u00f6sser) [<area>] {lock_states:state}",
-                        "Sy [<area>] aui (T\u00fcre|Tor|Schl\u00f6sser) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(Weles|Weli) (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) (isch|sy|si) {lock_states:state} [<area>]",
-                        "(Weles|weli) (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) [<area>] (isch|sy|si) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "Wie m\u00e4ng[s|i] (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) (isch|sy|si) {lock_states:state} [<area>]",
-                        "Wie m\u00e4ng[s|i] (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) [<area>] (isch|sy|si) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one",
                     "sentences": [
@@ -207,64 +154,73 @@
                     "sentences": [
                         "Wie m\u00e4ng[s|e|i] {cover_classes:device_class} (isch|sy|si) {cover_states:state} [<area>]",
                         "Wie m\u00e4ng[s|e|i] {cover_classes:device_class} <area> (isch|sy|si) {cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                }
-            ]
-        },
-        "HassTurnOff": {
-            "data": [
+                },
                 {
                     "requires_context": {
-                        "domain": "light"
+                        "domain": "lock"
                     },
-                    "response": "light",
+                    "response": "one_yesno",
                     "sentences": [
-                        "(Z\u00fcnd|Mach|L\u00f6sch|Schalt|Schaut) [<Liecht>] <name> <ab_us>"
+                        "Isch <name> {lock_states:state} [<area>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "lights_area",
+                    "response": "any",
                     "sentences": [
-                        "(Z\u00fcnd|Mach|Schalt|Schaut) (<Liecht>|<Liechter>) <ab_us> <area>",
-                        "(Z\u00fcnd|Mach|Schalt|Schaut) (<Liecht>|<Liechter>) <area> <ab_us>",
-                        "(Z\u00fcnd|Mach|Schalt|Schaut) <area> (<Liecht>|<Liechter>) [<ab_us>]",
-                        "L\u00f6sch <area> (<Liecht>|<Liechter>) [<ab_us>]",
-                        "L\u00f6sch (<Liecht>|<Liechter>) <area> [<ab_us>]",
-                        "L\u00f6sch (<Liecht>|<Liechter>) [<ab_us>] <area>"
+                        "Isch (e|es|ei) (T\u00fcr[e]|Tor|Schloss) {lock_states:state} [<area>]",
+                        "Isch [<area>] (e|es|ei) (T\u00fcr[e]|Tor|Schloss) {lock_states:state}"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "cover",
+                    "response": "all",
                     "sentences": [
-                        "<mach> <name> (zue|abe)"
+                        "Sy aui (T\u00fcre|Tor|Schl\u00f6sser) {lock_states:state} [<area>]",
+                        "Sy aui (T\u00fcre|Tor|Schl\u00f6sser) [<area>] {lock_states:state}",
+                        "Sy [<area>] aui (T\u00fcre|Tor|Schl\u00f6sser) {lock_states:state}"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "which",
                     "sentences": [
-                        "<mach> <cover> <area> (zue|abe)"
+                        "(Weles|Weli) (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) (isch|sy|si) {lock_states:state} [<area>]",
+                        "(Weles|weli) (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) [<area>] (isch|sy|si) {lock_states:state}"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "lock"
                     }
                 },
                 {
+                    "response": "how_many",
+                    "sentences": [
+                        "Wie m\u00e4ng[s|i] (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) (isch|sy|si) {lock_states:state} [<area>]",
+                        "Wie m\u00e4ng[s|i] (T\u00fcr[e]|Tor|Schloss|Schl\u00f6sser) [<area>] (isch|sy|si) {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                }
+            ]
+        },
+        "HassTurnOff": {
+            "data": [
+                {
                     "requires_context": {
                         "domain": "fan"
                     },
                     "response": "fan",
                     "sentences": [
                         "(Schalt|Schaut|Mach) <name> <ab_us>"
                     ],
@@ -301,95 +257,63 @@
                             "cover"
                         ]
                     },
                     "response": "default_area",
                     "sentences": [
                         "(Schalt|Schaut|Mach) <Ger\u00e4te> <area> <ab_us>"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "light",
-                            "fan",
-                            "cover",
-                            "scene",
-                            "script"
-                        ]
-                    },
-                    "sentences": [
-                        "(Schalt|Schaut|Schteu|Stell|Mach) <name> <a_y>"
-                    ]
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "light",
-                            "fan",
-                            "cover",
-                            "scene",
-                            "script"
-                        ]
-                    },
-                    "response": "default_area",
-                    "sentences": [
-                        "(Schalt|Schaut|Schteu|Stell|Mach) <Ger\u00e4te> <area> <a_y>"
-                    ]
                 },
                 {
                     "requires_context": {
-                        "domain": "scene"
+                        "domain": "light"
                     },
-                    "response": "scene",
+                    "response": "light",
                     "sentences": [
-                        "(Aktivier|Schalt|Schaut|Schteu|Stell|Mach) <name> [Szene] [<a_y>]",
-                        "(Aktivier|Schalt|Schaut|Schteu|Stell|Mach) [d[' '] Szene] <name> [<a_y>]"
+                        "(Z\u00fcnd|Mach|L\u00f6sch|Schalt|Schaut) [<Liecht>] <name> <ab_us>"
                     ],
                     "slots": {
-                        "domain": "scene"
+                        "domain": "light"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
+                    "response": "lights_area",
                     "sentences": [
-                        "(Aktivier|Start|Schtart) <name> [Script]",
-                        "(Aktivier|Start|Schtart) [(ds Script|dr Code)] <name>"
+                        "(Z\u00fcnd|Mach|Schalt|Schaut) (<Liecht>|<Liechter>) <ab_us> <area>",
+                        "(Z\u00fcnd|Mach|Schalt|Schaut) (<Liecht>|<Liechter>) <area> <ab_us>",
+                        "(Z\u00fcnd|Mach|Schalt|Schaut) <area> (<Liecht>|<Liechter>) [<ab_us>]",
+                        "L\u00f6sch <area> (<Liecht>|<Liechter>) [<ab_us>]",
+                        "L\u00f6sch (<Liecht>|<Liechter>) <area> [<ab_us>]",
+                        "L\u00f6sch (<Liecht>|<Liechter>) [<ab_us>] <area>"
                     ],
                     "slots": {
-                        "domain": "script"
+                        "domain": "light"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "fan"
-                    },
-                    "response": "fan",
+                    "response": "cover",
                     "sentences": [
-                        "(Schalt|Schaut|Schteu|Stell|Mach) <name> <a_y>"
+                        "<mach> <name> (zue|abe)"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "fans_area",
+                    "response": "cover_area",
                     "sentences": [
-                        "(Schalt|Schaut|Schteu|Stell|Mach) (d'|d|alli|aui) Ventilatore <area> <a_y>"
+                        "<mach> <cover> <area> (zue|abe)"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "cover"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "light",
                     "sentences": [
                         "(Z\u00fcnd|Mach|Schalt|Schaut) [<Liecht>] <name> [<a_y>]"
@@ -424,14 +348,90 @@
                     "response": "cover_area",
                     "sentences": [
                         "<mach> <cover> <area> (uf|uuf)"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "fan"
+                    },
+                    "response": "fan",
+                    "sentences": [
+                        "(Schalt|Schaut|Schteu|Stell|Mach) <name> <a_y>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "(Schalt|Schaut|Schteu|Stell|Mach) (d'|d|alli|aui) Ventilatore <area> <a_y>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "light",
+                            "fan",
+                            "cover",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "(Schalt|Schaut|Schteu|Stell|Mach) <name> <a_y>"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "light",
+                            "fan",
+                            "cover",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "default_area",
+                    "sentences": [
+                        "(Schalt|Schaut|Schteu|Stell|Mach) <Ger\u00e4te> <area> <a_y>"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
+                    "sentences": [
+                        "(Aktivier|Schalt|Schaut|Schteu|Stell|Mach) <name> [Szene] [<a_y>]",
+                        "(Aktivier|Schalt|Schaut|Schteu|Stell|Mach) [d[' '] Szene] <name> [<a_y>]"
+                    ],
+                    "slots": {
+                        "domain": "scene"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "(Aktivier|Start|Schtart) <name> [Script]",
+                        "(Aktivier|Start|Schtart) [(ds Script|dr Code)] <name>"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
                 }
             ]
         }
     },
     "language": "de-CH",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/de.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9824903804721513%*

 * *Differences: {"'expansion_rules'": "{'tuer': '[die] Tür[e|en]', 'schloss': '[das|die] (Schloss|Schlösser)'}",*

 * * "'intents'": "{'HassGetState': {'data': {insert: [(11, OrderedDict([('sentences', ['ist <name> "*

 * *              "{lock_states:state} [<area>]', 'ist <name> [<area>] {lock_states:state}', 'ist "*

 * *              "[<area>] <name> {lock_states:state}']), ('response', 'einzeln_janein'), "*

 * *              "('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]) […]*

```diff
@@ -19,85 +19,29 @@
         "garage": "(die Garage|die Garagen|das Garagentor|die Garagentore)",
         "licht": "([das] Licht|[die] Lampe|[die] Beleuchtung)",
         "lichter": "[die|der|von den] (Lichter|Lichtern|Lampen|Leuchten|Beleuchtungen)",
         "luefter": "(den Ventilator|die Ventilatoren|(den|die) L\u00fcfter)",
         "machen": "(mach[e|en])",
         "name": "[(der|den|dem|die|das)] {name}",
         "schliessen": "(schlie(\u00df|ss)|schlie(\u00df|ss)e|zumachen|zu machen)",
+        "schloss": "[das|die] (Schloss|Schl\u00f6sser)",
         "setzen": "(setz[e|en]|stell[e|en]|einstellen|\u00e4nder[e|n]|ver\u00e4nder[e|n])",
         "skript": "[das] Skript",
         "sperren": "(sperr|schlie(ss|\u00df))[e|en]",
         "szene": "[die] Szene",
         "temperature": "{temperature} [Grad] [{temperature_unit}]",
         "tor": "(das Tor|die Tore)",
+        "tuer": "[die] T\u00fcr[e|en]",
         "von_dem": "(von [dem]|vom)",
         "zu": "(zu|[he]runter|nach unten)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "einzeln_janein",
-                    "sentences": [
-                        "ist <name> {lock_states:state} [<area>]",
-                        "ist <name> [<area>] {lock_states:state}",
-                        "ist [<area>] <name> {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "irgendeins",
-                    "sentences": [
-                        "sind [irgendwelche|einige] {lock_domains:domain} {lock_states:state} [<area>]",
-                        "sind [irgendwelche|einige] {lock_domains:domain} [<area>] {lock_states:state}",
-                        "sind [<area>] [irgendwelche|einige] {lock_domains:domain} {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "alle",
-                    "sentences": [
-                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} {lock_states:state} [<area>]",
-                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} [<area>] {lock_states:state}",
-                        "(sind|ist) [<area>] (alle|jede[(r|s)]) {lock_domains:domain} {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "welches",
-                    "sentences": [
-                        "welche[(r|s)] {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
-                        "welche[(r|s)] {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
-                        "welche[(r|s)] {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "wie_viele",
-                    "sentences": [
-                        "wie viele {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
-                        "wie viele {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
-                        "wie viele {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "einzeln",
@@ -204,21 +148,116 @@
                         "wie viele {cover_classes:device_class} (ist|sind) {cover_states:state} [<area>]",
                         "wie viele {cover_classes:device_class} (ist|sind) [<area>] {cover_states:state}",
                         "wie viele {cover_classes:device_class} [<area>] (ist|sind) {cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "einzeln_janein",
+                    "sentences": [
+                        "ist <name> {lock_states:state} [<area>]",
+                        "ist <name> [<area>] {lock_states:state}",
+                        "ist [<area>] <name> {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "sind [irgendwelche|einige] {lock_domains:domain} {lock_states:state} [<area>]",
+                        "sind [irgendwelche|einige] {lock_domains:domain} [<area>] {lock_states:state}",
+                        "sind [<area>] [irgendwelche|einige] {lock_domains:domain} {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "alle",
+                    "sentences": [
+                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} {lock_states:state} [<area>]",
+                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} [<area>] {lock_states:state}",
+                        "(sind|ist) [<area>] (alle|jede[(r|s)]) {lock_domains:domain} {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "welches",
+                    "sentences": [
+                        "welche[(r|s)] {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
+                        "welche[(r|s)] {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
+                        "welche[(r|s)] {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "wie_viele",
+                    "sentences": [
+                        "wie viele {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
+                        "wie viele {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
+                        "wie viele {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "schalte <luefter> <area> <aus>",
+                        "schalte <area> <luefter> <aus>",
+                        "stoppe <luefter> <area> [<aus>]",
+                        "stoppe <area> <luefter> [<aus>]",
+                        "(mach|mache) <luefter> <area> <aus>",
+                        "(mach|mache) <area> <luefter> <aus>",
+                        "schalte <alle_luefter> [<area>] <aus>",
+                        "schalte [<area>] <alle_luefter> <aus>",
+                        "stoppe <alle_luefter> [<area>] [<aus>]",
+                        "stoppe [<area>] <alle_luefter> [<aus>]",
+                        "(mach|mache) <alle_luefter> [<area>] <aus>",
+                        "(mach|mache) [<area>] <alle_luefter> <aus>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "schalte <name> <aus>",
+                        "stoppe <name>",
+                        "<deaktivieren> <name>",
+                        "<name> <deaktivieren>",
+                        "<name> <aus>[schalten]"
+                    ]
+                },
+                {
+                    "sentences": [
                         "Schalte (<licht>|<lichter>) <area> <aus>",
                         "Schalte <area> (<licht>|<lichter>) <aus>",
                         "(<licht>|<lichter>) <area> <aus>schalten",
                         "<area> (<licht>|<lichter>) <aus>schalten",
                         "<machen> (<licht>|<lichter>) <area> <aus>",
                         "<machen> <area> (<licht>|<lichter>) <aus>",
                         "(<licht>|<lichter>) <area> <aus><machen>",
@@ -271,123 +310,50 @@
                         "(<sperren>|<machen>) <name> [<area>] auf",
                         "(<sperren>|<machen>) <area> <name> auf",
                         "<name> [<area>] (auf[machen]|<entsperren>)",
                         "<area> <name> (auf[machen]|<entsperren>)"
                     ]
                 },
                 {
-                    "sentences": [
-                        "schalte <luefter> <area> <aus>",
-                        "schalte <area> <luefter> <aus>",
-                        "stoppe <luefter> <area> [<aus>]",
-                        "stoppe <area> <luefter> [<aus>]",
-                        "(mach|mache) <luefter> <area> <aus>",
-                        "(mach|mache) <area> <luefter> <aus>",
-                        "schalte <alle_luefter> [<area>] <aus>",
-                        "schalte [<area>] <alle_luefter> <aus>",
-                        "stoppe <alle_luefter> [<area>] [<aus>]",
-                        "stoppe [<area>] <alle_luefter> [<aus>]",
-                        "(mach|mache) <alle_luefter> [<area>] <aus>",
-                        "(mach|mache) [<area>] <alle_luefter> <aus>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
+                    "requires_context": {
+                        "domain": "lock",
                         "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script"
-                        ]
                     },
+                    "response": "lock",
                     "sentences": [
-                        "schalte <name> <aus>",
-                        "stoppe <name>",
-                        "<deaktivieren> <name>",
-                        "<name> <deaktivieren>",
-                        "<name> <aus>[schalten]"
+                        "<entsperren> [alle] (<tuer>|<schloss>) <area>",
+                        "<entsperren> <area> [alle] (<tuer>|<schloss>)",
+                        "(<sperren>|<machen>) [alle] (<tuer>|<schloss>) <area> auf",
+                        "(<sperren>|<machen>) <area> [alle] (<tuer>|<schloss>) auf",
+                        "[alle] (<tuer>|<schloss>) <area> (auf[machen]|<entsperren>)",
+                        "<area> [alle] (<tuer>|<schloss>) (auf[machen]|<entsperren>)"
                     ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "scene"
                     },
                     "response": "scene",
                     "sentences": [
-                        "[<szene>] <name> (<aktivieren>|<ausfuehren>|<an>)",
+                        "[<szene>] <name> [<aktivieren>|<ausfuehren>|<an>]",
                         "<name> <szene> (<aktivieren>|<ausfuehren>|<an>)",
                         "f\u00fchre [<szene>] <name> aus",
                         "f\u00fchre <name> <szene> aus",
                         "<aktivieren> [<szene>] <name>",
                         "<aktivieren> <name> <szene>"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script"
-                        ]
-                    },
-                    "sentences": [
-                        "schalte <name> <an>",
-                        "starte <name>",
-                        "<aktivieren> <name>",
-                        "<name> <aktivieren>",
-                        "<name> <an>[schalten]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "(<sperren>|<machen>) <name> [<area>] [zu|ab]",
-                        "(<sperren>|<machen>) <area> <name> [zu|ab]",
-                        "<name> [<area>] (zu[machen]|<absperren>)",
-                        "<area> <name> (zu[machen]|<absperren>)",
-                        "<absperren> <name> [<area>]",
-                        "<absperren> <area> <name>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "schalte <luefter> <area> <an>",
-                        "schalte <area> <luefter> <an>",
-                        "starte <luefter> <area> [<an>]",
-                        "starte <area> <luefter> [<an>]",
-                        "(mach|mache) <luefter> <area> <an>",
-                        "(mach|mache) <area> <luefter> <an>",
-                        "starte <alle_luefter> [<area>] [<an>]",
-                        "starte [<area>] <alle_luefter> [<an>]",
-                        "schalte <alle_luefter> [<area>] <an>",
-                        "schalte [<area>] <alle_luefter> <an>",
-                        "(mach|mache) <alle_luefter> [<area>] <an>",
-                        "(mach|mache) [<area>] <alle_luefter> <an>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "sentences": [
                         "Schalte (<licht>|<lichter>) <area> <an>",
                         "Schalte <area> (<licht>|<lichter>) <an>",
                         "(<licht>|<lichter>) <area> <an>schalten",
                         "<area> (<licht>|<lichter>) <an>schalten",
                         "<machen> <area> (<licht>|<lichter>) <an>",
                         "<machen> (<licht>|<lichter>) <area> <an>",
@@ -403,31 +369,14 @@
                         "[<lichter>|<alle_lichter>] [<area>] <an><machen>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
-                    "sentences": [
-                        "[<skript>] <name> (<ausfuehren>|<aktivieren>)",
-                        "<name> <skript> (<ausfuehren>|<aktivieren>)",
-                        "f\u00fchre [<skript>] <name> aus",
-                        "f\u00fchre <name> <skript> aus",
-                        "<aktivieren> [<skript>] <name>",
-                        "<aktivieren> <name> <skript>"
-                    ],
-                    "slots": {
-                        "domain": "script"
-                    }
-                },
-                {
                     "response": "cover_area",
                     "sentences": [
                         "\u00f6ffne <area> (<abdeckung>|<tor>|<garage>)",
                         "\u00f6ffne (<abdeckung>|<tor>|<garage>) <area>",
                         "<machen> <area> (<abdeckung>|<tor>|<garage>) <auf>",
                         "<machen> (<abdeckung>|<tor>|<garage>) <area> <auf>"
                     ],
@@ -446,14 +395,97 @@
                         "\u00f6ffne (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) [<area>]",
                         "<machen> [<area>] (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) <auf>",
                         "<machen> (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) [<area>] <auf>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "schalte <luefter> <area> <an>",
+                        "schalte <area> <luefter> <an>",
+                        "starte <luefter> <area> [<an>]",
+                        "starte <area> <luefter> [<an>]",
+                        "(mach|mache) <luefter> <area> <an>",
+                        "(mach|mache) <area> <luefter> <an>",
+                        "starte <alle_luefter> [<area>] [<an>]",
+                        "starte [<area>] <alle_luefter> [<an>]",
+                        "schalte <alle_luefter> [<area>] <an>",
+                        "schalte [<area>] <alle_luefter> <an>",
+                        "(mach|mache) <alle_luefter> [<area>] <an>",
+                        "(mach|mache) [<area>] <alle_luefter> <an>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "(<sperren>|<machen>) <name> [<area>] [zu|ab]",
+                        "(<sperren>|<machen>) <area> <name> [zu|ab]",
+                        "<name> [<area>] (zu[machen]|<absperren>)",
+                        "<area> <name> (zu[machen]|<absperren>)",
+                        "<absperren> <name> [<area>]",
+                        "<absperren> <area> <name>"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock",
+                        "name": "all"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "(<sperren>|<machen>) [alle] (<tuer>|<schloss>) <area> [zu|ab]",
+                        "(<sperren>|<machen>) <area> [alle] (<tuer>|<schloss>) [zu|ab]",
+                        "[alle] (<tuer>|<schloss>) <area> (zu[machen]|<absperren>)",
+                        "<area> [alle] (<tuer>|<schloss>) (zu[machen]|<absperren>)",
+                        "<absperren> [alle] (<tuer>|<schloss>) <area>",
+                        "<absperren> <area> [alle] (<tuer>|<schloss>)"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "[<skript>] <name> (<ausfuehren>|<aktivieren>)",
+                        "<name> <skript> (<ausfuehren>|<aktivieren>)",
+                        "f\u00fchre [<skript>] <name> aus",
+                        "f\u00fchre <name> <skript> aus",
+                        "<aktivieren> [<skript>] <name>",
+                        "<aktivieren> <name> <skript>"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "schalte <name> <an>",
+                        "starte <name>",
+                        "<aktivieren> <name>",
+                        "<name> <aktivieren>",
+                        "<name> <an>[schalten]"
+                    ]
                 }
             ]
         }
     },
     "language": "de",
     "lists": {
         "brightness": {
@@ -570,19 +602,19 @@
                     "out": "lock"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "(([ab|zu]ge|ver)schlossen|verriegelt)",
+                    "in": "(([ab|zu]ge|ver)(schlossen|sperrt)|verriegelt)",
                     "out": "locked"
                 },
                 {
-                    "in": "(nicht ([ab|zu]ge|ver)schlossen|entriegelt)",
+                    "in": "(nicht (([ab|zu]ge|ver)(schlossen|sperrt)|verriegelt)|ent(riegelt|sperrt)|aufge(sperrt|schlossen))",
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
@@ -652,23 +684,23 @@
             "HassTurnOff": {
                 "close_all": "alle geschlossen",
                 "cover": "{{ slots.name }} geschlossen",
                 "cover_area": "{{ slots.area }} geschlossen",
                 "default": "{{ slots.name }} ausgeschaltet",
                 "fans_area": "Die Ventilatoren in {{ slots.area }} sind ausgeschaltet",
                 "lights_area": "Die Lampen in {{ slots.area }} sind ausgeschaltet",
-                "lock": "{{ slots.name }} entsperrt"
+                "lock": "entsperrt"
             },
             "HassTurnOn": {
                 "cover": "{{ slots.name }} ge\u00f6ffnet",
                 "cover_area": "{{ slots.area }} ge\u00f6ffnet",
                 "default": "{{ slots.name }} eingeschaltet",
                 "fans_area": "Die Ventilatoren in {{ slots.area }} sind eingeschaltet",
                 "lights_area": "Die Lampen in {{ slots.area }} sind eingeschaltet",
-                "lock": "{{ slots.name }} abgeschlossen",
+                "lock": "abgeschlossen",
                 "open_all": "alle ge\u00f6ffnet",
                 "scene": "{{ slots.name }} aktiviert",
                 "script": "{{ slots.name }} gestartet"
             }
         }
     },
     "skip_words": [
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/el.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9881448412698411%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {0: {'sentences': ['<turn_on> [<all>] <articles> <lights> "*

 * *              "<area>', '<turn_on> <area> [<all>] <articles> <lights>'], 'slots': "*

 * *              "OrderedDict([('domain', 'light'), ('name', 'all')])}, 1: {'sentences': ['<turn_on> "*

 * *              '[(πάνω | ψηλά)] [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) [(πάνω | '*

 * *              "ψηλά)]'], 'response': 'cover_device_class', 'slots': OrderedDict([('domain', "*

 * *              "'cover'), ('device_ […]*

```diff
@@ -16,14 +16,32 @@
         "turn_on": "(\u03ac\u03bd\u03bf\u03b9\u03be\u03b5 | \u03ac\u03c1\u03c7\u03b9\u03c3\u03b5 | \u03be\u03b5\u03ba\u03af\u03bd\u03b1 | \u03b5\u03bd\u03b5\u03c1\u03b3\u03bf\u03c0\u03bf\u03af\u03b7\u03c3\u03b5 | \u03ac\u03bd\u03b1\u03c8\u03b5 | \u03c3\u03ae\u03ba\u03c9\u03c3\u03b5 | \u03ac\u03bd\u03bf\u03b9\u03be\u03b5 | \u03b5\u03bd\u03b5\u03c1\u03b3\u03bf\u03c0\u03bf\u03af\u03b7\u03c3\u03b5 | \u03ac\u03c1\u03c7\u03b9\u03c3\u03b5 | \u03be\u03b5\u03ba\u03af\u03bd\u03b1 | \u03b1\u03bd\u03bf\u03af\u03be\u03b5\u03b9[\u03c2] | \u03b5\u03bd\u03b5\u03c1\u03b3\u03bf\u03c0\u03bf\u03b9\u03ae\u03c3\u03b5\u03b9\u03c2 | \u03b5\u03bd\u03b5\u03c1\u03b3\u03bf\u03c0\u03bf\u03b9\u03b7\u03b8\u03b5\u03af | \u03b1\u03c1\u03c7\u03af\u03c3\u03b5\u03b9[\u03c2] | \u03be\u03b5\u03ba\u03b9\u03bd\u03ae\u03c3\u03b5\u03b9[\u03c2])"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "<turn_off> [<all>] [<articles>] <fans> [<articles>] [<area>]",
+                        "<turn_off> [<articles>] [<area>] [<all>] [<articles>] <fans>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<turn_off> <articles> <name>",
+                        "<articles> <name> \u03bd\u03b1 <turn_off>",
+                        "\u03bd\u03b1 <turn_off> <articles> <name>",
+                        "\u03bd\u03b1 <turn_off> <articles> <name>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "<turn_off> [<all>] <articles> <lights> <area>",
                         "<turn_off> <area> [<all>] <articles> <lights>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
@@ -49,64 +67,21 @@
                         "<turn_off> [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) \u03c3\u03c4\u03b7\u03bd \u03c0\u03b5\u03c1\u03b9\u03bf\u03c7\u03ae <area>",
                         "<turn_off> [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) <articles> <area>",
                         "<turn_off> <articles> <area> [<all>] <articles> (<garage_doors> | <doors> | <covers>)"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> [<all>] [<articles>] <fans> [<articles>] [<area>]",
-                        "<turn_off> [<articles>] [<area>] [<all>] [<articles>] <fans>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> <articles> <name>",
-                        "<articles> <name> \u03bd\u03b1 <turn_off>",
-                        "\u03bd\u03b1 <turn_off> <articles> <name>",
-                        "\u03bd\u03b1 <turn_off> <articles> <name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<turn_on> <articles> <name>",
-                        "<articles> <name> \u03bd\u03b1 <turn_on>",
-                        "\u03bd\u03b1 <turn_on> <articles> <name>",
-                        "\u03bd\u03b1 <turn_on> <articles> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<turn_on> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)] [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) <articles> <area> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)]",
-                        "<turn_on> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)] <articles> <area> [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)]"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<turn_on> [<all>] [<articles>] <fans> [<articles>] [<area>]",
-                        "<turn_on> [<articles>] [<area>] [<all>] [<articles>] <fans>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
                         "<turn_on> [<all>] <articles> <lights> <area>",
                         "<turn_on> <area> [<all>] <articles> <lights>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
@@ -121,14 +96,39 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> [<all>] [<articles>] <fans> [<articles>] [<area>]",
+                        "<turn_on> [<articles>] [<area>] [<all>] [<articles>] <fans>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> <articles> <name>",
+                        "<articles> <name> \u03bd\u03b1 <turn_on>",
+                        "\u03bd\u03b1 <turn_on> <articles> <name>",
+                        "\u03bd\u03b1 <turn_on> <articles> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<turn_on> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)] [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) <articles> <area> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)]",
+                        "<turn_on> [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)] <articles> <area> [<all>] [<articles>] (<garage_doors> | <doors> | <covers>) [(\u03c0\u03ac\u03bd\u03c9 | \u03c8\u03b7\u03bb\u03ac)]"
+                    ]
                 }
             ]
         }
     },
     "language": "el",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991626913138541%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(119, OrderedDict([('sentences', ['is <name> "*

 * *              "{lock_states:state} [in <area>]']), ('response', 'one_yesno'), ('requires_context', "*

 * *              "OrderedDict([('domain', 'lock')])), ('slots', OrderedDict([('domain', "*

 * *              "'lock')]))])), (120, OrderedDict([('sentences', ['(is|are) any door[s] "*

 * *              "{lock_states:state} [in <area>]']), ('response', 'any'), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])),  […]*

```diff
@@ -14,62 +14,14 @@
         "what_is": "(what's|whats|what is)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "is <name> {lock_states:state} [in <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "(is|are) any door[s] {lock_states:state} [in <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "are all [the] door[s] {lock_states:state} [in <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(which|what) door[s] (is|are) {lock_states:state} [in <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "how many door[s] (is|are) {lock_states:state} [in <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "requires_context": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     },
                     "response": "one_yesno",
                     "sentences": [
                         "(is|are) <name> [battery] {bs_battery_states:state} [in <area>]"
                     ],
@@ -1371,94 +1323,67 @@
                     "response": "how_many",
                     "sentences": [
                         "how many {cover_classes:device_class} (is|are) {cover_states:state} [in <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                }
-            ]
-        },
-        "HassTurnOff": {
-            "data": [
+                },
                 {
-                    "response": "lights_area",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
                     "sentences": [
-                        "<turn> off [all] <light> in <area>",
-                        "<turn> off [all] <area> <light>",
-                        "[<turn>] [all] <area> <light> off",
-                        "[<turn>] [all] <light> [in] <area> off",
-                        "deactivate [all] <light> [in] <area>",
-                        "deactivate [all] <area> <light>"
+                        "is <name> {lock_states:state} [in <area>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "light_all",
+                    "response": "any",
                     "sentences": [
-                        "[<turn>] (all <light> off|<light> off everywhere)",
-                        "deactivate (all <light>|<light> everywhere)"
+                        "(is|are) any door[s] {lock_states:state} [in <area>]"
                     ],
                     "slots": {
-                        "area": "all",
-                        "domain": "light",
-                        "name": "all"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
-                    "sentences": [
-                        "<close> <name> [in <area>]"
-                    ]
-                },
-                {
-                    "response": "cover_device_class",
+                    "response": "all",
                     "sentences": [
-                        "<close> [the] garage door"
+                        "are all [the] door[s] {lock_states:state} [in <area>]"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "which",
                     "sentences": [
-                        "<close> [the] {cover_classes:device_class} in <area>",
-                        "<close> <area> {cover_classes:device_class}"
+                        "(which|what) door[s] (is|are) {lock_states:state} [in <area>]"
                     ],
                     "slots": {
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "requires_context": {
                         "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "unlock <name> [in <area>]"
-                    ]
+                    }
                 },
                 {
-                    "response": "lock",
+                    "response": "how_many",
                     "sentences": [
-                        "unlock [all] [the] [locks|doors] [in] <area>",
-                        "unlock [all] <area> [locks|doors]"
+                        "how many door[s] (is|are) {lock_states:state} [in <area>]"
                     ],
                     "slots": {
-                        "domain": "lock",
-                        "name": "all"
+                        "domain": "lock"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOff": {
+            "data": [
                 {
                     "response": "fans_area",
                     "sentences": [
                         "<turn> off [all] [the] fan[s] in <area>",
                         "<turn> off <area> fan[s]",
                         "[<turn>] [all] <area> fan[s] off",
                         "[<turn>] [all] [the] fan[s] [in] <area> off",
@@ -1494,80 +1419,104 @@
                         ]
                     },
                     "sentences": [
                         "<turn> off <name> [light[s]|switch[es]]",
                         "[<turn>] <name> [light[s]|switch[es]] [to] off",
                         "deactivate <name> [light[s]|switch[es]]"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                },
                 {
-                    "requires_context": {
-                        "domain": "scene"
-                    },
-                    "response": "scene",
+                    "response": "lights_area",
                     "sentences": [
-                        "[activate|<turn>] <name> [scene] [on]"
+                        "<turn> off [all] <light> in <area>",
+                        "<turn> off [all] <area> <light>",
+                        "[<turn>] [all] <area> <light> off",
+                        "[<turn>] [all] <light> [in] <area> off",
+                        "deactivate [all] <light> [in] <area>",
+                        "deactivate [all] <area> <light>"
                     ],
                     "slots": {
-                        "domain": "scene"
+                        "domain": "light"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
+                    "response": "light_all",
+                    "sentences": [
+                        "[<turn>] (all <light> off|<light> off everywhere)",
+                        "deactivate (all <light>|<light> everywhere)"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "light",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "cover"
                     },
+                    "response": "cover",
                     "sentences": [
-                        "<turn> on <name> [light[s]|switch[es]]",
-                        "[<turn>] <name> [light[s]|switch[es]] [to] on",
-                        "activate <name> [light[s]|switch[es]]"
+                        "<close> <name> [in <area>]"
                     ]
                 },
                 {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "<close> [the] garage door"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "<close> [the] {cover_classes:device_class} in <area>",
+                        "<close> <area> {cover_classes:device_class}"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
+                },
+                {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "lock",
                     "sentences": [
-                        "lock <name> [in <area>]"
+                        "unlock <name> [in <area>]"
                     ]
                 },
                 {
                     "response": "lock",
                     "sentences": [
-                        "lock [all] [the] [locks|doors] [in] <area>",
-                        "lock [all] <area> [locks|doors]"
+                        "unlock [all] [the] [locks|doors] [in] <area>",
+                        "unlock [all] <area> [locks|doors]"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
-                    "response": "fans_area",
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
                     "sentences": [
-                        "<turn> on [all] [the] fan[s] in <area>",
-                        "<turn> on <area> fan[s]",
-                        "[<turn>] [all] <area> fan[s] on",
-                        "activate [all] <area> fan[s]",
-                        "activate [all] fan[s] [in] <area>"
+                        "[activate|<turn>] <name> [scene] [on]"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "scene"
                     }
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
                         "<turn> on [all] <light> in <area>",
                         "<turn> on [all] <area> <light>",
@@ -1578,26 +1527,14 @@
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
-                    "sentences": [
-                        "[run|start|<turn>] <name> [script] [on]"
-                    ],
-                    "slots": {
-                        "domain": "script"
-                    }
-                },
-                {
-                    "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
                         "<open> <name> [in <area>]"
                     ]
                 },
@@ -1616,14 +1553,77 @@
                     "sentences": [
                         "<open> [the] {cover_classes:device_class} in <area>",
                         "<open> <area> {cover_classes:device_class}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn> on [all] [the] fan[s] in <area>",
+                        "<turn> on <area> fan[s]",
+                        "[<turn>] [all] <area> fan[s] on",
+                        "activate [all] <area> fan[s]",
+                        "activate [all] fan[s] [in] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "lock <name> [in <area>]"
+                    ]
+                },
+                {
+                    "response": "lock",
+                    "sentences": [
+                        "lock [all] [the] [locks|doors] [in] <area>",
+                        "lock [all] <area> [locks|doors]"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "[run|start|<turn>] <name> [script] [on]"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<turn> on <name> [light[s]|switch[es]]",
+                        "[<turn>] <name> [light[s]|switch[es]] [to] on",
+                        "activate <name> [light[s]|switch[es]]"
+                    ]
                 }
             ]
         }
     },
     "language": "en",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/es.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912037037037037%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(4, OrderedDict([('sentences', ['<enciende> "*

 * *              "[todos] [los|el] ventilador[es] <area>']), ('slots', OrderedDict([('domain', "*

 * *              "'fan'), ('name', 'all')])), ('response', 'fans_area')])), (5, "*

 * *              "OrderedDict([('sentences', ['<enciende> <name>', '<enciende> <name> <area>'])])), "*

 * *              "(6, OrderedDict([('sentences', ['<abre> <name>']), ('response', 'cover')])), (7, "*

 * *              "OrderedDict([('sentences', ['<ab […]*

```diff
@@ -117,14 +117,36 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<apaga> [todos] [el|los] ventilador[es] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<apaga> <name>",
+                        "<apaga> <name> <area>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<cierra> <name> [<area>]"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<apaga> [(la|las)] (luz | luces) <area>",
                         "<apaga> todas las luces <area>"
                     ],
                     "slots": {
                         "domain": "light",
@@ -160,70 +182,20 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<apaga> [todos] [el|los] ventilador[es] <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<apaga> <name>",
-                        "<apaga> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<cierra> <name> [<area>]"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "sentences": [
-                        "<enciende> <name>",
-                        "<enciende> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<abre> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<abre> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<enciende> [todos] [los|el] ventilador[es] <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "<enciende> ([la] luz | [las] luces) <area>",
                         "<enciende> todas las luces <area>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -258,14 +230,42 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<enciende> [todos] [los|el] ventilador[es] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<enciende> <name>",
+                        "<enciende> <name> <area>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<abre> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<abre> <name> <area>"
+                    ]
                 }
             ]
         }
     },
     "language": "es",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fa.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
 {
     "language": "fa",
     "intents": {
-        "HassTurnOn": {
+        "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "{name} (\u0631\u0627 | \u0631\u0648) \u0631\u0648\u0634\u0646 \u06a9\u0646"
+                        "{name} (\u0631\u0627 | \u0631\u0648) \u062e\u0627\u0645\u0648\u0634 \u06a9\u0646"
                     ]
                 }
             ]
         },
-        "HassTurnOff": {
+        "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "{name} (\u0631\u0627 | \u0631\u0648) \u062e\u0627\u0645\u0648\u0634 \u06a9\u0646"
+                        "{name} (\u0631\u0627 | \u0631\u0648) \u0631\u0648\u0634\u0646 \u06a9\u0646"
                     ]
                 }
             ]
         }
     },
     "responses": {
         "errors": {
@@ -26,29 +26,29 @@
             "no_area": "\u0648\u062c\u0648\u062f \u0646\u062f\u0627\u0631\u062f {{ area }} \u0647\u06cc\u0686 \u0645\u0646\u0637\u0642\u0647 \u0627\u06cc \u0628\u0647 \u0646\u0627\u0645",
             "no_domain": "\u0646\u06cc\u0633\u062a {{ domain }} \u062f\u0627\u0631\u0627\u06cc {{ area }}",
             "no_device_class": "\u0646\u06cc\u0633\u062a {{ device_class }} \u062f\u0627\u0631\u0627\u06cc {{ area }}",
             "no_entity": "\u0648\u062c\u0648\u062f \u0646\u062f\u0627\u0631\u062f {{ entity }} \u0647\u06cc\u0686 \u062f\u0633\u062a\u06af\u0627\u0647 \u06cc\u0627 \u0645\u0648\u062c\u0648\u062f\u06cc \u0628\u0647 \u0646\u0627\u0645",
             "handle_error": "\u0647\u0646\u06af\u0627\u0645 \u0627\u062c\u0631\u0627\u06cc \u0647\u062f\u0641 \u06cc\u06a9 \u062e\u0637\u0627\u06cc \u063a\u06cc\u0631 \u0645\u0646\u062a\u0638\u0631\u0647 \u0628\u0648\u062c\u0648\u062f \u0622\u0645\u062f "
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {
         "color": {
             "values": [
                 {
                     "in": "\u0633\u0641\u06cc\u062f",
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/fi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893766534391535%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(11, OrderedDict([('sentences', ['<onko> {name} "*

 * *              '{lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) '*

 * *              "<huone>]']), ('response', 'one_yesno'), ('requires_context', "*

 * *              "OrderedDict([('domain', 'lock')])), ('slots', OrderedDict([('domain', "*

 * *              "'lock')]))])), (12, OrderedDict([('sentences', ['(<onko>|<ovatko>) "*

 * *              '(<jokin>|<jotkut>) (ovi|ovet|lukko|lukot) {lock_stat […]*

```diff
@@ -72,62 +72,14 @@
         "v\u00e4rille": "(v\u00e4rille|[v\u00e4ri]s\u00e4vylle|v\u00e4rivivahteelle)",
         "v\u00e4rit": "(v\u00e4rit|[v\u00e4ri]s\u00e4vyt|v\u00e4rivivahdteet)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "<onko> {name} {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "(<onko>|<ovatko>) (<jokin>|<jotkut>) (ovi|ovet|lukko|lukot) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "(<onko>|<ovatko>) <kaikki> (ovi|ovet|lukko|lukot) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(mik\u00e4|mitk\u00e4) (ovi|ovet|lukko|lukot) (on|ovat) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "<montako> (ovi|ovet|ovea|ovia|lukko|lukot|lukkoa|lukkoja) (on|ovat) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "response": "one",
                     "sentences": [
                         "Paljonko {name} [[<alueessa>|<alueella>] <huone>] on"
                     ]
                 },
                 {
                     "excludes_context": {
@@ -207,20 +159,144 @@
                     "response": "how_many",
                     "sentences": [
                         "<montako> {cover_classes:device_class} on {cover_states:state} [[<alueessa>|<alueella>] <huone>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "<onko> {name} {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "(<onko>|<ovatko>) (<jokin>|<jotkut>) (ovi|ovet|lukko|lukot) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "(<onko>|<ovatko>) <kaikki> (ovi|ovet|lukko|lukot) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "(mik\u00e4|mitk\u00e4) (ovi|ovet|lukko|lukot) (on|ovat) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "<montako> (ovi|ovet|ovea|ovia|lukko|lukot|lukkoa|lukkoja) (on|ovat) {lock_states:state} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area_singular",
+                    "sentences": [
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> <tuuletin> <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> <tuuletin>",
+                        "<kytke> <tuuletin> <p\u00e4\u00e4lt\u00e4> <huone>",
+                        "<kytke> <tuuletin> <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> <tuuletin>",
+                        "<kytke> <huone> <tuuletin> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> <tuuletin> <huone>",
+                        "<pys\u00e4yt\u00e4> <huone> <tuuletin>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin>",
+                        "<kytke> <tuuletin> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> <tuuletin>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_area_plural",
+                    "sentences": [
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet> <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> [kaikki] <tuulettimet>",
+                        "<kytke> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4> <huone>",
+                        "<kytke> [kaikki] <tuulettimet> <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet>",
+                        "<kytke> <huone> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> [kaikki] <tuulettimet> <huone>",
+                        "<pys\u00e4yt\u00e4> <huone> [kaikki] <tuulettimet>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin> <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> jokainen <tuuletin>",
+                        "<kytke> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4> <huone>",
+                        "<kytke> jokainen <tuuletin> <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin>",
+                        "<kytke> <huone> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> jokainen <tuuletin> <huone>",
+                        "<pys\u00e4yt\u00e4> <huone> jokainen <tuuletin>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet>",
+                        "<kytke> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin>",
+                        "<kytke> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": "cover"
+                    },
+                    "sentences": [
+                        "<laita> <p\u00e4\u00e4lt\u00e4> {name}",
+                        "<laita> {name} <p\u00e4\u00e4lt\u00e4>",
+                        "<pys\u00e4yt\u00e4> {name}"
+                    ]
+                },
+                {
                     "response": "lights_area_singular",
                     "sentences": [
                         "(<kytke> <p\u00e4\u00e4lt\u00e4>|sammuta) <valo> <huone>",
                         "(<kytke> <p\u00e4\u00e4lt\u00e4>|sammuta) <huone> <valo>",
                         "<kytke> <valo> <p\u00e4\u00e4lt\u00e4> <huone>",
                         "<kytke> <valo> <huone> <p\u00e4\u00e4lt\u00e4>",
                         "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> <valo>",
@@ -334,124 +410,119 @@
                         "Avaa [lukosta|lukituksesta] [<kaikki>] [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> [lukot|ovet]",
                         "Avaa [lukosta|lukituksesta] [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> <kaikki> [lukot|ovet]"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
-                    "response": "fans_area_singular",
+                    "response": "lights_area_singular",
                     "sentences": [
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> <tuuletin> <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> <tuuletin>",
-                        "<kytke> <tuuletin> <p\u00e4\u00e4lt\u00e4> <huone>",
-                        "<kytke> <tuuletin> <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> <tuuletin>",
-                        "<kytke> <huone> <tuuletin> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> <tuuletin> <huone>",
-                        "<pys\u00e4yt\u00e4> <huone> <tuuletin>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin>",
-                        "<kytke> <tuuletin> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> <tuuletin>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <tuuletin>"
+                        "<kytke> <p\u00e4\u00e4lle> <valo> <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> <huone> <valo>",
+                        "<kytke> <valo> <p\u00e4\u00e4lle> <huone>",
+                        "<kytke> <valo> <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> <huone> <p\u00e4\u00e4lle> <valo>",
+                        "<kytke> <huone> <valo> <p\u00e4\u00e4lle>",
+                        "<kytke> <p\u00e4\u00e4lle> <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <valo>",
+                        "<kytke> <valo> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> <valo>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <valo> <p\u00e4\u00e4lle>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
-                    "response": "fans_area_plural",
+                    "response": "lights_area_plural",
                     "sentences": [
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet> <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> [kaikki] <tuulettimet>",
-                        "<kytke> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4> <huone>",
-                        "<kytke> [kaikki] <tuulettimet> <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet>",
-                        "<kytke> <huone> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> [kaikki] <tuulettimet> <huone>",
-                        "<pys\u00e4yt\u00e4> <huone> [kaikki] <tuulettimet>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin> <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> <huone> jokainen <tuuletin>",
-                        "<kytke> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4> <huone>",
-                        "<kytke> jokainen <tuuletin> <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> <huone> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin>",
-                        "<kytke> <huone> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> jokainen <tuuletin> <huone>",
-                        "<pys\u00e4yt\u00e4> <huone> jokainen <tuuletin>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet>",
-                        "<kytke> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> [kaikki] <tuulettimet>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> [kaikki] <tuulettimet> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <tuulettimet>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin>",
-                        "<kytke> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lt\u00e4> jokainen <tuuletin>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin> <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> jokainen <tuuletin> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<pys\u00e4yt\u00e4> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <tuuletin>"
+                        "<kytke> <p\u00e4\u00e4lle> [kaikki] <valot> <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> <huone> [kaikki] <valot>",
+                        "<kytke> [kaikki] <valot> <p\u00e4\u00e4lle> <huone>",
+                        "<kytke> [kaikki] <valot> <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> <huone> <p\u00e4\u00e4lle> [kaikki] <valot>",
+                        "<kytke> <huone> [kaikki] <valot> <p\u00e4\u00e4lle>",
+                        "<kytke> <p\u00e4\u00e4lle> jokainen <valo> <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> <huone> jokainen <valo>",
+                        "<kytke> jokainen <valo> <p\u00e4\u00e4lle> <huone>",
+                        "<kytke> jokainen <valo> <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> <huone> <p\u00e4\u00e4lle> jokainen <valo>",
+                        "<kytke> <huone> jokainen <valo> <p\u00e4\u00e4lle>",
+                        "<kytke> <p\u00e4\u00e4lle> [kaikki] <valot> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <valot>",
+                        "<kytke> [kaikki] <valot> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> [kaikki] <valot> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> [kaikki] <valot>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <valot> <p\u00e4\u00e4lle>",
+                        "<kytke> <p\u00e4\u00e4lle> jokainen <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <valo>",
+                        "<kytke> jokainen <valo> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> jokainen <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> jokainen <valo>",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <valo> <p\u00e4\u00e4lle>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": "cover"
-                    },
+                    "response": "lights_area_uncountable",
                     "sentences": [
-                        "<laita> <p\u00e4\u00e4lt\u00e4> {name}",
-                        "<laita> {name} <p\u00e4\u00e4lt\u00e4>",
-                        "<pys\u00e4yt\u00e4> {name}"
-                    ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                        "valaise <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> <huone> (<valaistus>|<valaistukset>)",
+                        "<kytke> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle> <huone>",
+                        "<kytke> (<valaistus>|<valaistukset>) <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> <huone> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>)",
+                        "<kytke> <huone> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle>",
+                        "<kytke> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>) (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> (<valaistus>|<valaistukset>)",
+                        "<kytke> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
+                        "<kytke> (<valaistus>|<valaistukset>) (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
+                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>)",
+                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
                 {
-                    "excludes_context": {
+                    "requires_context": {
                         "domain": "cover"
                     },
+                    "response": "cover",
                     "sentences": [
-                        "<laita> <p\u00e4\u00e4lle> {name}",
-                        "<laita> {name} <p\u00e4\u00e4lle>",
-                        "<k\u00e4ynnist\u00e4> {name}"
+                        "<avaa> {name} [[<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>]"
                     ]
                 },
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "Lukitse {name} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
-                    ]
+                        "<avaa> autotallin ovi"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
                 },
                 {
-                    "response": "lock",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "Lukitse [<kaikki>] [lukot|ovet] [<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>",
-                        "Lukitse [<kaikki>] [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> [lukot|ovet]",
-                        "Lukitse [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> <kaikki> [lukot|ovet]"
+                        "<avaa> {cover_classes:device_class} [<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>",
+                        "<avaa> [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> {cover_classes:device_class}"
                     ],
                     "slots": {
-                        "domain": "lock",
-                        "name": "all"
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area_singular",
                     "sentences": [
                         "<kytke> <p\u00e4\u00e4lle> <tuuletin> <huone>",
                         "<kytke> <p\u00e4\u00e4lle> <huone> <tuuletin>",
@@ -513,114 +584,43 @@
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "lights_area_singular",
-                    "sentences": [
-                        "<kytke> <p\u00e4\u00e4lle> <valo> <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> <huone> <valo>",
-                        "<kytke> <valo> <p\u00e4\u00e4lle> <huone>",
-                        "<kytke> <valo> <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> <huone> <p\u00e4\u00e4lle> <valo>",
-                        "<kytke> <huone> <valo> <p\u00e4\u00e4lle>",
-                        "<kytke> <p\u00e4\u00e4lle> <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <valo>",
-                        "<kytke> <valo> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> <valo>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <valo> <p\u00e4\u00e4lle>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
-                    "response": "lights_area_plural",
-                    "sentences": [
-                        "<kytke> <p\u00e4\u00e4lle> [kaikki] <valot> <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> <huone> [kaikki] <valot>",
-                        "<kytke> [kaikki] <valot> <p\u00e4\u00e4lle> <huone>",
-                        "<kytke> [kaikki] <valot> <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> <huone> <p\u00e4\u00e4lle> [kaikki] <valot>",
-                        "<kytke> <huone> [kaikki] <valot> <p\u00e4\u00e4lle>",
-                        "<kytke> <p\u00e4\u00e4lle> jokainen <valo> <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> <huone> jokainen <valo>",
-                        "<kytke> jokainen <valo> <p\u00e4\u00e4lle> <huone>",
-                        "<kytke> jokainen <valo> <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> <huone> <p\u00e4\u00e4lle> jokainen <valo>",
-                        "<kytke> <huone> jokainen <valo> <p\u00e4\u00e4lle>",
-                        "<kytke> <p\u00e4\u00e4lle> [kaikki] <valot> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <valot>",
-                        "<kytke> [kaikki] <valot> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> [kaikki] <valot> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> [kaikki] <valot>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> [kaikki] <valot> <p\u00e4\u00e4lle>",
-                        "<kytke> <p\u00e4\u00e4lle> jokainen <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <valo>",
-                        "<kytke> jokainen <valo> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> jokainen <valo> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> jokainen <valo>",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> jokainen <valo> <p\u00e4\u00e4lle>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
-                    "response": "lights_area_uncountable",
-                    "sentences": [
-                        "valaise <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> <huone> (<valaistus>|<valaistukset>)",
-                        "<kytke> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle> <huone>",
-                        "<kytke> (<valaistus>|<valaistukset>) <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> <huone> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>)",
-                        "<kytke> <huone> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle>",
-                        "<kytke> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>) (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> <p\u00e4\u00e4lle> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> (<valaistus>|<valaistukset>)",
-                        "<kytke> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone>",
-                        "<kytke> (<valaistus>|<valaistukset>) (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle>",
-                        "<kytke> (<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> <p\u00e4\u00e4lle> (<valaistus>|<valaistukset>)",
-                        "<kytke> (<alueen>|<alueessa>|<alueesta>|<alueeseen>|<alueella>|<alueelta>|<alueelle>) <huone> (<valaistus>|<valaistukset>) <p\u00e4\u00e4lle>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
                     "requires_context": {
-                        "domain": "cover"
+                        "domain": "lock"
                     },
-                    "response": "cover",
+                    "response": "lock",
                     "sentences": [
-                        "<avaa> {name} [[<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>]"
+                        "Lukitse {name} [(<alueessa>|<alueesta>|<alueella>|<alueelta>|<alueelle>) <huone>]"
                     ]
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "lock",
                     "sentences": [
-                        "<avaa> autotallin ovi"
+                        "Lukitse [<kaikki>] [lukot|ovet] [<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>",
+                        "Lukitse [<kaikki>] [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> [lukot|ovet]",
+                        "Lukitse [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> <kaikki> [lukot|ovet]"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<avaa> {cover_classes:device_class} [<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone>",
-                        "<avaa> [<alueen>|<alueessa>|<alueesta>|<alueella>|<alueelta>] <huone> {cover_classes:device_class}"
-                    ],
-                    "slots": {
+                    "excludes_context": {
                         "domain": "cover"
-                    }
+                    },
+                    "sentences": [
+                        "<laita> <p\u00e4\u00e4lle> {name}",
+                        "<laita> {name} <p\u00e4\u00e4lle>",
+                        "<k\u00e4ynnist\u00e4> {name}"
+                    ]
                 }
             ]
         }
     },
     "language": "fi",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gl.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.730828373015873%*

 * *Differences: {"'expansion_rules'": "{'name': '[o | a] {name}', 'area': '[en | no | na | de | do | da] {area}', "*

 * *                      "'brightness': '{brightness}[%| porcento]', 'temperature': '{temperature} "*

 * *                      "[graos] [{temperature_unit}]', 'acende': '(acende | activa)', 'temp': '[a] "*

 * *                      "(temperatura)', delete: ['regle', 'allume', 'eteins', 'lumiere', "*

 * *                      "'lumieres', 'ventilateur', 'ventilateurs', 'dans']}",*

 * * "'intents'": "{'HassTurnOn': {'data': {0: {'se […]*

```diff
@@ -1,216 +1,171 @@
 {
     "expansion_rules": {
-        "allume": "(allume | active | d\u00e9marre | ouvre)",
-        "area": "([le | la ] {area} | [l']{area})",
-        "brightness": "{brightness:brightness}[%| pourcent]",
-        "dans": "(dans | du | de)",
-        "eteins": "(\u00e9teint | \u00e9teins | d\u00e9sactive | stoppe | arr\u00eate | coupe | ferme )",
-        "lumiere": "(la lumi\u00e8re | la lampe | l'ampoule)",
-        "lumieres": "[les] (lumi\u00e8res | lampes | ampoules)",
-        "name": "([le | la | les] {name} | [l']{name})",
-        "regle": "(r\u00e8gle | met | ajuste | change)",
-        "temperature": "{temperature}[\u00b0| degr\u00e9s] [{temperature_unit}]",
-        "ventilateur": "(le ventilateur | l'\u00e9changeur d'air | la fan)",
-        "ventilateurs": "(les ventilateurs | les fans)"
+        "acende": "(acende | activa)",
+        "area": "[en | no | na | de | do | da] {area}",
+        "brightness": "{brightness}[%| porcento]",
+        "name": "[o | a] {name}",
+        "temp": "[a] (temperatura)",
+        "temperature": "{temperature} [graos] [{temperature_unit}]"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<eteins> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
+                        "apaga [todos] [os] ventiladores <area>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "(ferme | baisse) [la] porte du garage"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
+                        "apaga <name> <area>",
+                        "desactiva <name> <area>"
+                    ]
                 },
                 {
-                    "response": "cover_area",
                     "sentences": [
-                        "(ferme | baisse) [les] (stores | toiles| rideaux) <dans> <area>"
+                        "apaga (a luz | as luces | luces) <area>",
+                        "apaga todas as luces <area>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
+                        "domain": "light",
+                        "name": "all"
                     }
                 },
                 {
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<eteins> ([tous] | [toutes] ) <ventilateurs> <dans> [<area>]"
+                        "pecha [a] porta do garaxe"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_area",
                     "sentences": [
-                        "<eteins> <ventilateur> [<dans>] [<area>]"
+                        "pecha [a|as] <name> [<area>]"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ]
                     }
-                },
-                {
-                    "sentences": [
-                        "<eteins> <name> [dans|du|de] <area>",
-                        "<eteins> <name>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "(ferme | baisse) <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "(ferme | baisse) <name> <dans> <area>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<allume> <name>",
-                        "<allume> <name> [dans|du|de] <area>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "ouvre <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "ouvre <name> <dans> <area>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<allume> ([tous] | [toutes] ) (<ventilateur> | <ventilateurs>) [<dans>] [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<allume> (<ventilateur> | <ventilateurs>) [<dans>] [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<allume> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
+                        "<acende> ([a] luz | [as] luces) <area>",
+                        "<acende> todas as luces <area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "ouvre [la] porte du garage"
+                        "abre [a] porta do garaxe"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "ouvre [les] (stores | rideaux | toiles) <dans> <area>"
+                        "abre [a | as] (cortinas | persianas) <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "acende [todos] [os] ventiladores <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "acende <name>",
+                        "activa <name>"
+                    ]
                 }
             ]
         }
     },
-    "language": "fr-CA",
+    "language": "gl",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "(blanc|blanche)",
+                    "in": "blanco",
                     "out": "white"
                 },
                 {
-                    "in": "(noir | noire)",
+                    "in": "negro",
                     "out": "black"
                 },
                 {
-                    "in": "rouge",
+                    "in": "(vermello|vermella)",
                     "out": "red"
                 },
                 {
-                    "in": "orange",
+                    "in": "laranxa",
                     "out": "orange"
                 },
                 {
-                    "in": "jaune",
+                    "in": "amarelo",
                     "out": "yellow"
                 },
                 {
-                    "in": "(vert | verte)",
+                    "in": "verde",
                     "out": "green"
                 },
                 {
-                    "in": "(bleu | bleue)",
+                    "in": "azul",
                     "out": "blue"
                 },
                 {
-                    "in": "(violet | violette)",
+                    "in": "(lila|morado|p\u00farpura)",
                     "out": "purple"
                 },
                 {
-                    "in": "brun",
+                    "in": "marr\u00f3n",
                     "out": "brown"
-                },
-                {
-                    "in": "rose",
-                    "out": "pink"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
@@ -230,42 +185,41 @@
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Une erreur s'est produite pendant le traitement",
-            "no_area": "Aucune zone appel\u00e9e {{ area }}",
-            "no_device_class": "{{ area }} ne contient pas de {{ device_class }}",
-            "no_domain": "{{ area }} ne contient pas de {{ domain }}",
-            "no_entity": "Aucun appareil ou entit\u00e9 appel\u00e9 {{ entity }}",
-            "no_intent": "D\u00e9sol\u00e9, je n'ai pas compris"
+            "handle_error": "Un erro inesperado ocurreu intentando procesar a instrucci\u00f3n",
+            "no_area": "Non existe ningunha \u00e1rea chamada {{ area }}",
+            "no_device_class": "{{ area }} non ten {{ device_class }}",
+            "no_domain": "{{ area }} non ten {{ domain }}",
+            "no_entity": "Non existe dispositivo ou entidade chamado {{ entity }}",
+            "no_intent": "S\u00edntoo, non che entend\u00edn"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "{{ slots.name }} ferm\u00e9",
-                "cover_area": "Ouvrants de {{ slots.area }} ferm\u00e9s",
-                "cover_device_class": "{{ slots.device_class }} ferm\u00e9",
-                "default": "{{ slots.name }} \u00e9teint",
-                "fans_area": "ventilateurs de {{ slots.area }} \u00e9teints",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} \u00e9teintes"
+                "cover": "Closed {{ slots.name }}",
+                "cover_area": "Closed {{ slots.area }}",
+                "cover_device_class": "Closed {{ slots.device_class }}",
+                "default": "Turned off {{ slots.name }}",
+                "fans_area": "Turned off fans in {{ slots.area }}",
+                "lights_area": "Turned off lights in {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} ouvert",
-                "cover_area": "Ouvrants de {{ slots.area }} ouverts",
-                "cover_device_class": "{{ slots.device_class }} ouvert",
-                "default": "{{ slots.name }} allum\u00e9",
-                "fans_area": "Ventilateurs de {{ slots.area }} activ\u00e9",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} allum\u00e9es"
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}",
+                "cover_device_class": "Opened {{ slots.device_class }}",
+                "default": "Turned on {{ slots.name }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "lights_area": "Turned on lights in {{ slots.area }}"
             }
         }
     },
     "skip_words": [
-        "s'il te pla\u00eet",
-        "merci",
-        "peux-tu",
-        "s'il vous pla\u00eet",
-        "Heille"
+        "por favor",
+        "gracias",
+        "grazas",
+        "graci\u00f1as"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/it.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7207081916661164%*

 * *Differences: {"'expansion_rules'": "{'name': '{name}', 'area': '{area}', 'brightness': '{brightness}[%| "*

 * *                      "percento]', 'temperature': '{temperature}[°| gradi] [{temperature_unit}]', "*

 * *                      '\'the\': "(l(o|a|e) | i[l] | gli | l\')", \'in\': \'(in | '*

 * *                      "ne[i|gli|l[lo|la|le]])', 'of': '(de[i|gli|l[lo|la|le]]|di)', 'to': "*

 * *                      '\'a[l[lo|la|le] | gli]\', \'what_is\': "(qual[e] è | quant(o |\')è | com(e '*

 * *                      '|\')è | che)", \'turn […]*

```diff
@@ -1,584 +1,483 @@
 {
     "expansion_rules": {
-        "allume": "(allume|active|d\u00e9marre)",
-        "area": "([le|la] {area}|[l']{area})",
-        "brightness": "{brightness:brightness}[%| pourcent]",
-        "dans": "(dans|du|de)",
-        "eteins": "(\u00e9teint|\u00e9teins|d\u00e9sactive|stoppe|arr\u00eate|coupe)",
-        "lumiere": "(la lumi\u00e8re|la lampe|l'ampoule)",
-        "lumieres": "[les] (lumi\u00e8res|lampes|ampoules)",
-        "name": "([le|la|les] {name}|[l']{name})",
-        "regle": "(r\u00e8gle|met|ajuste)",
-        "temperature": "{temperature}[\u00b0| degr\u00e9s] [{temperature_unit}]",
-        "ventilateur": "(le ventilateur|le brasseur d'air)",
-        "ventilateurs": "(les ventilateurs|les brasseurs d'air)"
+        "area": "{area}",
+        "brightness": "{brightness}[%| percento]",
+        "close": "(chiud(i|ere) | abbass(a|are))",
+        "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|i))",
+        "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione | climatizzator(e|i) | condizionator(e|i))",
+        "in": "(in | ne[i|gli|l[lo|la|le]])",
+        "name": "{name}",
+        "of": "(de[i|gli|l[lo|la|le]]|di)",
+        "open": "(apr(i|ire) | alz(a|are))",
+        "set": "(impost(a|are) | cambi(a|are) | mett(i|ere) | modific(a|are))",
+        "temp": "[la] (temperatura)",
+        "temperature": "{temperature}[\u00b0| gradi] [{temperature_unit}]",
+        "the": "(l(o|a|e) | i[l] | gli | l')",
+        "to": "a[l[lo|la|le] | gli]",
+        "turn_off": "(spegn(i|ere) | disattiv(a|are))",
+        "turn_on": "(accend(i|ere) | attiv(a|are))",
+        "what_is": "(qual[e] \u00e8 | quant(o |')\u00e8 | com(e |')\u00e8 | che)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "<name> (est|est-elle) {lock_states:state} [\u00e0 cl\u00e9|\u00e0 clef] [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "(y a-t-il|il y a) (des|une) porte[s] [de] {lock_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "Toutes les porte[s] (sont|sont-elles) {lock_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(quelles|quelle) porte[s] (sont|est) {lock_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "combien de porte[s] sont {lock_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "scene",
-                            "script"
-                        ]
-                    },
                     "response": "one",
                     "sentences": [
-                        "quel est [l'etat de|le statut de ] <name> [(dans|de) <area>]"
+                        "<what_is> [lo stato <of>|stato ha[nno]] [<the>] <name> [(<in>|of) <area>]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "<name> [(dans|de) <area>] (est|est-elle) {on_off_states:state}"
+                        "[Lo stato <of>] [<the>] <name> \u00e8 {on_off_states:state} [<in> <area>]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "(certains|certaines) {on_off_domains:domain} [sont|sont-ils|sont-elles] {on_off_states:state} [dans <area>]"
+                        "(C'\u00e8 una|Ci sono delle) {on_off_domains:domain} [<of> <area>] {on_off_states:state} [<in> <area>]"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "(tous|toutes) les {on_off_domains:domain} [sont|sont-ils|sont-elles] {on_off_states:state} [dans <area>]"
+                        "[tutte] <the> {on_off_domains:domain} [<of> <area>] sono [tutt(i|e)] {on_off_states:state} [<in> <area>]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(quelle[s]|quel[s]) sont les {on_off_domains:domain} {on_off_states:state} [dans <area>]"
+                        "(Qual(i|e)|Che) {on_off_domains:domain} [<of> <area>] (\u00e8|sono) {on_off_states:state} [<in> <area>]"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "combien [(il y a|y a-t-il)] de {on_off_domains:domain} [sont] [d']{on_off_states:state} [dans <area>]"
+                        "Quant(i|e) {on_off_domains:domain} [<of> <area>] (\u00e8|sono) {on_off_states:state} [<in> <area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "<name> (est|est-il) {cover_states:state} [dans <area>]"
+                        "[<the>] <name> \u00e8 {cover_states:state} [<in> <area>]",
+                        "\u00e8 {cover_states:state} <name> [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "[Y a-t-il][il y a] (des|certains) {cover_classes:device_class} {cover_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "certains des {cover_classes:device_class} [dans|du] [<area>] [sont-ils] {cover_states:state}"
+                        "(C'\u00e8 una|Ci sono delle) {cover_classes:device_class} {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "tous [les] {cover_classes:device_class} [sont|sont-ils] {cover_states:state} [dans <area>]"
+                        "<the> {cover_classes:device_class} [<of> <area>] sono [tutt(i|e)] {cover_states:state} [<in> <area>]",
+                        "[tutt(i|e)] [<the>] {cover_classes:device_class} [(<of>|<in>) <area>] sono {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(quel|quels) {cover_classes:device_class} (sont) {cover_states:state} [dans <area>]"
+                        "(Qual(i|e)|Che) {cover_classes:device_class} [<of> <area>] (\u00e8|sono) {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "combien [Y a-t-il][il y a] de {cover_classes:device_class} [(sont|sont-ils|de)] {cover_states:state} [dans <area>]"
+                        "Quant(i|e) {cover_classes:device_class} [<of> <area>] (\u00e8|sono) {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<eteins> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
+                        "<turn_off> [(tutt(i|e))] [<the>]<fan> [(<of> | <in>)] <area>",
+                        "<turn_off> [<in>] <area> [(tutt(i|e))] [<the>]<fan>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "(ferme|baisse) [la] porte (du|de) garage",
-                        "ferme [le] garage"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
+                        "<turn_off> [<the>]<name>"
+                    ]
                 },
                 {
-                    "response": "cover_area",
                     "sentences": [
-                        "(ferme|baisse) [tous] [les|le] (store|stores|volet|volets) <dans> <area>"
+                        "<turn_off> [tutte] [l(a|e)] (luc(e|i)) [(<of>|<in>)] <area>",
+                        "<turn_off> [<in>] <area> [tutte] [l(a|e)] (luc(e|i))"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
+                        "domain": "light"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
                     "sentences": [
-                        "(ferme|baisse) tous [les] (stores|volets)"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
-                        "name": "all"
-                    }
+                        "<close> [<the>] <name> [[<of>|<in>] <area>]"
+                    ]
                 },
                 {
-                    "response": "fan_all",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_area",
                     "sentences": [
-                        "<eteins> [tous] <ventilateurs> <dans> [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
+                        "<close> [<the>] <cover> [[<in> | <of>] <area>]",
+                        "<close> [[<in>] <area>] [<the>] <cover>"
+                    ]
                 },
                 {
-                    "response": "fans_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<eteins> <ventilateur> [<dans>] [<area>]"
+                        "<close> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
+                        "<close> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "sentences": [
-                        "<eteins> <name>",
-                        "<eteins> <name> <dans> <area>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "(ferme|baisse) <name>"
-                    ]
-                },
-                {
                     "response": "cover_area",
                     "sentences": [
-                        "(ferme|baisse) <name> <dans> <area>"
-                    ]
+                        "<close> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
+                        "<close> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
+                    ],
+                    "slots": {
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
+                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<allume> <name>",
-                        "<allume> <name> <dans> <area>"
-                    ]
+                        "<turn_on> [tutte] [l(a|e)] (luc(e|i)) [(<of>|<in>)] <area>",
+                        "<turn_on> [<in>] <area> [tutte] [l(a|e)] (luc(e|i))"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
                     "response": "cover",
                     "sentences": [
-                        "(ouvre|monte) <name>"
+                        "<open> [<the>] <name> [[<of>|<in>] <area>]"
                     ]
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
                     "response": "cover_area",
                     "sentences": [
-                        "(ouvre|monte) <name> <dans> <area>"
+                        "<open> [<the>] <cover> [[<in> | <of>] <area>]",
+                        "<open> [[<in>] <area>] [<the>] <cover>"
                     ]
                 },
                 {
-                    "response": "fan_all",
-                    "sentences": [
-                        "<allume> [tous] (<ventilateur> | <ventilateurs>) (dans|du|de) [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<allume> (<ventilateur> | <ventilateurs>) [dans|du|de] [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<allume> [toutes] (<lumiere> | <lumieres>) (dans | du | de) <area>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
                     "response": "cover_device_class",
                     "sentences": [
-                        "(ouvre|monte) [la] porte (du|de) garage",
-                        "ouvre [le] garage"
+                        "<open> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
+                        "<open> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "(ouvre|monte) [tous] [les|le] (store|stores|volet|volets) <dans> <area>"
+                        "<open> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
+                        "<open> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "(ouvre|monte) tous [les] (stores|volets)"
+                        "<turn_on> [(tutt(i|e))] [<the>]<fan> [(<of> | <in>)] <area>",
+                        "<turn_on> [<in>] <area> [(tutt(i|e))] [<the>]<fan>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
+                        "domain": "fan",
                         "name": "all"
                     }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> [<the>]<name>"
+                    ]
                 }
             ]
         }
     },
-    "language": "fr",
+    "language": "it",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "(blanc|blanche)",
+                    "in": "bianco",
                     "out": "white"
                 },
                 {
-                    "in": "(noir|noire)",
+                    "in": "nero",
                     "out": "black"
                 },
                 {
-                    "in": "rouge",
+                    "in": "rosso",
                     "out": "red"
                 },
                 {
-                    "in": "orange",
+                    "in": "arancione",
                     "out": "orange"
                 },
                 {
-                    "in": "jaune",
+                    "in": "giallo",
                     "out": "yellow"
                 },
                 {
-                    "in": "(vert|verte)",
+                    "in": "verde",
                     "out": "green"
                 },
                 {
-                    "in": "(bleu|bleue)",
+                    "in": "blu",
                     "out": "blue"
                 },
                 {
-                    "in": "(violet|violette)",
+                    "in": "viola",
                     "out": "purple"
                 },
                 {
-                    "in": "marron",
+                    "in": "marrone",
                     "out": "brown"
-                },
-                {
-                    "in": "rose",
-                    "out": "pink"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "store[s]",
+                    "in": "tend(a|e) da sole",
                     "out": "awning"
                 },
                 {
-                    "in": "store[s]",
+                    "in": "persian(a|e)",
                     "out": "blind"
                 },
                 {
-                    "in": "rideau[x]",
+                    "in": "tend(a|e)",
                     "out": "curtain"
                 },
                 {
-                    "in": "porte[s]",
+                    "in": "port(a|e)",
                     "out": "door"
                 },
                 {
-                    "in": "portes[s] de garage[s]",
-                    "out": "garage door"
+                    "in": "(serrand(a|e) | port(a|e) [basculant(e|i)|de(l|i) garage] | saracinesc(a|he))",
+                    "out": "garage"
                 },
                 {
-                    "in": "portail[s]",
+                    "in": "cancell(o|i)",
                     "out": "gate"
                 },
                 {
-                    "in": "store[s]",
+                    "in": "venezian(a|e)",
                     "out": "shade"
                 },
                 {
-                    "in": "volet[s]",
+                    "in": "tapparell(a|e)",
                     "out": "shutter"
                 },
                 {
-                    "in": "fen\u00eatre[s]",
+                    "in": "finestr(a|e)",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "ouvert[e][s]",
+                    "in": "apert(a|o|e)",
                     "out": "open"
                 },
                 {
-                    "in": "ferm\u00e9[e][s]",
+                    "in": "chius(a|o|e)",
                     "out": "closed"
                 },
                 {
-                    "in": "ouverture",
+                    "in": "in apertura",
                     "out": "opening"
                 },
                 {
-                    "in": "fermeture",
+                    "in": "in chiusura",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "verrouill[e][er][\u00e9][\u00e9e][s]",
-                    "out": "locked"
-                },
-                {
-                    "in": "ferm[e][er][\u00e9][\u00e9e][s]",
+                    "in": "chiusa",
                     "out": "locked"
                 },
                 {
-                    "in": "d\u00e9verrouill[e][er][\u00e9][\u00e9e][s]",
-                    "out": "unlocked"
-                },
-                {
-                    "in": "ouvert[e][s]",
-                    "out": "unlocked"
-                },
-                {
-                    "in": "ouvr[e][s]",
-                    "out": "unlocked"
+                    "in": "aperta",
+                    "out": "aperto"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "lampe[s]|lumi\u00e8re[s]",
+                    "in": "luc(e|i)",
                     "out": "light"
                 },
                 {
-                    "in": "ventilateur[s]",
+                    "in": "(ventol(a|e)|ventilator(e|i)|ventilazione|climatizzator(e|i)|condizionator(e|i))",
                     "out": "fan"
                 },
                 {
-                    "in": "interrupteur[s]",
+                    "in": "(interruttor(e|i)|pres(a|e))",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "allum\u00e9[e][s]",
+                    "in": "(acces(o|i|a|e)|attiv(o|i|a|e))",
                     "out": "on"
                 },
                 {
-                    "in": "\u00e9teint[e][s]",
+                    "in": "(spent(o|i|a|e)|disattiv(o|i|a|e))",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "celsius",
+                "(celsius | centigradi)",
                 {
                     "in": "c",
                     "out": "celsius"
                 },
                 "fahrenheit",
                 {
                     "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Une erreur est intervenue pendant le traitement",
-            "no_area": "Aucune zone appel\u00e9e {{ area }}",
-            "no_device_class": "{{ area }} ne contient pas de {{ device_class }}",
-            "no_domain": "{{ area }} ne contient pas de {{ domain }}",
-            "no_entity": "Aucun appareil ou entit\u00e9 appel\u00e9 {{ entity }}",
-            "no_intent": "D\u00e9sol\u00e9, je n'ai pas compris"
+            "handle_error": "Si \u00e8 verificato un errore inatteso durante l'elaborazione",
+            "no_area": "Non esiste nessuna area chiamata {{ area }}",
+            "no_device_class": "{{ area }} non contiene {{ device_class }}",
+            "no_domain": "{{ area }} non contiene {{ domain }}",
+            "no_entity": "Non esiste nessun dispositivo o entit\u00e0 chiamato {{ entity }}",
+            "no_intent": "Mi dispiace, non ho capito"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  Oui\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = no_match | length | int %}\n  {% if no_match | length > 4 %}\n    Non, {{ no_match[:3] | join(\", \") }} et {{ (no_match | length - 3) }} autres, ne sont pas {{ state.state_with_unit }}\n  {% elif no_match | length == 1 %}\n    Non, l'appareil\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {%- endfor %}\n    n'est pas {{ state.state_with_unit }}\n  {%- else -%}\n    Non, les appareils \n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {%- endfor %}\n    ne sont pas {{ state.state_with_unit }}s\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = no_match | length | int %}\n  {% if match | length > 4 %}\n    Oui, {{ match[:3] | join(\", \") }} et {{ (match | length - 3) }} autres\n  {% elif no_match | length == 0 %}\n    Oui, l'appareil\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    est {{ state.state_with_unit }}\n  {%- else -%}\n    Oui, les appareils\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    sont {{ state.state_with_unit }}s\n  {% endif %}\n{% else %}\n  Non\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  S\u00ec\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length == 4 %}\n    No, {{ no_match[:3] | join(\", \") }} ed un altro no\n  {% elif no_match | length > 4 %}\n    No, {{ no_match[:3] | join(\", \") }} ed altri {{ (no_match | length - 3) }}\n  {%- else -%}\n    No,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor %} no\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length == 4 %}\n    S\u00ec, {{ match[:3] | join(\", \") }} ed un altro\n  {% elif match | length > 4 %}\n    S\u00ec, {{ match[:3] | join(\", \") }} ed altri {{ (match | length - 3) }}\n  {%- else -%}\n    S\u00ec,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  No\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "L'etat de l'appareil {{ slots.name | capitalize }} est {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  Oui\n{% else %}\n  Non, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  Aucun appareil\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = match | length | int %}\n  {% if match | length > 4 %}\n    Les appareils \n    {{ match[:3] | join(\", \") }} et {{ (match | length - 3) }} autres\n  {% elif match | length == 1 %}\n    L'appareil \n    {% for name in match %}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    est {{ state.state_with_unit }}\n  {% else %}\n    Les appareils \n    {% for name in match %}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    sont {{ state.state_with_unit }}s\n  {% endif %}\n{% endif %}\n"
+                "one": "{{ slots.name | capitalize }} \u00e8 {{ state.state_with_unit }}\n",
+                "one_yesno": "{% if query.matched %}\n  S\u00ec\n{% else %}\n  No, \u00e8 {{ state.state_with_unit }}\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  Nessuno\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length == 4 %}\n    {{ match[:3] | join(\", \") }} ed un altro\n  {% elif match | length > 4 %}\n    {{ match[:3] | join(\", \") }} ed altri {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "{{ slots.name }} ferm\u00e9",
-                "cover_area": "Ouvrants de {{ slots.area }} ferm\u00e9s",
-                "cover_device_class": "{{ slots.device_class }} ferm\u00e9",
-                "default": "{{ slots.name }} \u00e9teint",
-                "fan_all": "Tous les ventilateurs sont \u00e9teints",
-                "fans_area": "Ventilateurs de {{ slots.area }} \u00e9teints",
-                "light_all": "Toutes les lumi\u00e8res sont \u00e9teintes",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} \u00e9teintes"
+                "cover": "Ho chiuso {{ slots.name }}",
+                "cover_area": "Chiuse in {{ slots.area }}",
+                "cover_device_class": "Ho chiuso {{ slots.device_class }}",
+                "default": "Ho spento {{ slots.name }}",
+                "fans_area": "Ho spento la ventilazione in {{ slots.area }}",
+                "lights_area": "Ho spento le luci in {{ slots.area }}",
+                "scene": "Ho disattivato {{ slots.name }}",
+                "script": "Ho arrestato {{ slots.name }}"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} ouvert",
-                "cover_all": "Ouvre tous les ouvrants de {{ slots.area }}",
-                "cover_area": "Ouvrants de {{ slots.area }} ouverts",
-                "cover_device_class": "{{ slots.device_class }} ouvert",
-                "default": "{{ slots.name }} allum\u00e9",
-                "fan_all": "Allume tous les ventilateurs",
-                "fans_area": "Ventilateurs de {{ slots.area }} allum\u00e9s",
-                "light_all": "Allume toutes les lumi\u00e8res",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} allum\u00e9es"
+                "cover": "Ho aperto {{ slots.name }}",
+                "cover_area": "Aperte in {{ slots.area }}",
+                "cover_device_class": "Ho aperto {{ slots.device_class }}",
+                "default": "Ho acceso {{ slots.name }}",
+                "fans_area": "Ho acceso la ventilazione in {{ slots.area }}",
+                "lights_area": "Ho acceso le luci in {{ slots.area }}",
+                "scene": "Ho attivato {{ slots.name }}",
+                "script": "Ho avviato {{ slots.name }}"
             }
         }
     },
     "skip_words": [
-        "s'il te pla\u00eet",
-        "merci"
+        "per favore",
+        "potresti",
+        "puoi",
+        "puoi dirmi",
+        "dimmi",
+        "grazie"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ms.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7193335262345678%*

 * *Differences: {"'expansion_rules'": "{'area': '{area}', 'nama': '{name}', 'apakah': '(apa | apakah | apa itu)', "*

 * *                      "'berapa': '(berapa | berapakah)', 'imp_hidup': '(nyalakan | hidupkan)', "*

 * *                      "'imp_mati': '(padamkan | matikan)', 'imp_buka': '(buka | bukakan)', "*

 * *                      "'imp_tutup': '(tutup | tutupkan)', 'imp_set': '(tetapkan | setkan | set | "*

 * *                      "jadikan | ubahkan | ubah | tukarkan | tukar)', 'kecerahan': "*

 * *                      "'{brightness}[% […]*

```diff
@@ -1,170 +1,152 @@
 {
     "expansion_rules": {
-        "acende": "(acende | activa)",
-        "area": "[en | no | na | de | do | da] {area}",
-        "brightness": "{brightness}[%| porcento]",
-        "name": "[o | a] {name}",
-        "temp": "[a] (temperatura)",
-        "temperature": "{temperature} [graos] [{temperature_unit}]"
+        "apakah": "(apa | apakah | apa itu)",
+        "area": "{area}",
+        "berapa": "(berapa | berapakah)",
+        "imp_buka": "(buka | bukakan)",
+        "imp_hidup": "(nyalakan | hidupkan)",
+        "imp_mati": "(padamkan | matikan)",
+        "imp_set": "(tetapkan | setkan | set | jadikan | ubahkan | ubah | tukarkan | tukar)",
+        "imp_tutup": "(tutup | tutupkan)",
+        "kecerahan": "{brightness}[%| peratus]",
+        "nama": "{name}",
+        "suhu": "{temperature}[\u00b0| darjah] [{temperature_unit}]"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "apaga (a luz | as luces | luces) <area>",
-                        "apaga todas as luces <area>"
+                        "<imp_mati> [semua] kipas [di] <area>",
+                        "<imp_mati> [semua] kipas <area>"
                     ],
                     "slots": {
-                        "domain": "light",
-                        "name": "all"
+                        "area": "living_room",
+                        "domain": "fan"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "pecha [a] porta do garaxe"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
+                        "<imp_mati> <nama>"
+                    ]
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover_area",
                     "sentences": [
-                        "pecha [a|as] <name> [<area>]"
+                        "<imp_mati> [semua] lampu [di] <area>",
+                        "<imp_mati> [semua] lampu <area>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ]
+                        "domain": "light"
                     }
                 },
                 {
+                    "response": "cover_area",
                     "sentences": [
-                        "apaga [todos] [os] ventiladores <area>"
+                        "<imp_tutup> pagar [di] <area>",
+                        "<imp_tutup> pagar <area>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "area": "garaj",
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "apaga <name> <area>",
-                        "desactiva <name> <area>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "acende <name>",
-                        "activa <name>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "acende [todos] [os] ventiladores <area>"
+                        "<imp_hidup> [semua] lampu [di] <area>",
+                        "<imp_hidup> [semua] lampu <area>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
+                    "response": "cover_area",
                     "sentences": [
-                        "<acende> ([a] luz | [as] luces) <area>",
-                        "<acende> todas as luces <area>"
+                        "<imp_buka> [semua] langsir [di] <area>",
+                        "<imp_buka> [semua] langsir <area>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "area": "living_room",
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "abre [a] porta do garaxe"
+                        "<imp_hidup> [semua] kipas [di] <area>",
+                        "<imp_hidup> [semua] kipas <area>"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "area": "living_room",
+                        "domain": "fan"
                     }
                 },
                 {
-                    "response": "cover_area",
                     "sentences": [
-                        "abre [a | as] (cortinas | persianas) <area>"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
+                        "<imp_hidup> <nama>"
+                    ]
                 }
             ]
         }
     },
-    "language": "gl",
+    "language": "ms",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "blanco",
+                    "in": "putih",
                     "out": "white"
                 },
                 {
-                    "in": "negro",
+                    "in": "hitam",
                     "out": "black"
                 },
                 {
-                    "in": "(vermello|vermella)",
+                    "in": "merah",
                     "out": "red"
                 },
                 {
-                    "in": "laranxa",
+                    "in": "oren",
                     "out": "orange"
                 },
                 {
-                    "in": "amarelo",
+                    "in": "kuning",
                     "out": "yellow"
                 },
                 {
-                    "in": "verde",
+                    "in": "hijau",
                     "out": "green"
                 },
                 {
-                    "in": "azul",
+                    "in": "biru",
                     "out": "blue"
                 },
                 {
-                    "in": "(lila|morado|p\u00farpura)",
+                    "in": "ungu",
                     "out": "purple"
                 },
                 {
-                    "in": "marr\u00f3n",
+                    "in": "perang",
                     "out": "brown"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
@@ -174,52 +156,44 @@
         },
         "temperature_unit": {
             "values": [
                 "celsius",
                 {
                     "in": "c",
                     "out": "celsius"
-                },
-                "fahrenheit",
-                {
-                    "in": "f",
-                    "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Un erro inesperado ocurreu intentando procesar a instrucci\u00f3n",
-            "no_area": "Non existe ningunha \u00e1rea chamada {{ area }}",
-            "no_device_class": "{{ area }} non ten {{ device_class }}",
-            "no_domain": "{{ area }} non ten {{ domain }}",
-            "no_entity": "Non existe dispositivo ou entidade chamado {{ entity }}",
-            "no_intent": "S\u00edntoo, non che entend\u00edn"
+            "handle_error": "Maaf, berlaku ralat semasa intent sedang dijalankan",
+            "no_area": "Tiada {{ area }} dijumpai",
+            "no_device_class": "{{ device_class }} tiada di {{ area }}",
+            "no_domain": "{{ domain }} tiada di {{ area }}",
+            "no_entity": "Peranti atau entiti {{ entity }} tidak ditemui",
+            "no_intent": "Maaf, saya tidak faham arahan anda"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "Closed {{ slots.name }}",
-                "cover_area": "Closed {{ slots.area }}",
-                "cover_device_class": "Closed {{ slots.device_class }}",
-                "default": "Turned off {{ slots.name }}",
-                "fans_area": "Turned off fans in {{ slots.area }}",
-                "lights_area": "Turned off lights in {{ slots.area }}"
+                "cover": "{{ slots.name }} telah ditutupkan",
+                "cover_area": "Kawasan {{ slots.area }} telah ditutupkan",
+                "default": "{{ slots.name }} telah dimatikan",
+                "fans_area": "Semua kipas [di] {{ slots.area }} telah dimatikan",
+                "lights_area": "Semua lampu [di] {{ slots.area }} telah dipadamkan"
             },
             "HassTurnOn": {
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}",
-                "cover_device_class": "Opened {{ slots.device_class }}",
-                "default": "Turned on {{ slots.name }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "lights_area": "Turned on lights in {{ slots.area }}"
+                "cover": "{{ slots.name }} telah dibuka",
+                "cover_area": "Kawasan {{ slots.area }} telah dibuka",
+                "default": "{{ slots.name }} telah dihidupkan",
+                "fans_area": "Semua kipas [di] {{ slots.area }} telah dihidupkan",
+                "lights_area": "Semua lampu [di] {{ slots.area }} telah dinyalakan"
             }
         }
     },
     "skip_words": [
-        "por favor",
-        "gracias",
-        "grazas",
-        "graci\u00f1as"
+        "tolong",
+        "boleh tak",
+        "cuba"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/gu.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "{{ area }} \u0aa8\u0abe\u0aae\u0aa8\u0acb \u0a95\u0acb\u0a88 \u0ab5\u0abf\u0ab8\u0acd\u0aa4\u0abe\u0ab0 \u0aa8\u0aa5\u0ac0",
             "no_domain": "{{ area }} \u0aae\u0abe\u0a82 {{ domain }} \u0aa8\u0aa5\u0ac0",
             "no_device_class": "{{ area }} \u0aae\u0abe\u0a82 {{ device_class }} \u0aa8\u0aa5\u0ac0",
             "no_entity": "{{ entity }} \u0aa8\u0abe\u0aae\u0aa8\u0ac1\u0a82 \u0a95\u0acb\u0a88 \u0aa1\u0ac0\u0ab5\u0abe\u0a87\u0ab8 \u0a85\u0aa5\u0ab5\u0abe \u0a8f\u0aa8\u0acd\u0a9f\u0abf\u0a9f\u0ac0 \u0aa8\u0aa5\u0ac0",
             "handle_error": "\u0a88\u0aa8\u0acd\u0a9f\u0ac7\u0aa8\u0acd\u0a9f \u0ab8\u0a82\u0aad\u0abe\u0ab3\u0aa4\u0ac0 \u0ab5\u0a96\u0aa4\u0ac7 \u0a8f\u0a95 \u0a85\u0aa3\u0aa7\u0abe\u0ab0\u0ac0 \u0aad\u0ac2\u0ab2 \u0a86\u0ab5\u0ac0"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/he.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(3, OrderedDict([('sentences', "*

 * *              "['(הדלק|הדלקה|להדליק|תדליק) [של] [כל] [את] [ה](מאוורר|מאורר) ב<area>']), ('slots', "*

 * *              "OrderedDict([('domain', 'fan')]))])), (4, OrderedDict([('sentences', "*

 * *              "['(הדלק|הדלקה|להדליק|תדליק) [של] [כל] [את] [ה](מאווררים|מאוררים) ב<area>']), "*

 * *              "('slots', OrderedDict([('domain', 'fan'), ('name', 'all')]))])), (5, "*

 * *              "OrderedDict([('sentences', ['הדלק [את] [ה]<name>' […]*

```diff
@@ -102,14 +102,39 @@
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05db\u05d9\u05d1\u05d5\u05d9 [\u05e9\u05dc] [\u05d4]<name>",
+                        "\u05dc\u05db\u05d1\u05d5\u05ea [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05ea\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
@@ -139,71 +164,21 @@
                             "blind",
                             "curtain",
                             "shutter",
                             "garage"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05db\u05d9\u05d1\u05d5\u05d9 [\u05e9\u05dc] [\u05d4]<name>",
-                        "\u05dc\u05db\u05d1\u05d5\u05ea [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "\u05d4\u05d3\u05dc\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05d4\u05d3\u05dc\u05e7\u05d4 [\u05e9\u05dc] [\u05d4]<name>",
-                        "\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
-                    ],
-                    "slots": {
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
                         "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
@@ -233,14 +208,39 @@
                             "blind",
                             "curtain",
                             "shutter",
                             "garage"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "sentences": [
+                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "\u05d4\u05d3\u05dc\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05d4\u05d3\u05dc\u05e7\u05d4 [\u05e9\u05dc] [\u05d4]<name>",
+                        "\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05ea\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>"
+                    ]
                 }
             ]
         }
     },
     "language": "he",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hi.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "{{ area }} \u0928\u093e\u092e \u0915\u093e \u0915\u094b\u0908 \u0915\u094d\u0937\u0947\u0924\u094d\u0930 \u0928\u0939\u0940\u0902 \u0939\u0948",
             "no_domain": "{{ area }} \u0928\u093e\u092e \u0915\u0947 \u0915\u094d\u0937\u0947\u0924\u094d\u0930 \u092e\u0947\u0902 \u0915\u094b\u0908 {{ domain }} \u0928\u0939\u0940\u0902 \u0939\u0948",
             "no_device_class": "{{ area }} \u0928\u093e\u092e \u0915\u0947 \u0915\u094d\u0937\u0947\u0924\u094d\u0930 \u092e\u0947\u0902 \u0915\u094b\u0908 {{ device_class }} \u0928\u0939\u0940\u0902 \u0939\u0948",
             "no_entity": "{{ entity }} \u0928\u093e\u092e \u0915\u093e \u0915\u094b\u0908 \u0921\u093f\u0935\u093e\u0907\u0938 \u092f\u093e \u090f\u0902\u091f\u093f\u091f\u0940 \u0928\u0939\u0940\u0902 \u0939\u0948",
             "handle_error": "\u0907\u0902\u091f\u0947\u0902\u091f \u0915\u094b \u0938\u0902\u092d\u093e\u0932\u0924\u0947 \u0938\u092e\u092f \u090f\u0915 \u0905\u0928\u092a\u0947\u0915\u094d\u0937\u093f\u0924 \u090f\u0930\u0930 \u0939\u0941\u0906"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893794031803543%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(13, OrderedDict([('sentences', ['(jesu li|je "*

 * *              "li|da li (su|je)) <name> {lock_states:state}  [[u|na] <area>]']), ('response', "*

 * *              "'one_yesno'), ('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])), (14, OrderedDict([('sentences', ['(jesu "*

 * *              "li|da li su|ima li) [koja|kojih] <lock> {lock_states:state} [[u|na] <area>]', "*

 * *              "'(jesu li|da  […]*

```diff
@@ -15,64 +15,14 @@
         "uklju\u010di": "uklju\u010di[te|mo]|upali[te|mo]",
         "zatvori": "zatvori[te|mo]|spusti[te|mo]|navuci"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "(jesu li|je li|da li (su|je)) <name> {lock_states:state}  [[u|na] <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "(jesu li|da li su|ima li) [koja|kojih] <lock> {lock_states:state} [[u|na] <area>]",
-                        "(jesu li|da li su|ima li) [koja|kojih] {lock_states:state} <lock> [[u|na] <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "(jesu li|da li su) (sva|svi|sve) <lock> {lock_states:state} [[u|na] <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(koja|koji) [su] <lock> {lock_states:state} [[u|na] <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "(koliko ima|koliko je) {lock_states:state} <lock> [[u|na] <area>]",
-                        "(koliko ima|koliko je) <lock> {lock_states:state} [[u|na] <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "one",
@@ -170,20 +120,104 @@
                     "response": "how_many",
                     "sentences": [
                         "(koliko je) ({cover_classes:device_class}|{cover_states:state}) ({cover_states:state}|{cover_classes:device_class}) [[u|na|iz] <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "(jesu li|je li|da li (su|je)) <name> {lock_states:state}  [[u|na] <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "(jesu li|da li su|ima li) [koja|kojih] <lock> {lock_states:state} [[u|na] <area>]",
+                        "(jesu li|da li su|ima li) [koja|kojih] {lock_states:state} <lock> [[u|na] <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "(jesu li|da li su) (sva|svi|sve) <lock> {lock_states:state} [[u|na] <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "(koja|koji) [su] <lock> {lock_states:state} [[u|na] <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "(koliko ima|koliko je) {lock_states:state} <lock> [[u|na] <area>]",
+                        "(koliko ima|koliko je) <lock> {lock_states:state} [[u|na] <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<isklju\u010di> [sve] (ventilator[e]|ventilaciju) [u|na] <area>",
+                        "<isklju\u010di> <area> (ventilator[e]|ventilaciju)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<isklju\u010di> [sve|svu] (ventilatore|ventilaciju) [u (stanu|ku\u0107i)]"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover"
+                        ]
+                    },
+                    "response": "default_name",
+                    "sentences": [
+                        "<isklju\u010di> {name}",
+                        "<isklju\u010di> {name} [u|na] {area}"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<isklju\u010di> [svjetlo|svjetla|rasvjetu] [u|na] [prostoriji] <area>",
                         "<isklju\u010di> [sva] [svjetl(a|o)] [u] <area> [svjetla|rasvjetu]"
                     ],
                     "slots": {
                         "domain": "light"
@@ -258,108 +292,20 @@
                         "otklju\u010daj [sva|sve] <lock> [[u|na] <area>]",
                         "otklju\u010daj [sva|sve] <area> <lock>"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<isklju\u010di> [sve] (ventilator[e]|ventilaciju) [u|na] <area>",
-                        "<isklju\u010di> <area> (ventilator[e]|ventilaciju)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<isklju\u010di> [sve|svu] (ventilatore|ventilaciju) [u (stanu|ku\u0107i)]"
-                    ],
-                    "slots": {
-                        "area": "all",
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "cover"
-                        ]
-                    },
-                    "response": "default_name",
-                    "sentences": [
-                        "<isklju\u010di> {name}",
-                        "<isklju\u010di> {name} [u|na] {area}"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover"
-                        ]
-                    },
-                    "response": "default_name",
-                    "sentences": [
-                        "(<uklju\u010di>|<otvori>) {name}",
-                        "(<uklju\u010di>|<otvori>) {name} [u|na] {area}"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "zaklju\u010daj <name> [[u|na] <area>]"
-                    ]
-                },
-                {
-                    "response": "lock",
-                    "sentences": [
-                        "zaklju\u010daj [sva|sve] <lock> [[u|na] <area>]",
-                        "zaklju\u010daj [sva|sve] <area> <lock>"
-                    ],
-                    "slots": {
-                        "domain": "lock",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<uklju\u010di> [sve] (ventilator[e]|ventilaciju) [u|na] <area>",
-                        "<uklju\u010di> <area> (ventilator[e]|ventilaciju)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<uklju\u010di> [sve|svu] (ventilatore|ventilaciju) [u (stanu|ku\u0107i)]"
-                    ],
-                    "slots": {
-                        "area": "all",
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "<uklju\u010di> [svjetlo|svjetla|rasvjetu] [u|na] [prostoriji] <area>",
                         "<uklju\u010di> [sva] [svjetl(a|o)] [u] <area> [svjetla|rasvjetu]"
                     ],
                     "slots": {
                         "domain": "light"
@@ -414,14 +360,68 @@
                             "garage",
                             "gate",
                             "shade",
                             "shutter",
                             "window"
                         ]
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<uklju\u010di> [sve] (ventilator[e]|ventilaciju) [u|na] <area>",
+                        "<uklju\u010di> <area> (ventilator[e]|ventilaciju)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<uklju\u010di> [sve|svu] (ventilatore|ventilaciju) [u (stanu|ku\u0107i)]"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "zaklju\u010daj <name> [[u|na] <area>]"
+                    ]
+                },
+                {
+                    "response": "lock",
+                    "sentences": [
+                        "zaklju\u010daj [sva|sve] <lock> [[u|na] <area>]",
+                        "zaklju\u010daj [sva|sve] <area> <lock>"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover"
+                        ]
+                    },
+                    "response": "default_name",
+                    "sentences": [
+                        "(<uklju\u010di>|<otvori>) {name}",
+                        "(<uklju\u010di>|<otvori>) {name} [u|na] {area}"
+                    ]
                 }
             ]
         }
     },
     "language": "hr",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/hu.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(5, OrderedDict([('sentences', ['<turn_on> a "*

 * *              "(ventilátort | ventilátorokat | szellőztetést) <area>', '(ventilátort | "*

 * *              "szellőztetést) be <area> ']), ('slots', OrderedDict([('domain', 'fan'), ('name', "*

 * *              "'all')]))])), (6, OrderedDict([('sentences', ['<name> <turn_on>'])]))], delete: [1, "*

 * *              "0]}}, 'HassTurnOff': {'data': {insert: [(0, OrderedDict([('sentences', ['<turn_off> "*

 * *              "a (ventiláto […]*

```diff
@@ -10,14 +10,29 @@
         "turn_on": "[kapcsol | kapcsold | kapcsolj | nyisd] (be|fel|f\u00f6l)[kapcsol][\u00e1s]",
         "what_is": "(mi | mennyi)"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
+                    "sentences": [
+                        "<turn_off> a (ventil\u00e1tort | ventil\u00e1torokat | szell\u0151ztet\u00e9st) <area>",
+                        "(ventil\u00e1tort | szell\u0151ztet\u00e9st) ki <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<name> <turn_off>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_off> a (l\u00e1mp\u00e1t | l\u00e1mp\u00e1kat) <area>",
                         "<turn_off> <area> a (l\u00e1mp\u00e1t | l\u00e1mp\u00e1kat)"
                     ],
                     "slots": {
                         "domain": "light",
@@ -75,50 +90,20 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shade"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> a (ventil\u00e1tort | ventil\u00e1torokat | szell\u0151ztet\u00e9st) <area>",
-                        "(ventil\u00e1tort | szell\u0151ztet\u00e9st) ki <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<name> <turn_off>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "sentences": [
-                        "<name> <turn_on>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<turn_on> a (ventil\u00e1tort | ventil\u00e1torokat | szell\u0151ztet\u00e9st) <area>",
-                        "(ventil\u00e1tort | szell\u0151ztet\u00e9st) be <area> "
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_on> a (l\u00e1mp\u00e1t | l\u00e1mp\u00e1kat) <area>",
                         "<turn_on> <area> a (l\u00e1mp\u00e1t | l\u00e1mp\u00e1kat)"
                     ],
                     "slots": {
                         "domain": "light",
@@ -176,14 +161,29 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shade"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> a (ventil\u00e1tort | ventil\u00e1torokat | szell\u0151ztet\u00e9st) <area>",
+                        "(ventil\u00e1tort | szell\u0151ztet\u00e9st) be <area> "
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<name> <turn_on>"
+                    ]
                 }
             ]
         }
     },
     "language": "hu",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/id.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986111111111111%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(1, OrderedDict([('sentences', "*

 * *              "['<nyala_imperatif> <nama>'])]))], delete: [0]}}, 'HassTurnOff': {'data': {insert: "*

 * *              "[(1, OrderedDict([('sentences', ['<mati_imperatif> [semua] lampu [di] <area>', "*

 * *              "'<mati_imperatif> [semua] lampu <area>']), ('slots', OrderedDict([('domain', "*

 * *              "'light')]))]))], delete: [0]}}}"}*

```diff
@@ -13,43 +13,43 @@
         "tutup_imperatif": "(tutup | tutupin)"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "<mati_imperatif> <nama>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "<mati_imperatif> [semua] lampu [di] <area>",
                         "<mati_imperatif> [semua] lampu <area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
-                },
-                {
-                    "sentences": [
-                        "<mati_imperatif> <nama>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<nyala_imperatif> <nama>"
-                    ]
-                },
-                {
-                    "sentences": [
                         "<nyala_imperatif> [semua] lampu [di] <area>",
                         "<nyala_imperatif> [semua] lampu <area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
+                },
+                {
+                    "sentences": [
+                        "<nyala_imperatif> <nama>"
+                    ]
                 }
             ]
         }
     },
     "language": "id",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ur.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.717720984648068%*

 * *Differences: {"'expansion_rules'": "{'name': '{name} [کو] [کے] [کا]', 'area': '{area} [کا] [کے] [کو] [میں]', "*

 * *                      "'brightness': '{brightness} [پرسنٹ]', 'set': '[میں] [پر] (کر دیں | سیٹ کردو "*

 * *                      "| کردو | رکھلو | دالدو | دالو | سیٹ کرو | کرو | کر | کریں)', 'temp': '(درجہ "*

 * *                      "حرارت | ٹیمپریچر)', 'temperature': '{temperature} [ڈگری] [درجہ حرارت] "*

 * *                      "[{temperature_unit}]', 'all': '(تمام | سب | ساری | سارے)', delete: ['the', "*

 * *                  […]*

```diff
@@ -1,483 +1,474 @@
 {
     "expansion_rules": {
-        "area": "{area}",
-        "brightness": "{brightness}[%| percento]",
-        "close": "(chiud(i|ere) | abbass(a|are))",
-        "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|i))",
-        "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione | climatizzator(e|i) | condizionator(e|i))",
-        "in": "(in | ne[i|gli|l[lo|la|le]])",
-        "name": "{name}",
-        "of": "(de[i|gli|l[lo|la|le]]|di)",
-        "open": "(apr(i|ire) | alz(a|are))",
-        "set": "(impost(a|are) | cambi(a|are) | mett(i|ere) | modific(a|are))",
-        "temp": "[la] (temperatura)",
-        "temperature": "{temperature}[\u00b0| gradi] [{temperature_unit}]",
-        "the": "(l(o|a|e) | i[l] | gli | l')",
-        "to": "a[l[lo|la|le] | gli]",
-        "turn_off": "(spegn(i|ere) | disattiv(a|are))",
-        "turn_on": "(accend(i|ere) | attiv(a|are))",
-        "what_is": "(qual[e] \u00e8 | quant(o |')\u00e8 | com(e |')\u00e8 | che)"
+        "all": "(\u062a\u0645\u0627\u0645 | \u0633\u0628 | \u0633\u0627\u0631\u06cc | \u0633\u0627\u0631\u06d2)",
+        "area": "{area} [\u06a9\u0627] [\u06a9\u06d2] [\u06a9\u0648] [\u0645\u06cc\u06ba]",
+        "brightness": "{brightness} [\u067e\u0631\u0633\u0646\u0679]",
+        "name": "{name} [\u06a9\u0648] [\u06a9\u06d2] [\u06a9\u0627]",
+        "set": "[\u0645\u06cc\u06ba] [\u067e\u0631] (\u06a9\u0631 \u062f\u06cc\u06ba | \u0633\u06cc\u0679 \u06a9\u0631\u062f\u0648 | \u06a9\u0631\u062f\u0648 | \u0631\u06a9\u06be\u0644\u0648 | \u062f\u0627\u0644\u062f\u0648 | \u062f\u0627\u0644\u0648 | \u0633\u06cc\u0679 \u06a9\u0631\u0648 | \u06a9\u0631\u0648 | \u06a9\u0631 | \u06a9\u0631\u06cc\u06ba)",
+        "temp": "(\u062f\u0631\u062c\u06c1 \u062d\u0631\u0627\u0631\u062a | \u0679\u06cc\u0645\u067e\u0631\u06cc\u0686\u0631)",
+        "temperature": "{temperature} [\u0688\u06af\u0631\u06cc] [\u062f\u0631\u062c\u06c1 \u062d\u0631\u0627\u0631\u062a] [{temperature_unit}]"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "response": "one",
                     "sentences": [
-                        "<what_is> [lo stato <of>|stato ha[nno]] [<the>] <name> [(<in>|of) <area>]"
+                        "<name> [\u06a9\u0627] [\u062d\u0627\u0644|\u062d\u0627\u0644\u062a|\u0633\u0679\u0627\u0679\u0633|\u0627\u0633\u0679\u06cc\u0679] \u06a9\u06cc\u0627 [\u06c1\u06d2] [\u062d\u0627\u0644|\u062d\u0627\u0644\u062a|\u0633\u0679\u0627\u0679\u0633|\u0627\u0633\u0679\u06cc\u0679]",
+                        "\u06a9\u06cc\u0627 [\u062d\u0627\u0644|\u062d\u0627\u0644\u062a|\u0633\u0679\u0627\u0679\u0633|\u0627\u0633\u0679\u06cc\u0679] [\u06c1\u06d2] <name> [\u06a9\u0627]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[Lo stato <of>] [<the>] <name> \u00e8 {on_off_states:state} [<in> <area>]"
+                        "[\u06a9\u06cc\u0627] <name> {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]",
+                        "<name> [\u06a9\u06cc\u0627] {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "(C'\u00e8 una|Ci sono delle) {on_off_domains:domain} [<of> <area>] {on_off_states:state} [<in> <area>]"
+                        "[\u06a9\u06cc\u0627] \u06a9\u0648\u0626\u06cc [\u0628\u06be\u06cc] {on_off_domains:domain} {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]",
+                        "[\u06a9\u06cc\u0627] \u06a9\u0648\u0626\u06cc [\u0628\u06be\u06cc] {on_off_domains:domain} [<area>] {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] "
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "[tutte] <the> {on_off_domains:domain} [<of> <area>] sono [tutt(i|e)] {on_off_states:state} [<in> <area>]"
+                        "[\u06a9\u06cc\u0627] <all> {on_off_domains:domain} {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(Qual(i|e)|Che) {on_off_domains:domain} [<of> <area>] (\u00e8|sono) {on_off_states:state} [<in> <area>]"
+                        "(\u06a9\u0648\u0646\u0633\u06cc|\u06a9\u0648\u0646\u0633\u0627) {on_off_domains:domain} {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "Quant(i|e) {on_off_domains:domain} [<of> <area>] (\u00e8|sono) {on_off_states:state} [<in> <area>]"
+                        "(\u06a9\u062a\u0646\u06d2|\u06a9\u062a\u0646\u06cc) {on_off_domains:domain} {on_off_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[<the>] <name> \u00e8 {cover_states:state} [<in> <area>]",
-                        "\u00e8 {cover_states:state} <name> [<in> <area>]"
+                        "\u06a9\u06cc\u0627 <name> {cover_states:state} [area] [\u06c1\u06d2]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "(C'\u00e8 una|Ci sono delle) {cover_classes:device_class} {cover_states:state} [<in> <area>]"
+                        "[\u06a9\u06cc\u0627] \u06a9\u0648\u0626\u06cc [\u0628\u06be\u06cc] {cover_classes:device_class} {cover_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]",
+                        "[\u06a9\u06cc\u0627] \u06a9\u0648\u0626\u06cc [\u0628\u06be\u06cc] {cover_classes:device_class} [<area>] {cover_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "<the> {cover_classes:device_class} [<of> <area>] sono [tutt(i|e)] {cover_states:state} [<in> <area>]",
-                        "[tutt(i|e)] [<the>] {cover_classes:device_class} [(<of>|<in>) <area>] sono {cover_states:state} [<in> <area>]"
+                        "[\u06a9\u06cc\u0627] <all> {cover_classes:device_class} {cover_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(Qual(i|e)|Che) {cover_classes:device_class} [<of> <area>] (\u00e8|sono) {cover_states:state} [<in> <area>]"
+                        "(\u06a9\u0648\u0646\u0633\u06cc|\u06a9\u0648\u0646\u0633\u0627) {cover_classes:device_class} {cover_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "Quant(i|e) {cover_classes:device_class} [<of> <area>] (\u00e8|sono) {cover_states:state} [<in> <area>]"
+                        "(\u06a9\u062a\u0646\u06d2|\u06a9\u062a\u0646\u06cc) {cover_classes:device_class} {cover_states:state} [\u06be\u0648\u0627 \u0648\u0627] [\u06c1\u0648\u0626\u06cc] [\u0648\u06cc] [\u06c1\u06d2] [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<turn_off> [tutte] [l(a|e)] (luc(e|i)) [(<of>|<in>)] <area>",
-                        "<turn_off> [<in>] <area> [tutte] [l(a|e)] (luc(e|i))"
+                        "<area> [<all>] (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) [\u06a9\u0648] (\u0628\u0646\u062f | \u0622\u0641) [<set>]",
+                        "[<all>] (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) <area> (\u0628\u0646\u062f | \u0622\u0641) [<set>]",
+                        "[<all>] <area> (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) [\u06a9\u0648] (\u0628\u0646\u062f | \u0622\u0641) [<set>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
                     "sentences": [
-                        "<close> [<the>] <name> [[<of>|<in>] <area>]"
+                        "<name> (\u0628\u0646\u062f | \u0622\u0641) [<set>]",
+                        "(\u0628\u0646\u062f | \u0622\u0641) [<set>] <name> "
                     ]
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> [<the>] <cover> [[<in> | <of>] <area>]",
-                        "<close> [[<in>] <area>] [<the>] <cover>"
-                    ]
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<close> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
-                        "<close> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
-                        "<close> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
-                },
-                {
                     "sentences": [
-                        "<turn_off> [(tutt(i|e))] [<the>]<fan> [(<of> | <in>)] <area>",
-                        "<turn_off> [<in>] <area> [(tutt(i|e))] [<the>]<fan>"
+                        "<area> [<all>] (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s]) [\u06a9\u0648] (\u0628\u0646\u062f | \u0622\u0641 | \u0628\u062c\u06be\u0627\u062f\u0648) [<set>]",
+                        "[<all>] (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s]) <area> (\u0628\u0646\u062f | \u0622\u0641 | \u0628\u062c\u06be\u0627\u062f\u0648) [<set>]",
+                        "[<all>] <area> (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s]) [\u06a9\u0648] (\u0628\u0646\u062f | \u0622\u0641 | \u0628\u062c\u06be\u0627\u062f\u0648) [<set>]"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> [<the>]<name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<turn_on> [<the>]<name>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<turn_on> [(tutt(i|e))] [<the>]<fan> [(<of> | <in>)] <area>",
-                        "<turn_on> [<in>] <area> [(tutt(i|e))] [<the>]<fan>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<turn_on> [tutte] [l(a|e)] (luc(e|i)) [(<of>|<in>)] <area>",
-                        "<turn_on> [<in>] <area> [tutte] [l(a|e)] (luc(e|i))"
+                        "<area> [<all>] (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s] | \u0628\u062a\u06cc) [\u06a9\u0648] (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]",
+                        "[<all>] (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s] | \u0628\u062a\u06cc) <area> (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]",
+                        "[<all>] <area> (\u0644\u0627\u06cc\u0679 | \u0644\u0627\u06cc\u0679\u06cc\u06ba | light[s] | \u0628\u062a\u06cc) [\u06a9\u0648]  (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
-                    "sentences": [
-                        "<open> [<the>] <name> [[<of>|<in>] <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover_area",
-                    "sentences": [
-                        "<open> [<the>] <cover> [[<in> | <of>] <area>]",
-                        "<open> [[<in>] <area>] [<the>] <cover>"
-                    ]
-                },
-                {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<open> <the> (serranda | [porta [del garage]] [basculante] | saracinesca) [[(in | del)] garage]",
-                        "<open> [[<in>] garage] <the> (serranda | [porta [del garage]] [basculante] | saracinesca)"
+                        "<area> [<all>] (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) [\u06a9\u0648] (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]",
+                        "[<all>] (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) <area> (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]",
+                        "[<all>] <area> (\u067e\u0646\u06a9\u06be\u06d2 | \u067e\u0646\u06a9\u06be\u0627) [\u06a9\u0648] (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area",
                     "sentences": [
-                        "<open> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e)) [(<in> | <of>)] <area>",
-                        "<open> [<in>] <area> [l(a|e)] (tend(a|e) | tapparell(a|e) | venezian(a|e))"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
+                        "<name> (\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>]",
+                        "(\u06a9\u06be\u0648\u0644 \u062f\u0648 | \u06a9\u06be\u0648\u0644\u0648 | \u06a9\u06be\u0648\u0644\u0646\u0627 | \u0622\u0646) [<set>] <name>"
+                    ]
                 }
             ]
         }
     },
-    "language": "it",
+    "language": "ur",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "bianco",
+                    "in": "\u0633\u0641\u06cc\u062f",
                     "out": "white"
                 },
                 {
-                    "in": "nero",
+                    "in": "white",
+                    "out": "white"
+                },
+                {
+                    "in": "\u0633\u06cc\u0627\u06c1",
+                    "out": "black"
+                },
+                {
+                    "in": "\u06a9\u0627\u0644\u0627",
+                    "out": "black"
+                },
+                {
+                    "in": "black",
                     "out": "black"
                 },
                 {
-                    "in": "rosso",
+                    "in": "\u0633\u0631\u062e",
+                    "out": "red"
+                },
+                {
+                    "in": "\u0644\u0627\u0644",
+                    "out": "red"
+                },
+                {
+                    "in": "red",
                     "out": "red"
                 },
                 {
-                    "in": "arancione",
+                    "in": "\u0627\u0648\u0631\u0646\u062c",
+                    "out": "orange"
+                },
+                {
+                    "in": "\u0646\u0627\u0631\u0646\u062c\u06cc",
                     "out": "orange"
                 },
                 {
-                    "in": "giallo",
+                    "in": "orange",
+                    "out": "orange"
+                },
+                {
+                    "in": "\u067e\u06cc\u0644\u0627",
                     "out": "yellow"
                 },
                 {
-                    "in": "verde",
+                    "in": "yellow",
+                    "out": "yellow"
+                },
+                {
+                    "in": "\u0633\u0628\u0632",
+                    "out": "green"
+                },
+                {
+                    "in": "\u06c1\u0631\u0627",
                     "out": "green"
                 },
                 {
-                    "in": "blu",
+                    "in": "green",
+                    "out": "green"
+                },
+                {
+                    "in": "\u0646\u06cc\u0644\u0627",
+                    "out": "blue"
+                },
+                {
+                    "in": "blue",
                     "out": "blue"
                 },
                 {
-                    "in": "viola",
+                    "in": "\u062c\u0627\u0645\u0646\u06cc",
                     "out": "purple"
                 },
                 {
-                    "in": "marrone",
+                    "in": "purple",
+                    "out": "purple"
+                },
+                {
+                    "in": "\u067e\u0646\u06a9",
+                    "out": "pink"
+                },
+                {
+                    "in": "\u06af\u0644\u0627\u0628\u06cc",
+                    "out": "pink"
+                },
+                {
+                    "in": "pink",
+                    "out": "pink"
+                },
+                {
+                    "in": "\u0628\u0631\u0627\u0624\u0646",
                     "out": "brown"
+                },
+                {
+                    "in": "brown",
+                    "out": "brown"
+                },
+                {
+                    "in": "\u0622\u0633\u0645\u0627\u0646\u06cc",
+                    "out": "sky blue"
+                },
+                {
+                    "in": "sky blue",
+                    "out": "sky blue"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "tend(a|e) da sole",
-                    "out": "awning"
-                },
-                {
-                    "in": "persian(a|e)",
+                    "in": "\u0628\u0644\u0627\u06cc\u0646\u0688\u0632|\u0628\u0644\u0627\u06cc\u0646\u0688",
                     "out": "blind"
                 },
                 {
-                    "in": "tend(a|e)",
+                    "in": "\u067e\u0631\u062f\u06d2|\u067e\u0631\u062f\u0627\u06be",
                     "out": "curtain"
                 },
                 {
-                    "in": "port(a|e)",
+                    "in": "\u062f\u0631\u0648\u0627\u0632\u06c1",
                     "out": "door"
                 },
                 {
-                    "in": "(serrand(a|e) | port(a|e) [basculant(e|i)|de(l|i) garage] | saracinesc(a|he))",
+                    "in": "\u06af\u06cc\u0631\u0627\u062c",
                     "out": "garage"
                 },
                 {
-                    "in": "cancell(o|i)",
+                    "in": "\u06af\u06cc\u0679",
                     "out": "gate"
                 },
                 {
-                    "in": "venezian(a|e)",
+                    "in": "\u0634\u06cc\u0688\u0632|\u0634\u06cc\u0688",
                     "out": "shade"
                 },
                 {
-                    "in": "tapparell(a|e)",
+                    "in": "\u0634\u0679\u0631",
                     "out": "shutter"
                 },
                 {
-                    "in": "finestr(a|e)",
+                    "in": "\u06a9\u06be\u0691\u06a9\u06cc",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "apert(a|o|e)",
+                    "in": "\u06a9\u06be\u0644\u0627\u0648\u0627",
                     "out": "open"
                 },
                 {
-                    "in": "chius(a|o|e)",
-                    "out": "closed"
+                    "in": "\u06a9\u06be\u0644\u06cc",
+                    "out": "open"
                 },
                 {
-                    "in": "in apertura",
-                    "out": "opening"
+                    "in": "\u06a9\u06be\u0644\u0627",
+                    "out": "open"
                 },
                 {
-                    "in": "in chiusura",
-                    "out": "closing"
-                }
-            ]
-        },
-        "lock_states": {
-            "values": [
+                    "in": "[\u0648\u06cc]\u06a9\u06be\u0644\u06cc [\u06c1\u0648\u06cc]",
+                    "out": "open"
+                },
                 {
-                    "in": "chiusa",
-                    "out": "locked"
+                    "in": "\u0628\u0646\u062f",
+                    "out": "closed"
+                },
+                {
+                    "in": "\u06a9\u06be\u0644 \u0631\u06c1\u06c1\u0627",
+                    "out": "closing"
                 },
                 {
-                    "in": "aperta",
-                    "out": "aperto"
+                    "in": "\u0628\u0646\u062f \u06c1\u0648\u0631\u06be\u0627",
+                    "out": "closing"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "luc(e|i)",
+                    "in": "\u0644\u0627\u06cc\u0679|\u0644\u0627\u06cc\u0679\u06cc\u06ba",
                     "out": "light"
                 },
                 {
-                    "in": "(ventol(a|e)|ventilator(e|i)|ventilazione|climatizzator(e|i)|condizionator(e|i))",
+                    "in": "\u067e\u0646\u06a9\u06be\u0627|\u067e\u0646\u06a9\u06be\u06d2",
                     "out": "fan"
                 },
                 {
-                    "in": "(interruttor(e|i)|pres(a|e))",
+                    "in": "\u0633\u0648\u0626\u0686|\u0633\u0648\u0626\u0686\u0632|\u0628\u0679\u0646|\u0628\u0679\u0646\u0633|\u0628\u0679\u0646\u0632",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "(acces(o|i|a|e)|attiv(o|i|a|e))",
+                    "in": "\u06a9\u06be\u0644\u0627\u0648\u0627",
+                    "out": "on"
+                },
+                {
+                    "in": "\u06a9\u06be\u0644\u06cc",
+                    "out": "on"
+                },
+                {
+                    "in": "\u06a9\u06be\u0644\u0627",
+                    "out": "on"
+                },
+                {
+                    "in": "\u0622\u0646",
                     "out": "on"
                 },
                 {
-                    "in": "(spent(o|i|a|e)|disattiv(o|i|a|e))",
+                    "in": "\u0628\u0646\u062f",
+                    "out": "off"
+                },
+                {
+                    "in": "\u0622\u0641",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "(celsius | centigradi)",
+                "celsius",
                 {
                     "in": "c",
                     "out": "celsius"
                 },
+                {
+                    "in": "\u0633\u06cc\u0644\u0633\u06cc\u0633",
+                    "out": "celsius"
+                },
                 "fahrenheit",
                 {
                     "in": "f",
                     "out": "fahrenheit"
+                },
+                {
+                    "in": "\u0641\u0627\u0631\u0646\u06c1\u0627\u06cc\u0679",
+                    "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Si \u00e8 verificato un errore inatteso durante l'elaborazione",
-            "no_area": "Non esiste nessuna area chiamata {{ area }}",
-            "no_device_class": "{{ area }} non contiene {{ device_class }}",
-            "no_domain": "{{ area }} non contiene {{ domain }}",
-            "no_entity": "Non esiste nessun dispositivo o entit\u00e0 chiamato {{ entity }}",
-            "no_intent": "Mi dispiace, non ho capito"
+            "handle_error": "\u0622\u067e \u06a9\u06d2 \u062c\u0648\u0627\u0628 \u06a9\u0648 \u0633\u0646\u0628\u06be\u0627\u0644\u062a\u06d2 \u0648\u0642\u062a \u06a9\u0686\u06be \u0639\u062c\u06cc\u0628 \u0645\u0633\u0626\u0644\u06c1 \u0622\u06af\u06cc\u0627",
+            "no_area": "\u06a9\u0633\u06cc \u062c\u06af\u06c1 \u06a9\u0627 \u0646\u0627\u0645  {{ area }} \u0646\u06c1\u06cc\u06ba \u06be\u06d2",
+            "no_device_class": "{{ area }} \u0645\u06cc\u06ba {{ device_class }} \u0646\u06c1\u06cc\u06ba \u06c1\u06d2",
+            "no_domain": "{{ area }} \u0645\u06cc\u06ba {{ domain }} \u0646\u06c1\u06cc\u06ba \u06c1\u06d2",
+            "no_entity": "\u06a9\u0648\u0626\u06cc \u0688\u0648\u0627\u0626\u0633 \u06a9\u0627 \u0646\u0627\u0645 {{ entity }} \u0646\u06c1\u06cc\u06ba \u06be\u06d2 ",
+            "no_intent": "\u0645\u062c\u06be\u06d2 \u0633\u0645\u062c\u06be \u0645\u06cc\u06ba \u0646\u06c1\u06cc\u06ba \u0622\u06cc\u0627"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  S\u00ec\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length == 4 %}\n    No, {{ no_match[:3] | join(\", \") }} ed un altro no\n  {% elif no_match | length > 4 %}\n    No, {{ no_match[:3] | join(\", \") }} ed altri {{ (no_match | length - 3) }}\n  {%- else -%}\n    No,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor %} no\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length == 4 %}\n    S\u00ec, {{ match[:3] | join(\", \") }} ed un altro\n  {% elif match | length > 4 %}\n    S\u00ec, {{ match[:3] | join(\", \") }} ed altri {{ (match | length - 3) }}\n  {%- else -%}\n    S\u00ec,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  No\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  \u062c\u06cc \u06c1\u0627\u06ba\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u0646\u06c1\u06cc\u06ba\u060c {{ no_match[:3] | join(\", \") }} \u0627\u0648\u0631 {{ (no_match | length - 3) }} \u0627\u0648\u0631 \u0646\u06c1\u06cc\u06ba \u06be\u06cc\u06ba\n  {%- else -%}\n    \u0646\u06c1\u06cc\u06ba\u060c\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0627\u0648\u0631 {% endif -%}\n      {{ name }}\n    {%- endfor %} \u0646\u06c1\u06cc\u06ba \u06be\u06cc\u06ba\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u062c\u06cc\u060c {{ match[:3] | join(\", \") }} \u0627\u0648\u0631 {{ (match | length - 3) }} \u0627\u0648\u0631 \u062f\u0648\u0633\u0631\u06cc \u0686\u06cc\u0632\u06cc\u06ba \u0628\u06be\u06cc\n  {%- else -%}\n    \u062c\u06cc\u060c\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0627\u0648\u0631 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u0646\u06c1\u06cc\u06ba\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "{{ slots.name | capitalize }} \u00e8 {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  S\u00ec\n{% else %}\n  No, \u00e8 {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  Nessuno\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length == 4 %}\n    {{ match[:3] | join(\", \") }} ed un altro\n  {% elif match | length > 4 %}\n    {{ match[:3] | join(\", \") }} ed altri {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} e {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+                "one": "{{ slots.name | capitalize }} {{ state.state_with_unit }} \u06c1\u06d2\n",
+                "one_yesno": "{% if query.matched %}\n  \u062c\u06cc \u06c1\u0627\u06ba\n{% else %}\n  \u0646\u06c1\u06cc\u06ba\u060c {{ state.state_with_unit }} \u06c1\u06d2\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u06a9\u0648\u0626\u06cc \u0628\u06be\u06cc \u0646\u06c1\u06cc\u06ba\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0627\u0648\u0631 {{ (match | length - 3) }} \u0627\u0648\u0631\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0627\u0648\u0631 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "Ho chiuso {{ slots.name }}",
-                "cover_area": "Chiuse in {{ slots.area }}",
-                "cover_device_class": "Ho chiuso {{ slots.device_class }}",
-                "default": "Ho spento {{ slots.name }}",
-                "fans_area": "Ho spento la ventilazione in {{ slots.area }}",
-                "lights_area": "Ho spento le luci in {{ slots.area }}",
-                "scene": "Ho disattivato {{ slots.name }}",
-                "script": "Ho arrestato {{ slots.name }}"
+                "cover": "{{ slots.name }} \u06a9\u0648 \u0628\u0646\u062f \u06a9\u0631\u062f\u06cc\u0622 \u06be\u06d2",
+                "cover_area": "{{ slots.area }} \u06a9\u0648 \u0628\u0646\u062f \u06a9\u0631\u062f\u06cc\u0622 \u06be\u06d2",
+                "default": "{{ slots.name }} \u06a9\u0648 \u0628\u0646\u062f \u06a9\u0631\u062f\u06cc\u0622 \u06be\u06d2",
+                "fans_area": "{{ slots.area }} \u06a9\u06d2 \u067e\u0646\u06a9\u06be\u06d2 \u06a9\u0648 \u0628\u0646\u062f \u06a9\u0631\u062f\u06cc\u0622 \u06be\u06d2",
+                "lights_area": "{{ slots.area }} \u06a9\u06d2 \u0644\u0627\u06cc\u0679\u06cc\u06ba \u06a9\u0648 \u0628\u0646\u062f \u06a9\u0631\u062f\u06cc\u0622 \u06be\u06d2"
             },
             "HassTurnOn": {
-                "cover": "Ho aperto {{ slots.name }}",
-                "cover_area": "Aperte in {{ slots.area }}",
-                "cover_device_class": "Ho aperto {{ slots.device_class }}",
-                "default": "Ho acceso {{ slots.name }}",
-                "fans_area": "Ho acceso la ventilazione in {{ slots.area }}",
-                "lights_area": "Ho acceso le luci in {{ slots.area }}",
-                "scene": "Ho attivato {{ slots.name }}",
-                "script": "Ho avviato {{ slots.name }}"
+                "cover": "{{ slots.name }} \u06a9\u0648 \u06a9\u06be\u0648\u0644\u062f\u06cc\u0627 \u06be\u06d2",
+                "cover_area": "{{ slots.area }} \u06a9\u0648 \u06a9\u06be\u0648\u0644\u062f\u06cc\u0627 \u06be\u06d2",
+                "default": "{{ slots.name }} \u06a9\u0648 \u06a9\u06be\u0648\u0644\u062f\u06cc\u0627 \u06be\u06d2",
+                "fans_area": "{{ slots.area }} \u06a9\u06d2 \u067e\u0646\u06a9\u06be\u06d2 \u06a9\u0648 \u06a9\u06be\u0648\u0644\u062f\u06cc\u0627 \u06be\u06d2",
+                "lights_area": "{{ slots.area }} \u06a9\u06d2 \u0644\u0627\u06cc\u0679\u06cc\u06ba \u06a9\u0648 \u06a9\u06be\u0648\u0644\u062f\u06cc\u0627 \u06be\u06d2"
             }
         }
     },
     "skip_words": [
-        "per favore",
-        "potresti",
-        "puoi",
-        "puoi dirmi",
-        "dimmi",
-        "grazie"
+        "\u06cc\u0627\u0631",
+        "\u0632\u0631\u0627",
+        "please"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ka.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,32 +1,32 @@
 {
     "language": "ka",
     "intents": {
-        "HassTurnOn": {
+        "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "(<\u10e9\u10d0\u10e0\u10d7\u10d4> | <\u10d0\u10d0\u10dc\u10d7\u10d4>) <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0 <\u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0>",
-                        "<\u10d0\u10d0\u10dc\u10d7\u10d4> [\u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8] <\u10d0\u10e0\u10d4\u10d0>",
-                        "<\u10d0\u10d0\u10dc\u10d7\u10d4> <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8"
+                        "(<\u10d2\u10d0\u10db\u10dd\u10e0\u10d7\u10d4> | <\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4>) <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0 <\u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0>",
+                        "<\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4> [\u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8] <\u10d0\u10e0\u10d4\u10d0>",
+                        "<\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4> <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8"
                     ],
                     "slots": {
                         "domain": "light",
                         "area": "kitchen"
                     }
                 }
             ]
         },
-        "HassTurnOff": {
+        "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "(<\u10d2\u10d0\u10db\u10dd\u10e0\u10d7\u10d4> | <\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4>) <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0 <\u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0>",
-                        "<\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4> [\u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8] <\u10d0\u10e0\u10d4\u10d0>",
-                        "<\u10e9\u10d0\u10d0\u10e5\u10e0\u10d4> <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8"
+                        "(<\u10e9\u10d0\u10e0\u10d7\u10d4> | <\u10d0\u10d0\u10dc\u10d7\u10d4>) <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0 <\u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0>",
+                        "<\u10d0\u10d0\u10dc\u10d7\u10d4> [\u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8] <\u10d0\u10e0\u10d4\u10d0>",
+                        "<\u10d0\u10d0\u10dc\u10d7\u10d4> <\u10d0\u10e0\u10d4\u10d0> \u10e7\u10d5\u10d4\u10da\u10d0\u10e4\u10d4\u10e0\u10d8"
                     ],
                     "slots": {
                         "domain": "light",
                         "area": "kitchen"
                     }
                 }
             ]
@@ -38,29 +38,29 @@
             "no_area": "\u10d0\u10e0\u10d4\u10d0 \u10e1\u10d0\u10ee\u10d4\u10da\u10d8\u10d7 {{ area }}, \u10d0\u10e0 \u10d0\u10e0\u10e1\u10d4\u10d1\u10dd\u10d1\u10e1",
             "no_domain": "\u10d0\u10e0\u10d4\u10d0 {{ area }} \u10d0\u10e0 \u10e8\u10d4\u10d8\u10ea\u10d0\u10d5\u10e1 {{ domain }} \u10d3\u10dd\u10db\u10d4\u10dc\u10e1",
             "no_device_class": "\u10d0\u10e0\u10d4\u10d0 {{ area }} \u10d0\u10e0 \u10d0\u10e0\u10d8\u10e1 {{ device_class }} \u10db\u10dd\u10ec\u10e7\u10dd\u10d1\u10d8\u10da\u10dd\u10d1\u10d8\u10e1 \u10d9\u10da\u10d0\u10e1\u10d8\u10e1",
             "no_entity": "\u10db\u10dd\u10ec\u10e7\u10dd\u10d1\u10d8\u10da\u10dd\u10d1\u10d0 \u10d0\u10dc \u10d4\u10e0\u10d7\u10d4\u10e3\u10da\u10d8 \u10e1\u10d0\u10ee\u10d4\u10da\u10d8\u10d0\u10d3 {{ entity }}, \u10d0\u10e0 \u10d0\u10e0\u10e1\u10d4\u10d1\u10dd\u10d1\u10e1",
             "handle_error": "\u10d2\u10d0\u10e3\u10d7\u10d5\u10d0\u10da\u10d8\u10e1\u10ec\u10d8\u10dc\u10d4\u10d1\u10d4\u10da\u10d8 \u10e8\u10d4\u10ea\u10d3\u10dd\u10db\u10d0 \u10db\u10dd\u10ee\u10d3\u10d0 \u10d7\u10e5\u10d5\u10d4\u10dc\u10d8 \u10db\u10dd\u10d7\u10ee\u10dd\u10d5\u10dc\u10d8\u10e1 \u10d3\u10d0\u10db\u10e3\u10e8\u10d0\u10d5\u10d4\u10d1\u10d8\u10e1\u10d0\u10e1"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "\u10e9\u10d0\u10d5\u10e0\u10d7\u10d4 {{ slots.name }}",
-                "lights_area": "\u10d0\u10d5\u10d0\u10dc\u10d7\u10d4 \u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0 {{ slots.area }}\u10e8\u10d8",
-                "fans_area": "\u10e9\u10d0\u10d5\u10e0\u10d7\u10d4 \u10d5\u10d4\u10dc\u10e2\u10d8\u10da\u10d0\u10ea\u10d8\u10d0 {{ slots.area }}\u10e8\u10d8",
-                "cover": "\u10d2\u10d0\u10d5\u10d0\u10e6\u10d4 {{ slots.name }}",
-                "cover_area": "\u10d2\u10d0\u10d5\u10d0\u10e6\u10d4 {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "\u10d2\u10d0\u10db\u10dd\u10d5\u10e0\u10d7\u10d4 {{ slots.name }}",
                 "lights_area": "\u10e9\u10d0\u10d5\u10d0\u10e5\u10e0\u10d4 \u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0 {{ slots.area }}\u10e8\u10d8",
                 "fans_area": "\u10d2\u10d0\u10db\u10dd\u10d5\u10e0\u10d7\u10d4 \u10d5\u10d4\u10dc\u10e2\u10d8\u10da\u10d0\u10ea\u10d8\u10d0 {{ slots.area }}\u10e8\u10d8",
                 "cover": "\u10d3\u10d0\u10d5\u10ee\u10e3\u10e0\u10d4 {{ slots.name }}",
                 "cover_area": "\u10d3\u10d0\u10d5\u10ee\u10e3\u10e0\u10d4 {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "\u10e9\u10d0\u10d5\u10e0\u10d7\u10d4 {{ slots.name }}",
+                "lights_area": "\u10d0\u10d5\u10d0\u10dc\u10d7\u10d4 \u10d2\u10d0\u10dc\u10d0\u10d7\u10d4\u10d1\u10d0 {{ slots.area }}\u10e8\u10d8",
+                "fans_area": "\u10e9\u10d0\u10d5\u10e0\u10d7\u10d4 \u10d5\u10d4\u10dc\u10e2\u10d8\u10da\u10d0\u10ea\u10d8\u10d0 {{ slots.area }}\u10e8\u10d8",
+                "cover": "\u10d2\u10d0\u10d5\u10d0\u10e6\u10d4 {{ slots.name }}",
+                "cover_area": "\u10d2\u10d0\u10d5\u10d0\u10e6\u10d4 {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {
         "\u10d0\u10e0\u10d4\u10d0": "{area}[\u10e8\u10d8|\u10e1|\u10e1\u10d8|\u10d8\u10e1]",
         "\u10e9\u10d0\u10e0\u10d7\u10d4": "(\u10e9\u10d0\u10e0\u10d7\u10d4 | \u10d2\u10d0\u10e3\u10e8\u10d5\u10d8)",
         "\u10d2\u10d0\u10db\u10dd\u10e0\u10d7\u10d4": "(\u10d2\u10d0\u10db\u10dd\u10e0\u10d7\u10d4 | \u10d2\u10d0\u10d0\u10e9\u10d4\u10e0\u10d4)",
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/kn.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "TODO No area named {{ area }}",
             "no_domain": "TODO {{ area }} does not contain a {{ domain }}",
             "no_device_class": "TODO {{ area }} does not contain a {{ device_class }}",
             "no_entity": "TODO No device or entity named {{ entity }}",
             "handle_error": "TODO An unexpected error occurred while handling the intent"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lb.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(2, OrderedDict([('sentences', ['schalt <name> "*

 * *              "un', 'schalt <name> <area> un', 'aktivéier <name>', '<maach> <area> <name> <op>', "*

 * *              "'<maach> <name> <area> <op>'])])), (3, OrderedDict([('sentences', ['<maach> <area> "*

 * *              "(<window> | <garage>) <op>', '<maach> (<window> | <garage>) <area> <op>']), "*

 * *              "('response', 'cover_area')]))], delete: [1, 0]}}, 'HassTurnOff': {'data': {insert: "*

 * *              "[(2, Or […]*

```diff
@@ -115,14 +115,30 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "sentences": [
+                        "schalt <name> aus",
+                        "schalt <name> <area> aus",
+                        "stopp <name>",
+                        "<maach> <area> <name> <zou>",
+                        "<maach> <name> <area> <zou>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<maach> <area> (<window> | <garage>) <zou>",
+                        "<maach> (<window> | <garage>) <area> <zou>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<maach> [(all | alleguer)] <light> <area> aus",
                         "<maach> [(all | alleguer)] <area> <light> aus"
                     ],
                     "slots": {
                         "domain": "light",
@@ -139,52 +155,20 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "schalt <name> aus",
-                        "schalt <name> <area> aus",
-                        "stopp <name>",
-                        "<maach> <area> <name> <zou>",
-                        "<maach> <name> <area> <zou>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<maach> <area> (<window> | <garage>) <zou>",
-                        "<maach> (<window> | <garage>) <area> <zou>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "sentences": [
-                        "schalt <name> un",
-                        "schalt <name> <area> un",
-                        "aktiv\u00e9ier <name>",
-                        "<maach> <area> <name> <op>",
-                        "<maach> <name> <area> <op>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<maach> <area> (<window> | <garage>) <op>",
-                        "<maach> (<window> | <garage>) <area> <op>"
-                    ]
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "<maach> [(all | alleguer)] <light> <area> un",
                         "<maach> [(all | alleguer)] <area> <light> un"
                     ],
                     "slots": {
                         "domain": "light",
@@ -201,14 +185,30 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "schalt <name> un",
+                        "schalt <name> <area> un",
+                        "aktiv\u00e9ier <name>",
+                        "<maach> <area> <name> <op>",
+                        "<maach> <name> <area> <op>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<maach> <area> (<window> | <garage>) <op>",
+                        "<maach> (<window> | <garage>) <area> <op>"
+                    ]
                 }
             ]
         }
     },
     "language": "lb",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/lt.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992443783068783%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {0: {'sentences': ['<turn_on> [visas] "*

 * *              "<brightness_variations> <area>', '<turn_on> [visas] <area> "*

 * *              "<brightness_variations>'], 'slots': OrderedDict([('domain', 'light')]), 'response': "*

 * *              "'lights_area'}, 1: {'sentences': ['<open> (garažo | garaže) (duris | vartus)', "*

 * *              "'(Duris | Vartus) (garažo | garaže) <open>'], 'slots': {'device_class': 'garage', "*

 * *              "'domain': 'cover'}, 'response': 'cover_device_ […]*

```diff
@@ -60,35 +60,14 @@
                     ]
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "lights_area",
-                    "sentences": [
-                        "<turn_off> [visas] \u0161vies(as|\u0105) <area>",
-                        "<turn_off> [visas] <area> \u0161vies(as|\u0105)"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<close> (gara\u017eo | gara\u017ee) (duris | vartus)",
-                        "(Duris | Vartus) (gara\u017eo | gara\u017ee) <close>"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
                     "response": "fans_area",
                     "sentences": [
                         "<turn_off> [visus] ventiliatori(\u0173|us) <area>",
                         "<turn_off> [visus] <area> ventiliatori(\u0173|us)"
                     ],
                     "slots": {
                         "domain": "fan",
@@ -112,71 +91,92 @@
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ]
                     }
+                },
+                {
+                    "response": "lights_area",
+                    "sentences": [
+                        "<turn_off> [visas] \u0161vies(as|\u0105) <area>",
+                        "<turn_off> [visas] <area> \u0161vies(as|\u0105)"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "<close> (gara\u017eo | gara\u017ee) (duris | vartus)",
+                        "(Duris | Vartus) (gara\u017eo | gara\u017ee) <close>"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "lights_area",
                     "sentences": [
-                        "(<turn_on>|<open>) <name>",
-                        "(<turn_on>|<open>) <area> <name>",
-                        "(<turn_on>|<open>) <name> <area>"
-                    ]
+                        "<turn_on> [visas] <brightness_variations> <area>",
+                        "<turn_on> [visas] <area> <brightness_variations>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "(Roletus| U\u017euolaidas | \u017daliuzes) <area> <open>",
-                        "<open> (roletus| u\u017euolaidas | \u017ealiuzes) <area>",
-                        "<open> <area> (roletus| u\u017euolaidas | \u017ealiuzes)"
+                        "<open> (gara\u017eo | gara\u017ee) (duris | vartus)",
+                        "(Duris | Vartus) (gara\u017eo | gara\u017ee) <open>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ]
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area",
                     "sentences": [
                         "<turn_on> [visus] ventiliatori(\u0173|us) <area>",
                         "<turn_on> [visus] <area> ventiliatori(\u0173|us)"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "lights_area",
                     "sentences": [
-                        "<turn_on> [visas] <brightness_variations> <area>",
-                        "<turn_on> [visas] <area> <brightness_variations>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
+                        "(<turn_on>|<open>) <name>",
+                        "(<turn_on>|<open>) <area> <name>",
+                        "(<turn_on>|<open>) <name> <area>"
+                    ]
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover_area",
                     "sentences": [
-                        "<open> (gara\u017eo | gara\u017ee) (duris | vartus)",
-                        "(Duris | Vartus) (gara\u017eo | gara\u017ee) <open>"
+                        "(Roletus| U\u017euolaidas | \u017daliuzes) <area> <open>",
+                        "<open> (roletus| u\u017euolaidas | \u017ealiuzes) <area>",
+                        "<open> <area> (roletus| u\u017euolaidas | \u017ealiuzes)"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ]
                     }
                 }
             ]
         }
     },
     "language": "lt",
     "lists": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6645231064990179%*

 * *Differences: {"'expansion_rules'": "{replace: OrderedDict([('nome', '[(o[s]|a[s])] {name}'), ('zona', "*

 * *                      "'[(o[s]|a[s])] {area}'), ('na_zona', '(n[o|a]|d[a|o]) {area}'), ('ligar', "*

 * *                      "'(liga[r]|ligue|acende[r]|acenda|ativa[r]|ative)'), ('desligar', "*

 * *                      "'(desliga[r]|desligue|apaga[r]|apague|desativa[r]|desative)'), ('abrir', "*

 * *                      "'(abr[a|e]|abrir)'), ('fechar', '(fecha[r]|feche)'), ('mudar', "*

 * *                      "'(pôr|põe|ponha|muda[r] […]*

```diff
@@ -1,297 +1,347 @@
 {
     "expansion_rules": {
-        "area": "{area}",
-        "brightness": "{brightness}[%| procent(i|iem|u|us)]",
-        "close": "(aizver[iet] | nolaist)",
-        "iesl\u0113gt": "(palaid | iesl\u0113gt | iesl\u0113dz | iesl\u0113dziet)",
-        "izsl\u0113gt": "(atsl\u0113gt | atsl\u0113dz | izsl\u0113gt | izsl\u0113dz | izsl\u0113dziet)",
-        "name": "{name}",
-        "open": "(atver | pacel)",
-        "set": "(uzst\u0101di | ieliec[iet] | [(iz|pa)]maini[et] | uzseto)",
-        "temperature": "{temperature}[\u00b0| gr\u0101d(s|u|i|iem)] [p\u0113c] [{temperature_unit}]"
+        "abrir": "(abr[a|e]|abrir)",
+        "brilho": "{brightness}[%| porcento]",
+        "desligar": "(desliga[r]|desligue|apaga[r]|apague|desativa[r]|desative)",
+        "fechar": "(fecha[r]|feche)",
+        "ligar": "(liga[r]|ligue|acende[r]|acenda|ativa[r]|ative)",
+        "mudar": "(p\u00f4r|p\u00f5e|ponha|muda[r]|altera[r]|coloca[r]|deixa[r])",
+        "na_zona": "(n[o|a]|d[a|o]) {area}",
+        "nome": "[(o[s]|a[s])] {name}",
+        "temperatura": "{temperature}[\u00b0| graus] [{temperature_unit}]",
+        "zona": "[(o[s]|a[s])] {area}"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
                     "sentences": [
-                        "<izsl\u0113gt> [visas] (gaismas | lampas) <area>",
-                        "<izsl\u0113gt> [visas] <area> (gaismas | lampas)",
-                        "<izsl\u0113gt> <area> visas (gaismas | lampas)",
-                        "<izsl\u0113gt> [visu] (gaismu | apgaismojumu) <area>",
-                        "<izsl\u0113gt> [visu] <area> (gaismu | apgaismojumu)",
-                        "<izsl\u0113gt> <area> visu (gaismu | apgaismojumu)"
-                    ],
-                    "slots": {
-                        "domain": "light",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<close> [vis(as|us)] gar\u0101\u017e[(a|as|u)] durvis"
-                    ],
-                    "slots": {
-                        "area": "all",
-                        "device_class": "garage",
-                        "domain": "cover",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> [visas] gar\u0101\u017e[(a|as|u)] [durvis] <area>",
-                        "<close> <area> [visas] gar\u0101\u017e[(a|as|u)] [durvis]"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover",
-                        "name": "all"
-                    }
+                        "<desligar> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>"
+                    ]
                 },
                 {
-                    "response": "cover_area",
+                    "response": "lights_area",
                     "sentences": [
-                        "<close> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas) <area>",
-                        "<close> <area> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas)"
+                        "<desligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) <na_zona>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
+                    "response": "light_all",
                     "sentences": [
-                        "<izsl\u0113gt> [visus] ventilatoru[s] <area>",
-                        "<izsl\u0113gt> <area> [visus] ventilatoru[s]",
-                        "<izsl\u0113gt> visus <area> ventilatoru[s]"
+                        "<desligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) [da casa]"
                     ],
                     "slots": {
-                        "domain": "fan",
+                        "area": "all",
+                        "domain": "light",
                         "name": "all"
                     }
-                },
-                {
-                    "sentences": [
-                        "<izsl\u0113gt> <name>",
-                        "<izsl\u0113gt> <area> <name>",
-                        "<izsl\u0113gt> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<close> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> <name> <area>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "lights_area",
                     "sentences": [
-                        "<iesl\u0113gt> <name>",
-                        "<iesl\u0113gt> <area> <name>",
-                        "<iesl\u0113gt> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<open> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<open> <name> <area>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<iesl\u0113gt> [visus] ventilatoru[s] <area>",
-                        "<iesl\u0113gt> <area> [visus] ventilatoru[s]",
-                        "<iesl\u0113gt> [visus] <area> ventilatoru[s]"
+                        "<ligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) <na_zona>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
+                    "response": "light_all",
                     "sentences": [
-                        "<iesl\u0113gt> [visas] (gaismas | lampas) <area>",
-                        "<iesl\u0113gt> [visas] <area> (gaismas | lampas)",
-                        "<iesl\u0113gt> <area> visas (gaismas | lampas)",
-                        "<iesl\u0113gt> [visu] (gaismu | apgaismojumu) <area>",
-                        "<iesl\u0113gt> [visu] <area> (gaismu | apgaismojumu)",
-                        "<iesl\u0113gt> <area> visu (gaismu | apgaismojumu)"
-                    ],
-                    "slots": {
-                        "domain": "light",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<open> [vis(as|us)] gar\u0101\u017e[(a|\u0101|as|i|u)] (durvis | v\u0101rtus)"
+                        "<ligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) [da casa]"
                     ],
                     "slots": {
                         "area": "all",
-                        "device_class": "garage",
-                        "domain": "cover",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<open> [visas] gar\u0101\u017e[(a|\u0101|as|i|u)] [durvis | v\u0101rtus] <area>",
-                        "<open> <area> [visas] gar\u0101\u017e[(a|\u0101|as|i|u)] [durvis | v\u0101rtus]"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover",
+                        "domain": "light",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
                     "sentences": [
-                        "<open> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas) <area>",
-                        "<open> <area> [vis(us|as)] (aizkar(i|us) | \u017eal\u016bzijas)"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
-                        "name": "all"
-                    }
+                        "<ligar> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>"
+                    ]
                 }
             ]
         }
     },
-    "language": "lv",
+    "language": "pt-br",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
+        "brightness_level": {
+            "values": [
+                {
+                    "in": "(m\u00e1xim(o|a) | forte | alt(o|a))",
+                    "out": 100
+                },
+                {
+                    "in": "(m\u00ednim(o|a) | frac(o|a) | baix(o|a))",
+                    "out": 1
+                }
+            ]
+        },
         "color": {
             "values": [
                 {
-                    "in": "balt(s|a|\u0101|o)",
+                    "in": "branco",
                     "out": "white"
                 },
                 {
-                    "in": "meln(s|a|\u0101|o)",
+                    "in": "branca",
+                    "out": "white"
+                },
+                {
+                    "in": "preto",
+                    "out": "black"
+                },
+                {
+                    "in": "preta",
                     "out": "black"
                 },
                 {
-                    "in": "sarkan(s|a|\u0101|o)",
+                    "in": "vermelho",
                     "out": "red"
                 },
                 {
-                    "in": "oran\u017e(s|a|\u0101|o)",
+                    "in": "vermelha",
+                    "out": "red"
+                },
+                {
+                    "in": "laranja",
                     "out": "orange"
                 },
                 {
-                    "in": "dzelten(s|a|\u0101|o)",
+                    "in": "amarelo",
                     "out": "yellow"
                 },
                 {
-                    "in": "za\u013c(\u0161|a|\u0101|o)",
+                    "in": "amarela",
+                    "out": "yellow"
+                },
+                {
+                    "in": "verde",
                     "out": "green"
                 },
                 {
-                    "in": "zil(s|a|\u0101|o)",
+                    "in": "azul",
                     "out": "blue"
                 },
                 {
-                    "in": "violet(s|a|\u0101|o)",
+                    "in": "roxo",
+                    "out": "purple"
+                },
+                {
+                    "in": "roxa",
                     "out": "purple"
                 },
                 {
-                    "in": "br\u016bn(s|a|\u0101|o)",
+                    "in": "castanho",
+                    "out": "brown"
+                },
+                {
+                    "in": "castanha",
+                    "out": "brown"
+                },
+                {
+                    "in": "marrom",
                     "out": "brown"
                 }
             ]
         },
+        "cover_classes": {
+            "values": [
+                {
+                    "in": "awning[s]",
+                    "out": "awning"
+                },
+                {
+                    "in": "persiana[s]",
+                    "out": "blind"
+                },
+                {
+                    "in": "cortina[s]",
+                    "out": "curtain"
+                },
+                {
+                    "in": "porta[s]",
+                    "out": "door"
+                },
+                {
+                    "in": "(porta[s]|port\u00e3o|port\u00f5es) da garagem",
+                    "out": "garage"
+                },
+                {
+                    "in": "(port\u00e3o|port\u00f5es|porteira[s])",
+                    "out": "gate"
+                },
+                {
+                    "in": "shade[s]",
+                    "out": "shade"
+                },
+                {
+                    "in": "shutter[s]",
+                    "out": "shutter"
+                },
+                {
+                    "in": "janela[s]",
+                    "out": "window"
+                }
+            ]
+        },
+        "cover_states": {
+            "values": [
+                {
+                    "in": "(aberto[s]|aberta[s])",
+                    "out": "open"
+                },
+                {
+                    "in": "(fechado[s]|fechada[s])",
+                    "out": "closed"
+                },
+                {
+                    "in": "abrindo",
+                    "out": "opening"
+                },
+                {
+                    "in": "fechando",
+                    "out": "closing"
+                }
+            ]
+        },
+        "lock_states": {
+            "values": [
+                {
+                    "in": "trancada",
+                    "out": "locked"
+                },
+                {
+                    "in": "destrancada",
+                    "out": "unlocked"
+                }
+            ]
+        },
+        "on_off_domains": {
+            "values": [
+                {
+                    "in": "luz[es]",
+                    "out": "light"
+                },
+                {
+                    "in": "ventilador[es]",
+                    "out": "fan"
+                },
+                {
+                    "in": "interruptor[es]",
+                    "out": "switch"
+                }
+            ]
+        },
+        "on_off_states": {
+            "values": [
+                {
+                    "in": "(ligado[s]|ligada[s]|acesa[s]|aceso[s])",
+                    "out": "on"
+                },
+                {
+                    "in": "(desligado[s]|desligada[s]|apagada[s])",
+                    "out": "off"
+                }
+            ]
+        },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 {
-                    "in": "c | celsija | p\u0113c celsija",
+                    "in": "(celsius|c|cent\u00edgrados)",
                     "out": "celsius"
                 },
+                "fahrenheit",
                 {
-                    "in": "f | f\u0101renheita | p\u0113c f\u0101renheita",
+                    "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Apstr\u0101d\u0101jot nol\u016bku, rad\u0101s neparedz\u0113ta k\u013c\u016bda",
-            "no_area": "Nav zonas ar nosaukumu {{ area }}",
-            "no_device_class": "Zon\u0101 {{ area }} nav {{ device_class }}",
-            "no_domain": "Zon\u0101 {{ area }} nav {{ domain }}",
-            "no_entity": "Nav ier\u012bces vai ent\u012btijas ar nosaukumu {{ entity }}",
-            "no_intent": "Atvainojiet, es nevar\u0113ju to saprast"
+            "handle_error": "Um erro inesperado ocorreu ao processar o pedido",
+            "no_area": "N\u00e3o existe nenhuma \u00e1rea chamada {{ area }}",
+            "no_device_class": "{{ area }} n\u00e3o cont\u00e9m {{ device_class }}",
+            "no_domain": "{{ area }} n\u00e3o contem {{ domain }}",
+            "no_entity": "N\u00e3o existe nenhum dispositivo ou entidade com o nome {{ entity }}",
+            "no_intent": "Desculpe, n\u00e3o consegui entender seu pedido"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "Closed {{ slots.name }}",
-                "cover_area": "Closed {{ slots.area }}",
-                "cover_device_class": "Closed {{ slots.device_class }}",
-                "default": "Turned off {{ slots.name }}",
-                "fans_area": "Turned off fans in {{ slots.area }}",
-                "lights_area": "Turned off lights in {{ slots.area }}"
+                "cover": "Fechado",
+                "cover_device_class": "Fechado {{ slots.device_class }}",
+                "default": "{{ slots.name }} desligado",
+                "fan_all": "Todos ventiladores desligados",
+                "fans_area": "Ventiladores desligados",
+                "light_all": "Todas luzes apagadas",
+                "lights_area": "Luzes apagadas",
+                "lock": "Destrancado"
             },
             "HassTurnOn": {
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}",
-                "cover_device_class": "Opened {{ slots.device_class }}",
-                "default": "Turned on {{ slots.name }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "lights_area": "Turned on lights in {{ slots.area }}"
+                "cover": "Aberto",
+                "cover_device_class": "{{ slots.device_class }} aberto",
+                "default": "{{ slots.name }} ligado",
+                "fans_all": "Ligando todos ventiladores",
+                "fans_area": "Ligando ventiladores",
+                "light_all": "Acendendo todas luzes",
+                "lights_area": "Acendendo luzes",
+                "lock": "Trancado",
+                "scene": "Ativando cena {{slots.name}}",
+                "script": "Iniciado {{slots.name}}"
             }
         }
     },
     "skip_words": [
-        "l\u016bdzu",
-        "paldies",
-        "[vai] vari",
-        "ir",
-        "\u0101r\u0101",
-        "va\u013c\u0101"
+        "porfavor",
+        "por favor",
+        "por obsequio",
+        "por obs\u00e9quio",
+        "por gentileza",
+        "pode"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ml.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896660052910052%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {0: {'sentences': ['<turn_on> [<all>] (<light> | <lights>) "*

 * *              "<area><in>', '<turn_on> [<all>] <area>[<in>] (<light> | <lights>)', '<turn> [<all>] "*

 * *              "(<light> | <lights>) <area><in> <_on>'], 'slots': OrderedDict([('domain', "*

 * *              "'light')])}, 1: {'sentences': ['(<open> | ഉയർത്തുക) [<the>] ഗരാജ് വാതിൽ'], "*

 * *              "'response': 'cover_device_class', 'slots': OrderedDict([('device_class', 'garage'), "*

 * *              "('domain', ' […]*

```diff
@@ -31,14 +31,32 @@
         "window": "(\u0d1c\u0d28(\u0d7d|\u0d32\u0d41\u0d15\u0d7e)|\u0d2e\u0d31[\u0d15\u0d7e]|\u0d24\u0d3f\u0d30\u0d36\u0d4d\u0d36\u0d40\u0d32[\u0d15\u0d7e]|\u0d2c\u0d4d\u0d32\u0d48\u0d7b(\u0d21\u0d4d|\u0d21\u0d41\u0d15\u0d7e)|\u0d15\u0d7c\u0d1f\u0d4d\u0d1f(\u0d7b|\u0d28\u0d41\u0d15\u0d7e)|\u0d37\u0d1f\u0d4d\u0d1f(\u0d7c|\u0d31\u0d41\u0d15\u0d7e))"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "<turn_off> [<all>] [<the>] (<fan> | <fans>) [<the>] <area><in>",
+                        "<turn_off> <area>[<in>] (<fan> | <fans>)",
+                        "<turn> [<all>] <area>[<in>] (<fan> | <fans>) <_off>",
+                        "[<the>] <area>[<in>] [<all>] [<the>] (<fan> | <fans>) <turn_off>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<turn_off> [<the>] <name>",
+                        "[<the>] <name> <turn_off>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "<turn_off> [<all>] (<light>|<lights>) [<the>] <area><in>",
                         "<turn_off> [<all>] <area> (<light>|<lights>)",
                         "<turn> [<all>] (<light>|<lights>) <area><in> <_off>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
@@ -86,68 +104,21 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> [<all>] [<the>] (<fan> | <fans>) [<the>] <area><in>",
-                        "<turn_off> <area>[<in>] (<fan> | <fans>)",
-                        "<turn> [<all>] <area>[<in>] (<fan> | <fans>) <_off>",
-                        "[<the>] <area>[<in>] [<all>] [<the>] (<fan> | <fans>) <turn_off>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> [<the>] <name>",
-                        "[<the>] <name> <turn_off>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<turn_on> [<the>] <name>",
-                        "[<the>] <name> <turn_on>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "(<open> | \u0d09\u0d2f\u0d7c\u0d24\u0d4d\u0d24\u0d41\u0d15) <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "(<open> | \u0d09\u0d2f\u0d7c\u0d24\u0d4d\u0d24\u0d41\u0d15) [<the>] <name> <area><in>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<turn_on> [<all>] (<fan>|<fans>) [<the>] <area><in>",
-                        "<turn_on> <area>[<in>] (<fan>|<fans>)",
-                        "<turn> [<all>] <area>[<in>] (<fan>|<fans>) <_on>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
                         "<turn_on> [<all>] (<light> | <lights>) <area><in>",
                         "<turn_on> [<all>] <area>[<in>] (<light> | <lights>)",
                         "<turn> [<all>] (<light> | <lights>) <area><in> <_on>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
@@ -173,14 +144,43 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> [<all>] (<fan>|<fans>) [<the>] <area><in>",
+                        "<turn_on> <area>[<in>] (<fan>|<fans>)",
+                        "<turn> [<all>] <area>[<in>] (<fan>|<fans>) <_on>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> [<the>] <name>",
+                        "[<the>] <name> <turn_on>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "(<open> | \u0d09\u0d2f\u0d7c\u0d24\u0d4d\u0d24\u0d41\u0d15) <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "(<open> | \u0d09\u0d2f\u0d7c\u0d24\u0d4d\u0d24\u0d41\u0d15) [<the>] <name> <area><in>"
+                    ]
                 }
             ]
         }
     },
     "language": "ml",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/mn.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "{{ area }} \u043d\u044d\u0440 \u0430\u043b\u0433\u0430 \u0431\u0430\u0439\u043d\u0430",
             "no_domain": "{{ area }} \u04e9\u0440\u04e9\u04e9\u043d\u0434 {{ domain }} \u0431\u0430\u0439\u0445\u0433\u04af\u0439 \u0431\u0430\u0439\u043d\u0430",
             "no_device_class": "{{ area }} \u04e9\u0440\u04e9\u04e9\u043d\u0434 {{ device_class }} \u043d\u044d\u0440\u0442\u044d\u0439 \u0442\u04e9\u0445\u04e9\u04e9\u0440\u04e9\u043c\u0436 \u0431\u0430\u0439\u0445\u0433\u04af\u0439 \u0431\u0430\u0439\u043d\u0430",
             "no_entity": "\u0422\u0438\u0439\u043c \u043d\u044d\u0440\u0442\u044d\u0439 \u0442\u04e9\u0445\u04e9\u04e9\u0440\u04e9\u043c\u0436 \u0431\u0430\u0439\u0445\u0433\u04af\u0439 \u0431\u0430\u0439\u043d\u0430 {{ entity }}",
             "handle_error": "\u042f\u043c\u0430\u0440 \u043d\u044d\u0433 \u0430\u043b\u0434\u0430\u0430 \u0433\u0430\u0440\u043b\u0430\u0430"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "{{ slots.name }} \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
-                "lights_area": "{{ slots.area }} \u04e9\u0440\u04e9\u04e9\u043d\u0438\u0439 \u0433\u044d\u0440\u043b\u0438\u0439\u0433 \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
-                "fans_area": "{{ slots.area }} \u04e9\u0440\u04e9\u04e9\u043d\u0438\u0439 \u0441\u044d\u043d\u0441\u0438\u0439\u0433 \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
-                "cover": "{{ slots.name }} \u043d\u044d\u044d\u0441\u044d\u043d",
-                "cover_area": "{{ slots.area }} \u043d\u044d\u044d\u0441\u044d\u043d"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "{{ slots.name }} \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
+                "lights_area": "{{ slots.area }} \u04e9\u0440\u04e9\u04e9\u043d\u0438\u0439 \u0433\u044d\u0440\u043b\u0438\u0439\u0433 \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
+                "fans_area": "{{ slots.area }} \u04e9\u0440\u04e9\u04e9\u043d\u0438\u0439 \u0441\u044d\u043d\u0441\u0438\u0439\u0433 \u0430\u0441\u0430\u0430\u0441\u0430\u043d",
+                "cover": "{{ slots.name }} \u043d\u044d\u044d\u0441\u044d\u043d",
+                "cover_area": "{{ slots.area }} \u043d\u044d\u044d\u0441\u044d\u043d"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/tr.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7170066550925925%*

 * *Differences: {"'expansion_rules'": "{'area': '{area}<ismin_halleri>', 'ismin_halleri': "*

 * *                      "'[([(n|ın|in|un|ün|y|t|d|nd|nt)]ı|[(n|ın|in|un|ün|y|t|d|nd|nt)]i|[(n|ın|in|un|ün|y|t|d|nd|nt)]ü|[(n|ın|in|un|ün|y|t|d|nd|nt)]u|[(n|ın|in|un|ün|y|t|d|nd|nt)]e|[(n|ın|in|un|ün|y|t|d|nd|nt)]a)][n][ki]', "*

 * *                      "'cogulluk': '[(ler|leri|lar|ları)]', 'name': "*

 * *                      "'{name}<cogulluk><ismin_halleri>', 'temperature': '{temperature} "*

 * *                      "[{temperature_unit}]', delet […]*

```diff
@@ -1,199 +1,228 @@
 {
     "expansion_rules": {
-        "apakah": "(apa | apakah | apa itu)",
-        "area": "{area}",
-        "berapa": "(berapa | berapakah)",
-        "imp_buka": "(buka | bukakan)",
-        "imp_hidup": "(nyalakan | hidupkan)",
-        "imp_mati": "(padamkan | matikan)",
-        "imp_set": "(tetapkan | setkan | set | jadikan | ubahkan | ubah | tukarkan | tukar)",
-        "imp_tutup": "(tutup | tutupkan)",
-        "kecerahan": "{brightness}[%| peratus]",
-        "nama": "{name}",
-        "suhu": "{temperature}[\u00b0| darjah] [{temperature_unit}]"
+        "area": "{area}<ismin_halleri>",
+        "cogulluk": "[(ler|leri|lar|lar\u0131)]",
+        "ismin_halleri": "[([(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u0131|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]i|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u00fc|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]u|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]e|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]a)][n][ki]",
+        "name": "{name}<cogulluk><ismin_halleri>",
+        "temperature": "{temperature} [{temperature_unit}]"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<imp_mati> [semua] lampu [di] <area>",
-                        "<imp_mati> [semua] lampu <area>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
+                        "<name> (kapa | kapat | s\u00f6nd\u00fcr )"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<name> (kapa | kapat | indir ) "
+                    ]
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<imp_tutup> pagar [di] <area>",
-                        "<imp_tutup> pagar <area>"
+                        "<area> <name> (kapa | kapat | indir )"
+                    ]
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "garaj kap\u0131s\u0131n\u0131 (kapa | kapat | indir )"
                     ],
                     "slots": {
-                        "area": "garaj",
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
+                    "response": "cover_area",
                     "sentences": [
-                        "<imp_mati> [semua] kipas [di] <area>",
-                        "<imp_mati> [semua] kipas <area>"
+                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (kapa | kapat | indir | \u00e7ek)"
                     ],
                     "slots": {
-                        "area": "living_room",
-                        "domain": "fan"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<imp_mati> <nama>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<imp_hidup> <nama>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<imp_hidup> [semua] kipas [di] <area>",
-                        "<imp_hidup> [semua] kipas <area>"
-                    ],
-                    "slots": {
-                        "area": "living_room",
-                        "domain": "fan"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<imp_hidup> [semua] lampu [di] <area>",
-                        "<imp_hidup> [semua] lampu <area>"
+                        "garaj kap\u0131s\u0131n\u0131 (a\u00e7 | y\u00fckselt)"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<imp_buka> [semua] langsir [di] <area>",
-                        "<imp_buka> [semua] langsir <area>"
+                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (a\u00e7 | y\u00fckselt)"
                     ],
                     "slots": {
-                        "area": "living_room",
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<name> ( a\u00e7 | yak | \u00e7al\u0131\u015ft\u0131r)"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<name> (a\u00e7 | y\u00fckselt) "
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<area> <name> (a\u00e7 | y\u00fckselt)"
+                    ]
                 }
             ]
         }
     },
-    "language": "ms",
+    "language": "tr",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "putih",
+                    "in": "beyaz",
                     "out": "white"
                 },
                 {
-                    "in": "hitam",
+                    "in": "siyah",
                     "out": "black"
                 },
                 {
-                    "in": "merah",
+                    "in": "k\u0131rm\u0131z\u0131",
                     "out": "red"
                 },
                 {
-                    "in": "oren",
+                    "in": "turuncu",
                     "out": "orange"
                 },
                 {
-                    "in": "kuning",
+                    "in": "sar\u0131",
                     "out": "yellow"
                 },
                 {
-                    "in": "hijau",
+                    "in": "ye\u015fil",
                     "out": "green"
                 },
                 {
-                    "in": "biru",
+                    "in": "mavi",
                     "out": "blue"
                 },
                 {
-                    "in": "ungu",
+                    "in": "mor",
                     "out": "purple"
                 },
                 {
-                    "in": "perang",
+                    "in": "kahverengi",
                     "out": "brown"
+                },
+                {
+                    "in": "gri",
+                    "out": "grey"
+                },
+                {
+                    "in": "pembe",
+                    "out": "pink"
+                },
+                {
+                    "in": "turkuaz",
+                    "out": "turquoise"
+                },
+                {
+                    "in": "bordo",
+                    "out": "maroon"
+                },
+                {
+                    "in": "bej",
+                    "out": "beige"
+                },
+                {
+                    "in": "lacivert",
+                    "out": "navy"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 "celsius",
                 {
-                    "in": "c",
+                    "in": "c | santigrat",
                     "out": "celsius"
+                },
+                "fahrenheit",
+                {
+                    "in": "f | fahrenhayt",
+                    "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Maaf, berlaku ralat semasa intent sedang dijalankan",
-            "no_area": "Tiada {{ area }} dijumpai",
-            "no_device_class": "{{ device_class }} tiada di {{ area }}",
-            "no_domain": "{{ domain }} tiada di {{ area }}",
-            "no_entity": "Peranti atau entiti {{ entity }} tidak ditemui",
-            "no_intent": "Maaf, saya tidak faham arahan anda"
+            "handle_error": "\u0130stenilen ama\u00e7 i\u015flenirken bir hata olu\u015ftu.",
+            "no_area": "{{ area }}  ad\u0131nda alan yok.",
+            "no_device_class": "{{ area }}  bir {{ device_class }} i\u00e7ermiyor.",
+            "no_domain": "{{ area }}  bir {{ domain }} i\u00e7ermiyor.",
+            "no_entity": "{{ entity }} ad\u0131nda bir cihaz yok.",
+            "no_intent": "\u00dczg\u00fcn\u00fcm, bunu anlayamad\u0131m."
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "{{ slots.name }} telah ditutupkan",
-                "cover_area": "Kawasan {{ slots.area }} telah ditutupkan",
-                "default": "{{ slots.name }} telah dimatikan",
-                "fans_area": "Semua kipas [di] {{ slots.area }} telah dimatikan",
-                "lights_area": "Semua lampu [di] {{ slots.area }} telah dipadamkan"
+                "cover": "Closed {{ slots.name }}",
+                "cover_area": "Closed {{ slots.area }}",
+                "cover_device_class": "Closed {{ slots.device_class }}",
+                "default": "Turned off {{ slots.name }}",
+                "fans_area": "Turned off fans in {{ slots.area }}",
+                "lights_area": "Turned off lights in {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} telah dibuka",
-                "cover_area": "Kawasan {{ slots.area }} telah dibuka",
-                "default": "{{ slots.name }} telah dihidupkan",
-                "fans_area": "Semua kipas [di] {{ slots.area }} telah dihidupkan",
-                "lights_area": "Semua lampu [di] {{ slots.area }} telah dinyalakan"
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}",
+                "cover_device_class": "Opened {{ slots.device_class }}",
+                "default": "Turned on {{ slots.name }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "lights_area": "Turned on lights in {{ slots.area }}"
             }
         }
     },
     "skip_words": [
-        "tolong",
-        "boleh tak",
-        "cuba"
+        "L\u00fctfen"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nb.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.988936988936989%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(11, OrderedDict([('sentences', ['er <navn> "*

 * *              "{lock_states:state} [<i_på> <område>]']), ('response', 'one_yesno'), "*

 * *              "('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])), (12, OrderedDict([('sentences', ['er noen "*

 * *              "<dør> {lock_states:state} [<i_på> <område>]']), ('response', 'any'), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))]) […]*

```diff
@@ -31,62 +31,14 @@
         "\u00e5pen": "(\u00e5pen|\u00e5pnet [opp]|rullet opp|lukket opp)",
         "\u00e5pne": "(\u00e5pne [opp]|heis [opp]|lukk opp|rull opp)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "er <navn> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "er noen <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "er <alle> <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "<hvilke> <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "hvor mange <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "response": "one",
                     "sentences": [
                         "hva er [<tilstand>] [til] <navn> [<i_p\u00e5> <omr\u00e5de>]"
                     ]
                 },
                 {
                     "excludes_context": {
@@ -168,68 +120,67 @@
                     "response": "how_many",
                     "sentences": [
                         "hvor mange {cover_classes:device_class} er {cover_states:state} [<i_p\u00e5> <omr\u00e5de>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                }
-            ]
-        },
-        "HassTurnOff": {
-            "data": [
+                },
                 {
-                    "response": "lights_area",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
                     "sentences": [
-                        "<skru_av> [<alle>] <lys> [<i_p\u00e5>] <omr\u00e5de>",
-                        "<skru_av> [<alle>] <omr\u00e5de>[s][ ]<lys>",
-                        "<skru_av> <omr\u00e5de> [<alle>] <lys>"
+                        "er <navn> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
                     ],
                     "slots": {
-                        "domain": "light",
-                        "name": "all"
+                        "domain": "lock"
                     }
                 },
                 {
+                    "response": "any",
                     "sentences": [
-                        "<skru_av> <lys> <navn>"
+                        "er noen <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
+                    "response": "all",
                     "sentences": [
-                        "<lukk> <navn> [<i_p\u00e5> <omr\u00e5de>]"
-                    ]
+                        "er <alle> <d\u00f8r> {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "which",
                     "sentences": [
-                        "<lukk> <garasje>"
+                        "<hvilke> <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "how_many",
                     "sentences": [
-                        "<lukk> {cover_classes:device_class} <i_p\u00e5> <omr\u00e5de>",
-                        "<lukk> <omr\u00e5de>[s][ ]{cover_classes:device_class}"
+                        "hvor mange <d\u00f8r> er {lock_states:state} [<i_p\u00e5> <omr\u00e5de>]"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "lock"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOff": {
+            "data": [
                 {
                     "sentences": [
                         "<skru_av> [<alle>] <vifte> <i_p\u00e5> <omr\u00e5de>",
                         "<skru_av> [<alle>] <omr\u00e5de> <vifte>"
                     ],
                     "slots": {
                         "domain": "fan",
@@ -252,60 +203,78 @@
                             "lock"
                         ]
                     },
                     "sentences": [
                         "<lukk> <navn>",
                         "<lukk> <navn> <i_p\u00e5> <omr\u00e5de>"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                },
                 {
-                    "requires_context": {
-                        "domain": "scene"
-                    },
-                    "response": "scene",
+                    "response": "lights_area",
                     "sentences": [
-                        "<aktiver> <navn>[s][modus]"
+                        "<skru_av> [<alle>] <lys> [<i_p\u00e5>] <omr\u00e5de>",
+                        "<skru_av> [<alle>] <omr\u00e5de>[s][ ]<lys>",
+                        "<skru_av> <omr\u00e5de> [<alle>] <lys>"
                     ],
                     "slots": {
-                        "domain": "scene"
+                        "domain": "light",
+                        "name": "all"
                     }
                 },
                 {
                     "sentences": [
-                        "<skru_p\u00e5> <navn>",
-                        "(skru|sl\u00e5) <navn> p\u00e5"
-                    ]
+                        "<skru_av> <lys> <navn>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "scene",
-                            "sensor",
-                            "script",
-                            "lock"
-                        ]
+                    "requires_context": {
+                        "domain": "cover"
                     },
+                    "response": "cover",
                     "sentences": [
-                        "<\u00e5pne> <navn>",
-                        "<\u00e5pne> <navn> <i_p\u00e5> <omr\u00e5de>"
+                        "<lukk> <navn> [<i_p\u00e5> <omr\u00e5de>]"
                     ]
                 },
                 {
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<skru_p\u00e5> [<alle>] <vifte> <i_p\u00e5> <omr\u00e5de>",
-                        "<skru_p\u00e5> [<alle>] <omr\u00e5de> <vifte>"
+                        "<lukk> <garasje>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "<lukk> {cover_classes:device_class} <i_p\u00e5> <omr\u00e5de>",
+                        "<lukk> <omr\u00e5de>[s][ ]{cover_classes:device_class}"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
+                    "sentences": [
+                        "<aktiver> <navn>[s][modus]"
+                    ],
+                    "slots": {
+                        "domain": "scene"
                     }
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
                         "<skru_p\u00e5> [<alle>] <lys> [<i_p\u00e5>] <omr\u00e5de>",
                         "<skru_p\u00e5> [<alle>] <omr\u00e5de>[s][ ]<lys>",
@@ -322,26 +291,14 @@
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
-                    "sentences": [
-                        "(<aktiver>|<skru_p\u00e5>) <navn> [skript]"
-                    ],
-                    "slots": {
-                        "domain": "script"
-                    }
-                },
-                {
-                    "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
                         "<\u00e5pne> <navn> [<i_p\u00e5> <omr\u00e5de>]"
                     ]
                 },
@@ -360,14 +317,57 @@
                     "sentences": [
                         "<\u00e5pne> {cover_classes:device_class} <i_p\u00e5> <omr\u00e5de>",
                         "<\u00e5pne> <omr\u00e5de>[s][ ]{cover_classes:device_class}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<skru_p\u00e5> [<alle>] <vifte> <i_p\u00e5> <omr\u00e5de>",
+                        "<skru_p\u00e5> [<alle>] <omr\u00e5de> <vifte>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "(<aktiver>|<skru_p\u00e5>) <navn> [skript]"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<skru_p\u00e5> <navn>",
+                        "(skru|sl\u00e5) <navn> p\u00e5"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "scene",
+                            "sensor",
+                            "script",
+                            "lock"
+                        ]
+                    },
+                    "sentences": [
+                        "<\u00e5pne> <navn>",
+                        "<\u00e5pne> <navn> <i_p\u00e5> <omr\u00e5de>"
+                    ]
                 }
             ]
         }
     },
     "language": "nb",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/nl.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922691993464051%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(70, OrderedDict([('sentences', ['<is> [<in> "*

 * *              '<area>] [de [huidige] [(status|staat|stand) van]] <name> [<in> <area>] '*

 * *              "{lock_states:state} [<in> <area>]']), ('response', 'one_yesno'), "*

 * *              "('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])), (71, OrderedDict([('sentences', ['<is> er "*

 * *              "[<in> <area>] <slot> [<in> <area>] {lock_states […]*

```diff
@@ -40,65 +40,14 @@
         "zou": "(kan|kun[t]|zal|zou|wil[t]) [je|jij|u]"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "<is> [<in> <area>] [de [huidige] [(status|staat|stand) van]] <name> [<in> <area>] {lock_states:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "<is> er [<in> <area>] <slot> [<in> <area>] {lock_states:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "<is> [<in> <area>] [<alle>] <slot> [<in> <area>] {lock_states:state} [<in> <area>]",
-                        "<is> [<in> <area>] [<alle>] [de] deur[en] [<in> <area>] {door_lock_states:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "Welk[e] <slot> [<in> <area>] <is> [<in> <area>] {lock_states:state} [<in> <area>]",
-                        "Welk[e] deur[en] [<in> <area>] <is> [<in> <area>] {door_lock_states:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "Hoe[ ]veel <slot> <is> [er] [<in> <area>] {lock_states:state} [<in> <area>]",
-                        "Hoe[ ]veel deur[en] <is> [er] [<in> <area>] {door_lock_states:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "requires_context": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     },
                     "response": "bs_yesno",
                     "sentences": [
                         "<is> [de] [batterij[status]] [van] [<in> <area>][ ]<name>[ ][batterij] [<in> <area>] {bs_battery_states:state} [<in> <area>]"
                     ],
@@ -1009,20 +958,107 @@
                     "response": "how_many",
                     "sentences": [
                         "Hoe[ ]veel {cover_classes:device_class} [<in> <area>] <is> [er] [<in> <area>] {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "<is> [<in> <area>] [de [huidige] [(status|staat|stand) van]] <name> [<in> <area>] {lock_states:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "<is> er [<in> <area>] <slot> [<in> <area>] {lock_states:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "<is> [<in> <area>] [<alle>] <slot> [<in> <area>] {lock_states:state} [<in> <area>]",
+                        "<is> [<in> <area>] [<alle>] [de] deur[en] [<in> <area>] {door_lock_states:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "Welk[e] <slot> [<in> <area>] <is> [<in> <area>] {lock_states:state} [<in> <area>]",
+                        "Welk[e] deur[en] [<in> <area>] <is> [<in> <area>] {door_lock_states:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "Hoe[ ]veel <slot> <is> [er] [<in> <area>] {lock_states:state} [<in> <area>]",
+                        "Hoe[ ]veel deur[en] <is> [er] [<in> <area>] {door_lock_states:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] uit [[willen|kunnen] <doe>] <in> <area>",
+                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] uit [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] uit [[willen|kunnen] <doe>]",
+                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fan_all",
+                    "sentences": [
+                        "[<doe>|<zou>] ((overal|<alle>) <ventilator>|<ventilator> overal) uit [[willen|kunnen] <doe>]"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] uit [[willen|kunnen] <doe>]",
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "[<doe>|<zou>] [<alle>] <lamp> [<naar>] uit [[willen|kunnen] <doe>] <in> <area>",
                         "[<doe>|<zou>] [<alle>] <lamp> <in> <area> [<naar>] uit [[willen|kunnen] <doe>]",
                         "[<doe>|<zou>] [(<alle>|<in>)] <area>[ ]<lamp> [<naar>] uit [[willen|kunnen] <doe>]",
                         "[<zou>] [(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
                     ],
@@ -1138,50 +1174,14 @@
                         "<zou> [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>) [willen|kunnen] openen",
                         "<zou> [<alle>] <slot> [willen|kunnen] openen <in> <area>"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] uit [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fan_all",
-                    "sentences": [
-                        "[<doe>|<zou>] ((overal|<alle>) <ventilator>|<ventilator> overal) uit [[willen|kunnen] <doe>]"
-                    ],
-                    "slots": {
-                        "area": "all",
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "script"
-                        ]
-                    },
-                    "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "requires_context": {
@@ -1194,79 +1194,14 @@
                         "[<zou>] <name>[ ][scene|sc\u00e8ne] [willen|kunnen] (aan[ ]zetten|inschakelen|starten|activeren)"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "scene",
-                            "script"
-                        ]
-                    },
-                    "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
-                        "schakel <name>[ ][<type>] [<naar>] in",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock",
-                    "sentences": [
-                        "[<doe>|<zou>] <name_area> <op_slot> [[willen|kunnen] <doe>] [<in> <area>]",
-                        "vergrendel <name_area>",
-                        "<zou> <name_area> [willen|kunnen] vergrendelen [<in> <area>]",
-                        "[<doe>|<zou>] <slot_name_area> dicht [[willen|kunnen] <doe>] [<in> <area>]",
-                        "sluit <slot_name_area>",
-                        "<zou> <slot_name_area> [willen|kunnen] sluiten [<in> <area>]"
-                    ]
-                },
-                {
-                    "response": "lock_area",
-                    "sentences": [
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <in> <area> <op_slot> [[willen|kunnen] <doe>]",
-                        "vergrendel [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>)",
-                        "<zou> [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>) [willen|kunnen] vergrendelen",
-                        "<zou> [<alle>] (<slot>|deur[en]) [willen|kunnen] vergrendelen <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <in> <area>[ |<alle>]<slot> dicht [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> <in> <area> dicht [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> dicht [[willen|kunnen] <doe>] <in> <area>",
-                        "sluit [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>)",
-                        "<zou> [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>) [willen|kunnen] sluiten",
-                        "<zou> [<alle>] <slot> [willen|kunnen] sluiten <in> <area>"
-                    ],
-                    "slots": {
-                        "domain": "lock",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] aan [[willen|kunnen] <doe>] <in> <area>",
-                        "Schakel [<alle>] <ventilator> [<naar>] in <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] aan [[willen|kunnen] <doe>]",
-                        "Schakel [<alle>] <ventilator> <in> <area> [<naar>] in",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] aan [[willen|kunnen] <doe>]",
-                        "Schakel [(<alle>|<in>)] <area>[ ]<ventilator> [<naar>] in",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "[<doe>|<zou>] [<alle>] <lamp> [<naar>] aan [[willen|kunnen] <doe>] (in|op) <area>",
                         "Schakel [<alle>] <lamp> [<naar>] in (in|op) <area>",
                         "[<doe>|<zou>] [<alle>] <lamp> <in> <area> [<naar>] aan [[willen|kunnen] <doe>]",
                         "Schakel [<alle>] <lamp> <in> <area> in",
                         "[<doe>|<zou>] [(<alle>|<in>)] <area>[ ]<lamp> aan [[willen|kunnen] <doe>]",
@@ -1275,28 +1210,14 @@
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
-                    "sentences": [
-                        "(activeer|start|schakel) [script] <name>[ ][script] [<naar>] [in]",
-                        "[<doe>|<zou>] [script] <name>[ ][script] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
-                        "[<zou>] <name>[ ][script] [willen|kunnen] (aan[ ]zetten|inschakelen|starten|activeren)"
-                    ],
-                    "slots": {
-                        "domain": "script"
-                    }
-                },
-                {
                     "response": "cover",
                     "sentences": [
                         "open <name>",
                         "[<doe>|<zou>] <name> <open> [[willen|kunnen] <doe>]"
                     ],
                     "slots": {
                         "domain": "cover"
@@ -1353,14 +1274,93 @@
                         "device_class": [
                             "blind",
                             "shutter",
                             "shade"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] aan [[willen|kunnen] <doe>] <in> <area>",
+                        "Schakel [<alle>] <ventilator> [<naar>] in <in> <area>",
+                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] aan [[willen|kunnen] <doe>]",
+                        "Schakel [<alle>] <ventilator> <in> <area> [<naar>] in",
+                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] aan [[willen|kunnen] <doe>]",
+                        "Schakel [(<alle>|<in>)] <area>[ ]<ventilator> [<naar>] in",
+                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "[<doe>|<zou>] <name_area> <op_slot> [[willen|kunnen] <doe>] [<in> <area>]",
+                        "vergrendel <name_area>",
+                        "<zou> <name_area> [willen|kunnen] vergrendelen [<in> <area>]",
+                        "[<doe>|<zou>] <slot_name_area> dicht [[willen|kunnen] <doe>] [<in> <area>]",
+                        "sluit <slot_name_area>",
+                        "<zou> <slot_name_area> [willen|kunnen] sluiten [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "lock_area",
+                    "sentences": [
+                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>] <in> <area>",
+                        "[<doe>|<zou>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <in> <area> <op_slot> [[willen|kunnen] <doe>]",
+                        "vergrendel [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>)",
+                        "<zou> [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>) [willen|kunnen] vergrendelen",
+                        "<zou> [<alle>] (<slot>|deur[en]) [willen|kunnen] vergrendelen <in> <area>",
+                        "[<doe>|<zou>] [<alle>] <in> <area>[ |<alle>]<slot> dicht [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] [<alle>] <slot> <in> <area> dicht [[willen|kunnen] <doe>]",
+                        "[<doe>|<zou>] [<alle>] <slot> dicht [[willen|kunnen] <doe>] <in> <area>",
+                        "sluit [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>)",
+                        "<zou> [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>) [willen|kunnen] sluiten",
+                        "<zou> [<alle>] <slot> [willen|kunnen] sluiten <in> <area>"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "(activeer|start|schakel) [script] <name>[ ][script] [<naar>] [in]",
+                        "[<doe>|<zou>] [script] <name>[ ][script] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
+                        "[<zou>] <name>[ ][script] [willen|kunnen] (aan[ ]zetten|inschakelen|starten|activeren)"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "sentences": [
+                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
+                        "schakel <name>[ ][<type>] [<naar>] in",
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
+                    ]
                 }
             ]
         }
     },
     "language": "nl",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pl.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99095733709449%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(17, OrderedDict([('sentences', ['czy <name> są "*

 * *              "{lock_states:state} [<area>]']), ('requires_context', OrderedDict([('domain', "*

 * *              "'lock')])), ('slots', OrderedDict([('domain', 'lock')])), ('response', "*

 * *              "'one_yesno')])), (18, OrderedDict([('sentences', ['czy są "*

 * *              '[jakieś|któreś|jakiekolwiek|którekolwiek] (drzwi|zamki) {lock_states:state} '*

 * *              "[<area>]', 'czy są [jakieś|któreś|jakiekolwie […]*

```diff
@@ -23,64 +23,14 @@
         "unlock": "odblokuj",
         "what_is": "Jak[a|i] jest"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "czy <name> s\u0105 {lock_states:state} [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] (drzwi|zamki) {lock_states:state} [<area>]",
-                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] {lock_states:state} (drzwi|zamki) [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "czy <all> (drzwi|zamki) s\u0105 {lock_states:state} [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "kt\u00f3re (drzwi|zamki) s\u0105 {lock_states:state} [<area>]",
-                        "kt\u00f3ry zamek jest {lock_states:state} [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "ile (drzwi|zamk\u00f3w) jest {lock_states:state} [<area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "one",
@@ -266,20 +216,119 @@
                     "sentences": [
                         "ile (rolet|\u017caluzji|zas\u0142on) jest {cover_states:state} [<area>]",
                         "ile {cover_classes:device_class} jest {cover_states:state} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "czy <name> s\u0105 {lock_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] (drzwi|zamki) {lock_states:state} [<area>]",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] {lock_states:state} (drzwi|zamki) [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "czy <all> (drzwi|zamki) s\u0105 {lock_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "kt\u00f3re (drzwi|zamki) s\u0105 {lock_states:state} [<area>]",
+                        "kt\u00f3ry zamek jest {lock_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "ile (drzwi|zamk\u00f3w) jest {lock_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fan_area",
+                    "sentences": [
+                        "<turn_off> (wentylator|wiatrak) <area>",
+                        "<turn_off> <area> (wentylator|wiatrak)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_off> [<all>] (wentylatory|wiatraki) <area>",
+                        "<turn_off> <area> [<all>] (wentylatory|wiatraki)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_all",
+                    "sentences": [
+                        "<turn_off> <all> (wentylatory|wiatraki)"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "response": "default",
+                    "sentences": [
+                        "(<turn_off>|<turn_off_light>) <name>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "(<turn_off>|<turn_off_light>) [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o] <area>",
                         "(<turn_off>|<turn_off_light>) <area> [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o]"
                     ],
                     "slots": {
                         "domain": "light"
@@ -411,63 +460,14 @@
                         "<open> <area> [<all>] zamki",
                         "<area> <open> [<all>] zamki"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
-                {
-                    "response": "fan_area",
-                    "sentences": [
-                        "<turn_off> (wentylator|wiatrak) <area>",
-                        "<turn_off> <area> (wentylator|wiatrak)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_off> [<all>] (wentylatory|wiatraki) <area>",
-                        "<turn_off> <area> [<all>] (wentylatory|wiatraki)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "fans_all",
-                    "sentences": [
-                        "<turn_off> <all> (wentylatory|wiatraki)"
-                    ],
-                    "slots": {
-                        "area": "all",
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
-                    "response": "default",
-                    "sentences": [
-                        "(<turn_off>|<turn_off_light>) <name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "requires_context": {
@@ -478,89 +478,82 @@
                         "[<activate>|<turn_on>] scen\u0119 <name>"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
-                    "response": "default",
+                    "response": "lights_area",
                     "sentences": [
-                        "(<turn_on>|<turn_on_light>) <name>"
-                    ]
+                        "(<turn_on>|<turn_on_light>) [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o] <area>",
+                        "(<turn_on>|<turn_on_light>) <area> [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o]"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "lock_lock_door",
+                    "response": "light_all",
                     "sentences": [
-                        "<lock> <name> [<area>]"
-                    ]
+                        "(<turn_on>|<turn_on_light>) <all> \u015bwiat\u0142a"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "light",
+                        "name": "all"
+                    }
                 },
                 {
                     "requires_context": {
-                        "domain": "lock"
+                        "domain": "cover"
                     },
-                    "response": "lock_close_door",
+                    "response": "cover",
                     "sentences": [
-                        "<close> <name> [<area>]"
+                        "(<open>|<open_blind>) <name>"
                     ]
                 },
                 {
-                    "response": "lock_lock_door",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_area_blind",
                     "sentences": [
-                        "<lock> [<all>] drzwi <area>",
-                        "<lock> <area> [<all>] drzwi"
-                    ],
-                    "slots": {
-                        "domain": "lock",
-                        "name": "all"
-                    }
+                        "(<open>|<open_blind>) <name> <area>"
+                    ]
                 },
                 {
-                    "response": "lock_lock_lock",
+                    "response": "cover_garage",
                     "sentences": [
-                        "<lock> [<all>] zamki <area>",
-                        "<lock> <area> [<all>] zamki"
+                        "<open> gara\u017c",
+                        "<open> (drzwi|bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu)",
+                        "(Drzwi|Bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu) <open>"
                     ],
                     "slots": {
-                        "domain": "lock",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "lock_close_door",
+                    "response": "cover_blind",
                     "sentences": [
-                        "<close> [<all>] drzwi <area>",
-                        "<close> <area> [<all>] drzwi"
+                        "(<open>|<open_blind>) [<all>] rolety"
                     ],
                     "slots": {
-                        "domain": "lock",
-                        "name": "all"
+                        "device_class": "curtain",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "lock_close_lock",
+                    "response": "cover_area_blinds",
                     "sentences": [
-                        "<close> [<all>] zamki <area>",
-                        "<close> <area> [<all>] zamki"
+                        "(<open>|<open_blind>) [<all>] rolety <area>",
+                        "(<open>|<open_blind>) <area> [<all>] rolety"
                     ],
                     "slots": {
-                        "domain": "lock",
-                        "name": "all"
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "fan_area",
                     "sentences": [
                         "<turn_on> (wentylator|wiatrak) <area>",
                         "<turn_on> <area> (wentylator|wiatrak)"
@@ -589,95 +582,102 @@
                     "slots": {
                         "area": "all",
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "lights_area",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock_lock_door",
                     "sentences": [
-                        "(<turn_on>|<turn_on_light>) [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o] <area>",
-                        "(<turn_on>|<turn_on_light>) <area> [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o]"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
+                        "<lock> <name> [<area>]"
+                    ]
                 },
                 {
-                    "response": "light_all",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock_close_door",
                     "sentences": [
-                        "(<turn_on>|<turn_on_light>) <all> \u015bwiat\u0142a"
+                        "<close> <name> [<area>]"
+                    ]
+                },
+                {
+                    "response": "lock_lock_door",
+                    "sentences": [
+                        "<lock> [<all>] drzwi <area>",
+                        "<lock> <area> [<all>] drzwi"
                     ],
                     "slots": {
-                        "area": "all",
-                        "domain": "light",
+                        "domain": "lock",
                         "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "script"
-                    },
-                    "response": "script",
+                    "response": "lock_lock_lock",
                     "sentences": [
-                        "[<turn_on>] skrypt <name>"
+                        "<lock> [<all>] zamki <area>",
+                        "<lock> <area> [<all>] zamki"
                     ],
                     "slots": {
-                        "domain": "script"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
-                    "sentences": [
-                        "(<open>|<open_blind>) <name>"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover_area_blind",
-                    "sentences": [
-                        "(<open>|<open_blind>) <name> <area>"
-                    ]
-                },
-                {
-                    "response": "cover_garage",
+                    "response": "lock_close_door",
                     "sentences": [
-                        "<open> gara\u017c",
-                        "<open> (drzwi|bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu)",
-                        "(Drzwi|Bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu) <open>"
+                        "<close> [<all>] drzwi <area>",
+                        "<close> <area> [<all>] drzwi"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_blind",
+                    "response": "lock_close_lock",
                     "sentences": [
-                        "(<open>|<open_blind>) [<all>] rolety"
+                        "<close> [<all>] zamki <area>",
+                        "<close> <area> [<all>] zamki"
                     ],
                     "slots": {
-                        "device_class": "curtain",
-                        "domain": "cover"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area_blinds",
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
                     "sentences": [
-                        "(<open>|<open_blind>) [<all>] rolety <area>",
-                        "(<open>|<open_blind>) <area> [<all>] rolety"
+                        "[<turn_on>] skrypt <name>"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "script"
                     }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "response": "default",
+                    "sentences": [
+                        "(<turn_on>|<turn_on_light>) <name>"
+                    ]
                 }
             ]
         }
     },
     "language": "pl",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/pt.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920634920634921%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(3, OrderedDict([('sentences', ['(liga | ligue | "*

 * *              "ligar) [todas] as ventoinhas <na_zona>']), ('slots', OrderedDict([('domain', "*

 * *              "'fan'), ('name', 'all')])), ('response', 'fans_area')])), (4, "*

 * *              "OrderedDict([('sentences', ['<liga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] "*

 * *              "<nome>', '<liga> <nome>']), ('excludes_context', OrderedDict([('domain', "*

 * *              "['binary_sensor', 'cover', 'lock',  […]*

```diff
@@ -112,14 +112,39 @@
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "(desliga | desligue | desligar) [todas] as ventoinhas <na_zona>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<desliga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>",
+                        "<desliga> <nome>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "<desliga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) <na_zona>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
@@ -141,71 +166,20 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "(desliga | desligue | desligar) [todas] as ventoinhas <na_zona>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
-                    "sentences": [
-                        "<desliga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>",
-                        "<desliga> <nome>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
-                    "sentences": [
-                        "<liga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>",
-                        "<liga> <nome>"
-                    ]
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "(liga | ligue | ligar) [todas] as ventoinhas <na_zona>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "sentences": [
                         "<liga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) <na_zona>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
@@ -228,14 +202,40 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "(liga | ligue | ligar) [todas] as ventoinhas <na_zona>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<liga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>",
+                        "<liga> <nome>"
+                    ]
                 }
             ]
         }
     },
     "language": "pt",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ro.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9899290524290524%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(40, OrderedDict([('sentences', ['<name> [<din> "*

 * *              "<area>] e[ste] {on_off_states_singular:state}', 'e[ste] "*

 * *              "{on_off_states_singular:state} <name> [<din> <area>]']), ('response', 'one_yesno'), "*

 * *              "('requires_context', OrderedDict([('domain', 'light')]))])), (41, "*

 * *              "OrderedDict([('sentences', ['(e[ste] | exist(ă|a)) [<vreun>] <lumina> "*

 * *              "{on_off_states_singular:state} [<in> <area>]', '(sun […]*

```diff
@@ -58,115 +58,14 @@
         "vreun": "(vre(o|un))"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "<name> [<din> <area>] e[ste] {on_off_states_singular:state}",
-                        "e[ste] {on_off_states_singular:state} <name> [<din> <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "any",
-                    "sentences": [
-                        "(e[ste] | exist(\u0103|a)) [<vreun>] <lumina> {on_off_states_singular:state} [<in> <area>]",
-                        "(sunt | exist(\u0103|a)) <luminile> {on_off_states_plural:state} [<in> <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "all",
-                    "sentences": [
-                        "sunt toate <luminile> {on_off_states_plural:state} [<in> <area>]",
-                        "toate <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "which",
-                    "sentences": [
-                        "<care> <lumina> e[ste] {on_off_states_singular:state} [<in> <area>]",
-                        "<care> <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "light"
-                    },
-                    "response": "how_many",
-                    "sentences": [
-                        "<cate> <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
-                    ]
-                },
-                {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "<name> [<din> <area>] e[ste] {lock_states_singular:state}",
-                        "e[ste] {lock_states_singular:state} <name> [<din> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "(e[ste] | exist(\u0103|a)) [<vreun>] <usa> {lock_states_singular:state} [<in> <area>]",
-                        "(sunt | exist(\u0103|a)) <usile> {lock_states_plural:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "sunt toate <usile> {lock_states_plural:state} [<in> <area>]",
-                        "toate <usile> sunt {lock_states_plural:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "<care> <usa> e[ste] {lock_states_singular:state} [<in> <area>]",
-                        "<care> <usile> sunt {lock_states_plural:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "<cate> <usile> sunt {lock_states_plural:state} [<in> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "requires_context": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     },
                     "response": "one_yesno",
                     "sentences": [
                         "[bateria [<din>]] <name> [<din> <area>] e[ste] {bs_battery_states_singular:state}",
                         "e[ste] {bs_battery_states_singular:state} [bateria [<din>]] <name> [<din> <area>]"
@@ -760,71 +659,120 @@
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "how_many",
                     "sentences": [
                         "<cate> {cover_classes_plural:device_class} sunt {cover_states_plural:state} [<in> <area>]"
                     ]
-                }
-            ]
-        },
-        "HassTurnOff": {
-            "data": [
+                },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
-                    "response": "light",
+                    "response": "one_yesno",
                     "sentences": [
-                        "<opreste> <name>"
+                        "<name> [<din> <area>] e[ste] {on_off_states_singular:state}",
+                        "e[ste] {on_off_states_singular:state} <name> [<din> <area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "any",
+                    "sentences": [
+                        "(e[ste] | exist(\u0103|a)) [<vreun>] <lumina> {on_off_states_singular:state} [<in> <area>]",
+                        "(sunt | exist(\u0103|a)) <luminile> {on_off_states_plural:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "all",
+                    "sentences": [
+                        "sunt toate <luminile> {on_off_states_plural:state} [<in> <area>]",
+                        "toate <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "which",
+                    "sentences": [
+                        "<care> <lumina> e[ste] {on_off_states_singular:state} [<in> <area>]",
+                        "<care> <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "how_many",
+                    "sentences": [
+                        "<cate> <luminile> sunt {on_off_states_plural:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "<name> [<din> <area>] e[ste] {lock_states_singular:state}",
+                        "e[ste] {lock_states_singular:state} <name> [<din> <area>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "lights_area",
+                    "response": "any",
                     "sentences": [
-                        "<opreste> (<lumina> | [toate] <luminile>) [<din>] <area>",
-                        "<opreste> [<din>] <area> (<lumina> | [toate] <luminile>)"
+                        "(e[ste] | exist(\u0103|a)) [<vreun>] <usa> {lock_states_singular:state} [<in> <area>]",
+                        "(sunt | exist(\u0103|a)) <usile> {lock_states_plural:state} [<in> <area>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "requires_context": {
-                        "area": null
-                    },
-                    "response": "lights_area",
+                    "response": "all",
                     "sentences": [
-                        "<opreste> (<lumina> | [toate] <luminile>)"
+                        "sunt toate <usile> {lock_states_plural:state} [<in> <area>]",
+                        "toate <usile> sunt {lock_states_plural:state} [<in> <area>]"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
-                    },
-                    "response": "cover",
+                    "response": "which",
                     "sentences": [
-                        "<inchide> <name> [[<din>] <area>]"
-                    ]
+                        "<care> <usa> e[ste] {lock_states_singular:state} [<in> <area>]",
+                        "<care> <usile> sunt {lock_states_plural:state} [<in> <area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 },
                 {
-                    "response": "covers_area",
+                    "response": "how_many",
                     "sentences": [
-                        "<inchide> ({cover_classes_singular:device_class} | [toate] {cover_classes_plural:device_class}) [<din>] <area>"
+                        "<cate> <usile> sunt {lock_states_plural:state} [<in> <area>]"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "lock"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOff": {
+            "data": [
                 {
                     "response": "fans_area",
                     "sentences": [
                         "<opreste> (<ventilatorul> | [toate] <ventilatoarele>) [<din>] <area>",
                         "<opreste> [<din>] <area> (<ventilatorul> | [toate] <ventilatoarele>)"
                     ],
                     "slots": {
@@ -852,65 +800,81 @@
                             "script",
                             "sensor"
                         ]
                     },
                     "sentences": [
                         "<opreste> <name>"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                },
                 {
                     "requires_context": {
-                        "domain": "scene"
+                        "domain": "light"
                     },
-                    "response": "scene",
+                    "response": "light",
                     "sentences": [
-                        "<porneste> [scena] <name>"
+                        "<opreste> <name>"
                     ],
                     "slots": {
-                        "domain": "scene"
+                        "domain": "light"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "light",
-                            "cover",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
+                    "response": "lights_area",
+                    "sentences": [
+                        "<opreste> (<lumina> | [toate] <luminile>) [<din>] <area>",
+                        "<opreste> [<din>] <area> (<lumina> | [toate] <luminile>)"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "area": null
                     },
+                    "response": "lights_area",
                     "sentences": [
-                        "<porneste> <name>"
+                        "<opreste> (<lumina> | [toate] <luminile>)"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
+                    "sentences": [
+                        "<inchide> <name> [[<din>] <area>]"
                     ]
                 },
                 {
-                    "response": "fans_area",
+                    "response": "covers_area",
                     "sentences": [
-                        "<porneste> (<ventilatorul> | [toate] <ventilatoarele>) <din> <area>",
-                        "<porneste> <din> <area> (<ventilatorul> | [toate] <ventilatoarele>)"
+                        "<inchide> ({cover_classes_singular:device_class} | [toate] {cover_classes_plural:device_class}) [<din>] <area>"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "cover"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
                     "requires_context": {
-                        "area": null
+                        "domain": "scene"
                     },
-                    "response": "fans_area",
+                    "response": "scene",
                     "sentences": [
-                        "<porneste> (<ventilatorul> | [toate] <ventilatoarele>)"
+                        "<porneste> [scena] <name>"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "scene"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "light",
@@ -941,41 +905,77 @@
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
-                        "domain": "script"
+                        "domain": "cover"
                     },
-                    "response": "script",
+                    "response": "cover",
                     "sentences": [
-                        "<ruleaza> [script[ul]] <name>"
+                        "<deschide> <name> [[<din>] <area>]"
+                    ]
+                },
+                {
+                    "response": "covers_area",
+                    "sentences": [
+                        "<deschide> ({cover_classes_singular:device_class} | [toate] {cover_classes_plural:device_class}) [<din>] <area>"
                     ],
                     "slots": {
-                        "domain": "script"
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<porneste> (<ventilatorul> | [toate] <ventilatoarele>) <din> <area>",
+                        "<porneste> <din> <area> (<ventilatorul> | [toate] <ventilatoarele>)"
+                    ],
+                    "slots": {
+                        "domain": "fan"
                     }
                 },
                 {
                     "requires_context": {
-                        "domain": "cover"
+                        "area": null
                     },
-                    "response": "cover",
+                    "response": "fans_area",
                     "sentences": [
-                        "<deschide> <name> [[<din>] <area>]"
-                    ]
+                        "<porneste> (<ventilatorul> | [toate] <ventilatoarele>)"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
                 },
                 {
-                    "response": "covers_area",
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
                     "sentences": [
-                        "<deschide> ({cover_classes_singular:device_class} | [toate] {cover_classes_plural:device_class}) [<din>] <area>"
+                        "<ruleaza> [script[ul]] <name>"
                     ],
                     "slots": {
-                        "domain": "cover"
+                        "domain": "script"
                     }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "light",
+                            "cover",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<porneste> <name>"
+                    ]
                 }
             ]
         }
     },
     "language": "ro",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/uk.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7328011138167388%*

 * *Differences: {"'expansion_rules'": "{'area': '[в|у|на] {area}', 'brightness': '{brightness}[%| "*

 * *                      "відсотк(ів|а|и)]', 'temperature': '{temperature} [градус(ів|и|а)] "*

 * *                      "[{temperature_unit}]', 'ввімкни': '(в|у)вімкни | включи', 'вимкни': 'вимкни "*

 * *                      "| виключи', 'зміни': 'зміни | встанови | зроби', 'відкрий': 'відкрий | "*

 * *                      "розкрий | підніми | відчини', 'закрий': 'закрий | опусти | зачини', delete: "*

 * *                      "['temp', 'turn_o […]*

```diff
@@ -1,455 +1,452 @@
 {
     "expansion_rules": {
-        "area": "[\u0432|\u0432\u043e|\u043d\u0430] {area}",
-        "brightness": "{brightness}[%| \u043f\u0440\u043e\u0446\u0435\u043d\u0442[\u043e\u0432|\u0430]]",
-        "close": "(\u0437\u0430\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043f\u0440\u0438\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043e\u043f\u0443\u0441\u0442\u0438[\u0442\u044c])",
+        "area": "[\u0432|\u0443|\u043d\u0430] {area}",
+        "brightness": "{brightness}[%| \u0432\u0456\u0434\u0441\u043e\u0442\u043a(\u0456\u0432|\u0430|\u0438)]",
         "name": "{name}",
-        "open": "(\u043e\u0442\u043a\u0440(\u043e\u0439|\u044b\u0442\u044c)|\u043f\u043e\u0434\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c))",
-        "set": "(\u0441\u0434\u0435\u043b\u0430(\u0439|\u0442\u044c)|\u0443\u0441\u0442\u0430\u043d\u043e\u0432\u0438[\u0442\u044c]|\u043f\u043e\u0441\u0442\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043f\u043e\u043c\u0435\u043d\u044f(\u0439|\u0442\u044c)|\u0438\u0437\u043c\u0435\u043d\u0438[\u0442\u044c]|\u0432\u044b\u0441\u0442\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043f\u0435\u0440\u0435\u043a\u043b\u044e\u0447\u0438[\u0442\u044c]|\u043f\u0435\u0440\u0435\u0432\u0435(\u0441\u0442\u0438|\u0434\u0438)|\u0443\u0432\u0435\u043b\u0438\u0447(\u044c|\u0438\u0442\u044c)|\u0443\u043c\u0435\u043d\u044c\u0448(\u0438|\u0438\u0442\u044c)|\u043f\u043e\u0434\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c)|\u043e\u043f\u0443\u0441\u0442\u0438[\u0442\u044c]|\u043f\u0440\u0438\u0431\u0430\u0432(\u044c|\u0438\u0442\u044c)|\u043e\u0442\u043d(\u0438\u043c\u0438|\u044f\u0442\u044c)|\u043f\u043e\u0432\u044b\u0441(\u044c|\u0438\u0442\u044c)|\u043f\u043e\u043d\u0438\u0437(\u044c|\u0438\u0442\u044c))",
-        "temp": "(\u0442\u0435\u043c\u043f\u0435\u0440\u0430\u0442\u0443\u0440(\u0430|\u0443)|\u0433\u0440\u0430\u0434\u0443\u0441[\u043e\u0432|\u0430])",
-        "temperature": "{temperature}[\u00b0|\u0433\u0440\u0430\u0434\u0443\u0441[\u043e\u0432|\u0430]] [{temperature_unit}]",
-        "turn_off": "(\u0432\u044b\u043a\u043b\u044e\u0447\u0438|\u043e\u0442\u043a\u043b\u044e\u0447\u0438)[\u0442\u044c]",
-        "turn_on": "(\u0437\u0430\u043f\u0443\u0441\u0442\u0438|\u0432\u043a\u043b\u044e\u0447\u0438)[\u0442\u044c]"
+        "temperature": "{temperature} [\u0433\u0440\u0430\u0434\u0443\u0441(\u0456\u0432|\u0438|\u0430)] [{temperature_unit}]",
+        "\u0432\u0432\u0456\u043c\u043a\u043d\u0438": "(\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0438 | \u0432\u043a\u043b\u044e\u0447\u0438",
+        "\u0432\u0438\u043c\u043a\u043d\u0438": "\u0432\u0438\u043c\u043a\u043d\u0438 | \u0432\u0438\u043a\u043b\u044e\u0447\u0438",
+        "\u0432\u0456\u0434\u043a\u0440\u0438\u0439": "\u0432\u0456\u0434\u043a\u0440\u0438\u0439 | \u0440\u043e\u0437\u043a\u0440\u0438\u0439 | \u043f\u0456\u0434\u043d\u0456\u043c\u0438 | \u0432\u0456\u0434\u0447\u0438\u043d\u0438",
+        "\u0437\u0430\u043a\u0440\u0438\u0439": "\u0437\u0430\u043a\u0440\u0438\u0439 | \u043e\u043f\u0443\u0441\u0442\u0438 | \u0437\u0430\u0447\u0438\u043d\u0438",
+        "\u0437\u043c\u0456\u043d\u0438": "\u0437\u043c\u0456\u043d\u0438 | \u0432\u0441\u0442\u0430\u043d\u043e\u0432\u0438 | \u0437\u0440\u043e\u0431\u0438"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "scene",
-                            "script"
-                        ]
-                    },
                     "response": "one",
                     "sentences": [
-                        "\u0427\u0442\u043e \u0441[\u043e] <name> [<area>]",
-                        "\u041a\u0430\u043a(\u043e\u0435|\u043e\u0432\u043e|\u0430\u044f|\u043e\u0439) [\u0441\u043e\u0441\u0442\u043e\u044f\u043d\u0438\u0435] [\u0443] <name> [<area>]"
+                        "\u0449\u043e \u0437 <name> [<area>]",
+                        "\u044f\u043a\u0438\u0439 \u0441\u0442\u0430\u043d <name> [<area>]",
+                        "\u0432 \u044f\u043a\u043e\u043c\u0443 \u0441\u0442\u0430\u043d\u0456 <name> [<area>]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "<name> [<area>] {on_off_states:state}",
-                        "{on_off_states:state} [\u043b\u0438] <name> [<area>]"
+                        "\u0447\u0438 {on_off_states:state} <name> [<area>]"
                     ]
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "[\u0415\u0441\u0442\u044c] [\u043b\u0438] [\u043a\u0430\u043a(\u043e\u0439|\u043e\u0435|\u0438\u0435)-\u043d\u0438\u0431\u0443\u0434\u044c] {on_off_states:state} {on_off_domains:domain} [<area>]",
-                        "[\u0415\u0441\u0442\u044c] [\u043b\u0438] [<area>] [\u043a\u0430\u043a(\u043e\u0439|\u043e\u0435|\u0438\u0435)-\u043d\u0438\u0431\u0443\u0434\u044c] {on_off_states:state} {on_off_domains:domain}"
+                        "\u0447\u0438 \u0454 {on_off_states:state} {on_off_domains:domain} [<area>]"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "(\u0412\u0441\u0435|\u0432\u0435\u0441\u044c) [\u043b\u0438] {on_off_domains:domain} {on_off_states:state} [<area>]",
-                        "{on_off_states:state} [\u043b\u0438] (\u0432\u0441\u0435|\u0432\u0435\u0441\u044c) {on_off_domains:domain} [<area>]"
+                        "\u0447\u0438 \u0432\u0441[\u0456|\u0435] {on_off_domains:domain} {on_off_states:state} [<area>]"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {on_off_domains:domain} {on_off_states:state} [<area>]",
-                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {on_off_domains:domain} [<area>] {on_off_states:state}"
+                        "(\u044f\u043a\u0456|\u043a\u043e\u0442\u0440\u0456) {on_off_domains:domain} {on_off_states:state} [<area>]"
                     ]
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_domains:domain} {on_off_states:state} [<area>]",
-                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_domains:domain} [<area>] {on_off_states:state}",
-                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {on_off_states:state} {on_off_domains:domain} [<area>]"
+                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {on_off_domains:domain} [<area>] {on_off_states:state}",
+                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438 [\u0454]|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {on_off_states:state} {on_off_domains:domain} [<area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "{cover_states:state} [\u043b\u0438] <name> [<area>]"
+                        "\u0447\u0438 {cover_states:state} <name> [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "\u0415\u0441\u0442\u044c [\u043b\u0438] {cover_states:state} {cover_classes:device_class} [<area>]"
+                        "\u0447\u0438 \u0454 {cover_states:state} {cover_classes:device_class} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "\u0412\u0441\u0435 [\u043b\u0438] {cover_classes:device_class} [<area>] {cover_states:state}"
+                        "\u0447\u0438 \u0432\u0441\u0456 {cover_classes:device_class} {cover_states:state} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(\u041a\u0430\u043a\u0438\u0435|\u043a\u043e\u0442\u043e\u0440\u044b\u0435) {cover_classes:device_class} {cover_states:state} [<area>]"
+                        "(\u044f\u043a\u0456|\u043a\u043e\u0442\u0440\u0456) {cover_classes:device_class} {cover_states:state} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "\u0421\u043a\u043e\u043b\u044c\u043a\u043e {cover_classes:device_class} {cover_states:state} [<area>]"
+                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {cover_classes:device_class} {cover_states:state} [<area>]",
+                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438 [\u0454]|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {cover_states:state} {cover_classes:device_class} [<area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438] <area>",
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438]",
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e <area>",
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <name> <area>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442",
-                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
-                        "<turn_off> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442",
-                        "<turn_off> <area> <name>",
-                        "<turn_off> <name> <area>"
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <area>",
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<close> [\u0434\u0432\u0435\u0440\u044c] \u0433\u0430\u0440\u0430\u0436\u0430",
-                        "<close> \u0433\u0430\u0440\u0430\u0436\u043d\u0443\u044e \u0434\u0432\u0435\u0440\u044c"
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> [\u0434\u0432\u0435\u0440\u0456] [\u0443|\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> \u0433\u0430\u0440\u0430\u0436\u043d\u0456 \u0434\u0432\u0435\u0440\u0456"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<close> (\u0448\u0442\u043e\u0440(\u044b|\u0443)|\u0437\u0430\u043d\u0430\u0432\u0435\u0441\u043a(\u0438|\u0443)|\u0436\u0430\u043b\u044e\u0437\u0438|\u043e\u043a\u043d(\u043e|\u0430)) <area>"
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438)) <area>",
+                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <area> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438))"
                     ],
                     "slots": {
                         "device_class": [
-                            "window",
                             "blind",
                             "curtain",
-                            "shutter"
+                            "shutter",
+                            "window"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_off> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b] <area>",
-                        "<turn_off> <area> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<turn_off> <name>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<close> <name>",
-                        "<close> <name> <area>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "sentences": [
-                        "<turn_on> <name>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<open> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<open> <name> <area>"
-                    ]
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_on> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b] <area>",
-                        "<turn_on> <area> [\u0432\u0441\u0435] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_on> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
-                        "<turn_on> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <area>",
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<open> [\u0434\u0432\u0435\u0440\u044c] \u0433\u0430\u0440\u0430\u0436[\u0430]",
-                        "<open> \u0433\u0430\u0440\u0430\u0436\u043d\u0443\u044e \u0434\u0432\u0435\u0440\u044c"
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> [\u0434\u0432\u0435\u0440\u0456] [\u0443|\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> \u0433\u0430\u0440\u0430\u0436\u043d\u0456 \u0434\u0432\u0435\u0440\u0456"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<open> (\u0448\u0442\u043e\u0440(\u044b|\u0443)|\u0437\u0430\u043d\u0430\u0432\u0435\u0441\u043a(\u0438|\u0443)|\u0436\u0430\u043b\u044e\u0437\u0438) <area>"
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438)) <area>",
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <area> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438))"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
-                            "shutter"
+                            "shutter",
+                            "window"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438] <area>",
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438]",
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e <area>",
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <name> <area>"
+                    ]
                 }
             ]
         }
     },
-    "language": "ru",
+    "language": "uk",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
         "color": {
             "values": [
                 {
-                    "in": "\u0431\u0435\u043b\u044b\u0439|\u0431\u0435\u043b\u043e\u0433\u043e|\u0431\u0435\u043b\u044b\u043c",
+                    "in": "\u0431\u0456\u043b\u0438\u0439 | \u0431\u0456\u043b(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "white"
                 },
                 {
-                    "in": "\u0447\u0435\u0440\u043d\u044b\u0439|\u0447\u0435\u0440\u043d\u043e\u0433\u043e|\u0447\u0451\u0440\u043d\u044b\u0439|\u0447\u0451\u0440\u043d\u043e\u0433\u043e|\u0447\u0435\u0440\u043d\u044b\u043c|\u0447\u0451\u0440\u043d\u044b\u043c",
+                    "in": "\u0447\u043e\u0440\u043d\u0438\u0439 | \u0447\u043e\u0440\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "black"
                 },
                 {
-                    "in": "\u043a\u0440\u0430\u0441\u043d\u044b\u0439|\u043a\u0440\u0430\u0441\u043d\u043e\u0433\u043e|\u043a\u0440\u0430\u0441\u043d\u044b\u043c",
+                    "in": "\u0447\u0435\u0440\u0432\u043e\u043d\u0438\u0439 | \u0447\u0435\u0440\u0432\u043e\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "red"
                 },
                 {
-                    "in": "\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u044b\u0439|\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u043e\u0433\u043e|\u043e\u0440\u0430\u043d\u0436\u0435\u0432\u044b\u043c",
+                    "in": "\u043f\u043e\u043c\u0430\u0440\u0430\u043d\u0447\u0435\u0432\u0438\u0439 | \u043f\u043e\u043c\u0430\u0440\u0430\u043d\u0447\u0435\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "orange"
                 },
                 {
-                    "in": "\u0436\u0435\u043b\u0442\u044b\u0439|\u0436\u0435\u043b\u0442\u043e\u0433\u043e|\u0436\u0451\u043b\u0442\u044b\u0439|\u0436\u0451\u043b\u0442\u043e\u0433\u043e|\u0436\u0435\u043b\u0442\u044b\u043c|\u0436\u0451\u043b\u0442\u044b\u043c",
+                    "in": "\u0436\u043e\u0432\u0442\u0438\u0439 | \u0436\u043e\u0432\u0442(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u0437\u0435\u043b\u0435\u043d\u044b\u0439|\u0437\u0435\u043b\u0451\u043d\u044b\u0439|\u0437\u0435\u043b\u0435\u043d\u043e\u0433\u043e|\u0437\u0435\u043b\u0451\u043d\u043e\u0433\u043e|\u0437\u0435\u043b\u0435\u043d\u044b\u043c|\u0437\u0435\u043b\u0451\u043d\u044b\u043c",
+                    "in": "\u0437\u0435\u043b\u0435\u043d\u0438\u0439 | \u0437\u0435\u043b\u0435\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "green"
                 },
                 {
-                    "in": "\u0441\u0438\u043d\u0438\u0439|\u0441\u0438\u043d\u0435\u0433\u043e|\u0441\u0438\u043d\u0438\u043c",
+                    "in": "\u0441\u0438\u043d\u0456\u0439 | \u0441\u0438\u043d(\u0456\u043c|\u044c\u043e\u044e|\u044c\u043e\u0433\u043e)",
                     "out": "blue"
                 },
                 {
-                    "in": "\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u044b\u0439|\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u043e\u0433\u043e|\u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u044b\u043c",
+                    "in": "\u0444\u0456\u043e\u043b\u0435\u0442\u043e\u0432\u0438\u0439 | \u0444\u0456\u043e\u043b\u0435\u0442\u043e\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "purple"
                 },
                 {
-                    "in": "\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u044b\u0439|\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u043e\u0433\u043e|\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u044b\u043c",
+                    "in": "\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u0438\u0439 | \u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
                     "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "\u043d\u0430\u0432\u0435\u0441[\u0430|\u044b|\u043e\u043c|\u0430\u043c\u0438]",
+                    "in": "awning[s]",
                     "out": "awning"
                 },
                 {
-                    "in": "\u0436\u0430\u043b\u044e\u0437\u0438",
+                    "in": "\u0436\u0430\u043b\u044e\u0437\u0456",
                     "out": "blind"
                 },
                 {
-                    "in": "\u0448\u0442\u043e\u0440[\u0430|\u044b|\u043e\u043c|\u0430\u043c\u0438]",
+                    "in": "\u0448\u0442\u043e\u0440[\u0430|\u0438]",
                     "out": "curtain"
                 },
                 {
-                    "in": "\u0434\u0432\u0435\u0440(\u044c[\u044e]|\u043c\u0438)",
+                    "in": "\u0434\u0432\u0435\u0440\u0456 | \u0434\u0432\u0435\u0440\u0435\u0439",
                     "out": "door"
                 },
                 {
-                    "in": "\u0433\u0430\u0440\u0430\u0436\u043d(\u0430\u044f|\u0443\u044e|\u043e\u0439|\u044b\u043c\u0438) \u0434\u0432\u0435\u0440(\u044c[\u044e]|\u043c\u0438)",
+                    "in": "\u0434\u0432\u0435\u0440[\u0456|\u0435\u0439] [\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
                     "out": "garage"
                 },
                 {
-                    "in": "gate[s]",
+                    "in": "\u0431\u0440\u0430\u043c[\u0430|\u0438] | \u0432\u043e\u0440(\u043e|\u0456)\u0442[\u0430]",
                     "out": "gate"
                 },
                 {
                     "in": "shade[s]",
                     "out": "shade"
                 },
                 {
-                    "in": "\u0441\u0442\u0430\u0432\u043d(\u044f[\u043c\u0438]|\u0438)",
+                    "in": "\u0441\u0442\u0430\u0432\u043d\u0456 | \u0441\u0442\u0430\u0432\u0435\u043d\u044c",
                     "out": "shutter"
                 },
                 {
-                    "in": "\u043e\u043a\u043d(\u043e[\u043c]|\u0430[\u043c\u0438])",
+                    "in": "\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0432\u0456\u043a\u043e\u043d",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "\u043e\u0442\u043a\u0440\u044b\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043d\u0435[ ]\u0437\u0430\u0434\u0435\u0440\u043d\u0443\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043f\u043e\u0434\u043d\u044f\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]",
-                    "out": "\u043e\u0442\u043a\u0440\u044b\u0442\u0430"
+                    "in": "\u0432\u0456\u0434\u043a\u0440\u0438\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e) | \u043f\u0456\u0434\u043d\u044f\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "out": "open"
                 },
                 {
-                    "in": "\u0437\u0430\u043a\u0440\u044b\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u0437\u0430\u0434\u0435\u0440\u043d\u0443\u0442[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]|\u043e\u043f\u0443\u0449\u0435\u043d[\u0430|\u043e|\u044b|\u043e\u0439|\u0430\u044f|\u044b\u0435|\u0443\u044e]",
-                    "out": "\u0437\u0430\u043a\u0440\u044b\u0442\u0430"
+                    "in": "\u0437\u0430\u043a\u0440\u0438\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e) | \u043e\u043f\u0443\u0449\u0435(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "out": "closed"
                 },
                 {
-                    "in": "\u043e\u0442\u043a\u0440\u044b\u0432\u0430(\u0435|\u044e)\u0442\u0441\u044f|\u043f\u043e\u0434\u043d\u0438\u043c\u0430(\u0435|\u044e)\u0442\u0441\u044f",
-                    "out": "\u043e\u0442\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f"
+                    "in": "\u0432\u0456\u0434\u043a\u0440\u0438\u0432\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f | \u043f\u0456\u0434\u043d\u0456\u043c\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f",
+                    "out": "opening"
                 },
                 {
-                    "in": "\u0437\u0430\u043a\u0440\u044b\u0432\u0430(\u0435|\u044e)\u0442\u0441\u044f|\u043e\u043f\u0443\u0441\u043a\u0430(\u0435|\u044e)\u0442\u0441\u044f",
-                    "out": "\u0437\u0430\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f"
+                    "in": "\u0437\u0430\u043a\u0440\u0438\u0432\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f | \u043e\u043f\u0443\u0441\u043a\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f",
+                    "out": "closing"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "(\u0441\u0432\u0435\u0442[\u0430]|\u043e\u0441\u0432\u0435\u0449\u0435\u043d\u0438\u0435|\u043b\u0430\u043c\u043f[\u0430|\u044b|\u043e\u0439|\u0430\u043c\u0438|\u0443]|\u0441\u0432\u0435\u0442\u0438\u043b\u044c\u043d\u0438\u043a(\u0430|\u0443|\u043e\u043c|\u0438|\u0430\u043c\u0438))",
+                    "in": "\u0441\u0432\u0456\u0442\u043b\u043e|\u0441\u0432\u0456\u0442\u0438\u043b\u044c\u043d\u0438\u043a[\u0438|\u0456\u0432]|\u043b\u0430\u043c\u043f[\u0438]",
                     "out": "light"
                 },
                 {
-                    "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u044b]",
+                    "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0430|\u0438|\u0456\u0432]",
                     "out": "fan"
                 },
                 {
-                    "in": "\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b(\u0438|\u044c|\u0435\u0439|\u0435\u043c|\u044f\u043c\u0438)",
+                    "in": "\u0432\u043c\u0438\u043a\u0430\u0447[\u0430|\u0456|\u0456\u0432] | \u0432\u0438\u043c\u0438\u043a\u0430\u0447[\u0430|\u0456|\u0456\u0432]",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "\u0432\u043a\u043b\u044e\u0447\u0435\u043d[\u043d][\u0430|\u044b[\u0435]|\u043e[\u0439]]",
-                    "out": "\u0432\u043a\u043b\u044e\u0447\u0435\u043d"
+                    "in": "(\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0435\u043d(\u0438\u0439|\u043d\u0430|\u0456|\u0438\u0445|\u043e) | (\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0443\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "out": "on"
                 },
                 {
-                    "in": "\u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d[\u043d][\u0430|\u044b[\u0435]|\u043e[\u0439]]",
-                    "out": "\u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d"
+                    "in": "\u0432\u0438\u043c\u043a\u043d\u0435\u043d(\u0438\u0439|\u043d\u0430|\u0456|\u0438\u0445|\u043e) | \u0432\u0438\u043c\u043a\u043d\u0443\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 {
-                    "in": "c|\u0446\u0435\u043b\u044c\u0441\u0438\u044f|\u043f\u043e \u0446\u0435\u043b\u044c\u0441\u0438\u044e",
+                    "in": "c | \u0446\u0435\u043b\u044c\u0441\u0456\u044e | \u0437\u0430 \u0446\u0435\u043b\u044c\u0441\u0456\u0454\u043c",
                     "out": "celsius"
                 },
                 {
-                    "in": "f|\u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0430|\u043f\u043e \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0443",
+                    "in": "f | \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0443 | \u0437\u0430 \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u043e\u043c",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u0412\u043e \u0432\u0440\u0435\u043c\u044f \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0438 \u043d\u0430\u043c\u0435\u0440\u0435\u043d\u0438\u044f \u043f\u0440\u043e\u0438\u0437\u043e\u0448\u043b\u0430 \u043d\u0435\u043f\u0440\u0435\u0434\u0432\u0438\u0434\u0435\u043d\u043d\u0430\u044f \u043e\u0448\u0438\u0431\u043a\u0430",
-            "no_area": "\u041d\u0435\u0442 \u0437\u043e\u043d\u044b, \u043d\u0430\u0437\u0432\u0430\u043d\u043d\u043e\u0439 {{ area }}",
-            "no_device_class": "\u0412 \u0437\u043e\u043d\u0435 {{ area }} \u043d\u0435\u0442 \u0443\u0441\u0442\u0440\u043e\u0439\u0441\u0442\u0432 {{ device_class }}",
-            "no_domain": "\u0412 \u0437\u043e\u043d\u0435 {{ area }} \u043d\u0435\u0442 \u043e\u0431\u044a\u0435\u043a\u0442\u043e\u0432 {{ domain }}",
-            "no_entity": "\u041d\u0435\u0442 \u0443\u0441\u0442\u0440\u043e\u0439\u0441\u0442\u0432\u0430 \u0438\u043b\u0438 \u0441\u0443\u0449\u043d\u043e\u0441\u0442\u0438, \u043d\u0430\u0437\u0432\u0430\u043d\u043d\u043e\u0439 {{ entity }}",
-            "no_intent": "\u041f\u0440\u043e\u0448\u0443 \u043f\u0440\u043e\u0449\u0435\u043d\u0438\u044f, \u043e\u0431\u0440\u0430\u0449\u0435\u043d\u0438\u0435 \u043d\u0435 \u0440\u0430\u0441\u043f\u043e\u0437\u043d\u0430\u043d\u043e"
+            "handle_error": "\u041d\u0435\u043e\u0447\u0456\u043a\u0443\u0432\u0430\u043d\u0430 \u043f\u043e\u043c\u0438\u043b\u043a\u0430 \u0432\u0438\u043d\u0438\u043a\u043b\u0430 \u043f\u0456\u0434 \u0447\u0430\u0441 \u0432\u0438\u043a\u043e\u043d\u0430\u043d\u043d\u044f \u0437\u0430\u043f\u0438\u0442\u0443",
+            "no_area": "\u041d\u0435\u043c\u0430\u0454 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f \u043f\u0456\u0434 \u043d\u0430\u0437\u0432\u043e\u044e {{ area }}",
+            "no_device_class": "\u041f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f {{ area }} \u043d\u0435 \u043c\u0456\u0441\u0442\u0438\u0442\u044c {{ device_class }}",
+            "no_domain": "\u041f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f {{ area }} \u043d\u0435 \u043c\u0456\u0441\u0442\u0438\u0442\u044c {{ domain }}",
+            "no_entity": "\u041d\u0435\u043c\u0430\u0454 \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u044e \u0447\u0438 \u0441\u0443\u0442\u043d\u043e\u0441\u0442\u0456 \u043f\u0456\u0434 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }}",
+            "no_intent": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u044f \u0446\u044c\u043e\u0433\u043e \u043d\u0435 \u0440\u043e\u0437\u0443\u043c\u0456\u044e"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  \u0414\u0430\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    {{ no_match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (no_match | length - 3) }} \u2014 \u043d\u0435\u0442\n  {%- else -%}\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }} \u2014 \u043d\u0435\u0442\n    {%- endfor %}\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0414\u0430, {{ match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (match | length - 3) }}\n  {%- else -%}\n    \u0414\u0430,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u041d\u0435\u0442\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  \u0422\u0430\u043a\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u041d\u0456, {{ no_match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (no_match | length - 3) }} \u043d\u0456\n  {%- else -%}\n    \u041d\u0456,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor %} \u043d\u0456\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0422\u0430\u043a, {{ match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (match | length - 3) }}\n  {%- else -%}\n    \u0422\u0430\u043a,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u041d\u0456\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
                 "one": "{{ slots.name | capitalize }} {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  \u0414\u0430\n{% else %}\n  \u041d\u0435\u0442, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  \u041d\u0438 \u043e\u0434\u043d\u043e\u0433\u043e\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+                "one_yesno": "{% if query.matched %}\n  \u0422\u0430\u043a\n{% else %}\n  \u041d\u0456, {{ state.state_with_unit }}\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u0442\u0430\u043a\u0438\u0445 \u043d\u0435\u043c\u0430\u0454\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0456 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.name }}",
-                "cover_area": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.area }}",
-                "cover_device_class": "\u0417\u0430\u043a\u0440\u044b\u0442\u043e {{ slots.device_class }}",
-                "default": "{{ slots.name }} \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d",
-                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432 {{ slots.area }}",
-                "lights_area": "\u0412\u044b\u043a\u043b\u044e\u0447\u0435\u043d \u0441\u0432\u0435\u0442 \u0432 {{ slots.area }}"
+                "cover": "{{ slots.name }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
+                "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
+                "cover_device_class": "{{ slots.device_class }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
+                "default": "{{ slots.name }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
+                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
+                "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e"
             },
             "HassTurnOn": {
-                "cover": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.name }}",
-                "cover_area": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.area }}",
-                "cover_device_class": "\u041e\u0442\u043a\u0440\u044b\u0442\u043e {{ slots.device_class }}",
-                "default": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d {{ slots.name }}",
-                "fans_area": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432 {{ slots.area }}",
-                "lights_area": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d \u0441\u0432\u0435\u0442 \u0432 {{ slots.area }}"
+                "cover": "{{ slots.name }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
+                "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
+                "cover_device_class": "{{ slots.device_class }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
+                "default": "{{ slots.name }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
+                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
+                "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e"
             }
         }
     },
     "skip_words": [
-        "\u043f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430",
-        "\u043c\u043e\u0436\u0435\u0448\u044c",
-        "\u0441\u043a\u0430(\u0436\u0438|\u0437\u0430\u0442\u044c)",
-        "\u043f\u0440\u043e\u0448\u0443",
-        "\u0443\u0437\u043d\u0430(\u0439|\u0442\u044c)"
+        "\u0431\u0443\u0434\u044c \u043b\u0430\u0441\u043a\u0430",
+        "\u0437\u0430\u0440\u0430\u0437",
+        "\u0441\u044c\u043e\u0433\u043e\u0434\u043d\u0456"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sk.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922438672438673%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {1: {'sentences': ['(<turn_on>|<turn_on_light>) "*

 * *              "[(všetky|všetko)] [(svetlá|osvetlenie|lampy)] [(v|vo|na|pred|pod|pri)] <area>'], "*

 * *              "'slots': OrderedDict([('domain', 'light'), ('name', 'all')]), 'response': "*

 * *              "'lights_area'}, 2: {'sentences': ['<open> garáž', '<open> garážovú bránu'], "*

 * *              "'response': 'cover_device_class', 'slots': OrderedDict([('device_class', 'garage'), "*

 * *              "('domain', 'cover')])}, 3 […]*

```diff
@@ -65,58 +65,14 @@
                     ]
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "light",
-                    "sentences": [
-                        "(<turn_off>|<turn_off_light>) (svetlo|lampu) <area>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
-                    "response": "lights_area",
-                    "sentences": [
-                        "(<turn_off>|<turn_off_light>) [(v\u0161etky|v\u0161etko)] [(svetl\u00e1|osvetlenie|lampy)] [(v|vo|na|pred|pod|pri)] <area>"
-                    ],
-                    "slots": {
-                        "domain": "light",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<close> gar\u00e1\u017e",
-                        "<close> gar\u00e1\u017eov\u00fa br\u00e1nu"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<close> (rolety|\u017eal\u00fazie|z\u00e1ves[y]|z\u00e1clon(u|y)) [v|na] {area}"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
-                },
-                {
                     "response": "fan",
                     "sentences": [
                         "<turn_off> (ventil\u00e1tor|vetr\u00e1k) [(v|vo)] <area>"
                     ],
                     "slots": {
                         "domain": "fan"
                     }
@@ -153,65 +109,63 @@
                     ]
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
                         "<close> {name} [v|vo|na|pred|za|pod|pred] {area}"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
-                {
-                    "sentences": [
-                        "<turn_on> <name>"
-                    ]
                 },
                 {
-                    "response": "cover",
-                    "sentences": [
-                        "<open> {name}"
-                    ]
-                },
-                {
-                    "response": "cover_area",
+                    "response": "light",
                     "sentences": [
-                        "<open> {name} [v|vo|na|pred|za|pod|pred] {area}"
-                    ]
+                        "(<turn_off>|<turn_off_light>) (svetlo|lampu) <area>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "response": "fan",
+                    "response": "lights_area",
                     "sentences": [
-                        "<turn_on> (ventil\u00e1tor|vetr\u00e1k) [(v|vo)] <area>"
+                        "(<turn_off>|<turn_off_light>) [(v\u0161etky|v\u0161etko)] [(svetl\u00e1|osvetlenie|lampy)] [(v|vo|na|pred|pod|pri)] <area>"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "light",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "fans_ventilation",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<turn_on> (ventil\u00e1ciu|vetranie) [(v|vo)] <area>"
+                        "<close> gar\u00e1\u017e",
+                        "<close> gar\u00e1\u017eov\u00fa br\u00e1nu"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "fans_area",
+                    "response": "cover_area",
                     "sentences": [
-                        "<turn_on> [(v\u0161etky|v\u0161etko)] (ventil\u00e1tory|vetr\u00e1ky|ventil\u00e1ciu|vetranie) [(v|vo)] <area>"
+                        "<close> (rolety|\u017eal\u00fazie|z\u00e1ves[y]|z\u00e1clon(u|y)) [v|na] {area}"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": [
+                            "blind",
+                            "curtain",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
                     "response": "light",
                     "sentences": [
                         "(<turn_on>|<turn_on_light>) (svetlo|lampu) <area>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -247,14 +201,60 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fan",
+                    "sentences": [
+                        "<turn_on> (ventil\u00e1tor|vetr\u00e1k) [(v|vo)] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan"
+                    }
+                },
+                {
+                    "response": "fans_ventilation",
+                    "sentences": [
+                        "<turn_on> (ventil\u00e1ciu|vetranie) [(v|vo)] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_on> [(v\u0161etky|v\u0161etko)] (ventil\u00e1tory|vetr\u00e1ky|ventil\u00e1ciu|vetranie) [(v|vo)] <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<turn_on> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<open> {name}"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "<open> {name} [v|vo|na|pred|za|pod|pred] {area}"
+                    ]
                 }
             ]
         }
     },
     "language": "sk",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sl.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,29 +7,29 @@
             "no_area": "Obmo\u010dje z imenom {{ area }} ne obstaja",
             "no_domain": "V obmo\u010dju {{ area }} ne obstaja {{ domain }}",
             "no_device_class": "V obmo\u010dju {{ area }} ne obstaja {{ device_class }}",
             "no_entity": "Ni naprave ali entitete z imenom {{ entity }}",
             "handle_error": "Med izvajanjem je pri\u0161lo do nepri\u010dakovane napake"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Naprava {{ slots.name }} je vklopljena",
-                "lights_area": "Lu\u010di v {{ slots.area }} so vklopljene",
-                "fans_area": "Ventilatorji v {{ slots.area }} so vklopljeni",
-                "cover": "Sen\u010dilo {{ slots.name }} je odprto",
-                "cover_area": "Sen\u010dila v {{ slots.area }} so odprta"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Naprava {{ slots.name }} je izklopljena",
                 "lights_area": "Lu\u010di v {{ slots.area }} so izklopljene",
                 "fans_area": "Ventilatorji v {{ slots.area }} so izklopljeni",
                 "cover": "Sen\u010dilo {{ slots.name }} je zaprto",
                 "cover_area": "Sen\u010dila v {{ slots.area }} so zaprta"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Naprava {{ slots.name }} je vklopljena",
+                "lights_area": "Lu\u010di v {{ slots.area }} so vklopljene",
+                "fans_area": "Ventilatorji v {{ slots.area }} so vklopljeni",
+                "cover": "Sen\u010dilo {{ slots.name }} je odprto",
+                "cover_area": "Sen\u010dila v {{ slots.area }} so odprta"
+            }
         }
     },
     "lists": {
         "color": {
             "values": [
                 {
                     "in": "bela",
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,28 +1,28 @@
 {
     "language": "sr",
     "intents": {
-        "HassTurnOn": {
+        "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<\u0443\u043f\u0430\u043b\u0438> [\u0441\u0432\u0430] [\u0441\u0432\u0435\u0442\u043b(\u043e|\u0430)] <area>"
+                        "<\u0443\u0433\u0430\u0441\u0438> [\u0441\u0432\u0430] [\u0441\u0432\u0435\u0442\u043b(\u043e|\u0430)] <area>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 }
             ]
         },
-        "HassTurnOff": {
+        "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<\u0443\u0433\u0430\u0441\u0438> [\u0441\u0432\u0430] [\u0441\u0432\u0435\u0442\u043b(\u043e|\u0430)] <area>"
+                        "<\u0443\u043f\u0430\u043b\u0438> [\u0441\u0432\u0430] [\u0441\u0432\u0435\u0442\u043b(\u043e|\u0430)] <area>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 }
             ]
@@ -34,31 +34,31 @@
             "no_area": "\u041d\u0435 \u043f\u043e\u0441\u0442\u043e\u0458\u0438 \u043f\u0440\u043e\u0441\u0442\u043e\u0440\u0438\u0458\u0430 \u0441\u0430 \u0438\u043c\u0435\u043d\u043e\u043c {{ area }}",
             "no_domain": "\u041f\u0440\u043e\u0441\u0442\u043e\u0440\u0438\u0458\u0430 {{ area }} \u043d\u0435 \u043f\u043e\u0441\u0442\u043e\u0458\u0438 \u0443 \u043e\u043a\u0432\u0438\u0440\u0443 \u043f\u043e\u0434\u0440\u0443\u0447\u0458\u0430 {{ domain }}",
             "no_device_class": "\u041f\u0440\u043e\u0441\u0442\u043e\u0440\u0438\u0458\u0430 {{ area }} \u043d\u0435 \u0441\u0430\u0434\u0440\u0436\u0438 {{ device_class }}",
             "no_entity": "\u041d\u0435 \u043f\u043e\u0441\u0442\u043e\u0458\u0438 \u043d\u0438 \u0443\u0440\u0435\u0452\u0430\u0458 \u043d\u0438 \u0435\u043d\u0442\u0438\u0442\u0435\u0442 \u043f\u043e\u0434 \u0438\u043c\u0435\u043d\u043e\u043c {{ entity }}",
             "handle_error": "\u0414\u043e\u0448\u043b\u043e \u0458\u0435 \u0434\u043e \u043d\u0435\u043e\u0447\u0435\u043a\u0438\u0432\u0430\u043d\u0435 \u0433\u0440\u0435\u0448\u043a\u0435 \u043f\u0440\u0438\u043b\u0438\u043a\u043e\u043c \u043e\u0431\u0440\u0430\u0434\u0435 \u0437\u0430\u0445\u0442\u0435\u0432\u0430"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "\u041f\u0430\u043b\u0438\u043c {{ state.domain }}",
-                "default_name": "\u041f\u0430\u043b\u0438\u043c {{ slots.name }}",
-                "lights_area": "{{ slots.area }}, \u043f\u0430\u043b\u0438\u043c \u0441\u0432\u0435\u0442\u043b\u0430",
-                "fans_area": "{{ slots.area }}, \u0443\u043a\u0459\u0443\u0447\u0443\u0458\u0435\u043c \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0435",
-                "cover_device_class": "\u041e\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.device_class }}",
-                "cover_single": "\u041e\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.name }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "\u0413\u0430\u0441\u0438\u043c {{ state.domain }}",
                 "default_name": "\u0413\u0430\u0441\u0438\u043c {{ slots.name }}",
                 "lights_area": "{{ slots.area }}, \u0433\u0430\u0441\u0438\u043c \u0441\u0432\u0435\u0442\u043b\u0430",
                 "fans_area": "{{ slots.area }}, \u0433\u0430\u0441\u0438\u043c \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0435",
                 "cover_device_class": "\u0417\u0430\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.device_class }}",
                 "cover_single": "\u0417\u0430\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.name }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "\u041f\u0430\u043b\u0438\u043c {{ state.domain }}",
+                "default_name": "\u041f\u0430\u043b\u0438\u043c {{ slots.name }}",
+                "lights_area": "{{ slots.area }}, \u043f\u0430\u043b\u0438\u043c \u0441\u0432\u0435\u0442\u043b\u0430",
+                "fans_area": "{{ slots.area }}, \u0443\u043a\u0459\u0443\u0447\u0443\u0458\u0435\u043c \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0435",
+                "cover_device_class": "\u041e\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.device_class }}",
+                "cover_single": "\u041e\u0442\u0432\u0430\u0440\u0430\u043c {{ slots.name }}"
+            }
         }
     },
     "lists": {
         "color": {
             "values": [
                 {
                     "in": "\u0431\u0435\u043b(\u0430|\u043e|\u0443)",
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sv.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(4, OrderedDict([('sentences', ['<slå_på> [alla] "*

 * *              "(fläkten | fläktar | fläktarna) <i_på> <area>']), ('slots', OrderedDict([('domain', "*

 * *              "'fan'), ('name', 'all')]))])), (5, OrderedDict([('sentences', ['<slå_på> "*

 * *              "<name>'])])), (6, OrderedDict([('sentences', ['<öppna_gardiner> <name>']), "*

 * *              "('response', 'cover')]))], delete: [2, 1, 0]}}, 'HassTurnOff': {'data': {insert: "*

 * *              "[(0, OrderedDict […]*

```diff
@@ -71,14 +71,34 @@
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
+                        "<sl\u00e5_av> [alla] (fl\u00e4kten | fl\u00e4ktar | fl\u00e4ktarna) <i_p\u00e5> <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<sl\u00e5_av> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<st\u00e4ng_gardiner> <name>"
+                    ]
+                },
+                {
+                    "sentences": [
                         "<sl\u00e5_av> [<alla>] <ljusk\u00e4llor> <i_p\u00e5> <area>",
                         "<sl\u00e5_av> [<alla>] <area> <ljusk\u00e4llor>",
                         "<sl\u00e5_av> <area> [<alla>] <ljusk\u00e4llor>",
                         "<sl\u00e5_av> [<alla>] <area>[s]<ljusk\u00e4llor>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -113,61 +133,21 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
-                },
-                {
-                    "sentences": [
-                        "<sl\u00e5_av> [alla] (fl\u00e4kten | fl\u00e4ktar | fl\u00e4ktarna) <i_p\u00e5> <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
-                        "<sl\u00e5_av> <name>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<st\u00e4ng_gardiner> <name>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "<sl\u00e5_p\u00e5> <name>"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<\u00f6ppna_gardiner> <name>"
-                    ]
-                },
-                {
-                    "sentences": [
-                        "<sl\u00e5_p\u00e5> [alla] (fl\u00e4kten | fl\u00e4ktar | fl\u00e4ktarna) <i_p\u00e5> <area>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "sentences": [
                         "<sl\u00e5_p\u00e5> [<alla>] <ljusk\u00e4llor> <i_p\u00e5> <area>",
                         "<sl\u00e5_p\u00e5> [<alla>] <area> <ljusk\u00e4llor>",
                         "<sl\u00e5_p\u00e5>  <area> [<alla>] <ljusk\u00e4llor>",
                         "<sl\u00e5_p\u00e5> [<alla>] <area>[s]<ljusk\u00e4llor>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -202,14 +182,34 @@
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "<sl\u00e5_p\u00e5> [alla] (fl\u00e4kten | fl\u00e4ktar | fl\u00e4ktarna) <i_p\u00e5> <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "<sl\u00e5_p\u00e5> <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "<\u00f6ppna_gardiner> <name>"
+                    ]
                 }
             ]
         }
     },
     "language": "sv",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/sw.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "TODO No area named {{ area }}",
             "no_domain": "TODO {{ area }} does not contain a {{ domain }}",
             "no_device_class": "TODO {{ area }} does not contain a {{ device_class }}",
             "no_entity": "TODO No device or entity named {{ entity }}",
             "handle_error": "TODO An unexpected error occurred while handling the intent"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/te.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -7,28 +7,28 @@
             "no_area": "{{ area }} \u0c05\u0c28\u0c46 \u0c17\u0c26\u0c3f \u0c32\u0c46\u0c26\u0c41",
             "no_domain": "{{ area }} \u0c32\u0c4a {{ domain }} \u0c32\u0c47\u0c26\u0c41",
             "no_device_class": "{{ area }} \u0c32\u0c4a {{ device_class }}  \u0c32\u0c47\u0c26\u0c41",
             "no_entity": "{{ entity }} \u0c2a\u0c46\u0c30\u0c41\u0c24\u0c4a \u0c0e\u0c1f\u0c41\u0c35\u0c02\u0c1f\u0c3f \u0c2a\u0c30\u0c3f\u0c15\u0c30\u0c2e\u0c41 \u0c32\u0c47\u0c26\u0c41",
             "handle_error": "\u0c0a\u0c39\u0c3f\u0c02\u0c1a\u0c28\u0c3f \u0c38\u0c2e\u0c38\u0c4d\u0c2f \u0c0e\u0c26\u0c41\u0c30\u0c48\u0c28\u0c26\u0c3f"
         },
         "intents": {
-            "HassTurnOn": {
-                "default": "Turned on {{ slots.name }}",
-                "lights_area": "Turned on lights in {{ slots.area }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}"
-            },
+            "HassGetState": {},
             "HassTurnOff": {
                 "default": "Turned off {{ slots.name }}",
                 "lights_area": "Turned off lights in {{ slots.area }}",
                 "fans_area": "Turned off fans in {{ slots.area }}",
                 "cover": "Closed {{ slots.name }}",
                 "cover_area": "Closed {{ slots.area }}"
             },
-            "HassGetState": {}
+            "HassTurnOn": {
+                "default": "Turned on {{ slots.name }}",
+                "lights_area": "Turned on lights in {{ slots.area }}",
+                "fans_area": "Turned on fans in {{ slots.area }}",
+                "cover": "Opened {{ slots.name }}",
+                "cover_area": "Opened {{ slots.area }}"
+            }
         }
     },
     "lists": {},
     "expansion_rules": {},
     "skip_words": []
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/is.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6629546957671958%*

 * *Differences: {"'expansion_rules'": "{'area': '{area}[(inu|nu|ið|ð|inni|nni|nu|num)]', 'name': "*

 * *                      "'{name}[(inu|nu|ið|ð|inni|nni|nu|num)]', 'turn-on': '(kveikja|kveiktu[ "*

 * *                      "á]|kveikt þú á|kveikt á|kveikja [á])', 'turn-off': '(slökkva|slökktu[ "*

 * *                      "á]|slökkt þú á|slökkt á|slökkva [á])', 'light': "*

 * *                      "'(ljósinu|ljósunum|ljósin|ljós)', 'all': '(öll|öllum|öllu|allt)', delete: "*

 * *                      "['ismin_halleri', 'cogulluk', 'temperature' […]*

```diff
@@ -1,228 +1,143 @@
 {
     "expansion_rules": {
-        "area": "{area}<ismin_halleri>",
-        "cogulluk": "[(ler|leri|lar|lar\u0131)]",
-        "ismin_halleri": "[([(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u0131|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]i|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]\u00fc|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]u|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]e|[(n|\u0131n|in|un|\u00fcn|y|t|d|nd|nt)]a)][n][ki]",
-        "name": "{name}<cogulluk><ismin_halleri>",
-        "temperature": "{temperature} [{temperature_unit}]"
+        "all": "(\u00f6ll|\u00f6llum|\u00f6llu|allt)",
+        "area": "{area}[(inu|nu|i\u00f0|\u00f0|inni|nni|nu|num)]",
+        "light": "(lj\u00f3sinu|lj\u00f3sunum|lj\u00f3sin|lj\u00f3s)",
+        "name": "{name}[(inu|nu|i\u00f0|\u00f0|inni|nni|nu|num)]",
+        "turn-off": "(sl\u00f6kkva|sl\u00f6kktu[ \u00e1]|sl\u00f6kkt \u00fe\u00fa \u00e1|sl\u00f6kkt \u00e1|sl\u00f6kkva [\u00e1])",
+        "turn-on": "(kveikja|kveiktu[ \u00e1]|kveikt \u00fe\u00fa \u00e1|kveikt \u00e1|kveikja [\u00e1])"
     },
     "intents": {
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "cover_device_class",
+                    "response": "lights_area",
                     "sentences": [
-                        "garaj kap\u0131s\u0131n\u0131 (kapa | kapat | indir )"
+                        "<turn-off> <light> \u00ed <area>",
+                        "<turn-off> <all> [<light>] \u00ed <area>",
+                        "<turn-off> <area><light>"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "light"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "lights_name",
                     "sentences": [
-                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (kapa | kapat | indir | \u00e7ek)"
+                        "<turn-off> <name> [\u00ed <area>]"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
+                        "domain": "light"
                     }
-                },
-                {
-                    "sentences": [
-                        "<name> (kapa | kapat | s\u00f6nd\u00fcr )"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<name> (kapa | kapat | indir ) "
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> <name> (kapa | kapat | indir )"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "lights_area",
                     "sentences": [
-                        "<name> ( a\u00e7 | yak | \u00e7al\u0131\u015ft\u0131r)"
-                    ]
-                },
-                {
-                    "response": "cover",
-                    "sentences": [
-                        "<name> (a\u00e7 | y\u00fckselt) "
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<area> <name> (a\u00e7 | y\u00fckselt)"
-                    ]
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "garaj kap\u0131s\u0131n\u0131 (a\u00e7 | y\u00fckselt)"
+                        "<turn-on> <light> \u00ed <area>",
+                        "<turn-on> <all> [<light>] \u00ed <area>",
+                        "<turn-on> <area>[ ]<light>"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "light"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "lights_name",
                     "sentences": [
-                        "<area> (perde|jaluzi|kepeng|panjur)<cogulluk><ismin_halleri> (a\u00e7 | y\u00fckselt)"
+                        "<turn-on> <name> [\u00ed <area>]"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
+                        "domain": "light"
                     }
                 }
             ]
         }
     },
-    "language": "tr",
+    "language": "is",
     "lists": {
-        "brightness": {
-            "range": {
-                "from": 0,
-                "to": 100,
-                "type": "percentage"
-            }
-        },
         "color": {
             "values": [
                 {
-                    "in": "beyaz",
+                    "in": "hv\u00edt(t|ur|an|a|um|ri|u|s|rar)",
                     "out": "white"
                 },
                 {
-                    "in": "siyah",
+                    "in": "(svart|svartur|sv\u00f6rt)",
                     "out": "black"
                 },
                 {
-                    "in": "k\u0131rm\u0131z\u0131",
+                    "in": "(rau\u00f0ur|rautt|rau\u00f0)",
                     "out": "red"
                 },
                 {
-                    "in": "turuncu",
+                    "in": "(appels\u00ednugulur|appels\u00ednugult|apples\u00ednugul)",
                     "out": "orange"
                 },
                 {
-                    "in": "sar\u0131",
+                    "in": "(gulur|gul|gult)",
                     "out": "yellow"
                 },
                 {
-                    "in": "ye\u015fil",
+                    "in": "(gr\u00e6nn|gr\u00e6nt|gr\u00e6n)",
                     "out": "green"
                 },
                 {
-                    "in": "mavi",
+                    "in": "(bl\u00e1r|bl\u00e1|bl\u00e1tt)",
                     "out": "blue"
                 },
                 {
-                    "in": "mor",
+                    "in": "(fj\u00f3lubl\u00e1tt|fj\u00f3lubl\u00e1r|j\u00f3lubl\u00e1)",
                     "out": "purple"
                 },
                 {
-                    "in": "kahverengi",
+                    "in": "(br\u00fann|br\u00fan|br\u00fant)",
                     "out": "brown"
                 },
                 {
-                    "in": "gri",
-                    "out": "grey"
-                },
-                {
-                    "in": "pembe",
+                    "in": "(bleikur|bleikt|bleik)",
                     "out": "pink"
-                },
-                {
-                    "in": "turkuaz",
-                    "out": "turquoise"
-                },
-                {
-                    "in": "bordo",
-                    "out": "maroon"
-                },
-                {
-                    "in": "bej",
-                    "out": "beige"
-                },
-                {
-                    "in": "lacivert",
-                    "out": "navy"
-                }
-            ]
-        },
-        "temperature": {
-            "range": {
-                "from": 0,
-                "to": 100,
-                "type": "temperature"
-            }
-        },
-        "temperature_unit": {
-            "values": [
-                "celsius",
-                {
-                    "in": "c | santigrat",
-                    "out": "celsius"
-                },
-                "fahrenheit",
-                {
-                    "in": "f | fahrenhayt",
-                    "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u0130stenilen ama\u00e7 i\u015flenirken bir hata olu\u015ftu.",
-            "no_area": "{{ area }}  ad\u0131nda alan yok.",
-            "no_device_class": "{{ area }}  bir {{ device_class }} i\u00e7ermiyor.",
-            "no_domain": "{{ area }}  bir {{ domain }} i\u00e7ermiyor.",
-            "no_entity": "{{ entity }} ad\u0131nda bir cihaz yok.",
-            "no_intent": "\u00dczg\u00fcn\u00fcm, bunu anlayamad\u0131m."
+            "handle_error": "Vi\u00f0 me\u00f0h\u00f6ndlun \u00e1setningsins kom \u00f3v\u00e6nt villa upp",
+            "no_area": "Ekkert sv\u00e6\u00f0i {{ area }} fannst",
+            "no_device_class": "{{ area }} er ekki me\u00f0 t\u00e6kja tegund {{ device_class }}",
+            "no_domain": "\u00cd {{ area }} er ekkert {{ domain }}",
+            "no_entity": "Ekkert t\u00e6ki e\u00f0a engin eining me\u00f0 nafni {{ entity }} fannst",
+            "no_intent": "Fyrirgef\u00f0u en \u00e9g n\u00e1\u00f0i \u00feessu ekki"
         },
         "intents": {
             "HassGetState": {},
             "HassTurnOff": {
-                "cover": "Closed {{ slots.name }}",
-                "cover_area": "Closed {{ slots.area }}",
-                "cover_device_class": "Closed {{ slots.device_class }}",
-                "default": "Turned off {{ slots.name }}",
-                "fans_area": "Turned off fans in {{ slots.area }}",
-                "lights_area": "Turned off lights in {{ slots.area }}"
+                "cover": "Loka\u00f0i {{ slots.name }}",
+                "cover_area": "Loka\u00f0i {{ slots.area }}",
+                "default": "Sl\u00f6kkti \u00e1 {{ slots.domain }}",
+                "fans_area": "Sl\u00f6kkti \u00e1 viftum \u00ed {{ slots.area }}",
+                "lights_area": "Sl\u00f6kkti \u00e1 lj\u00f3sum \u00ed {{ slots.area }}",
+                "lights_name": "Sl\u00f6kkti \u00e1 {{ slots.name }}"
             },
             "HassTurnOn": {
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}",
-                "cover_device_class": "Opened {{ slots.device_class }}",
-                "default": "Turned on {{ slots.name }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "lights_area": "Turned on lights in {{ slots.area }}"
+                "cover": "Opna\u00f0i {{ slots.name }}",
+                "cover_area": "Opna\u00f0i {{ slots.area }}",
+                "default": "Kveikti \u00e1 {{ slots.domain }}",
+                "fans_area": "Kveikti \u00e1 viftum \u00ed {{ slots.area }}",
+                "lights_area": "Kveikti \u00e1 lj\u00f3sum \u00ed {{ slots.area }}",
+                "lights_name": "Kveikti \u00e1 {{ slots.name }}"
             }
         }
     },
     "skip_words": [
-        "L\u00fctfen"
+        "\u00fe\u00fa",
+        "getur\u00f0u",
+        "getur \u00fe\u00fa",
+        "viltu",
+        "vilt \u00fe\u00fa"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/ar.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.711016027753049%*

 * *Differences: {"'expansion_rules'": "{'name': '[ال]{name}', 'area': '[ال]{area}', 'brightness': '{brightness}[% "*

 * *                      "| بالمائة]', 'temperature': '{temperature}[°| درجة] [{temperature_unit}]', "*

 * *                      "'colors': '[ال]{color}', 'script': "*

 * *                      "'[ال](برنامج|برامج|مسار|مسارات|سيناريو)', 'what_is': '(ما هو|ما هي|ماذا "*

 * *                      "يكون|ماذا تكون|كم هي|كم هو|هل هي|هل هو)', 'light': "*

 * *                      "'[ال](اضواء|اضاءة|ضوء|مصابيح|مصباح|انوار|نور|لمبة|لمبات| […]*

```diff
@@ -1,452 +1,455 @@
 {
     "expansion_rules": {
-        "area": "[\u0432|\u0443|\u043d\u0430] {area}",
-        "brightness": "{brightness}[%| \u0432\u0456\u0434\u0441\u043e\u0442\u043a(\u0456\u0432|\u0430|\u0438)]",
-        "name": "{name}",
-        "temperature": "{temperature} [\u0433\u0440\u0430\u0434\u0443\u0441(\u0456\u0432|\u0438|\u0430)] [{temperature_unit}]",
-        "\u0432\u0432\u0456\u043c\u043a\u043d\u0438": "(\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0438 | \u0432\u043a\u043b\u044e\u0447\u0438",
-        "\u0432\u0438\u043c\u043a\u043d\u0438": "\u0432\u0438\u043c\u043a\u043d\u0438 | \u0432\u0438\u043a\u043b\u044e\u0447\u0438",
-        "\u0432\u0456\u0434\u043a\u0440\u0438\u0439": "\u0432\u0456\u0434\u043a\u0440\u0438\u0439 | \u0440\u043e\u0437\u043a\u0440\u0438\u0439 | \u043f\u0456\u0434\u043d\u0456\u043c\u0438 | \u0432\u0456\u0434\u0447\u0438\u043d\u0438",
-        "\u0437\u0430\u043a\u0440\u0438\u0439": "\u0437\u0430\u043a\u0440\u0438\u0439 | \u043e\u043f\u0443\u0441\u0442\u0438 | \u0437\u0430\u0447\u0438\u043d\u0438",
-        "\u0437\u043c\u0456\u043d\u0438": "\u0437\u043c\u0456\u043d\u0438 | \u0432\u0441\u0442\u0430\u043d\u043e\u0432\u0438 | \u0437\u0440\u043e\u0431\u0438"
+        "all": "(\u0643\u0644|\u062c\u0645\u064a\u0639)",
+        "area": "[\u0627\u0644]{area}",
+        "awning": "[\u0627\u0644](\u0645\u0638\u0644\u0629|\u0645\u0638\u0644\u0627\u062a)",
+        "brightness": "{brightness}[% | \u0628\u0627\u0644\u0645\u0627\u0626\u0629]",
+        "close": "(\u0627\u063a\u0644\u0642|\u0627\u0642\u0641\u0644|\u0627\u062e\u0641\u0636|\u0627\u0646\u0632\u0644|\u0646\u0632\u0644)",
+        "color": "[\u0627\u0644](\u0644\u0648\u0646|\u0627\u0644\u0648\u0627\u0646)",
+        "colors": "[\u0627\u0644]{color}",
+        "curtain": "[\u0627\u0644](\u0633\u062a\u0627\u0626\u0631|\u0633\u062a\u0627\u0631\u0629|\u0633\u062a\u0627\u0631\u0627\u062a)",
+        "door": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628)",
+        "fan": "[\u0627\u0644](\u0645\u0631\u0648\u062d\u0629|\u0645\u0631\u0627\u0648\u062d|\u0645\u0631\u0648\u062d\u0627\u062a)",
+        "garage": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628|\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a) [\u0627\u0644]\u062c\u0631\u0627\u062c",
+        "gate": "[\u0627\u0644](\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a)",
+        "in": "(\u0641\u064a|\u062f\u0627\u062e\u0644)",
+        "intensity": "[\u0627\u0644](\u062f\u0631\u062c\u0629 [\u0627\u0644]\u0633\u0637\u0648\u0639|[\u0634\u062f\u0629] [\u0627\u0644]\u0633\u0637\u0648\u0639|\u0642\u0648\u0629|\u0634\u062f\u0629)",
+        "light": "[\u0627\u0644](\u0627\u0636\u0648\u0627\u0621|\u0627\u0636\u0627\u0621\u0629|\u0636\u0648\u0621|\u0645\u0635\u0627\u0628\u064a\u062d|\u0645\u0635\u0628\u0627\u062d|\u0627\u0646\u0648\u0627\u0631|\u0646\u0648\u0631|\u0644\u0645\u0628\u0629|\u0644\u0645\u0628\u0627\u062a|\u0627\u0646\u0648\u0627\u0631)",
+        "name": "[\u0627\u0644]{name}",
+        "open": "(\u0627\u0641\u062a\u062d|\u0627\u0631\u0641\u0639)",
+        "script": "[\u0627\u0644](\u0628\u0631\u0646\u0627\u0645\u062c|\u0628\u0631\u0627\u0645\u062c|\u0645\u0633\u0627\u0631|\u0645\u0633\u0627\u0631\u0627\u062a|\u0633\u064a\u0646\u0627\u0631\u064a\u0648)",
+        "switch": "[\u0627\u0644](\u0645\u0641\u062a\u0627\u062d|\u0645\u0641\u0627\u062a\u064a\u062d)",
+        "temp": "(\u0628\u0627\u0631\u062f\u0629|\u062f\u0627\u0641\u0626\u0629|\u0644\u0637\u064a\u0641\u0629|\u062d\u0627\u0631\u0629|\u062f\u0631\u062c\u0629 [\u0627\u0644]\u062d\u0631\u0627\u0631\u0629)",
+        "temperature": "{temperature}[\u00b0| \u062f\u0631\u062c\u0629] [{temperature_unit}]",
+        "turn": "(\u063a\u064a\u0631|\u0627\u0636\u0628\u0637|\u0636\u0628\u0637)",
+        "turn_off": "(\u0627\u063a\u0644\u0642|\u0627\u0637\u0641\u0626|\u0637\u0641\u064a)",
+        "turn_on": "(\u0627\u0641\u062a\u062d|\u0634\u063a\u0644|\u0627\u0634\u0639\u0644|\u0627\u0634\u063a\u0644|\u0627\u0628\u062f\u0623|\u0634\u0639\u0644|\u0641\u0639\u0644|\u062a\u0641\u0639\u064a\u0644|\u062a\u0634\u063a\u064a\u0644|\u0641\u0639\u0644)",
+        "what_is": "(\u0645\u0627 \u0647\u0648|\u0645\u0627 \u0647\u064a|\u0645\u0627\u0630\u0627 \u064a\u0643\u0648\u0646|\u0645\u0627\u0630\u0627 \u062a\u0643\u0648\u0646|\u0643\u0645 \u0647\u064a|\u0643\u0645 \u0647\u0648|\u0647\u0644 \u0647\u064a|\u0647\u0644 \u0647\u0648)",
+        "window": "[\u0627\u0644](\u0646\u0627\u0641\u0630\u0629|\u0646\u0648\u0627\u0641\u0630|\u0646\u0627\u0641\u0630\u0627\u062a|\u0634\u0628\u0627\u0643|\u0634\u0628\u0627\u0628\u064a\u0643)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "response": "one",
-                    "sentences": [
-                        "\u0449\u043e \u0437 <name> [<area>]",
-                        "\u044f\u043a\u0438\u0439 \u0441\u0442\u0430\u043d <name> [<area>]",
-                        "\u0432 \u044f\u043a\u043e\u043c\u0443 \u0441\u0442\u0430\u043d\u0456 <name> [<area>]"
-                    ]
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "cover"
-                        ]
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "\u0447\u0438 {on_off_states:state} <name> [<area>]"
-                    ]
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "\u0447\u0438 \u0454 {on_off_states:state} {on_off_domains:domain} [<area>]"
-                    ]
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "\u0447\u0438 \u0432\u0441[\u0456|\u0435] {on_off_domains:domain} {on_off_states:state} [<area>]"
-                    ]
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "(\u044f\u043a\u0456|\u043a\u043e\u0442\u0440\u0456) {on_off_domains:domain} {on_off_states:state} [<area>]"
-                    ]
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {on_off_domains:domain} [<area>] {on_off_states:state}",
-                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438 [\u0454]|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {on_off_states:state} {on_off_domains:domain} [<area>]"
-                    ]
-                },
-                {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "\u0447\u0438 {cover_states:state} <name> [<area>]"
+                        "\u0647\u0644 <name> {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "\u0447\u0438 \u0454 {cover_states:state} {cover_classes:device_class} [<area>]"
+                        "\u0647\u0644 \u0647\u0646\u0627\u0643 {cover_classes:device_class} {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "\u0447\u0438 \u0432\u0441\u0456 {cover_classes:device_class} {cover_states:state} [<area>]"
+                        "\u0647\u0644 \u062c\u0645\u064a\u0639 {cover_classes:device_class} {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(\u044f\u043a\u0456|\u043a\u043e\u0442\u0440\u0456) {cover_classes:device_class} {cover_states:state} [<area>]"
+                        "\u0627\u064a {cover_classes:device_class} {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {cover_classes:device_class} {cover_states:state} [<area>]",
-                        "(\u0441\u043a\u0456\u043b\u044c\u043a\u0438 [\u0454]|\u044f\u043a\u0430 \u043a\u0456\u043b\u044c\u043a\u0456\u0441\u0442\u044c) {cover_states:state} {cover_classes:device_class} [<area>]"
+                        "(\u0643\u0645|\u0645\u0627|\u0645\u0627\u0647\u0648|\u0645\u0627\u0630\u0627) [\u0639\u062f\u062f] {cover_classes:device_class} [\u0627\u0644\u0644\u062a\u064a] {cover_states:state} [<in> <area>]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
-                    "response": "lights_area",
                     "sentences": [
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <area>",
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
+                        "<turn_off> [<all>] <fan> [<in>] <area>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> [\u0434\u0432\u0435\u0440\u0456] [\u0443|\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> \u0433\u0430\u0440\u0430\u0436\u043d\u0456 \u0434\u0432\u0435\u0440\u0456"
+                        "<turn_off> [<all>] <fan>"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "response": "default",
+                    "sentences": [
+                        "<turn_off> [<light> | <switch>] <name>"
+                    ]
+                },
+                {
+                    "response": "lights_area",
                     "sentences": [
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438)) <area>",
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <area> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438))"
+                        "<turn_off> [<all>] <light> [<in>] <area>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter",
-                            "window"
-                        ],
-                        "domain": "cover"
+                        "domain": "light",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "fans_area",
+                    "response": "light_all",
                     "sentences": [
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438] <area>",
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438]",
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e <area>",
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e"
+                        "<turn_off> [<all>] <light>"
                     ],
                     "slots": {
-                        "domain": "fan",
+                        "area": "all",
+                        "domain": "light",
                         "name": "all"
                     }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
                     "sentences": [
-                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <name>"
+                        "<close> <name> [<in> <area>]"
                     ]
                 },
                 {
-                    "response": "cover",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <name>"
-                    ]
+                        "<close> \u0628\u0627\u0628 \u0627\u0644\u062c\u0631\u0627\u062c"
+                    ],
+                    "slots": {
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0437\u0430\u043a\u0440\u0438\u0439> <name> <area>"
-                    ]
+                        "<close> {cover_classes:device_class} [<in>] <area>"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "response": "lights_area",
                     "sentences": [
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <name>"
-                    ]
+                        "<turn_on> [<all>] <light> [<in>] <area>"
+                    ],
+                    "slots": {
+                        "domain": "light",
+                        "name": "all"
+                    }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
                     "response": "cover",
                     "sentences": [
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <name> <area>"
+                        "<open> <name> [<in>] [<area>]"
                     ]
                 },
                 {
-                    "response": "fans_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438] <area>",
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438]",
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e <area>",
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e"
+                        "<open> \u0628\u0627\u0628 \u0627\u0644\u062c\u0631\u0627\u062c"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "lights_area",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <area>",
-                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
+                        "<open> {cover_classes:device_class} <in> <area>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_device_class",
                     "sentences": [
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> [\u0434\u0432\u0435\u0440\u0456] [\u0443|\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> \u0433\u0430\u0440\u0430\u0436\u043d\u0456 \u0434\u0432\u0435\u0440\u0456"
+                        "<turn_on> [<all>] <fan> [<in>] <area>"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
                     "sentences": [
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438)) <area>",
-                        "<\u0432\u0456\u0434\u043a\u0440\u0438\u0439> <area> [\u0432\u0441\u0456] (\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0436\u0430\u043b\u044e\u0437\u0456 | \u0448\u0442\u043e\u0440(\u0443|\u0438))"
+                        "[<turn_on>] [<script>] <name>",
+                        "[<script>] <name> <turn_on>"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter",
-                            "window"
-                        ],
-                        "domain": "cover"
+                        "domain": "script"
                     }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "response": "default",
+                    "sentences": [
+                        "<turn_on> [<light> | <switch>] <name>"
+                    ]
                 }
             ]
         }
     },
-    "language": "uk",
+    "language": "ar",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
+        "brightness_level": {
+            "values": [
+                {
+                    "in": "(\u0639\u0627\u0644\u064a|\u0642\u0635\u0648\u0649)",
+                    "out": 100
+                },
+                {
+                    "in": "\u0645\u0646\u062e\u0641\u0636",
+                    "out": 1
+                }
+            ]
+        },
         "color": {
             "values": [
                 {
-                    "in": "\u0431\u0456\u043b\u0438\u0439 | \u0431\u0456\u043b(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0627\u0628\u064a\u0636",
                     "out": "white"
                 },
                 {
-                    "in": "\u0447\u043e\u0440\u043d\u0438\u0439 | \u0447\u043e\u0440\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0627\u0633\u0648\u062f",
                     "out": "black"
                 },
                 {
-                    "in": "\u0447\u0435\u0440\u0432\u043e\u043d\u0438\u0439 | \u0447\u0435\u0440\u0432\u043e\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0627\u062d\u0645\u0631",
                     "out": "red"
                 },
                 {
-                    "in": "\u043f\u043e\u043c\u0430\u0440\u0430\u043d\u0447\u0435\u0432\u0438\u0439 | \u043f\u043e\u043c\u0430\u0440\u0430\u043d\u0447\u0435\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0628\u0631\u062a\u0642\u0627\u0644\u064a",
                     "out": "orange"
                 },
                 {
-                    "in": "\u0436\u043e\u0432\u0442\u0438\u0439 | \u0436\u043e\u0432\u0442(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0627\u0635\u0641\u0631",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u0437\u0435\u043b\u0435\u043d\u0438\u0439 | \u0437\u0435\u043b\u0435\u043d(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0627\u062e\u0636\u0631",
                     "out": "green"
                 },
                 {
-                    "in": "\u0441\u0438\u043d\u0456\u0439 | \u0441\u0438\u043d(\u0456\u043c|\u044c\u043e\u044e|\u044c\u043e\u0433\u043e)",
+                    "in": "\u0627\u0632\u0631\u0642",
                     "out": "blue"
                 },
                 {
-                    "in": "\u0444\u0456\u043e\u043b\u0435\u0442\u043e\u0432\u0438\u0439 | \u0444\u0456\u043e\u043b\u0435\u0442\u043e\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0628\u0646\u0641\u0633\u062c\u064a",
                     "out": "purple"
                 },
                 {
-                    "in": "\u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u0438\u0439 | \u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432(\u0438\u043c|\u043e\u044e|\u043e\u0433\u043e)",
+                    "in": "\u0628\u0646\u064a",
                     "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "awning[s]",
+                    "in": "<awning>",
                     "out": "awning"
                 },
                 {
-                    "in": "\u0436\u0430\u043b\u044e\u0437\u0456",
-                    "out": "blind"
-                },
-                {
-                    "in": "\u0448\u0442\u043e\u0440[\u0430|\u0438]",
+                    "in": "<curtain>",
                     "out": "curtain"
                 },
                 {
-                    "in": "\u0434\u0432\u0435\u0440\u0456 | \u0434\u0432\u0435\u0440\u0435\u0439",
+                    "in": "<door>",
                     "out": "door"
                 },
                 {
-                    "in": "\u0434\u0432\u0435\u0440[\u0456|\u0435\u0439] [\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
+                    "in": "<garage>",
                     "out": "garage"
                 },
                 {
-                    "in": "\u0431\u0440\u0430\u043c[\u0430|\u0438] | \u0432\u043e\u0440(\u043e|\u0456)\u0442[\u0430]",
+                    "in": "<gate>",
                     "out": "gate"
                 },
                 {
-                    "in": "shade[s]",
-                    "out": "shade"
-                },
-                {
-                    "in": "\u0441\u0442\u0430\u0432\u043d\u0456 | \u0441\u0442\u0430\u0432\u0435\u043d\u044c",
-                    "out": "shutter"
-                },
-                {
-                    "in": "\u0432\u0456\u043a\u043d(\u043e|\u0430) | \u0432\u0456\u043a\u043e\u043d",
+                    "in": "<window>",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "\u0432\u0456\u0434\u043a\u0440\u0438\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e) | \u043f\u0456\u0434\u043d\u044f\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "in": "\u0645\u0641\u062a\u0648\u062d",
                     "out": "open"
                 },
                 {
-                    "in": "\u0437\u0430\u043a\u0440\u0438\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e) | \u043e\u043f\u0443\u0449\u0435(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "in": "(\u0645\u063a\u0644\u0642|\u0645\u0642\u0641\u0648\u0644)",
                     "out": "closed"
                 },
                 {
-                    "in": "\u0432\u0456\u0434\u043a\u0440\u0438\u0432\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f | \u043f\u0456\u0434\u043d\u0456\u043c\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f",
+                    "in": "\u064a\u0641\u062a\u062d",
                     "out": "opening"
                 },
                 {
-                    "in": "\u0437\u0430\u043a\u0440\u0438\u0432\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f | \u043e\u043f\u0443\u0441\u043a\u0430(\u0454|\u044e)\u0442\u044c\u0441\u044f",
+                    "in": "\u064a\u063a\u0644\u0642",
                     "out": "closing"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "\u0441\u0432\u0456\u0442\u043b\u043e|\u0441\u0432\u0456\u0442\u0438\u043b\u044c\u043d\u0438\u043a[\u0438|\u0456\u0432]|\u043b\u0430\u043c\u043f[\u0438]",
+                    "in": "<light>",
                     "out": "light"
                 },
                 {
-                    "in": "\u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0430|\u0438|\u0456\u0432]",
+                    "in": "<fan>",
                     "out": "fan"
                 },
                 {
-                    "in": "\u0432\u043c\u0438\u043a\u0430\u0447[\u0430|\u0456|\u0456\u0432] | \u0432\u0438\u043c\u0438\u043a\u0430\u0447[\u0430|\u0456|\u0456\u0432]",
+                    "in": "<switch>",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "(\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0435\u043d(\u0438\u0439|\u043d\u0430|\u0456|\u0438\u0445|\u043e) | (\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0443\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "in": "\u0634\u063a\u0644",
                     "out": "on"
                 },
                 {
-                    "in": "\u0432\u0438\u043c\u043a\u043d\u0435\u043d(\u0438\u0439|\u043d\u0430|\u0456|\u0438\u0445|\u043e) | \u0432\u0438\u043c\u043a\u043d\u0443\u0442(\u0438\u0439|\u0430|\u0456|\u0438\u0445|\u043e)",
+                    "in": "\u0627\u0637\u0641\u064a",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
+                "\u0645\u0626\u0648\u064a\u0629",
                 {
-                    "in": "c | \u0446\u0435\u043b\u044c\u0441\u0456\u044e | \u0437\u0430 \u0446\u0435\u043b\u044c\u0441\u0456\u0454\u043c",
+                    "in": "c",
                     "out": "celsius"
                 },
+                "\u0641\u0647\u0631\u0646\u0647\u0627\u064a\u062a",
                 {
-                    "in": "f | \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u0443 | \u0437\u0430 \u0444\u0430\u0440\u0435\u043d\u0433\u0435\u0439\u0442\u043e\u043c",
+                    "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u041d\u0435\u043e\u0447\u0456\u043a\u0443\u0432\u0430\u043d\u0430 \u043f\u043e\u043c\u0438\u043b\u043a\u0430 \u0432\u0438\u043d\u0438\u043a\u043b\u0430 \u043f\u0456\u0434 \u0447\u0430\u0441 \u0432\u0438\u043a\u043e\u043d\u0430\u043d\u043d\u044f \u0437\u0430\u043f\u0438\u0442\u0443",
-            "no_area": "\u041d\u0435\u043c\u0430\u0454 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f \u043f\u0456\u0434 \u043d\u0430\u0437\u0432\u043e\u044e {{ area }}",
-            "no_device_class": "\u041f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f {{ area }} \u043d\u0435 \u043c\u0456\u0441\u0442\u0438\u0442\u044c {{ device_class }}",
-            "no_domain": "\u041f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f {{ area }} \u043d\u0435 \u043c\u0456\u0441\u0442\u0438\u0442\u044c {{ domain }}",
-            "no_entity": "\u041d\u0435\u043c\u0430\u0454 \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u044e \u0447\u0438 \u0441\u0443\u0442\u043d\u043e\u0441\u0442\u0456 \u043f\u0456\u0434 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }}",
-            "no_intent": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u044f \u0446\u044c\u043e\u0433\u043e \u043d\u0435 \u0440\u043e\u0437\u0443\u043c\u0456\u044e"
+            "handle_error": "\u062d\u062f\u062b \u062e\u0637\u0623 \u0627\u062b\u0646\u0627\u0621 \u0645\u0639\u0627\u0644\u062c\u0629 \u0627\u0644\u0646\u0635",
+            "no_area": "\u0644\u0627 \u062a\u0648\u062c\u062f \u0645\u0646\u0637\u0642\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ area }}",
+            "no_device_class": "\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }} \u0644\u0627 \u062a\u062d\u062a\u0648\u0649 \u0639\u0644\u0649 \u0641\u0626\u0629 \u0627\u0644\u0623\u062c\u0647\u0632\u0629 {{ device_class }}",
+            "no_domain": "\u0627\u0644\u0646\u0637\u0627\u0642 {{ domain }} \u063a\u064a\u0631 \u0645\u0648\u062c\u0648\u062f \u0628\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }}",
+            "no_entity": "\u0644\u0627 \u064a\u0648\u062c\u062f \u062c\u0647\u0627\u0632 \u0627\u0648 \u062e\u0627\u0635\u064a\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ entity }}",
+            "no_intent": "\u0639\u0641\u0648\u0627, \u0644\u0645 \u0627\u0641\u0647\u0645 \u0647\u0630\u0627"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  \u0422\u0430\u043a\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u041d\u0456, {{ no_match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (no_match | length - 3) }} \u043d\u0456\n  {%- else -%}\n    \u041d\u0456,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor %} \u043d\u0456\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0422\u0430\u043a, {{ match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (match | length - 3) }}\n  {%- else -%}\n    \u0422\u0430\u043a,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u041d\u0456\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  \u0627\u062c\u0644\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u0644\u0627, {{ no_match[:3] | join(\", \") }} \u0648 {{ (no_match | length - 3) }} \u0627\u064a\u0636\u0627\n  {%- else -%}\n    \u0644\u0627,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor %} \u0644\u064a\u0633\u062a\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0627\u062c\u0644, {{ match[:3] | join(\", \") }} \u0648 {{ (match | length - 3) }} \u0627\u064a\u0636\u0627\n  {%- else -%}\n    \u0627\u062c\u0644,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u0644\u0627\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "{{ slots.name | capitalize }} {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  \u0422\u0430\u043a\n{% else %}\n  \u041d\u0456, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  \u0442\u0430\u043a\u0438\u0445 \u043d\u0435\u043c\u0430\u0454\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0456 \u0449\u0435 {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0456 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
+                "one": "{{ slots.name | capitalize }} \u0647\u0648 {{ state.state_with_unit }}\n",
+                "one_yesno": "{% if query.matched %}\n  \u0627\u062c\u0644\n{% else %}\n  \u0644\u0627, {{ state.state_with_unit }}\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u0644\u0627 \u064a\u0648\u062c\u062f\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0648 {{ (match | length - 3) }} \u0627\u064a\u0636\u0627\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "{{ slots.name }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
-                "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
-                "cover_device_class": "{{ slots.device_class }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
-                "default": "{{ slots.name }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
-                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
-                "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e"
+                "cover": "\u062a\u0645 \u0627\u0644\u0627\u063a\u0644\u0627\u0642",
+                "cover_device_class": "\u062a\u0645 \u0627\u063a\u0644\u0627\u0642 {{ slots.device_class }}",
+                "default": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 {{state.domain}}",
+                "fan_all": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u062c\u0645\u064a\u0639 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
+                "fans_area": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
+                "light_all": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u062c\u0645\u064a\u0639 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
+                "lights_area": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
+                "lock": "\u062a\u0645 \u0627\u0644\u0641\u062a\u062d"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
-                "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
-                "cover_device_class": "{{ slots.device_class }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
-                "default": "{{ slots.name }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
-                "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
-                "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e"
+                "cover": "\u062a\u0645 \u0627\u0644\u0641\u062a\u062d",
+                "cover_device_class": "\u062a\u0645 \u0641\u062a\u062d {{ slots.device_class }}",
+                "default": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 {{state.domain}}",
+                "fans_area": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
+                "lights_area": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
+                "lock": "\u062a\u0645 \u0627\u0644\u0642\u0641\u0644",
+                "scene": "\u062a\u0645 \u0627\u0644\u062a\u0641\u0639\u064a\u0644",
+                "script": "\u062a\u0645 \u0627\u0644\u0628\u062f\u0621"
             }
         }
     },
     "skip_words": [
-        "\u0431\u0443\u0434\u044c \u043b\u0430\u0441\u043a\u0430",
-        "\u0437\u0430\u0440\u0430\u0437",
-        "\u0441\u044c\u043e\u0433\u043e\u0434\u043d\u0456"
+        "(\u0645\u0646 \u0641\u0636\u0644\u0643|\u0644\u0648 \u0633\u0645\u062d\u062a)",
+        "(\u0647\u0644 \u064a\u0645\u0643\u0646\u0643|\u062a\u0642\u062f\u0631)"
     ]
 }
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/vi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931106701940036%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {0: {'sentences': ['<turn> [toàn bộ | tất cả] đèn [trong | "*

 * *              "bên trong] <area>', '<turn> đèn <area>'], 'slots': OrderedDict([('domain', "*

 * *              "'light')])}, 1: {'sentences': ['mở cửa cuốn'], 'response': 'cover_device_class', "*

 * *              "'slots': OrderedDict([('device_class', 'garage_door'), ('domain', 'cover')])}, 2: "*

 * *              "{'sentences': ['mở rèm cuốn trong <area>'], 'slots': OrderedDict([('device_class', "*

 * *              "['window […]*

```diff
@@ -107,34 +107,14 @@
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "<turn_off> [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] (\u0111\u00e8n) trong <area>",
-                        "<turn_off> [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] \u0111\u00e8n <area>",
-                        "<turn_off> \u0111\u00e8n <area>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "\u0111\u00f3ng c\u1eeda cu\u1ed1n"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "sentences": [
                         "t\u1eaft <name> <area>",
                         "t\u1eaft <name> [trong]  <area>",
                         "t\u1eaft [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] <name> [trong] <area>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
@@ -159,46 +139,39 @@
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
                         "\u0111\u00f3ng h\u1ebft <name> <area>",
                         "k\u00e9o to\u00e0n b\u1ed9 <name> trong <area> xu\u1ed1ng"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
-                {
-                    "sentences": [
-                        "b\u1eadt <name>"
-                    ]
                 },
                 {
-                    "response": "cover",
                     "sentences": [
-                        "m\u1edf <name>"
-                    ]
-                },
-                {
-                    "response": "cover_area",
-                    "sentences": [
-                        "m\u1edf <name> trong <area>"
-                    ]
+                        "<turn_off> [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] (\u0111\u00e8n) trong <area>",
+                        "<turn_off> [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] \u0111\u00e8n <area>",
+                        "<turn_off> \u0111\u00e8n <area>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
+                    "response": "cover_device_class",
                     "sentences": [
-                        "b\u1eadt <name> <area>",
-                        "b\u1eadt [h\u1ebft | t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] <name> <area>"
+                        "\u0111\u00f3ng c\u1eeda cu\u1ed1n"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
                     "sentences": [
                         "<turn> [to\u00e0n b\u1ed9 | t\u1ea5t c\u1ea3] \u0111\u00e8n [trong | b\u00ean trong] <area>",
                         "<turn> \u0111\u00e8n <area>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -224,14 +197,41 @@
                             "window",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
+                },
+                {
+                    "sentences": [
+                        "b\u1eadt <name> <area>",
+                        "b\u1eadt [h\u1ebft | t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] <name> <area>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "sentences": [
+                        "b\u1eadt <name>"
+                    ]
+                },
+                {
+                    "response": "cover",
+                    "sentences": [
+                        "m\u1edf <name>"
+                    ]
+                },
+                {
+                    "response": "cover_area",
+                    "sentences": [
+                        "m\u1edf <name> trong <area>"
+                    ]
                 }
             ]
         }
     },
     "language": "vi",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908163265306122%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(11, OrderedDict([('sentences', "*

 * *              "['[<area>]{name}(是不是|有没有){lock_states:state}', "*

 * *              "'[<area>]{name}[是|有]{lock_states:state}[吗|不]']), ('response', 'one_yesno'), "*

 * *              "('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])), (12, OrderedDict([('sentences', "*

 * *              "['[{area}][有|有没有](门|锁|门锁)[是]{lock_states:state}[吗|不]', "*

 * *              "'{area}(门|锁 […]*

```diff
@@ -18,68 +18,14 @@
         "what_is": "\u662f\u4ec0\u4e48",
         "which": "[\u6709|\u6709\u6ca1\u6709|\u6709\u7121]\u54ea[\u4e00](\u4e2a|\u4e9b)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "[<area>]{name}(\u662f\u4e0d\u662f|\u6709\u6ca1\u6709){lock_states:state}",
-                        "[<area>]{name}[\u662f|\u6709]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "[{area}][\u6709|\u6709\u6ca1\u6709](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}[\u5417|\u4e0d]",
-                        "{area}(\u95e8|\u9501|\u95e8\u9501)[\u6709|\u6709\u6ca1\u6709]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "[<area>][<all>](\u95e8|\u9501|\u95e8\u9501)[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{lock_states:state}[\u5417|\u4e0d]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "[<area>](<which>|\u54ea[\u4e00]\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "(<which>|\u54ea[\u4e00]\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "<area>(\u95e8|\u9501|\u95e8\u9501)(<which>|\u54ea[\u4e00]\u6247)[\u662f]{lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "[{area}](<how_many_is>|\u6709\u51e0\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "(<how_many_is>|\u6709\u51e0\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
-                        "{area}(\u95e8|\u9501|\u95e8\u9501)(<how_many_is>|\u6709\u51e0\u6247)[\u662f]{lock_states:state}"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "one",
@@ -172,20 +118,101 @@
                     "sentences": [
                         "[{area}]<how_many_is>{cover_classes:device_class}[\u662f]{cover_states:state}",
                         "<how_many_is>[<area>]{cover_classes:device_class}[\u662f]{cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "[<area>]{name}(\u662f\u4e0d\u662f|\u6709\u6ca1\u6709){lock_states:state}",
+                        "[<area>]{name}[\u662f|\u6709]{lock_states:state}[\u5417|\u4e0d]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "[{area}][\u6709|\u6709\u6ca1\u6709](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}[\u5417|\u4e0d]",
+                        "{area}(\u95e8|\u9501|\u95e8\u9501)[\u6709|\u6709\u6ca1\u6709]{lock_states:state}[\u5417|\u4e0d]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "[<area>][<all>](\u95e8|\u9501|\u95e8\u9501)[\u662f|\u662f\u4e0d\u662f]\u90fd[\u662f]{lock_states:state}[\u5417|\u4e0d]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "[<area>](<which>|\u54ea[\u4e00]\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "(<which>|\u54ea[\u4e00]\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "<area>(\u95e8|\u9501|\u95e8\u9501)(<which>|\u54ea[\u4e00]\u6247)[\u662f]{lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "[{area}](<how_many_is>|\u6709\u51e0\u6247)(\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "(<how_many_is>|\u6709\u51e0\u6247)[<area>](\u95e8|\u9501|\u95e8\u9501)[\u662f]{lock_states:state}",
+                        "{area}(\u95e8|\u9501|\u95e8\u9501)(<how_many_is>|\u6709\u51e0\u6247)[\u662f]{lock_states:state}"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_off><area>(\u98ce\u6247|\u540a\u6247)",
+                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_off>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<turn_off>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_off>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_off><area><light>",
                         "[<let>]<area><light><turn_off>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -236,41 +263,14 @@
                         "[\u6253|\u89e3]\u5f00<area>[<all>][\u95e8]\u9501",
                         "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u6253\u5f00|\u89e3\u9501)",
                         "{area}(\u5f00|\u89e3)\u9501"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_off><area>(\u98ce\u6247|\u540a\u6247)",
-                        "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_off>"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
-                    "sentences": [
-                        "<turn_off>[<area>]{name}",
-                        "[<let>][<area>]{name}<turn_off>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "requires_context": {
@@ -282,69 +282,82 @@
                         "<name>[\u573a\u666f|\u6a21\u5f0f]\u5f00\u542f"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
-                    },
+                    "response": "lights_area",
                     "sentences": [
-                        "<turn_on>[<area>]{name}",
-                        "[<let>][<area>]{name}<turn_on>"
-                    ]
+                        "<turn_on><area><light>",
+                        "[<let>]<area><light><turn_on>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
                     "requires_context": {
-                        "domain": "lock"
+                        "domain": "cover"
                     },
-                    "response": "lock",
                     "sentences": [
-                        "\u5173(\u95ed|\u4e0a)[<area>]{name}[[\u7684]\u9501]",
-                        "[<let>][<area>]{name}[[\u7684]\u9501](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)"
+                        "<open>[<area>]{name}",
+                        "[<let>][<area>]{name}<open>"
                     ]
                 },
                 {
-                    "response": "lock",
                     "sentences": [
-                        "\u5173(\u95ed|\u4e0a)<area>[<all>][\u95e8]\u9501",
-                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)",
-                        "{area}(\u4e0a|\u5173)\u9501"
+                        "<open>\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8",
+                        "[<let>]\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8<open>"
                     ],
                     "slots": {
-                        "domain": "lock"
+                        "device_class": "garage",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover_device_class",
+                    "sentences": [
+                        "<open>[<area>]{cover_classes:device_class}",
+                        "[<let>][<area>]{cover_classes:device_class}<open>"
+                    ],
+                    "slots": {
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area",
                     "sentences": [
                         "<turn_on><area>(\u98ce\u6247|\u540a\u6247)",
                         "[<let>]<area>(\u98ce\u6247|\u540a\u6247)<turn_on>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "lights_area",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
                     "sentences": [
-                        "<turn_on><area><light>",
-                        "[<let>]<area><light><turn_on>"
+                        "\u5173(\u95ed|\u4e0a)[<area>]{name}[[\u7684]\u9501]",
+                        "[<let>][<area>]{name}[[\u7684]\u9501](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)"
+                    ]
+                },
+                {
+                    "response": "lock",
+                    "sentences": [
+                        "\u5173(\u95ed|\u4e0a)<area>[<all>][\u95e8]\u9501",
+                        "[<let>]<area>[<all>][\u95e8]\u9501[\u90fd](\u5173(\u95ed|\u4e0a)|\u4e0a\u9501)",
+                        "{area}(\u4e0a|\u5173)\u9501"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "lock"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "script"
                     },
                     "response": "script",
@@ -352,41 +365,28 @@
                         "[\u8fd0\u884c|\u6267\u884c]<name>[\u811a\u672c]"
                     ],
                     "slots": {
                         "domain": "script"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
                     },
                     "sentences": [
-                        "<open>[<area>]{name}",
-                        "[<let>][<area>]{name}<open>"
+                        "<turn_on>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_on>"
                     ]
-                },
-                {
-                    "sentences": [
-                        "<open>\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8",
-                        "[<let>]\u8f66\u5e93[\u7684][\u5927|\u5377\u95f8]\u95e8<open>"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<open>[<area>]{cover_classes:device_class}",
-                        "[<let>][<area>]{cover_classes:device_class}<open>"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
                 }
             ]
         }
     },
     "language": "zh-cn",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'intents'": "{'HassTurnOn': {'data': {insert: [(4, OrderedDict([('sentences', "*

 * *              "['<turn_on><area>(風扇|吊扇)']), ('slots', OrderedDict([('domain', 'fan'), ('name', "*

 * *              "'all')])), ('response', 'fans_area')])), (5, OrderedDict([('sentences', "*

 * *              "['<turn_on>[<area>]{name}', '[<let>][<area>]{name}<turn_on>']), "*

 * *              "('excludes_context', OrderedDict([('domain', 'cover')]))]))], delete: [1, 0]}}, "*

 * *              "'HassTurnOff': {'data': {insert: [(0, OrderedDict([ […]*

```diff
@@ -118,14 +118,33 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_off> <area> (\u98a8\u6247 | \u540a\u6247)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": "cover"
+                    },
+                    "sentences": [
+                        "<turn_off>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_off>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_off> <area> <light>",
                         "[<let>] <area> <light> <turn_off>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -155,58 +174,20 @@
                     "sentences": [
                         "<close>[<area>]{cover_classes:device_class}",
                         "[<let>][<area>]{cover_classes:device_class}<close>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_off> <area> (\u98a8\u6247 | \u540a\u6247)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "excludes_context": {
-                        "domain": "cover"
-                    },
-                    "sentences": [
-                        "<turn_off>[<area>]{name}",
-                        "[<let>][<area>]{name}<turn_off>"
-                    ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
-                    "excludes_context": {
-                        "domain": "cover"
-                    },
-                    "sentences": [
-                        "<turn_on>[<area>]{name}",
-                        "[<let>][<area>]{name}<turn_on>"
-                    ]
-                },
-                {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_on><area>(\u98a8\u6247|\u540a\u6247)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_on> <area> <light>",
                         "[<let>] <area> <light> <turn_on>"
                     ],
                     "slots": {
                         "domain": "light"
@@ -236,14 +217,33 @@
                     "sentences": [
                         "<open>[<area>]{cover_classes:device_class}",
                         "[<let>][<area>]{cover_classes:device_class}<open>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_on><area>(\u98a8\u6247|\u540a\u6247)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": "cover"
+                    },
+                    "sentences": [
+                        "<turn_on>[<area>]{name}",
+                        "[<let>][<area>]{name}<turn_on>"
+                    ]
                 }
             ]
         }
     },
     "language": "zh-hk",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928246819561158%*

 * *Differences: {"'intents'": "{'HassGetState': {'data': {insert: [(41, OrderedDict([('sentences', "*

 * *              "['[<area>][<name>][(是|是不是)]{lock_states:state}[著][(的|了)][嗎]']), ('response', "*

 * *              "'one_yesno'), ('requires_context', OrderedDict([('domain', 'lock')])), ('slots', "*

 * *              "OrderedDict([('domain', 'lock')]))])), (42, OrderedDict([('sentences', "*

 * *              "['[<area>][(有 | 有沒有 | 有任何)][<door>][是] [沒有]{lock_states:state}[著][的][嗎]']), "*

 * *              "('response', 'any'), ('slots', OrderedD […]*

```diff
@@ -26,62 +26,14 @@
         "window": "(\u7a97\u6236 | \u7a97\u7c3e | \u6372\u7c3e | \u7f85\u99ac\u7c3e  | \u767e\u8449\u7a97)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
-                        "domain": "lock"
-                    },
-                    "response": "one_yesno",
-                    "sentences": [
-                        "[<area>][<name>][(\u662f|\u662f\u4e0d\u662f)]{lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "[<area>][(\u6709 | \u6709\u6c92\u6709 | \u6709\u4efb\u4f55)][<door>][\u662f] [\u6c92\u6709]{lock_states:state}[\u8457][\u7684][\u55ce]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "all",
-                    "sentences": [
-                        "[<area>][<all>][<door>][(\u90fd|\u90fd\u662f|\u662f|\u662f\u4e0d\u662f)]{lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "which",
-                    "sentences": [
-                        "[<area>] [<which>][<door>][\u662f] {lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "response": "how_many",
-                    "sentences": [
-                        "[<area>]<how_many>[(\u6247|\u9053)][<door>][\u662f]{lock_states:state}[\u8457][\u7684][\u55ce]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
-                },
-                {
-                    "requires_context": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     },
                     "response": "one_yesno",
                     "sentences": [
                         "[<area>]<name>\u96fb\u91cf[(\u76ee\u524d | \u73fe\u5728)]{bs_battery_states:state}[\u55ce]"
                     ],
@@ -573,20 +525,110 @@
                     "response": "how_many",
                     "sentences": [
                         "[<area>] <how_many> [\u6247] {cover_classes:device_class} \u662f {cover_states:state}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "[<area>][<name>][(\u662f|\u662f\u4e0d\u662f)]{lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "[<area>][(\u6709 | \u6709\u6c92\u6709 | \u6709\u4efb\u4f55)][<door>][\u662f] [\u6c92\u6709]{lock_states:state}[\u8457][\u7684][\u55ce]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "[<area>][<all>][<door>][(\u90fd|\u90fd\u662f|\u662f|\u662f\u4e0d\u662f)]{lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "[<area>] [<which>][<door>][\u662f] {lock_states:state}[\u8457][(\u7684|\u4e86)][\u55ce]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "[<area>]<how_many>[(\u6247|\u9053)][<door>][\u662f]{lock_states:state}[\u8457][\u7684][\u55ce]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_off>[\u6240\u6709|\u5168\u90e8]<area>[\u7684][\u6240\u6709|\u5168\u90e8]<fan>",
+                        "[<let>][\u6240\u6709|\u5168\u90e8][\u7684]<area>[\u7684][\u6240\u6709|\u5168\u90e8]<fan><turn_off>",
+                        "<turn_off> <area> (\u98a8\u6247|\u540a\u6247)",
+                        "<let>  <area> [<all>] (\u98a8\u6247 | \u540a\u6247) <turn_off>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "response": "light_all",
+                    "sentences": [
+                        "<turn_off><all>[<area>][\u7684][\u6240\u6709|\u5168\u90e8]<fan>",
+                        "[<let>]<all>[\u7684][<area>][\u7684][\u6240\u6709|\u5168\u90e8]<fan><turn_off>",
+                        "<let>[<area>]<all>(\u98a8\u6247 | \u540a\u6247)<turn_off>"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
+                    "sentences": [
+                        "<turn_off> [<area>] <name>[(<light>|<switch>)]",
+                        "[<let>] [<area>] <name>[(<light>|<switch>)]<turn_off>"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_off><area>[<all>]<light>",
                         "<turn_off>[<all>]<area><light>",
                         "[<let>]<area>[<all>]<light><turn_off>",
                         "[<let>][<all>]<area><light><turn_off>"
                     ],
@@ -672,86 +714,83 @@
                     "sentences": [
                         "[<let>][<area>]<all>(<name>|\u9580\u9396|\u9396|\u9580)(\u6253\u958b|\u958b\u555f|\u89e3\u9396)"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
-                },
+                }
+            ]
+        },
+        "HassTurnOn": {
+            "data": [
                 {
-                    "response": "fans_area",
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
                     "sentences": [
-                        "<turn_off>[\u6240\u6709|\u5168\u90e8]<area>[\u7684][\u6240\u6709|\u5168\u90e8]<fan>",
-                        "[<let>][\u6240\u6709|\u5168\u90e8][\u7684]<area>[\u7684][\u6240\u6709|\u5168\u90e8]<fan><turn_off>",
-                        "<turn_off> <area> (\u98a8\u6247|\u540a\u6247)",
-                        "<let>  <area> [<all>] (\u98a8\u6247 | \u540a\u6247) <turn_off>"
+                        "[\u555f\u52d5]<name>[\u5834\u666f]"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "scene"
                     }
                 },
                 {
-                    "response": "light_all",
+                    "response": "lights_area",
                     "sentences": [
-                        "<turn_off><all>[<area>][\u7684][\u6240\u6709|\u5168\u90e8]<fan>",
-                        "[<let>]<all>[\u7684][<area>][\u7684][\u6240\u6709|\u5168\u90e8]<fan><turn_off>",
-                        "<let>[<area>]<all>(\u98a8\u6247 | \u540a\u6247)<turn_off>"
+                        "<turn_on><area>[<all>]<light>",
+                        "<turn_on>[<all>]<area><light>",
+                        "[<let>]<area>[<all>]<light><turn_on>",
+                        "[<let>][<all>]<area><light><turn_on>"
                     ],
                     "slots": {
-                        "area": "all",
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "light"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "binary_sensor",
-                            "cover",
-                            "lock",
-                            "scene",
-                            "script",
-                            "sensor"
-                        ]
+                    "requires_context": {
+                        "domain": "cover"
                     },
+                    "response": "cover",
                     "sentences": [
-                        "<turn_off> [<area>] <name>[(<light>|<switch>)]",
-                        "[<let>] [<area>] <name>[(<light>|<switch>)]<turn_off>"
+                        "<open> [<area>] <name>",
+                        "<let> [<area>] <name> <open>"
                     ]
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                },
                 {
-                    "requires_context": {
-                        "domain": "scene"
-                    },
-                    "response": "scene",
+                    "response": "cover_device_class",
                     "sentences": [
-                        "[\u555f\u52d5]<name>[\u5834\u666f]"
+                        "<let> \u8eca\u5eab\u9580 <open>",
+                        "<open> \u8eca\u5eab\u9580"
                     ],
                     "slots": {
-                        "domain": "scene"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "cover",
-                            "scene",
-                            "sensor",
-                            "script"
-                        ]
-                    },
+                    "response": "cover_device_class",
                     "sentences": [
-                        "<turn_on> [<area>] <name>[(<light>|<switch>)]",
-                        "[<let>][<area>]<name>[(<light>|<switch>)]<turn_on>"
-                    ]
+                        "<open> <area> {cover_classes:device_class}",
+                        "<let> <area> {cover_classes:device_class} <open>"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "fans_area",
+                    "sentences": [
+                        "<turn_on><area>(\u98a8\u6247|\u540a\u6247)"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
                 },
                 {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "lock",
                     "sentences": [
@@ -784,77 +823,38 @@
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "fans_area",
-                    "sentences": [
-                        "<turn_on><area>(\u98a8\u6247|\u540a\u6247)"
-                    ],
-                    "slots": {
-                        "domain": "fan",
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "lights_area",
-                    "sentences": [
-                        "<turn_on><area>[<all>]<light>",
-                        "<turn_on>[<all>]<area><light>",
-                        "[<let>]<area>[<all>]<light><turn_on>",
-                        "[<let>][<all>]<area><light><turn_on>"
-                    ],
-                    "slots": {
-                        "domain": "light"
-                    }
-                },
-                {
                     "requires_context": {
                         "domain": "script"
                     },
                     "response": "script",
                     "sentences": [
                         "[(\u57f7\u884c|\u958b\u59cb)]<name>[\u8173\u672c]"
                     ],
                     "slots": {
                         "domain": "script"
                     }
                 },
                 {
-                    "requires_context": {
-                        "domain": "cover"
+                    "excludes_context": {
+                        "domain": [
+                            "cover",
+                            "scene",
+                            "sensor",
+                            "script"
+                        ]
                     },
-                    "response": "cover",
                     "sentences": [
-                        "<open> [<area>] <name>",
-                        "<let> [<area>] <name> <open>"
+                        "<turn_on> [<area>] <name>[(<light>|<switch>)]",
+                        "[<let>][<area>]<name>[(<light>|<switch>)]<turn_on>"
                     ]
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<let> \u8eca\u5eab\u9580 <open>",
-                        "<open> \u8eca\u5eab\u9580"
-                    ],
-                    "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "cover_device_class",
-                    "sentences": [
-                        "<open> <area> {cover_classes:device_class}",
-                        "<let> <area> {cover_classes:device_class} <open>"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
                 }
             ]
         }
     },
     "language": "zh-tw",
     "lists": {
         "brightness": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/fr.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9913194444444445%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {0: {'sentences': ['<regle> [toutes] <lumieres> <dans> "*

 * *              "<area> à <brightness>']}, 1: {'sentences': ['<regle> <name> <dans> <area> à "*

 * *              "<brightness>']}, 2: {'sentences': ['<regle> [la couleur] [de | des] [toutes] "*

 * *              "<lumieres> <dans> <area> [avec la couleur | de couleur | en] {color}']}, 3: "*

 * *              "{'sentences': ['<regle> [la couleur de] <name> <dans> <area> [avec la couleur | de "*

 * *              "couleur | en] {colo […]*

```diff
@@ -1,39 +1,39 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness_area",
                     "sentences": [
-                        "<regle> [toutes] <lumieres> de <area> \u00e0 <brightness>"
+                        "<regle> [toutes] <lumieres> <dans> <area> \u00e0 <brightness>"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
                     "response": "brightness_area",
                     "sentences": [
-                        "<regle> <name> [dans|du|de] <area> \u00e0 <brightness>"
+                        "<regle> <name> <dans> <area> \u00e0 <brightness>"
                     ]
                 },
                 {
                     "response": "color_area",
                     "sentences": [
-                        "<regle> [la couleur] [de | des] [toutes] <lumieres> de <area> [avec la couleur | de couleur | en] {color}"
+                        "<regle> [la couleur] [de | des] [toutes] <lumieres> <dans> <area> [avec la couleur | de couleur | en] {color}"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
                     "response": "color_area",
                     "sentences": [
-                        "<regle> [la couleur de] <name> [dans|du|de] <area> [avec la couleur | de couleur | en] {color}"
+                        "<regle> [la couleur de] <name> <dans> <area> [avec la couleur | de couleur | en] {color}"
                     ]
                 }
             ]
         }
     },
     "language": "fr",
     "responses": {
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.4.17/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.3.29
+Version: 2023.4.17
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.3.29/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.4.17/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 home_assistant_intents/__init__.py
+home_assistant_intents/domains.py
 home_assistant_intents.egg-info/PKG-INFO
 home_assistant_intents.egg-info/SOURCES.txt
 home_assistant_intents.egg-info/dependency_links.txt
 home_assistant_intents.egg-info/top_level.txt
 home_assistant_intents.egg-info/zip-safe
 home_assistant_intents/data/homeassistant/ar.json
 home_assistant_intents/data/homeassistant/bg.json
```

### Comparing `home-assistant-intents-2023.3.29/pyproject.toml` & `home-assistant-intents-2023.4.17/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.3.29"
+version     = "2023.4.17"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

