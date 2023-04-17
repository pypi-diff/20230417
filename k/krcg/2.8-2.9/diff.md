# Comparing `tmp/krcg-2.8.tar.gz` & `tmp/krcg-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krcg-2.8.tar", last modified: Mon Feb  1 12:14:16 2021, max compression
+gzip compressed data, was "dist/krcg-2.9.tar", last modified: Tue Feb 16 09:35:39 2021, max compression
```

## Comparing `krcg-2.8.tar` & `krcg-2.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:16.511163 krcg-2.8/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     9509 2021-02-01 12:14:15.000000 krcg-2.8/CHANGELOG.rst
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2021-02-01 12:14:15.000000 krcg-2.8/LICENSE
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      249 2021-02-01 12:14:15.000000 krcg-2.8/MANIFEST.in
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    18607 2021-02-01 12:14:16.511414 krcg-2.8/PKG-INFO
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    14496 2021-02-01 12:14:15.000000 krcg-2.8/README.md
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:16.493390 krcg-2.8/krcg/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:15.000000 krcg-2.8/krcg/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    10992 2021-02-01 12:14:15.000000 krcg-2.8/krcg/analyzer.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    38165 2021-02-01 12:14:15.000000 krcg-2.8/krcg/cards.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    11505 2021-02-01 12:14:15.000000 krcg-2.8/krcg/config.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    15443 2021-02-01 12:14:15.000000 krcg-2.8/krcg/deck.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1735 2021-02-01 12:14:15.000000 krcg-2.8/krcg/logging.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    23805 2021-02-01 12:14:15.000000 krcg-2.8/krcg/parser.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1841 2021-02-01 12:14:15.000000 krcg-2.8/krcg/rulings.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     6067 2021-02-01 12:14:15.000000 krcg-2.8/krcg/sets.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3431 2021-02-01 12:14:15.000000 krcg-2.8/krcg/twda.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     9731 2021-02-01 12:14:15.000000 krcg-2.8/krcg/utils.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2926 2021-02-01 12:14:15.000000 krcg-2.8/krcg/vtes.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:16.511006 krcg-2.8/krcg.egg-info/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2116 2021-02-01 12:14:16.000000 krcg-2.8/krcg.egg-info/SOURCES.txt
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:16.494622 krcg-2.8/rulings/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:15.000000 krcg-2.8/rulings/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   288415 2021-02-01 12:14:15.000000 krcg-2.8/rulings/cards-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    21300 2021-02-01 12:14:15.000000 krcg-2.8/rulings/general-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   100856 2021-02-01 12:14:15.000000 krcg-2.8/rulings/rulings-links.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1247 2021-02-01 12:14:16.512050 krcg-2.8/setup.cfg
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2021-02-01 12:14:15.000000 krcg-2.8/setup.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:16.510778 krcg-2.8/twda_fix/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1906 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2010hunrb.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3219 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2010pwbla1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1781 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2010pwblaQ.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1727 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2during.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      998 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2eclastq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1776 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2gothenburg.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2gothenburgapr.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1615 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2newyork.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1262 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2orccon2.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2pariseq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2615 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2sydney.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1807 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2torrancejan.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1627 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2ukqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1957 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2watfordapr.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2248 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k2watfordmay.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      945 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3cadaverous.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2022 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3ec.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1958 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3frenchecq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2326 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3gothenburgblizzard.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2252 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3helsinki5.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2939 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3italyqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3psmilwaukee.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2206 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3rome.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1509 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3sdgothenburg.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3tcithaca.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1698 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k3winnipegapril.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2091 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k4gks.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1967 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k4littlesister.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1594 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k4norms.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2483 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k4volkerpit.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1611 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5blackutrecht.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3963 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5dcqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2090 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5dreamboston.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1712 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5leicesteraug.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1643 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5ropecon.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1832 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k5valhallajuly.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1337 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k6aussiechamp.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2077 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k6faceaface.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2176 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k6nerq-templecon.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1144 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k6praxispoitiers.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1545 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k6sonarba.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2295 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k7campeonatojuizforano.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2309 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k7comjust.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1209 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k7palmaqual.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3394 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k7woaboston.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1618 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k8sequeenslandcq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3021 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k8torunminiq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1682 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/2k9mojlp.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2278 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/Brian.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1324 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/ckgc2k.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3903 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/crusadelisbon2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1775 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/dallas.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1901 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/damnans.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3327 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/darbyla2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1292 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/gothenburg2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2324 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/joshphiladelphia.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2039 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/leedec99.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1430 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/lurequebec2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1753 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/matt-alamut.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1616 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/palma2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1970 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/portoct99.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2706 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/quebec.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2207 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/rob.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2015 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/swkc.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1965 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/theobell2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2961 2021-02-01 12:14:15.000000 krcg-2.8/twda_fix/watford-ts.html
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659711 krcg-2.9/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     9567 2021-02-16 09:35:39.000000 krcg-2.9/CHANGELOG.rst
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2021-02-16 09:35:39.000000 krcg-2.9/LICENSE
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      249 2021-02-16 09:35:39.000000 krcg-2.9/MANIFEST.in
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    18607 2021-02-16 09:35:39.659942 krcg-2.9/PKG-INFO
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    14496 2021-02-16 09:35:39.000000 krcg-2.9/README.md
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.639412 krcg-2.9/krcg/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/krcg/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    10992 2021-02-16 09:35:39.000000 krcg-2.9/krcg/analyzer.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    38165 2021-02-16 09:35:39.000000 krcg-2.9/krcg/cards.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    11505 2021-02-16 09:35:39.000000 krcg-2.9/krcg/config.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    15443 2021-02-16 09:35:39.000000 krcg-2.9/krcg/deck.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1735 2021-02-16 09:35:39.000000 krcg-2.9/krcg/logging.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    23805 2021-02-16 09:35:39.000000 krcg-2.9/krcg/parser.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1841 2021-02-16 09:35:39.000000 krcg-2.9/krcg/rulings.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     6067 2021-02-16 09:35:39.000000 krcg-2.9/krcg/sets.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3431 2021-02-16 09:35:39.000000 krcg-2.9/krcg/twda.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     9731 2021-02-16 09:35:39.000000 krcg-2.9/krcg/utils.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2926 2021-02-16 09:35:39.000000 krcg-2.9/krcg/vtes.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659554 krcg-2.9/krcg.egg-info/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2116 2021-02-16 09:35:39.000000 krcg-2.9/krcg.egg-info/SOURCES.txt
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.640780 krcg-2.9/rulings/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/rulings/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   288493 2021-02-16 09:35:39.000000 krcg-2.9/rulings/cards-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    21300 2021-02-16 09:35:39.000000 krcg-2.9/rulings/general-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   100957 2021-02-16 09:35:39.000000 krcg-2.9/rulings/rulings-links.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1247 2021-02-16 09:35:39.660610 krcg-2.9/setup.cfg
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2021-02-16 09:35:39.000000 krcg-2.9/setup.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659329 krcg-2.9/twda_fix/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1906 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010hunrb.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3219 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010pwbla1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1781 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010pwblaQ.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1727 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2during.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      998 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2eclastq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1776 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2gothenburg.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2gothenburgapr.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1615 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2newyork.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1262 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2orccon2.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2pariseq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2615 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2sydney.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1807 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2torrancejan.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1627 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2ukqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1957 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2watfordapr.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2248 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2watfordmay.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      945 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3cadaverous.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2022 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3ec.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1958 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3frenchecq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2326 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3gothenburgblizzard.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2252 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3helsinki5.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2939 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3italyqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3psmilwaukee.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2206 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3rome.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1509 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3sdgothenburg.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3tcithaca.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1698 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3winnipegapril.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2091 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4gks.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1967 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4littlesister.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1594 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4norms.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2483 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4volkerpit.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1611 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5blackutrecht.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3963 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5dcqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2090 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5dreamboston.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1712 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5leicesteraug.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1643 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5ropecon.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1832 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5valhallajuly.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1337 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6aussiechamp.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2077 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6faceaface.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2176 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6nerq-templecon.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1144 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6praxispoitiers.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1545 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6sonarba.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2295 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7campeonatojuizforano.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2309 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7comjust.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1209 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7palmaqual.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3394 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7woaboston.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1618 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k8sequeenslandcq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3021 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k8torunminiq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1682 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k9mojlp.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2278 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/Brian.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1324 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/ckgc2k.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3903 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/crusadelisbon2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1775 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/dallas.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1901 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/damnans.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3327 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/darbyla2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1292 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/gothenburg2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2324 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/joshphiladelphia.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2039 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/leedec99.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1430 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/lurequebec2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1753 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/matt-alamut.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1616 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/palma2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1970 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/portoct99.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2706 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/quebec.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2207 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/rob.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2015 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/swkc.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1965 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/theobell2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2961 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/watford-ts.html
```

### Comparing `krcg-2.8/CHANGELOG.rst` & `krcg-2.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.9 (2021-02-16)
+----------------
+
+- Additional rulings
+
+
 2.8 (2021-02-01)
 ----------------
 
 - Additional rulings
 
 
 2.7 (2021-01-29)
