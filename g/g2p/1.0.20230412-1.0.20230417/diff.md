# Comparing `tmp/g2p-1.0.20230412.tar.gz` & `tmp/g2p-1.0.20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-1.0.20230412.tar", last modified: Wed Apr 12 22:08:22 2023, max compression
+gzip compressed data, was "g2p-1.0.20230417.tar", last modified: Mon Apr 17 18:58:21 2023, max compression
```

## Comparing `g2p-1.0.20230412.tar` & `g2p-1.0.20230417.tar`

### file list

```diff
@@ -1,430 +1,430 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 22:08:04.000000 g2p-1.0.20230412/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 22:08:04.000000 g2p-1.0.20230412/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-12 22:08:22.338273 g2p-1.0.20230412/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-12 22:08:04.000000 g2p-1.0.20230412/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p/
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/create_fallback_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/create_ipa_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.258272 g2p-1.0.20230412/g2p/mappings/langs/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/alq/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/alq/alq_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/alq/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/atj/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/atj_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/ckt/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/clc/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/clc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/clc/doulos.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crg/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crj/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crk/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crl/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/crm/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/crx/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/csw/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/ctp/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.278272 g2p-1.0.20230412/g2p/mappings/langs/eng/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  4215929 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/dummy_to_arpabet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_inventory.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/make_alignments.sh
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/make_ipa_cmudict.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/reverse_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.278272 g2p-1.0.20230412/g2p/mappings/langs/fin/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fin/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fin/fin_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.282272 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/fn_unicode.csv
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/hei_doulos.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/hei_times.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/nav_times.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.282272 g2p-1.0.20230412/g2p/mappings/langs/fra/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/fra_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/fra_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/git/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/APA.csv
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Ortho_variables.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Orthography.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Orthography_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/RAPA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/RAPA_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/gla/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/gla_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/gwi/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/haa/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/ikt/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/ikt_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/iku/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_sro_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_to_iku_equiv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/kkz/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/kwk/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/umista_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)  7050749 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/langs.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/lml/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/lml_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/mic/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/mic_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/moe_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/moe_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/moh/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_to_festival.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/network.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/panphon_preprocessor.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/tone-map.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/oji/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/oji_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/oka/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/oka_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/oka_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/see/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/see/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/see/see_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/srs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/srs_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/str/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/str_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/str_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tau/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/tau_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/tau_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tce/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/tce_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/tce_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tgx/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tli/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/tli_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/tli_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/ttm/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/ttm_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/ttm_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/und/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/und_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/win/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/hoocak_alphabet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/win_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/blockly_main.js
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/blocks.js
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/echart_custom.js
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/languages-network.json
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/skeleton.css
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.314272 g2p-1.0.20230412/g2p/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/templates/docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.318272 g2p-1.0.20230412/g2p/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.318272 g2p-1.0.20230412/g2p/tests/public/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.326273 g2p-1.0.20230412/g2p/tests/public/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crg.psv
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crj.psv
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crm.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/csw.psv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ctp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/eng.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fin.psv
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fn_unicode.psv
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra.psv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams_NFD.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_simple.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/git.psv
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/gwi.psv
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/haa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ikt.psv
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/iku-sro.psv
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/iku.psv
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/kwk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/lml.psv
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/mic.psv
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/moe.psv
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/moh.psv
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oji-syl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oji.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oka.csv
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/srs.psv
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/str.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/str_un_human_rights.txt
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tau.psv
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tce.csv
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tli.csv
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ttm.csv
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/win.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviation_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviation_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.psv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.substring.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.242272 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.242272 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_lexicon_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose2-3.csv
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion.csv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion_config_csv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion_config_json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/g2p_studio.csv
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/g2p_studio2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/hello.aligned.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/lexicon_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/malformed_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.csv
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.psv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/no_escape.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/null.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/null_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/rule-ordering.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/test_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/tokenize_punct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/tokenize_punct_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/sample_response.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4682 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_api_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_check_ipa_arpabet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16189 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6249 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_create_mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_doctor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_doctor_expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_fallback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23149 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_indices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_lexicon_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13478 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_mappings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_studio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5937 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_tokenize_and_map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5723 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11446 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_unidecode_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10254 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9835 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_z_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/time_panphon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/g2p/transducer/
--rw-r--r--   0 runner    (1001) docker     (123)    49089 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/transducer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:08:21.000000 g2p-1.0.20230412/g2p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 22:08:22.338273 g2p-1.0.20230412/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 22:08:04.000000 g2p-1.0.20230412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-17 18:58:05.000000 g2p-1.0.20230417/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 18:58:05.000000 g2p-1.0.20230417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-17 18:58:21.870860 g2p-1.0.20230417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-17 18:58:05.000000 g2p-1.0.20230417/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28100 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/create_fallback_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/create_ipa_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/alq/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/alq/alq_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/alq/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/atj/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/atj_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/ckt/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/clc/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/clc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/clc/doulos.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/crg/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crj/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crk/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crm/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crx/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/ctp/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.830860 g2p-1.0.20230417/g2p/mappings/langs/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/eng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  4215929 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/dummy_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/make_alignments.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/make_ipa_cmudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/reverse_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/fin/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fin/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fin/fin_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/fn_unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/hei_doulos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/hei_times.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/nav_times.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/fra/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/fra_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/fra_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.838860 g2p-1.0.20230417/g2p/mappings/langs/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/git/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/APA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Ortho_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Orthography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Orthography_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/RAPA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/RAPA_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/gla/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/gla_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/gwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/haa/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/ikt/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/ikt_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/iku/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_sro_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_to_iku_equiv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/kkz/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/kwk/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/umista_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  7050749 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/langs.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/lml/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/lml_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/mic_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/moe_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/moe_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/moh/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_festival.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/network.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/panphon_preprocessor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/tone-map.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/oji/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/oji_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/oka/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/oka_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/oka_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/see/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/see/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/see/see_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/srs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/srs_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/str/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/str_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/str_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tau/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/tau_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/tau_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tce/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/tce_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/tce_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tli/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/tli_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/tli_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/ttm/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/ttm_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/ttm_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/mappings/langs/und/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/und_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/mappings/langs/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/hoocak_alphabet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/win_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/blockly_main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/blocks.js
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/echart_custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/languages-network.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.858860 g2p-1.0.20230417/g2p/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/templates/docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.862860 g2p-1.0.20230417/g2p/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.862860 g2p-1.0.20230417/g2p/tests/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.866860 g2p-1.0.20230417/g2p/tests/public/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crg.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crj.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crm.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/csw.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ctp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/eng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fin.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fn_unicode.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams_NFD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/git.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/gwi.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/haa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ikt.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/iku-sro.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/iku.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/kwk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/lml.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/mic.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/moe.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/moh.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oji-syl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oji.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oka.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/srs.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/str.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/str_un_human_rights.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tau.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tce.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ttm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/win.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviation_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviation_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.substring.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.810860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.810860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_lexicon_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose2-3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion_config_csv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion_config_json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/g2p_studio.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/g2p_studio2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/hello.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/lexicon_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/malformed_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/no_escape.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/null.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/null_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/rule-ordering.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/test_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/tokenize_punct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/tokenize_punct_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/sample_response.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4682 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_api_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_check_ipa_arpabet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16189 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6249 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_create_mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_doctor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_doctor_expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_fallback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23149 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_indices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_lexicon_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13478 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_mappings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_studio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5937 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_tokenize_and_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5723 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_tokenizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11446 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_unidecode_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10830 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9835 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_z_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/time_panphon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)    49089 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/transducer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 18:58:21.874860 g2p-1.0.20230417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 18:58:06.000000 g2p-1.0.20230417/setup.py
```

### Comparing `g2p-1.0.20230412/LICENSE` & `g2p-1.0.20230417/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/PKG-INFO` & `g2p-1.0.20230417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230412
+Version: 1.0.20230417
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g2p-1.0.20230412/README.md` & `g2p-1.0.20230417/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/api.py` & `g2p-1.0.20230417/g2p/api.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/app.py` & `g2p-1.0.20230417/g2p/app.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/cli.py` & `g2p-1.0.20230417/g2p/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Command line interface to the g2p system
 """
+import io
 import json
 import os
 import pprint
 import re
 import sys
 
 import click
@@ -42,14 +43,20 @@
 )
 from g2p.mappings.utils import is_ipa, is_xsampa, load_mapping_from_path, normalize
 from g2p.static import __file__ as static_file
 from g2p.transducer import Transducer
 
 PRINTER = pprint.PrettyPrinter(indent=4)
 
+if "pytest" not in sys.modules:  # pragma: no cover
+    if sys.stdout.encoding != "utf8" and hasattr(sys.stdout, "buffer"):
+        sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf8")
+    if sys.stderr.encoding != "utf8" and hasattr(sys.stderr, "buffer"):
+        sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf8")
+
 
 def create_app():
     """Return the flask app for g2p"""
     return APP
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
```

### Comparing `g2p-1.0.20230412/g2p/exceptions.py` & `g2p-1.0.20230417/g2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/__init__.py` & `g2p-1.0.20230417/g2p/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/create_fallback_mapping.py` & `g2p-1.0.20230417/g2p/mappings/create_fallback_mapping.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/create_ipa_mapping.py` & `g2p-1.0.20230417/g2p/mappings/create_ipa_mapping.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/__init__.py` & `g2p-1.0.20230417/g2p/mappings/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/atj/atj_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/atj/atj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crg/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/crg/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crj/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/crj/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crk/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/crk/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crl/README.md` & `g2p-1.0.20230417/g2p/mappings/langs/crl/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crl/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/crl/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crm/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/crm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv` & `g2p-1.0.20230417/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv` & `g2p-1.0.20230417/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/csw/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/csw/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ctp/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/ctp/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/README.md` & `g2p-1.0.20230417/g2p/mappings/langs/eng/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt` & `g2p-1.0.20230417/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/eng/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json` & `g2p-1.0.20230417/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/make_alignments.sh` & `g2p-1.0.20230417/g2p/mappings/langs/eng/make_alignments.sh`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/eng/make_ipa_cmudict.py` & `g2p-1.0.20230417/g2p/mappings/langs/eng/make_ipa_cmudict.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/README.md` & `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/fn_unicode.csv` & `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/fn_unicode.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/fra/README.txt` & `g2p-1.0.20230417/g2p/mappings/langs/fra/README.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/fra/fra_to_ipa.csv` & `g2p-1.0.20230417/g2p/mappings/langs/fra/fra_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/generated/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/APA.csv` & `g2p-1.0.20230417/g2p/mappings/langs/git/APA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/Orthography.csv` & `g2p-1.0.20230417/g2p/mappings/langs/git/Orthography.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/Orthography_Deterministic.csv` & `g2p-1.0.20230417/g2p/mappings/langs/git/Orthography_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/RAPA.csv` & `g2p-1.0.20230417/g2p/mappings/langs/git/RAPA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/RAPA_Deterministic.csv` & `g2p-1.0.20230417/g2p/mappings/langs/git/RAPA_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/git/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/git/git_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/git/git_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/gla/gla_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/gla/gla_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/gwi/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/gwi/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/haa/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/haa/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/haa/haa_abbs.csv` & `g2p-1.0.20230417/g2p/mappings/langs/haa/haa_abbs.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/haa/haa_to_ipa.csv` & `g2p-1.0.20230417/g2p/mappings/langs/haa/haa_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ikt/ikt_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/ikt/ikt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/iku/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/iku/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_equiv_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_equiv_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_sro_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_sro_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_to_iku_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_to_iku_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kkz/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/kkz/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_ubc.csv` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_ubc.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_uvic.csv` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_uvic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/kwk/umista_equiv.csv` & `g2p-1.0.20230417/g2p/mappings/langs/kwk/umista_equiv.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/langs.pkl` & `g2p-1.0.20230417/g2p/mappings/langs/langs.pkl`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/mic/mic_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/mic/mic_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/moe/moe_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/moe/moe_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/moh/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/moh/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/moh/moh_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/moh/moh_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/moh/moh_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/network.pkl` & `g2p-1.0.20230417/g2p/mappings/langs/network.pkl`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/norm/tone-map.txt` & `g2p-1.0.20230417/g2p/mappings/langs/norm/tone-map.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/oji/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/oji/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv` & `g2p-1.0.20230417/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/srs/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/srs/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/srs/srs_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/srs/srs_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/str/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/str/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/str/str_equiv.json` & `g2p-1.0.20230417/g2p/mappings/langs/str/str_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/str/str_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/str/str_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tau/config.yml` & `g2p-1.0.20230417/g2p/mappings/langs/tau/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tau/tau_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/tau/tau_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tce/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/tce/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tce/tce_to_ipa.csv` & `g2p-1.0.20230417/g2p/mappings/langs/tce/tce_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tgx/config.yml` & `g2p-1.0.20230417/g2p/mappings/langs/tgx/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tli/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/tli/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/tli/tli_to_ipa.csv` & `g2p-1.0.20230417/g2p/mappings/langs/tli/tli_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/ttm/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/ttm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/und/config.yaml` & `g2p-1.0.20230417/g2p/mappings/langs/und/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/und/und_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/und/und_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/utils.py` & `g2p-1.0.20230417/g2p/mappings/langs/utils.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/langs/win/win_to_ipa.json` & `g2p-1.0.20230417/g2p/mappings/langs/win/win_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/tokenizer.py` & `g2p-1.0.20230417/g2p/mappings/tokenizer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/mappings/utils.py` & `g2p-1.0.20230417/g2p/mappings/utils.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/blockly_main.js` & `g2p-1.0.20230417/g2p/static/blockly_main.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/blocks.js` & `g2p-1.0.20230417/g2p/static/blocks.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/custom.css` & `g2p-1.0.20230417/g2p/static/custom.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/custom.js` & `g2p-1.0.20230417/g2p/static/custom.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/echart_custom.js` & `g2p-1.0.20230417/g2p/static/echart_custom.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/languages-network.json` & `g2p-1.0.20230417/g2p/static/languages-network.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/normalize.css` & `g2p-1.0.20230417/g2p/static/normalize.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/skeleton.css` & `g2p-1.0.20230417/g2p/static/skeleton.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/static/swagger.json` & `g2p-1.0.20230417/g2p/static/swagger.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/templates/docs.html` & `g2p-1.0.20230417/g2p/templates/docs.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/templates/index.html` & `g2p-1.0.20230417/g2p/templates/index.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/__init__.py` & `g2p-1.0.20230417/g2p/tests/public/data/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/crl.psv` & `g2p-1.0.20230417/g2p/tests/public/data/crl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/fin.psv` & `g2p-1.0.20230417/g2p/tests/public/data/fin.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/fra.psv` & `g2p-1.0.20230417/g2p/tests/public/data/fra.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams.txt` & `g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams_NFD.txt` & `g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams_NFD.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/gwi.psv` & `g2p-1.0.20230417/g2p/tests/public/data/gwi.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/haa.csv` & `g2p-1.0.20230417/g2p/tests/public/data/haa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/ikt.psv` & `g2p-1.0.20230417/g2p/tests/public/data/ikt.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/iku-sro.psv` & `g2p-1.0.20230417/g2p/tests/public/data/iku-sro.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/kwk.psv` & `g2p-1.0.20230417/g2p/tests/public/data/kwk.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/mic.psv` & `g2p-1.0.20230417/g2p/tests/public/data/mic.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/moh.psv` & `g2p-1.0.20230417/g2p/tests/public/data/moh.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/oji-syl.psv` & `g2p-1.0.20230417/g2p/tests/public/data/oji-syl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/oka.csv` & `g2p-1.0.20230417/g2p/tests/public/data/oka.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/tau.psv` & `g2p-1.0.20230417/g2p/tests/public/data/tau.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/data/tli.csv` & `g2p-1.0.20230417/g2p/tests/public/data/tli.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/git_to_ipa.json` & `g2p-1.0.20230417/g2p/tests/public/git_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/README.md` & `g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/config.yaml` & `g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/mappings/gen-map_config.yaml` & `g2p-1.0.20230417/g2p/tests/public/mappings/gen-map_config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/mappings/minimal.xlsx` & `g2p-1.0.20230417/g2p/tests/public/mappings/minimal.xlsx`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/mappings/minimal_configs.yaml` & `g2p-1.0.20230417/g2p/tests/public/mappings/minimal_configs.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/public/sample_response.json` & `g2p-1.0.20230417/g2p/tests/public/sample_response.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/run.py` & `g2p-1.0.20230417/g2p/tests/run.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_api_resources.py` & `g2p-1.0.20230417/g2p/tests/test_api_resources.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_check_ipa_arpabet.py` & `g2p-1.0.20230417/g2p/tests/test_check_ipa_arpabet.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_cli.py` & `g2p-1.0.20230417/g2p/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_create_mapping.py` & `g2p-1.0.20230417/g2p/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_doctor.py` & `g2p-1.0.20230417/g2p/tests/test_doctor.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_doctor_expensive.py` & `g2p-1.0.20230417/g2p/tests/test_doctor_expensive.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_fallback.py` & `g2p-1.0.20230417/g2p/tests/test_fallback.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_indices.py` & `g2p-1.0.20230417/g2p/tests/test_indices.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_langs.py` & `g2p-1.0.20230417/g2p/tests/test_langs.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_lexicon_transducer.py` & `g2p-1.0.20230417/g2p/tests/test_lexicon_transducer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_mappings.py` & `g2p-1.0.20230417/g2p/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_network.py` & `g2p-1.0.20230417/g2p/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_studio.py` & `g2p-1.0.20230417/g2p/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_tokenize_and_map.py` & `g2p-1.0.20230417/g2p/tests/test_tokenize_and_map.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_tokenizer.py` & `g2p-1.0.20230417/g2p/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_transducer.py` & `g2p-1.0.20230417/g2p/tests/test_transducer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_unidecode_transducer.py` & `g2p-1.0.20230417/g2p/tests/test_unidecode_transducer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/test_utils.py` & `g2p-1.0.20230417/g2p/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 from collections import defaultdict
 from unittest import TestCase, main
 
 import yaml
 
+from g2p import get_arpabet_langs
 from g2p.exceptions import IncorrectFileType, MalformedMapping, RecursionError
 from g2p.log import LOGGER
 from g2p.mappings import Mapping, utils
 from g2p.tests.public import PUBLIC_DIR
 
 
 class UtilsTest(TestCase):
@@ -242,10 +243,22 @@
             ("é", [(0, 0), (1, 0)]),
         )
         self.assertEqual(
             utils.normalize_with_indices("é", "NFKD"),
             (e_acute_nfd, [(0, 0), (0, 1)]),
         )
 
+    def test_get_arpabet_langs(self):
+        LANGS, LANG_NAMES = get_arpabet_langs()
+        self.assertEqual(LANGS, sorted(LANGS))
+        self.assertEqual(list(LANG_NAMES.keys()), sorted(LANG_NAMES.keys()))
+        self.assertEqual(LANGS, list(LANG_NAMES.keys()))
+        self.assertTrue("kwk-umista" in LANG_NAMES)
+        self.assertTrue("str" in LANG_NAMES)
+        self.assertGreater(len(LANGS), 40)
+        LANGS2, LANG_NAMES2 = get_arpabet_langs()
+        self.assertIs(LANGS2, LANGS)
+        self.assertIs(LANG_NAMES2, LANG_NAMES)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230412/g2p/tests/test_z_local_config.py` & `g2p-1.0.20230417/g2p/tests/test_z_local_config.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/tests/time_panphon.py` & `g2p-1.0.20230417/g2p/tests/time_panphon.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p/transducer/__init__.py` & `g2p-1.0.20230417/g2p/transducer/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/g2p.egg-info/PKG-INFO` & `g2p-1.0.20230417/g2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230412
+Version: 1.0.20230417
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g2p-1.0.20230412/g2p.egg-info/SOURCES.txt` & `g2p-1.0.20230417/g2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230412/setup.py` & `g2p-1.0.20230417/setup.py`

 * *Files identical despite different names*