```

### Comparing `krcg-2.8/LICENSE` & `krcg-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `krcg-2.8/PKG-INFO` & `krcg-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krcg
-Version: 2.8
+Version: 2.9
 Summary: "CLI, web API and Discord bot for VTES cards and TWDA.",
 Home-page: http://github.com/lionel-panhaleux/krcg
 Author: lionelpx
 Author-email: lionel.panhaleux@gmail.com
 License: "MIT"
 Description: # KRCG
```

### Comparing `krcg-2.8/README.md` & `krcg-2.9/README.md`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/analyzer.py` & `krcg-2.9/krcg/analyzer.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/cards.py` & `krcg-2.9/krcg/cards.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/config.py` & `krcg-2.9/krcg/config.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/deck.py` & `krcg-2.9/krcg/deck.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/logging.py` & `krcg-2.9/krcg/logging.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/parser.py` & `krcg-2.9/krcg/parser.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/rulings.py` & `krcg-2.9/krcg/rulings.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/sets.py` & `krcg-2.9/krcg/sets.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/twda.py` & `krcg-2.9/krcg/twda.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/utils.py` & `krcg-2.9/krcg/utils.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg/vtes.py` & `krcg-2.9/krcg/vtes.py`

 * *Files identical despite different names*

### Comparing `krcg-2.8/krcg.egg-info/SOURCES.txt` & `krcg-2.9/krcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krcg-2.8/rulings/cards-rulings.yaml` & `krcg-2.9/rulings/cards-rulings.yaml`

 * *Files identical despite different names*

```diff
@@ -111,14 +111,15 @@
   - "Unused prevention does not carry over. [LSJ 20001114]"
 100092|Army of Apparitions:
   - "[chi] Cannot be used during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
 100096|The Art of Love:
   - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
 100097|The Art of Memory:
   - "The effect is applied after resolving the action, including after all combats. [LSJ 20031112]"
+  - "Can be used ot retrieve the action card itself (if any). [LSJ 20041115]"
 100100|Art's Traumatic Essence:
   - "The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]"
 100103|Asanbonsam Ghoul:
   - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
   - "If another effect also sets the range, the first to resolve has priority (eg. {Squirrel's Balance} resolves before, {Neutral Guard} resolves after). [PIB 20120214]"
 100105|Ashes to Ashes:
   - "[thn], [THN] The end of combat is triggered by the vampire going to torpor - this can be interrupted by cards such as {Undying Tenacity} or {Undead Persistence}, but the vampire would still be wounded. [LSJ 20021122]"
```

### Comparing `krcg-2.8/rulings/general-rulings.yaml` & `krcg-2.9/rulings/general-rulings.yaml`

 * *Files identical despite different names*

### Comparing `krcg-2.8/rulings/rulings-links.yaml` & `krcg-2.9/rulings/rulings-links.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,15 @@
 LSJ 20040802: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/b6V_OGl-TgE/bi8evHga9X8J
 LSJ 20040805: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WuER8RUMzTE/OmQhmQFkFLkJ
 LSJ 20040812: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/n_0DGDsWG0E/lxG2zMPetwAJ
 LSJ 20040928: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GBcR6aNjIk4/DXPyqBM1R8kJ
 LSJ 20041015: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jonKzp3f8wA/Dgropqbf_WwJ
 LSJ 20041022: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gqhND6kd2wE/LDmEotxa_4kJ
 LSJ 20041022-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/UAhJ3vWLyMM/m/gp04WTgORSQJ
+LSJ 20041115: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ZCmZl5xUhis/m/YoKKqsiFLFgJ
 LSJ 20041119: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HMV_pN5mJhQ/tzkinpwUq-MJ
 LSJ 20041130: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6uTPqRg387A/fa9DW8-Hu38J
 LSJ 20041202: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8MwcrUpCdBc/E5hnEF8WU8UJ
 LSJ 20041203: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_iogrCkrCmc/hTkREMXGFR0J
 LSJ 20041207: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6oC7FtG2Ac4/lI5hqeuSioIJ
 LSJ 20050105-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vze_ZUJmzu8/cSZJ6ku_bSsJ
 LSJ 20050105-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/sAErRDiSXfU/GMQXJ7TvOrsJ
```

### Comparing `krcg-2.8/setup.cfg` & `krcg-2.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = krcg
-version = 2.8
+version = 2.9
 author = lionelpx
 author_email = lionel.panhaleux@gmail.com
 url = http://github.com/lionel-panhaleux/krcg
 description = "CLI, web API and Discord bot for VTES cards and TWDA.",
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "MIT"
```

### Comparing `krcg-2.8/twda_fix/2010hunrb.html` & `krcg-2.9/twda_fix/2010hunrb.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2010pwbla1.html` & `krcg-2.9/twda_fix/2010pwbla1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2010pwblaQ.html` & `krcg-2.9/twda_fix/2010pwblaQ.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2during.html` & `krcg-2.9/twda_fix/2k2during.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2eclastq.html` & `krcg-2.9/twda_fix/2k2eclastq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2gothenburg.html` & `krcg-2.9/twda_fix/2k2gothenburg.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2gothenburgapr.html` & `krcg-2.9/twda_fix/2k2gothenburgapr.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2newyork.html` & `krcg-2.9/twda_fix/2k2newyork.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2orccon2.html` & `krcg-2.9/twda_fix/2k2orccon2.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2pariseq.html` & `krcg-2.9/twda_fix/2k2pariseq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2sydney.html` & `krcg-2.9/twda_fix/2k2sydney.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2torrancejan.html` & `krcg-2.9/twda_fix/2k2torrancejan.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2ukqualifier.html` & `krcg-2.9/twda_fix/2k2ukqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2watfordapr.html` & `krcg-2.9/twda_fix/2k2watfordapr.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k2watfordmay.html` & `krcg-2.9/twda_fix/2k2watfordmay.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3cadaverous.html` & `krcg-2.9/twda_fix/2k3cadaverous.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3ec.html` & `krcg-2.9/twda_fix/2k3ec.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3frenchecq.html` & `krcg-2.9/twda_fix/2k3frenchecq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3gothenburgblizzard.html` & `krcg-2.9/twda_fix/2k3gothenburgblizzard.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3helsinki5.html` & `krcg-2.9/twda_fix/2k3helsinki5.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3italyqualifier.html` & `krcg-2.9/twda_fix/2k3italyqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3psmilwaukee.html` & `krcg-2.9/twda_fix/2k3psmilwaukee.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3rome.html` & `krcg-2.9/twda_fix/2k3rome.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3sdgothenburg.html` & `krcg-2.9/twda_fix/2k3sdgothenburg.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3tcithaca.html` & `krcg-2.9/twda_fix/2k3tcithaca.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k3winnipegapril.html` & `krcg-2.9/twda_fix/2k3winnipegapril.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k4gks.html` & `krcg-2.9/twda_fix/2k4gks.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k4littlesister.html` & `krcg-2.9/twda_fix/2k4littlesister.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k4norms.html` & `krcg-2.9/twda_fix/2k4norms.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k4volkerpit.html` & `krcg-2.9/twda_fix/2k4volkerpit.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5blackutrecht.html` & `krcg-2.9/twda_fix/2k5blackutrecht.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5dcqualifier.html` & `krcg-2.9/twda_fix/2k5dcqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5dreamboston.html` & `krcg-2.9/twda_fix/2k5dreamboston.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5leicesteraug.html` & `krcg-2.9/twda_fix/2k5leicesteraug.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5ropecon.html` & `krcg-2.9/twda_fix/2k5ropecon.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k5valhallajuly.html` & `krcg-2.9/twda_fix/2k5valhallajuly.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k6aussiechamp.html` & `krcg-2.9/twda_fix/2k6aussiechamp.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k6faceaface.html` & `krcg-2.9/twda_fix/2k6faceaface.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k6nerq-templecon.html` & `krcg-2.9/twda_fix/2k6nerq-templecon.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k6praxispoitiers.html` & `krcg-2.9/twda_fix/2k6praxispoitiers.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k6sonarba.html` & `krcg-2.9/twda_fix/2k6sonarba.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k7campeonatojuizforano.html` & `krcg-2.9/twda_fix/2k7campeonatojuizforano.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k7comjust.html` & `krcg-2.9/twda_fix/2k7comjust.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k7palmaqual.html` & `krcg-2.9/twda_fix/2k7palmaqual.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k7woaboston.html` & `krcg-2.9/twda_fix/2k7woaboston.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k8sequeenslandcq.html` & `krcg-2.9/twda_fix/2k8sequeenslandcq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k8torunminiq.html` & `krcg-2.9/twda_fix/2k8torunminiq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/2k9mojlp.html` & `krcg-2.9/twda_fix/2k9mojlp.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/Brian.html` & `krcg-2.9/twda_fix/Brian.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/ckgc2k.html` & `krcg-2.9/twda_fix/ckgc2k.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/crusadelisbon2k1.html` & `krcg-2.9/twda_fix/crusadelisbon2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/dallas.html` & `krcg-2.9/twda_fix/dallas.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/damnans.html` & `krcg-2.9/twda_fix/damnans.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/darbyla2k1.html` & `krcg-2.9/twda_fix/darbyla2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/gothenburg2k1.html` & `krcg-2.9/twda_fix/gothenburg2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/joshphiladelphia.html` & `krcg-2.9/twda_fix/joshphiladelphia.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/leedec99.html` & `krcg-2.9/twda_fix/leedec99.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/lurequebec2k1.html` & `krcg-2.9/twda_fix/lurequebec2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/matt-alamut.html` & `krcg-2.9/twda_fix/matt-alamut.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/palma2k1.html` & `krcg-2.9/twda_fix/palma2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/portoct99.html` & `krcg-2.9/twda_fix/portoct99.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/quebec.html` & `krcg-2.9/twda_fix/quebec.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/rob.html` & `krcg-2.9/twda_fix/rob.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/swkc.html` & `krcg-2.9/twda_fix/swkc.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/theobell2k1.html` & `krcg-2.9/twda_fix/theobell2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.8/twda_fix/watford-ts.html` & `krcg-2.9/twda_fix/watford-ts.html`

 * *Files identical despite different names*

