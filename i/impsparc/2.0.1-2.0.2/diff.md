# Comparing `tmp/impsparc-2.0.1.tar.gz` & `tmp/impsparc-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/impsparc-2.0.1.tar", last modified: Tue Mar 14 14:43:59 2023, max compression
+gzip compressed data, was "impsparc-2.0.2.tar", last modified: Mon Apr 17 16:25:04 2023, max compression
```

## Comparing `impsparc-2.0.1.tar` & `impsparc-2.0.2.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.150410 impsparc-2.0.1/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1064 2022-06-08 04:47:51.000000 impsparc-2.0.1/LICENSE.md
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      244 2022-06-08 10:04:39.000000 impsparc-2.0.1/MANIFEST.in
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1098 2023-03-14 14:43:59.149722 impsparc-2.0.1/PKG-INFO
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      625 2022-07-19 15:54:12.000000 impsparc-2.0.1/README.md
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.773737 impsparc-2.0.1/cvsvc_apirisk/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.860618 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   363678 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   262350 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      615 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      753 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    23616 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    16394 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    16378 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.866587 impsparc-2.0.1/cvsvc_apirisk/score/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2891 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.883763 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967       80 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    59695 2023-03-14 11:28:56.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1503 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.922751 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2433 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2453 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2662 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2684 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2697 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2117 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2387 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2385 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2393 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2391 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2722 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2731 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.941816 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2346 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2474 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2477 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2459 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2462 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2760 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     3365 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/json_line.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.979442 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        0 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2084 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2418 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2339 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2867 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2292 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2163 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     5141 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2685 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2635 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2479 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2769 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.987877 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.769235 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.063346 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.083567 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    15291 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    16918 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    15192 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    28781 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    11370 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1363 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    11350 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    11421 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      966 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.136941 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      423 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    16193 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      209 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     3581 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     3478 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     3944 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      309 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      406 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     6482 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     9574 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1212 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    88994 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.994933 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:58.765887 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.008367 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   207965 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      687 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      756 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     2033 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.015400 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    59219 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   195090 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     4023 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    56178 2023-03-14 11:28:49.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.026681 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   100782 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   163872 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    80388 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    11245 2022-07-19 15:54:12.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      393 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.052344 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   181852 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   105536 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    60520 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    23940 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   388460 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967   154228 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    10556 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     4960 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     5478 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     3151 2023-03-14 10:44:59.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    26301 2023-03-14 10:31:55.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 priyank.chheda (1093858269) 347102967    12521 2022-06-08 04:47:51.000000 impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py
-drwxr-xr-x   0 priyank.chheda (1093858269) 347102967        0 2023-03-14 14:43:59.148295 impsparc-2.0.1/impsparc.egg-info/
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1098 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     6730 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967        1 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      165 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967      180 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/requires.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967       14 2023-03-14 14:43:58.000000 impsparc-2.0.1/impsparc.egg-info/top_level.txt
--rw-r--r--   0 priyank.chheda (1093858269) 347102967       38 2023-03-14 14:43:59.150676 impsparc-2.0.1/setup.cfg
--rw-r--r--   0 priyank.chheda (1093858269) 347102967     1191 2023-03-14 14:42:06.000000 impsparc-2.0.1/setup.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.560164 impsparc-2.0.2/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.2/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.2/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.559888 impsparc-2.0.2/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.2/README.md
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.338197 impsparc-2.0.2/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.357154 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.358863 impsparc-2.0.2/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.2/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.370710 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59992 2023-04-17 15:04:42.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.424161 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.472904 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.488972 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.490411 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.333743 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.537608 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.544739 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.556058 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.493009 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.330965 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.500709 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.505305 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.513775 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.530448 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    14646 2023-04-17 15:02:09.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.559378 impsparc-2.0.2/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      185 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-17 16:25:04.560245 impsparc-2.0.2/setup.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1196 2023-04-17 14:30:26.000000 impsparc-2.0.2/setup.py
```

### Comparing `impsparc-2.0.1/LICENSE.md` & `impsparc-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/PKG-INFO` & `impsparc-2.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.1
+Version: 2.0.2
 Summary: API Specification Analysis for Risks and Compliance
-Home-page: UNKNOWN
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
-License: UNKNOWN
-Description: # ImpSpARC
-        API Specification Analysis for Risks and Compliance
-        
-        ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
-        
-        API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
-        
-        ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# ImpSpARC
+
+API Specification Analysis for Risks and Compliance
+
+ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
+
+API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
+
+ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
+
```

### Comparing `impsparc-2.0.1/README.md` & `impsparc-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # ImpSpARC
+
 API Specification Analysis for Risks and Compliance
 
 ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
 
 API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
 
 ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/base.py` & `impsparc-2.0.2/cvsvc_apirisk/score/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         -------
         result: int
             Result desc
         """
         self.score = None
         self.meta = None
         self.children = {}      # If empty, means leaf node
+        self.score = 0
 
         return
 
     def __repr__(self):
         """
         Description
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,105 +13,119 @@
 from datetime import datetime
 import operator
 from collections import Counter
 import string
 import random
 import shutil
 import hashlib
-#import ipdb
 
 from jinja2 import Environment, FileSystemLoader
-from openapi_spec_validator.exceptions import OpenAPIValidationError
+from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 import numpy as np
-#import spacy
 
-from cvsvc_apirisk.score.spec_security.sps_main import SpecSecMain
 from cvsvc_apirisk.score.spec_security.sps_main_cr import SpecSecCustomRulesMain
 from cvsvc_apirisk.score.spec_security.sps_common import \
-        SEVERITY_CTGS, get_severity, init_rules_ds
+    SEVERITY_CTGS, get_severity, init_rules_ds
 from cvsvc_apirisk.score.spec_security.sps_common import get_api2 as api_fn
 from cvsvc_apirisk.score.spec_security.sps_common import get_api2_op as api_op_fn
 from cvsvc_apirisk.score.spec_security.sps_common import get_api2_param as api_param_fn
 from cvsvc_apirisk.score.spec_security.json_line import SaveLineRangeDecoder
-
+from cvsvc_apirisk.score.spec_security.yaml_line import LineLoader as YamlLineLoader
 
 UNZIP_DIR = '/tmp/cvapispecrisk_'
 # https://spacy.io/api/annotation#pos-tagging
 EXCL_POS = set(['NUM', 'PROPN', 'PUNCT', 'X', 'SYM', 'SPACE', 'NOUN'])
 qspecs = {}
 
+RISK_CTGS = {
+    'Security': 0,
+    'Data': 1,
+    'Format': 2
+}
+
+RISK_SUBCTGS = {
+    'Security': {
+        'Authentication': 0,
+        'Authorization': 1,
+        'Transport': 2
+    },
+    'Data': {},
+    'Format': {}
+}
+
 
 def print_heading(title):
     print()
     print(title)
-    print('-'*len(title))
-    return
+    print('-' * len(title))
 
 
 def check_one_spec(abs_path, report, cvrules_path, rules_path=None):
     target_obj = {}
 
-    print('-'*10)
+    print('-' * 10)
     print('- Analyzing %s...' % abs_path)
     with open(abs_path) as inf:
         report['files'][abs_path] = {}
         try:
             if abs_path.endswith('.json'):
                 raw_spec = json.load(inf)
                 inf.seek(0)
                 linenum_mapping = json.load(inf, cls=SaveLineRangeDecoder)
             elif abs_path.endswith('.yaml'):
                 raw_spec = yaml.safe_load(inf)
-                linenum_mapping = None
+                inf.seek(0)
+                loader = YamlLineLoader(inf)
+                linenum_mapping = loader.get_single_data()
             else:
                 raise ValueError('Incorrect input file. Should be JSON/YAML.')
 
-            #ipdb.set_trace()
+            # ipdb.set_trace()
 
             # Check whether OpenAPI v2 or v3
             if 'swagger' in raw_spec:
                 openapi_ver = 'v2'
             elif 'openapi' in raw_spec:
                 openapi_ver = 'v3'
             else:
                 raise ValueError('Incorrect specification format')
 
             target_obj['raw_spec'] = raw_spec
             spec_main_cr = \
-                    SpecSecCustomRulesMain(target_obj=target_obj,
-                                           target_filename=abs_path,
-                                           linenum_mapping=linenum_mapping,
-                                           openapi_ver=openapi_ver)
+                SpecSecCustomRulesMain(target_obj=target_obj,
+                                       target_filename=abs_path,
+                                       linenum_mapping=linenum_mapping,
+                                       openapi_ver=openapi_ver)
 
             rule_exps = {}
             for rules_file in filter(None, [cvrules_path, rules_path]):
 
                 if rules_file.endswith('.txt'):
                     rule_exps1 = spec_main_cr.read_rules_raw(rules_file)
                 elif rules_file.endswith('.json'):
                     rule_exps1 = spec_main_cr.read_rules_json(rules_file)
                 rule_exps.update(rule_exps1)
 
-            spec_main_cr.analyze_rules(rule_exps)
+            spec_main_cr.analyze_rules(rule_exps, abs_path=abs_path)
             spec_main = spec_main_cr.spec_main
 
             global RISK_CTGS, RISK_SUBCTGS
 
             RISK_CTGS, RISK_SUBCTGS = init_rules_ds(rule_exps)
             report['files'][abs_path]['status'] = 'valid'
             report['files'][abs_path]['score'] = spec_main.score
             report['files'][abs_path]['meta'] = spec_main.meta
             report['files'][abs_path]['num_apis'] = \
-                            len(spec_main.qspec.spec_obj['paths'])
+                len(spec_main.qspec.spec_obj['paths'])
             report['files'][abs_path]['num_params'] = \
-                            len(spec_main.qspec.get_param_objs()[0])
+                len(spec_main.qspec.get_param_objs()[0])
             report['files'][abs_path]['version'] = \
-                            target_obj['raw_spec']['info']['version']
+                target_obj['raw_spec']['info']['version']
             report['files'][abs_path]['num_evaluations'] = \
-                            spec_main_cr.num_evaluations
+                spec_main_cr.num_evaluations
             report['files'][abs_path]['req_method'] = spec_main.qspec.get_method_objs()
             report['files'][abs_path]['response_codes'] = spec_main.qspec.get_response_objs()[1]
             report['files'][abs_path]['data_types'] = spec_main.qspec.get_param_objs()[1]
 
             qspecs[abs_path] = spec_main.qspec
 
             # Init API data structures
@@ -121,19 +135,17 @@
                 init_api_ds(report, abs_path, api)
 
         except OpenAPIValidationError as e:
             report['files'][abs_path]['status'] = 'err'
             report['files'][abs_path]['meta'] = str(e)
             print('-> Error encountered for ', abs_path)
 
-    return
-
 
 def check_specs(spec_zip, cvrules_path, rules_path=None):
-    report = {}
+    report = dict()
 
     # Get the filename
     report['file_name'] = spec_zip
 
     # Get the file timestamp
     report['file_modified_time'] = \
         str(datetime.fromtimestamp(int(os.path.getmtime(spec_zip))))
@@ -153,29 +165,28 @@
         abs_path = '%s/%s' % (unzip_dir, filename)
         check_one_spec(abs_path, report, cvrules_path, rules_path=rules_path)
 
     return report, unzip_dir
 
 
 def analyze_apps(report):
-
     print_heading('App analysis')
 
     report['pdf']['page1']['sec2'] = {}
 
     ## Top-level app insights
     # Risk defined across all services
     risk_scores = [report['files'][f]['score'] for f in report['files'] \
-                                            if 'score' in report['files'][f]]
-    report['max_risk'] = max(risk_scores)
+                   if 'score' in report['files'][f]]
+    report['max_risk'] = max(risk_scores) if len(risk_scores) > 0 else 0
     print(('* Max risk across all application services:\t%d (%s)' %
            (report['max_risk'], get_severity(report['max_risk']))).expandtabs(20))
 
     # Risk statistics
-    report['avg_risk'] = round(np.mean(risk_scores), 2)
+    report['avg_risk'] = round(np.mean(risk_scores), 2) if len(risk_scores) > 0 else 0
     print(('* Average risk across all application services:\t%d' %
            report['avg_risk']).expandtabs(20))
 
     num_nz_risk = len(list(filter(lambda x: x > 0, risk_scores)))
     print(('* Number of application services with non-zero risk:\t%d' %
            num_nz_risk).expandtabs(20))
     num_z_risk = len(list(filter(lambda x: x == 0, risk_scores)))
@@ -189,39 +200,38 @@
     file_severities = []
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
         severities.append(get_severity(report['files'][f]['score']))
         file_severities.append((f, report['files'][f]['score']))
     print('* Number of application services by Severity:')
-    #for k, v in Counter(severities).items():
+    # for k, v in Counter(severities).items():
     ctr = Counter(severities)
     for k in SEVERITY_CTGS:
         print(('\t%s\t%d' % (k, ctr[k])).expandtabs(10))
         report['pdf']['page1']['sec2']['2a'][k] = ctr[k]
 
     print('* Top 5 application services ranked by Severity:')
     for f, score in sorted(file_severities, key=operator.itemgetter(1),
-            reverse=True)[:5]:
+                           reverse=True)[:5]:
         print(('    %s\t%s' % (f.split('/')[-1],
                                get_severity(score))).expandtabs(20))
 
-
     app_severity_riskctg = {}
     app_severity_risksubctg = {}
     ## Severity/Category-based app insights
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
 
         if f not in app_severity_riskctg:
             app_severity_riskctg[f] = {}
             app_severity_risksubctg[f] = {}
 
-        #for attr_score, remed_clue in report['files'][f]['meta']:
+        # for attr_score, remed_clue in report['files'][f]['meta']:
         for v in report['files'][f]['meta']:
             severity = get_severity(v['v_score'])
 
             if severity not in app_severity_riskctg[f]:
                 app_severity_riskctg[f][severity] = {}
                 app_severity_risksubctg[f][severity] = {}
 
@@ -252,111 +262,107 @@
                     severity_ctg_cnts[severity][risk_ctg] = 0
                 severity_ctg_cnts[severity][risk_ctg] += 1
 
     report['pdf']['page1']['sec2']['2b'] = {}
     # Initialize the data structure
     for sev in SEVERITY_CTGS:
         report['pdf']['page1']['sec2']['2b'][sev] = {}
-        for risk in RISK_CTGS:
+        for risk in RISK_CTGS or []:
             report['pdf']['page1']['sec2']['2b'][sev][risk] = 0
 
     # Now print
     for severity in sorted(severity_ctg_cnts, key=lambda s: SEVERITY_CTGS[s]):
         for ctg in sorted(severity_ctg_cnts[severity],
                           key=lambda r: RISK_CTGS[r]):
             print(('    %s\t%s\t%d' % (severity, ctg,
-                            severity_ctg_cnts[severity][ctg])).expandtabs(20))
+                                       severity_ctg_cnts[severity][ctg])).expandtabs(20))
             report['pdf']['page1']['sec2']['2b'][severity][ctg] = \
                 severity_ctg_cnts[severity][ctg]
-    return
 
 
 def analyze_apis_riskctg(report, api_riskctg_severity):
-
     report['pdf']['page1']['sec3']['3b'] = {}
     # Initialize the data structure
     for sev in SEVERITY_CTGS:
         report['pdf']['page1']['sec3']['3b'][sev] = {}
         for risk in RISK_CTGS:
             report['pdf']['page1']['sec3']['3b'][sev][risk] = 0
 
     print('* Number of APIs by RiskCategory-Severity:')
-    #for riskctg, severity_dict in api_riskctg_severity.items():
+    # for riskctg, severity_dict in api_riskctg_severity.items():
     for riskctg in sorted(api_riskctg_severity, key=lambda r: RISK_CTGS[r]):
         severity_dict = api_riskctg_severity[riskctg]
-        #for severity in severity_dict:
+        # for severity in severity_dict:
         for severity in sorted(severity_dict, key=lambda s: SEVERITY_CTGS[s]):
             print(('    %s\t%s\t%d' % (severity, riskctg,
-                        len(severity_dict[severity]['apis']))).expandtabs(20))
+                                       len(severity_dict[severity]['apis']))).expandtabs(20))
             report['pdf']['page1']['sec3']['3b'][severity][riskctg] = \
-                        len(severity_dict[severity]['apis'])
+                len(severity_dict[severity]['apis'])
 
     '''
     report['pdf']['page1']['sec3']['3c'] = {}
     # Initialize the data structure
     for sev in SEVERITY_CTGS:
         report['pdf']['page1']['sec3']['3c'][sev] = {}
         for risk in ['AuthN/AuthZ', 'API Transport']:
             report['pdf']['page1']['sec3']['3c'][sev][risk] = {}
             for subctg in RISK_SUBCTGS[risk]:
                 report['pdf']['page1']['sec3']['3c'][sev][risk][subctg] = 0
     '''
 
     print('* Number of APIs by RiskCategory-Severity-RiskSubCategory:')
-    #for riskctg, severity_dict in api_riskctg_severity.items():
+    # for riskctg, severity_dict in api_riskctg_severity.items():
     for riskctg in sorted(api_riskctg_severity, key=lambda r: RISK_CTGS[r]):
         severity_dict = api_riskctg_severity[riskctg]
-        #for severity in severity_dict:
+        # for severity in severity_dict:
         for severity in sorted(severity_dict, key=lambda s: SEVERITY_CTGS[s]):
             for risksubctg, apilist in \
                     severity_dict[severity]['subctgs'].items():
                 print(('    %s\t%s\t%s\t%d' % (severity, riskctg, risksubctg,
-                                             len(apilist))).expandtabs(20))
+                                               len(apilist))).expandtabs(20))
     '''
                 report['pdf']['page1']['sec3']['3c'][severity][riskctg][risksubctg] = \
                                              len(apilist)
     '''
 
     return
 
 
 def analyze_apis_uniq_severity_old(report, api_riskctg_severity):
-
     api_severity = Counter()
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
         for api in report['files'][f]['apis']:
             ctr = Counter(report['files'][f]['apis'][api]['severities'])
             for severity in ctr:
                 api_severity[severity] += 1
 
     print('* Number of APIs by Severity:')
-    #for k, v in api_severity.items():
-    #for severity in sorted(api_severity, key=lambda s: SEVERITY_CTGS[s]):
-    #for severity in SEVERITY_CTGS:
+    # for k, v in api_severity.items():
+    # for severity in sorted(api_severity, key=lambda s: SEVERITY_CTGS[s]):
+    # for severity in SEVERITY_CTGS:
     for severity in sorted(api_severity, key=lambda s: SEVERITY_CTGS[s]):
         print(('    %s\t%d' % (severity, api_severity[severity])).expandtabs(20))
-        #print(('    %s\t%d' % (severity, api_severity.get(severity,
+        # print(('    %s\t%d' % (severity, api_severity.get(severity,
         #                                                  0))).expandtabs(20))
 
     analyze_apis_riskctg(api_riskctg_severity)
 
     return
 
 
 def analyze_apis_uniq_api_new(report, api_riskctg_severity):
-
     severity_cntr = Counter()
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
         for api in report['files'][f]['apis']:
             max_score = max([v['v_score'] for v in \
-                                report['files'][f]['apis'][api]['meta']],
+                             report['files'][f]['apis'][api]['meta']],
                             default=0)
             max_score_severity = get_severity(max_score)
             severity_cntr[max_score_severity] += 1
 
     report['pdf']['page1']['sec3']['3a'] = {}
     # Initialize the data structure
     for sev in SEVERITY_CTGS:
@@ -376,23 +382,22 @@
     analyze_apis_riskctg(report, api_riskctg_severity)
 
     return
 
 
 def init_api_ds(report, f, api):
     report['files'][f]['apis'][api] = {}
-    #report['files'][f]['apis'][api]['severities'] = []
-    #report['files'][f]['apis'][api]['risk_ctg'] = []
-    #report['files'][f]['apis'][api]['risk_subctg'] = []
+    # report['files'][f]['apis'][api]['severities'] = []
+    # report['files'][f]['apis'][api]['risk_ctg'] = []
+    # report['files'][f]['apis'][api]['risk_subctg'] = []
     report['files'][f]['apis'][api]['meta'] = []
     return
 
 
 def analyze_apis(report):
-
     print_heading('API analysis')
 
     report['pdf']['page1']['sec3'] = {}
 
     api_riskctg_severity = {}
     ## Severity/Category-based API insights
     for f in report['files']:
@@ -409,44 +414,43 @@
             api = f.split('/')[-1] + ':' + api
             if api not in report['files'][f]['apis']:
                 init_api_ds(report, f, api)
 
             report['files'][f]['apis'][api]['meta'].append(v)
 
             severity = get_severity(v['v_score'])
-            #report['files'][f]['apis'][api]['severities'].append(severity)
+            # report['files'][f]['apis'][api]['severities'].append(severity)
             risk_ctg, risk_subctg = v['v_risk_ctg'], v['v_risk_subctg']
-            #report['files'][f]['apis'][api]['risk_ctg'].append(risk_ctg)
-            #if risk_subctg is not None:
+            # report['files'][f]['apis'][api]['risk_ctg'].append(risk_ctg)
+            # if risk_subctg is not None:
             #    report['files'][f]['apis'][api]['risk_subctg'].append(risk_subctg)
 
             if risk_ctg not in api_riskctg_severity:
                 api_riskctg_severity[risk_ctg] = {}
             if severity not in api_riskctg_severity[risk_ctg]:
                 api_riskctg_severity[risk_ctg][severity] = {}
                 api_riskctg_severity[risk_ctg][severity]['apis'] = set()
                 api_riskctg_severity[risk_ctg][severity]['subctgs'] = {}
             api_riskctg_severity[risk_ctg][severity]['apis'].add(api)
             if risk_subctg is not None:
                 if (risk_subctg not in
-                     api_riskctg_severity[risk_ctg][severity]['subctgs']):
-                    api_riskctg_severity[risk_ctg][severity]['subctgs'][risk_subctg] =  set()
+                        api_riskctg_severity[risk_ctg][severity]['subctgs']):
+                    api_riskctg_severity[risk_ctg][severity]['subctgs'][risk_subctg] = set()
                 api_riskctg_severity[risk_ctg][severity]['subctgs'][risk_subctg].add(api)
 
-    #analyze_apis_uniq_severity_old(report, api_riskctg_severity)
+    # analyze_apis_uniq_severity_old(report, api_riskctg_severity)
 
     analyze_apis_uniq_api_new(report, api_riskctg_severity)
 
-    #return api_riskctg_severity
+    # return api_riskctg_severity
 
     return
 
 
 def common_themes(report, nlp):
-
     print_heading('Common themes')
 
     report['pdf']['page1']['sec5'] = {}
 
     # Theme 1: Most frequently occuring violation
 
     violation2file = {}
@@ -465,68 +469,66 @@
     for code in violation2file:
         if len(violation2file[code]) > max_frq:
             most_frq_code = code
             max_frq = len(violation2file[code])
 
     if most_frq_code is not None:
         p1_1_text = '* Most frequently occuring violation:\t%s (%d)' % \
-                                (most_frq_code, max_frq)
+                    (most_frq_code, max_frq)
         print(p1_1_text.expandtabs(10))
 
-
         # Find the corresponding file
         file_ctr = sorted(Counter(violation2file[most_frq_code]).items(),
                           key=operator.itemgetter(1), reverse=True)
         most_frq_file, file_frq = file_ctr[0]
-        p1_2_text = 'App with the largest number of this violation: %s (%d)' %\
-                                    (most_frq_file.split('/')[-1], file_frq)
+        p1_2_text = 'App with the largest number of this violation: %s (%d)' % \
+                    (most_frq_file.split('/')[-1], file_frq)
 
         report['pdf']['page1']['sec5']['p1'] = p1_1_text + p1_2_text
 
     # Theme 2: Apps with multiple RiskSubCtg
     file2subctg = {}
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
 
         file2subctg[f] = {}
-        #for attr_score, remed_clue in report['files'][f]['meta']:
+        # for attr_score, remed_clue in report['files'][f]['meta']:
         for v in report['files'][f]['meta']:
             risk_ctg, risk_subctg = v['v_risk_ctg'], v['v_risk_subctg']
             if risk_subctg is None:
                 continue
             if risk_subctg not in file2subctg:
                 file2subctg[f][risk_subctg] = 0
             file2subctg[f][risk_subctg] += 1
 
     intr_files = []
     for f in file2subctg:
         if (('Authorization' in file2subctg[f]) and
                 ('Authentication' in file2subctg[f])):
             cnt = file2subctg[f]['Authorization'] + \
-                        file2subctg[f]['Authentication']
+                  file2subctg[f]['Authentication']
             intr_files.append((f, cnt))
     sorted_intr_files = sorted(intr_files, key=operator.itemgetter(1),
                                reverse=True)
 
     if len(sorted_intr_files) > 0:
-        p2_text = '* %d application service(s) contain both Authorization and '\
-              'Authentication based Security violations. Most violations occur'\
-              ' for the app: %s.' % (len(intr_files),
-                                     sorted_intr_files[0][0].split('/')[-1])
+        p2_text = '* %d application service(s) contain both Authorization and ' \
+                  'Authentication based Security violations. Most violations occur' \
+                  ' for the app: %s.' % (len(intr_files),
+                                         sorted_intr_files[0][0].split('/')[-1])
         print(p2_text)
         report['pdf']['page1']['sec5']['p2'] = p2_text
 
     # Description stats
-    #get_description_stats(report, nlp)
+    # get_description_stats(report, nlp)
     return
 
 
 def high_level_info(report):
-
     print_heading('Basic information')
 
     ## High level info
     print(('* Zip file name:\t%s' % report['file_name']).expandtabs(80))
     print(('* Zip file uploaded on:\t%s' % report['file_modified_time']).expandtabs(80))
     report['num_appsvcs'] = len(report['files'])
 
@@ -546,113 +548,112 @@
 
     print(('* Total number of application services:\t%d' %
            total_files).expandtabs(80))
     report['total_apis'] = total_apis
     print(('* Total number of APIs observed across all services:\t%d' %
            report['total_apis']).expandtabs(80))
 
-    #print(('* Total number of Parameters observed across all services:\t%d' %
+    # print(('* Total number of Parameters observed across all services:\t%d' %
     #       total_params).expandtabs(80))
 
     print(('* Total number of violations across all services:\t%d (out of'
            ' %d checks)' %
            (total_violations, total_evaluations)).expandtabs(80))
     report['pdf']['page1']['sec4'] = {}
     report['pdf']['page1']['sec4']['total_violations'] = total_violations
     report['pdf']['page1']['sec4']['total_evaluations'] = total_evaluations
 
     # Top 5 apps by APIs
     print('* Top 5 application services by num APIs')
-    #return report
+    # return report
     data = sorted({k: v['num_apis'] for k, v in report['files'].items() \
-                                        if 'num_apis' in v}.items(),
+                   if 'num_apis' in v}.items(),
                   key=operator.itemgetter(1), reverse=True)
     for filename, num_apis in data[:5]:
         print(('    %s\t%d' % (filename.split('/')[-1], num_apis)).expandtabs(40))
 
     return
 
 
 def insights(report):
-
     print_heading('Insights')
 
     api2op = {}
     api2params = {}
     for f in report['files']:
         if report['files'][f]['status'] == 'err':
             continue
 
-        #for attr_score, remed_clue in report['files'][f]['meta']:
+        # for attr_score, remed_clue in report['files'][f]['meta']:
         for v in report['files'][f]['meta']:
             remed_clue = '%s %s %s' % (v['v_ruleid'], v['v_entity'],
                                        v['v_description'])
             api = api_fn(remed_clue)
             if api is None:
                 continue
             api = f.split('/')[-1] + ':' + api
-            #print(api)
+            # print(api)
             if api not in api2op:
                 api2op[api] = {}
                 api2params[api] = {}
 
             api_op = api_op_fn(remed_clue)
             api_param = api_param_fn(remed_clue)
 
             if api_param is not None:
                 api2params[api][api_param] = True
 
-            #print(api_op)
-            #print(attr_score)
-            #print(remed_clue)
+            # print(api_op)
+            # print(attr_score)
+            # print(remed_clue)
             severity = get_severity(v['v_score'])
             if severity == 'Critical' and api_op in ('post', 'put'):
                 api2op[api]['postput'] = 1
             if severity == 'Critical' and api_op in ('get', 'post'):
                 api2op[api]['getpost'] = 1
 
     if len(api2op) > 0:
         # 1. POST/PUT
         num = len([a for a in api2op if 'postput' in api2op[a]])
         den = len(api2op)
-        perc1 = num*100.0/den
+        perc1 = num * 100.0 / den
         if perc1 > 0.0:
-            data_in_text = '* %02d%% of APIs have Critical violations among'\
-                'POST/PUT operations which bring data into your environment.' % perc1
+            data_in_text = '* %02d%% of APIs have Critical violations among' \
+                           'POST/PUT operations which bring data into your environment.' % perc1
             print(data_in_text)
             report['pdf']['page1']['sec4']['data_in'] = data_in_text
 
         # 2. GET/POST
         num = len([a for a in api2op if 'getpost' in api2op[a]])
         den = len(api2op)
-        perc2 = num*100.0/den
+        perc2 = num * 100.0 / den
         if perc2 > 0.0:
-            data_out_text = '* %02d%% of APIs have Critical violations among'\
-                'GET/POST operations which pull data out of your environment.' % perc2
+            data_out_text = '* %02d%% of APIs have Critical violations among' \
+                            'GET/POST operations which pull data out of your environment.' % perc2
             print(data_out_text)
             report['pdf']['page1']['sec4']['data_out'] = data_out_text
 
     if len(api2params) > 0:
-        #print(api2params)
+        # print(api2params)
         # 3. Num of APIs with high param violations
         num = len([a for a in api2params if len(api2params[a]) > 3])
         den = len(api2params)
-        perc3 = num*100.0/den
+        perc3 = num * 100.0 / den
         if perc3 > 0.0:
-            problem_parameters = '* %02d%% of APIs have more than 3 '\
-                'parameters that have contributed to a violation.' % perc3
+            problem_parameters = '* %02d%% of APIs have more than 3 ' \
+                                 'parameters that have contributed to a violation.' % perc3
             print(problem_parameters)
             report['pdf']['page1']['sec4']['problem_parameters'] = problem_parameters
 
     return
 
 
 def print_samples(report, spec_path):
     f = spec_path
-    print('-'*100)
+    print('-' * 100)
     print('Spec: %s\n' % f)
 
     if report['files'][f]['status'] == 'err':
         return
 
     grouped_violations = {}
     for v in report['files'][f]['meta']:
@@ -662,43 +663,43 @@
         if api not in grouped_violations:
             grouped_violations[api] = []
         grouped_violations[api].append(v)
 
     # Print the global violations first
     if None in grouped_violations:
         for v in grouped_violations.get(None):
-            print('-'*20)
+            print('-' * 20)
             print(('\t%s\n\t%d\t%s\t%s\n\t%s' % (v['v_description'],
                                                  v['v_score'],
                                                  get_severity(v['v_score']),
                                                  v['v_ruleid'],
                                                  v['v_entity']
                                                  )).expandtabs(10))
-        del(grouped_violations[None])
+        del (grouped_violations[None])
 
     for api in grouped_violations:
         for v in grouped_violations[api]:
-            print('-'*20)
+            print('-' * 20)
             print(('\t%s\n\t%d\t%s\t%s\n\t%s' % (v['v_description'],
                                                  v['v_score'],
                                                  get_severity(v['v_score']),
                                                  v['v_ruleid'],
                                                  v['v_entity']
                                                  )).expandtabs(10))
 
     return
 
 
 def is_english_sentence(astr, nlp):
     doc = nlp(astr)
     legit_pos = list(filter(lambda token: token.pos_ not in EXCL_POS, doc))
 
-    verdict = (len(legit_pos) >= 2)     # "2" to reduce FPs such as addresses
+    verdict = (len(legit_pos) >= 2)  # "2" to reduce FPs such as addresses
 
-    #print(astr, verdict)
+    # print(astr, verdict)
 
     return verdict
 
 
 def get_description_stats(report, nlp):
     global qspecs
 
@@ -710,21 +711,20 @@
             # Get the desc string
             desc_str_node = list(qspec.G.neighbors(desc_node))[0]
             desc_str = qspec.G.nodes[desc_str_node]['nodenameraw']
             total_desc += 1
             if is_english_sentence(desc_str, nlp):
                 engl_desc += 1
 
-    redo_desc = (1 - (engl_desc*1.0/total_desc))*100.0
+    redo_desc = (1 - (engl_desc * 1.0 / total_desc)) * 100.0
     print('* %02d%% of descriptions need work.' % redo_desc)
     return
 
 
 def most_frq_violation(filename, report):
-
     codes = []
     for v in report['files'][filename]['meta']:
         code_str = '[%s] %s' % (v['v_ruleid'], v['v_description'])
         codes.append(code_str)
 
     try:
         mfrq = sorted(Counter(codes).items(), key=operator.itemgetter(1),
@@ -733,27 +733,26 @@
         # no violations
         mfrq = ('-', 0)
 
     return mfrq
 
 
 def write_pdf_json(report, output_json, cvrules_path):
-
     # Page 1 data
 
     # Page 1: Section 1
     report['pdf']['page1']['sec1'] = {}
     now = datetime.now()
     report['pdf']['page1']['sec1']['today'] = \
-                                    datetime.strftime(now, '%a, %B %d, %Y')
+        datetime.strftime(now, '%a, %B %d, %Y')
     report['pdf']['page1']['sec1']['file_name'] = \
-                                    report['file_name'].split('/')[-1]
+        report['file_name'].split('/')[-1]
     report['pdf']['page1']['sec1']['max_risk_score'] = report['max_risk']
     report['pdf']['page1']['sec1']['severity'] = \
-                                    get_severity(report['max_risk'])
+        get_severity(report['max_risk'])
     report['pdf']['page1']['sec1']['num_appsvcs'] = report['num_appsvcs']
     report['pdf']['page1']['sec1']['total_apis'] = report['total_apis']
 
     # Page 2 data
     with open(cvrules_path) as inf:
         rules_dict = json.load(inf)
         ruleid2impact = {}
@@ -805,129 +804,126 @@
 
         # Finally drop the original key
         report['pdf']['page2'].pop(sev)
 
     if output_json is not None:
         # Write the data structure
         with open(output_json, 'w') as outf:
-            json.dump(report, outf)
+            json.dump(report, outf, indent=1)
 
     return
 
 
 def write_json(report, output_json):
-
     # Repurpose the "report" data structure
     for f in report['files']:
 
         report['files'][f]['properties'] = {}
         if report['files'][f]['status'] == 'err':
             report['files'][f]['properties']['status'] = \
-                                report['files'][f].pop('status')
+                report['files'][f].pop('status')
             report['files'][f]['properties']['err_detail'] = \
-                                report['files'][f].pop('meta')
+                report['files'][f].pop('meta')
             report['files'][f]['violations'] = []
         else:
             # Rename the "meta" key to "violations"
             report['files'][f]['violations'] = report['files'][f].pop('meta')
             # Bring file properties together
             report['files'][f]['properties'] = {}
             report['files'][f]['properties']['score'] = \
-                                report['files'][f].pop('score')
+                report['files'][f].pop('score')
             report['files'][f]['properties']['status'] = \
-                                report['files'][f].pop('status')
+                report['files'][f].pop('status')
             report['files'][f]['properties']['num_apis'] = \
-                                report['files'][f].pop('num_apis')
+                report['files'][f].pop('num_apis')
             report['files'][f]['properties']['num_params'] = \
-                                report['files'][f].pop('num_params')
+                report['files'][f].pop('num_params')
             report['files'][f]['properties']['num_evaluations'] = \
-                                report['files'][f].pop('num_evaluations')
+                report['files'][f].pop('num_evaluations')
             report['files'][f]['properties']['version'] = \
-                                report['files'][f].pop('version')
+                report['files'][f].pop('version')
 
             for api in report['files'][f]['apis']:
                 report['files'][f]['apis'][api]['violations'] = \
-                        report['files'][f]['apis'][api].pop('meta')
+                    report['files'][f]['apis'][api].pop('meta')
 
     if output_json is not None:
         # Write the data structure
         with open(output_json, 'w') as outf:
-            json.dump(report, outf)
+            json.dump(report, outf, indent=1)
 
     return
 
 
 def compare_specs(ospec, uspec, output_json, cvrules_path, rules_path=None):
-
     report = {}
     report['pdf'] = {}
     report['pdf']['page1'] = {}
 
     report['files'] = {}
     for abs_path in (ospec, uspec):
         check_one_spec(abs_path, report, cvrules_path, rules_path=rules_path)
 
     # Now get statistics between the two files
-    print('-'*100)
+    print('-' * 100)
     print(('\t*** Spec Comparison ***\n\n').expandtabs(40))
     print(('* File:\t%s\t%s' % (ospec, uspec)).expandtabs(40))
     print(('* Version:\t%s\t%s' % (report['files'][ospec]['version'],
-                            report['files'][uspec]['version'])).expandtabs(40))
+                                   report['files'][uspec]['version'])).expandtabs(40))
 
     num_violations_o = len(report['files'][ospec]['meta'])
     num_violations_u = len(report['files'][uspec]['meta'])
     print(('* Number of violations:\t%d\t%d' % (num_violations_o,
-                                            num_violations_u)).expandtabs(40))
+                                                num_violations_u)).expandtabs(40))
 
     ospec_score = report['files'][ospec]['score']
     ospec_severity = get_severity(ospec_score)
     uspec_score = report['files'][uspec]['score']
     uspec_severity = get_severity(uspec_score)
     print(('* Score:\t%d\t%d' % (ospec_score, uspec_score)).expandtabs(40))
     print(('* Severity:\t%s\t%s' % (ospec_severity,
                                     uspec_severity)).expandtabs(40))
     # Most frequent violation
     mfrq_ospec = most_frq_violation(ospec, report)
     mfrq_uspec = most_frq_violation(uspec, report)
     print(('* Most frq violation:\t%s (%d)\t%s (%d)' % \
-            (mfrq_ospec[0], mfrq_ospec[1], mfrq_uspec[0], mfrq_uspec[1])).expandtabs(40))
+           (mfrq_ospec[0], mfrq_ospec[1], mfrq_uspec[0], mfrq_uspec[1])).expandtabs(40))
 
     write_json(report, output_json)
 
     return
 
 
 def generate_report_zip(spec_zip, output_json, cvrules_path,
                         rules_path=None):
-
     report, unzip_dir = check_specs(spec_zip, cvrules_path,
                                     rules_path=rules_path)
 
-    print('='*100)
-    print('\t'*3, '** Imperva API Risk Assessment Report **')
-    print('\t'*3, '-'*45, '\n'*2)
+    print('=' * 100)
+    print('\t' * 3, '** Imperva API Risk Assessment Report **')
+    print('\t' * 3, '-' * 45, '\n' * 2)
 
-    nlp = None  #spacy.load("en_core_web_sm")
+    nlp = None  # spacy.load("en_core_web_sm")
     print('Initializing...')
-    #return report
+    # return report
 
-    print('-'*100)
+    print('-' * 100)
     high_level_info(report)
-    print('-'*100)
+    print('-' * 100)
     analyze_apps(report)
-    print('-'*100)
+    print('-' * 100)
     analyze_apis(report)
-    print('-'*100)
+    print('-' * 100)
     common_themes(report, nlp)
-    print('-'*100)
+    print('-' * 100)
     insights(report)
-    print('-'*100)
+    print('-' * 100)
     if spec_zip.endswith('orangebank.zip'):
         spec_path = '%s/orangebank_stores.json' % unzip_dir
-        #spec_path = random.sample(report['files'].keys(), 1)[0]
+        # spec_path = random.sample(report['files'].keys(), 1)[0]
         print_samples(report, spec_path)
 
     write_json(report, output_json)
     write_pdf_json(report, output_json, cvrules_path)
 
     return report
 
@@ -949,33 +945,33 @@
     report['files'] = {}
     check_one_spec(spec_path, report, cvrules_path, rules_path=rules_path)
 
     # Check for errors
     if report['files'][spec_path]['status'] == 'err':
         return report
 
-    print('-'*100)
+    print('-' * 100)
     high_level_info(report)
-    print('-'*100)
+    print('-' * 100)
     analyze_apps(report)
-    print('-'*100)
+    print('-' * 100)
     analyze_apis(report)
 
     # Num APIs
     print(('* Number of APIs:\t%d' %
-                    report['files'][spec_path]['num_apis']).expandtabs(40))
+           report['files'][spec_path]['num_apis']).expandtabs(40))
     # Num parameters
     print(('* Number of parameters:\t%d' %
-                    report['files'][spec_path]['num_params']).expandtabs(40))
+           report['files'][spec_path]['num_params']).expandtabs(40))
 
     # Num of violations
     total_violations = len(report['files'][spec_path]['meta'])
     total_evaluations = report['files'][spec_path]['num_evaluations']
     print(('* Number of violations:\t%d (out of %d checks)' %
-                    (total_violations, total_evaluations)).expandtabs(40))
+           (total_violations, total_evaluations)).expandtabs(40))
 
     # Score assigned
     print(('* Score:\t%d' % report['files'][spec_path]['score']).expandtabs(40))
     # Severity assigned
     severity = get_severity(report['files'][spec_path]['score'])
     print(('* Severity:\t%s' % severity).expandtabs(40))
     # All violations
@@ -983,14 +979,15 @@
 
     # Always remove PDF data
     report.pop('pdf', None)
     write_json(report, output_json)
 
     return report
 
+
 def check_cicd_criteria(report, cicd_criteria_path):
     scores = []
     for f in report['files']:
         if report['files'][f]['properties']['status'] == 'err':
             continue
         scores.append(report['files'][f]['properties']['score'])
 
@@ -1030,17 +1027,17 @@
 def main(argv=sys.argv):
     apar = ArgumentParser()
     subpar = apar.add_subparsers(help='sub-command help', dest='command')
 
     parser_eval_risk = subpar.add_parser('eval_risk', help='eval_risk help')
     group = parser_eval_risk.add_mutually_exclusive_group()
     group.add_argument('-z', dest='spec_zip_path',
-                                  help='Spec zip path')
+                       help='Spec zip path')
     group.add_argument('-s', dest='spec_file_path',
-                                  help='Spec file path')
+                       help='Spec file path')
     parser_eval_risk.add_argument('-i', dest='cv_rules_path',
                                   help='Imperva rules path')
     parser_eval_risk.add_argument('-r', dest='custom_rules_path',
                                   help='Custom rules path')
     parser_eval_risk.add_argument('-o', dest='output_json_path',
                                   required=True, help='Output JSON path')
     parser_eval_risk.add_argument('-c', dest='cicd_criteria_path',
@@ -1093,14 +1090,15 @@
                                           args.cv_rules_path,
                                           args.custom_rules_path)
         if args.cicd_criteria_path:
             check_cicd_criteria(report, args.cicd_criteria_path)
 
     return
 
+
 def compute_counts(report):
     """
     {
         'num_of_params': 12,
         'num_of_data_types': 1,
         'response_codes': [
             '200',
@@ -1184,31 +1182,35 @@
         req_method_list.append(req_method.upper())
         req_method_count.append(req_count)
     counts['req_method_list'] = req_method_list
     counts['req_method_count'] = req_method_count
 
     return counts
 
+
 def contains_param(entity):
+    if isinstance(entity, dict):
+        entity = entity['reference_path']
     if entity.startswith('(#->paths') and "parameters->" in entity:
         return True
     return False
 
+
 def get_highest_sev_params_api_count(report, sev, ctg):
     param_list = set()
     api_list = set()
     files = report.get('files', {})
     for file_name, val in files.items():
         apis = val.get('apis', {})
         for api, api_val in apis.items():
             violations = api_val.get('violations', [])
             for violation in violations:
                 entity = violation.get('v_entity', '')
                 if violation.get('v_severity', '') == sev and violation.get('v_risk_ctg', '') == ctg:
-                    if contains_param(entity): 
+                    if contains_param(entity):
                         param_list.add(get_param_from_entity(entity))
                     api_list.add(api)
     return len(param_list), len(api_list)
 
 
 def compute_violation_counts(report):
     """
@@ -1264,25 +1266,25 @@
 
             highest_sev = None
             if risk_ctg in violation_counts:
                 risk_ctg_counts = violation_counts[risk_ctg]
 
                 if risk_sub_ctg in risk_ctg_counts.get('risk_sub_ctg', {}):
                     risk_ctg_counts['risk_sub_ctg'][risk_sub_ctg] += 1
-                else: 
+                else:
                     risk_ctg_counts['risk_sub_ctg'][risk_sub_ctg] = 1
 
                 if severity in risk_ctg_counts:
                     risk_ctg_counts[severity] += 1
                 else:
                     risk_ctg_counts[severity] = 1
 
                 if 'total_count' in risk_ctg_counts:
                     risk_ctg_counts['total_count'] += 1
-                else: 
+                else:
                     risk_ctg_counts['total_count'] = 1
 
                 if 'highest_sev' in risk_ctg_counts:
                     highest_sev = risk_ctg_counts['highest_sev']
                     if highest_sev.lower() == 'critical':
                         continue
                     elif highest_sev.lower() == 'high' and severity.lower() == 'critical':
@@ -1318,42 +1320,48 @@
         sev = violation_counts[k]['highest_sev']
         param_count, api_count = get_highest_sev_params_api_count(report, sev, k)
         violation_counts[k]['highest_sev_param_count'] = param_count
         violation_counts[k]['highest_sev_api_count'] = api_count
         violation_counts[k]['highest_sev_count'] = violation_counts[k][sev]
     return violation_counts
 
+
 def get_param_from_entity(entity):
     param = ''
+    if isinstance(entity, dict):
+        entity = entity['reference_path']
     start = entity.index('(') + len('(')
     end = entity.index(')', start)
     api_param = entity[start:end]
     split_list = api_param.split('->')
     for i in range(6):
         param = param + '->' + split_list[i]
     return param
 
+
 def initialise_issue_insights(issue_insights, risk_ctg, risk_sub_ctg, i_type):
     issue_insights[risk_ctg][risk_sub_ctg][i_type] = set()
-    issue_insights[risk_ctg][risk_sub_ctg]['critical_'+i_type] = set()
-    issue_insights[risk_ctg][risk_sub_ctg]['high_'+i_type] = set()
-    issue_insights[risk_ctg][risk_sub_ctg]['medium_'+i_type] = set()
-    issue_insights[risk_ctg][risk_sub_ctg]['low_'+i_type] = set()
+    issue_insights[risk_ctg][risk_sub_ctg]['critical_' + i_type] = set()
+    issue_insights[risk_ctg][risk_sub_ctg]['high_' + i_type] = set()
+    issue_insights[risk_ctg][risk_sub_ctg]['medium_' + i_type] = set()
+    issue_insights[risk_ctg][risk_sub_ctg]['low_' + i_type] = set()
+
 
 def add_sev_issue_insights(issue_insights, risk_ctg, risk_sub_ctg, i_type, val, severity):
     if not val: return
     issue_insights[risk_ctg][risk_sub_ctg][i_type].add(val)
     if severity == 'critical':
-        issue_insights[risk_ctg][risk_sub_ctg]['critical_'+i_type].add(val)
+        issue_insights[risk_ctg][risk_sub_ctg]['critical_' + i_type].add(val)
     elif severity == 'high':
-        issue_insights[risk_ctg][risk_sub_ctg]['high_'+i_type].add(val)
+        issue_insights[risk_ctg][risk_sub_ctg]['high_' + i_type].add(val)
     elif severity == 'medium':
-        issue_insights[risk_ctg][risk_sub_ctg]['medium_'+i_type].add(val)
+        issue_insights[risk_ctg][risk_sub_ctg]['medium_' + i_type].add(val)
     else:
-        issue_insights[risk_ctg][risk_sub_ctg]['low_'+i_type].add(val)
+        issue_insights[risk_ctg][risk_sub_ctg]['low_' + i_type].add(val)
+
 
 def add_violation(issue_insights, violation, file_name, api=''):
     violation_hash = hashlib.md5((json.dumps(violation) + file_name).encode()).hexdigest()
     if violation_hash in issue_insights.get('hash_list', set()):
         return
     risk_ctg = violation.get('v_risk_ctg', '')
     risk_sub_ctg = violation.get('v_risk_subctg', '')
@@ -1392,14 +1400,15 @@
         issue_insights[risk_ctg]['api_list'].add(api)
         add_sev_issue_insights(issue_insights, risk_ctg, risk_sub_ctg, 'apis', api, severity)
     if contains_param(entity):
         param = get_param_from_entity(entity)
         issue_insights[risk_ctg]['param_list'].add(param)
         add_sev_issue_insights(issue_insights, risk_ctg, risk_sub_ctg, 'params', param, severity)
 
+
 def get_issue_insights(report):
     """
     {
         'Data Type Definitions': {
             'Undefined Bounds': {
                 'apis': {
                     'orangebank_user.json:/history'
@@ -1421,35 +1430,37 @@
             for each_violation in violations:
                 add_violation(issue_insights, each_violation, file_name, api)
         violations = record.get('violations', [])
         for violation in violations:
             add_violation(issue_insights, violation, file_name)
     return issue_insights
 
+
 def copytree(src, dst, symlinks=False, ignore=None):
     for item in os.listdir(src):
         try:
             s = os.path.join(src, item)
             d = os.path.join(dst, item)
             if os.path.isdir(s):
                 shutil.copytree(s, d, symlinks, ignore)
             else:
                 shutil.copy2(s, d)
         except FileExistsError:
             pass
 
+
 def generate_html_new(report, output_path, customer_name='N/A'):
     curr_dir = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(curr_dir, 'sparc-templates-new')
     output_dir = os.path.join(os.path.dirname(os.path.abspath(output_path)), 'sparc_report')
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     # Copy css files to output directory
-    copytree(templates_dir, output_dir, symlinks = True)
+    copytree(templates_dir, output_dir, symlinks=True)
     os.remove(os.path.join(output_dir, 'risk-report-template-generic.html'))
 
     # NOTE: I have deleted index_raw.html from the template folder but for
     # some reason this file is still present on pypi server.
     # TODO: delete next 3 lines when index_raw.html is removed from pypi package
     index_raw = os.path.join(output_dir, 'index_raw.html')
     if os.path.isfile(index_raw):
@@ -1474,44 +1485,43 @@
         elif 'medium' in key.lower():
             violation_details['Major'].update(value)
         elif 'low' in key.lower():
             violation_details['Minor'].update(value)
 
     with open(html_file, 'w') as fh:
         fh.write(template.render(
-            customer_name = customer_name,
-            created_time = dt_string,
-            file_name = report.get('file_name', 'N/A'),
-            num_of_files = len(report.get('files')),
-            num_of_apis = report.get('total_apis', 0),
-            num_of_params = counts.get('num_of_params', 0),
-            num_of_data_types = counts.get('num_of_data_types', 0),
-            response_codes = counts.get('response_codes', []),
-            r_codes_count = counts.get('response_codes_count', []),
-            data_types = counts.get('d_types', []),
-            data_type_counts = counts.get('d_type_counts', []),
-            req_method_list = counts.get('req_method_list', []),
-            req_method_count = counts.get('req_method_count', []),
-            violations = violation_counts,
-            num_of_evaluations = counts.get('num_evaluations', 0),
-            issue_insights = issue_insights,
-            violation_details = violation_details,
+            customer_name=customer_name,
+            created_time=dt_string,
+            file_name=report.get('file_name', 'N/A'),
+            num_of_files=len(report.get('files')),
+            num_of_apis=report.get('total_apis', 0),
+            num_of_params=counts.get('num_of_params', 0),
+            num_of_data_types=counts.get('num_of_data_types', 0),
+            response_codes=counts.get('response_codes', []),
+            r_codes_count=counts.get('response_codes_count', []),
+            data_types=counts.get('d_types', []),
+            data_type_counts=counts.get('d_type_counts', []),
+            req_method_list=counts.get('req_method_list', []),
+            req_method_count=counts.get('req_method_count', []),
+            violations=violation_counts,
+            num_of_evaluations=counts['num_evaluations'] if counts.get('num_evaluations', 0) > 0 else -1,
+            issue_insights=issue_insights,
+            violation_details=violation_details,
         ))
-    return
 
 
 def generate_html(report, output_path):
     curr_dir = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(curr_dir, 'sparc-templates')
     output_dir = os.path.join(os.path.dirname(os.path.abspath(output_path)), 'sparc_report_old')
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
-    #Copy css files to output directory
-    copytree(templates_dir, output_dir, symlinks = True)
+    # Copy css files to output directory
+    copytree(templates_dir, output_dir, symlinks=True)
 
     html_file = os.path.join(output_dir, 'index.html')
 
     current_time = datetime.now()
     dt_string = current_time.strftime("%B %d, %Y %H:%M:%S")
 
     env = Environment(loader=FileSystemLoader(templates_dir))
@@ -1520,27 +1530,28 @@
     counts = compute_counts(report)
     violation_counts = compute_violation_counts(report)
     issue_insights = get_issue_insights(report)
     violation_details = report.get('pdf', {}).get('page2', {})
 
     with open(html_file, 'w') as fh:
         fh.write(template.render(
-            created_time = dt_string,
-            num_of_files = len(report.get('files')),
-            num_of_apis = report.get('total_apis', 0),
-            num_of_params = counts.get('num_of_params', 0),
-            num_of_data_types = counts.get('num_of_data_types', 0),
-            response_codes = counts.get('response_codes', []),
-            r_codes_count = counts.get('response_codes_count', []),
-            data_types = counts.get('d_types', []),
-            data_type_counts = counts.get('d_type_counts', []),
-            req_method_list = counts.get('req_method_list', []),
-            req_method_count = counts.get('req_method_count', []),
-            violations = violation_counts,
-            num_of_evaluations = counts.get('num_evaluations', 0),
-            issue_insights = issue_insights,
-            violation_details = violation_details,
+            created_time=dt_string,
+            num_of_files=len(report.get('files')),
+            num_of_apis=report.get('total_apis', 0),
+            num_of_params=counts.get('num_of_params', 0),
+            num_of_data_types=counts.get('num_of_data_types', 0),
+            response_codes=counts.get('response_codes', []),
+            r_codes_count=counts.get('response_codes_count', []),
+            data_types=counts.get('d_types', []),
+            data_type_counts=counts.get('d_type_counts', []),
+            req_method_list=counts.get('req_method_list', []),
+            req_method_count=counts.get('req_method_count', []),
+            violations=violation_counts,
+            num_of_evaluations=counts.get('num_evaluations', 0),
+            issue_insights=issue_insights,
+            violation_details=violation_details,
         ))
     return
 
+
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+
 #
 # Custom scanner factory
 #   context: the custom JSONDecoder object
 #
 def make_my_scanner(context):
     # reference to actual scanner (defined by the JSONDecoder)
     interal_scanner = json.scanner.py_make_scanner(context)
@@ -12,70 +13,69 @@
     # customized _myscan
     #   string is the json string buf
     #   idx starts w 0 and advance as the parser scans
     #
     def _myscan(string, idx):
         try:
             nextchar = string[idx]
-        except IndexError:      # ignore testing nextchar
+        except IndexError:  # ignore testing nextchar
             pass
 
         #
         # passing down custom parser
         #   before recursively parsing down, calculate the start line number
         #   when done, calculate the line number again to get the range
         #
         #   a dict object is added to the existing dict or appended to the array
         #   secret-handshake cvlrange26uel7Ao is entirely arbitrary to avoid conliction
         #
         if nextchar == '{':
             context.countlines(string, idx)
             startline = context.lineno
             (theobj, l) = context.parse_object((string, idx + 1),
-                                          context.strict,
-                                          _myscan,
-                                          context.object_hook,
-                                          context.object_pairs_hook)
+                                               context.strict,
+                                               _myscan,
+                                               context.object_hook,
+                                               context.object_pairs_hook)
             context.countlines(string, l)
-            theobj['cvlrange26uel7Ao']=(startline, context.lineno)
+            theobj['cvlrange26uel7Ao'] = (startline, context.lineno)
             return (theobj, l)
         elif nextchar == '[':
             context.countlines(string, idx)
             startline = context.lineno
-            (theobj,l) = context.parse_array((string, idx + 1),
-                                         _myscan)
+            (theobj, l) = context.parse_array((string, idx + 1),
+                                              _myscan)
             context.countlines(string, l)
-            theobj.append({'cvlrange26uel7Ao':(startline, context.lineno)})
+            theobj.append({'cvlrange26uel7Ao': (startline, context.lineno)})
             return (theobj, l)
         else:
             context.countlines(string, idx)
             startline = context.lineno
             (theobj, l) = interal_scanner(string, idx)
             context.countlines(string, idx)
-            newobj = (theobj, {'cvlrange26uel7Ao':(startline, context.lineno)})
+            newobj = (theobj, {'cvlrange26uel7Ao': (startline, context.lineno)})
             return (newobj, l)
 
     return _myscan
 
 
 class SaveLineRangeDecoder(json.JSONDecoder):
-
     #
-    # It is an one pass scanner, lineno starts with 1
+    # It is a one pass scanner, lineno starts with 1
     #  to make it efficient, everytime it is called, it
     #  counts lineno from last scanned indx
     #
     lastindx = 0
     lineno = 1
 
     def countlines(self, string, endindx):
-        if (endindx >= len(string)):
+        if endindx >= len(string):
             return
         while self.lastindx <= endindx:
-            if (string[self.lastindx] == '\n'):
+            if string[self.lastindx] == '\n':
                 self.lineno += 1
             self.lastindx += 1
 
     def __init__(self, object_hook=None, parse_float=None, parse_int=None,
                  parse_constant=None, strict=True, object_pairs_hook=None):
 
         json.JSONDecoder.__init__(self, object_hook=object_hook,
@@ -85,8 +85,7 @@
                                   strict=strict,
                                   object_pairs_hook=object_pairs_hook)
 
         self.lastindx = 0
         self.lineno = 1
         # override scanner, it was called scan_once in JSONDecoder
         self.scan_once = make_my_scanner(self)
-        return
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,28 +17,26 @@
         Returns
         -------
         result: int
             Result desc
         """
         super().__init__()
 
-        #self.fix_template = \
+        # self.fix_template = \
         #    '[CVSPS107] [%s]: Security scope not in "securityDefinitions".'
-        #self.fix_template = {
+        # self.fix_template = {
         #        'ruleid': 'CVSPS100a',
         #        'description': 'Security scope not in "securityDefinitions".'
         #        }
 
         self.qspec = qspec
         self.openapi_ver = openapi_ver
         self.target_obj = target_obj
         self.attr_wt = attr_wt
 
-        return
-
     def __repr__(self):
         """
         Description
 
         Params
         ------
         p1 : float
@@ -69,36 +67,35 @@
         result: int
             Result desc
         """
         meta = []
 
         secdefn_node = '%s->securityDefinitions' % self.qspec.ROOT_NODE
         for security_node in self.qspec.get_security_objs():
-            for security_idx_node in self.qspec.G.neighbors(security_node):
-                for secschm_name_node in self.qspec.G.neighbors(security_idx_node):
-                    secschm_name = self.qspec.G.nodes[secschm_name_node]['nodenameraw']
-                    for scope_node_idx in self.qspec.G.neighbors(secschm_name_node):
-                        for scope_node in self.qspec.G.neighbors(scope_node_idx):
-                            scope_name = self.qspec.G.nodes[scope_node]['nodenameraw']
+            for security_idx_node in self.qspec.G.iterNeighbors(self.qspec.node_id_mapping[security_node]):
+                for secschm_name_node in self.qspec.G.iterNeighbors(security_idx_node):
+                    secschm_name = self.qspec.node_attributes['node_name_raw'][secschm_name_node]
+                    for scope_node_idx in self.qspec.G.iterNeighbors(secschm_name_node):
+                        for scope_node in self.qspec.G.iterNeighbors(scope_node_idx):
+                            scope_name = self.qspec.node_attributes['node_name_raw'][scope_node]
                             target_node = '%s->%s->scopes->%s' % \
-                                        (secdefn_node, secschm_name, scope_name)
+                                          (secdefn_node, secschm_name, scope_name)
 
-                            if not self.qspec.G.has_node(target_node):
-                                #v = self.fix_template.copy()
-                                #v['entity'] = scope_node
-                                #v['score'] = self.attr_wt
-                                #meta.append(v['entity'])
+                            if not self.qspec.G.hasNode(
+                                    self.qspec.node_id_mapping.get(target_node, self.qspec.total_node_plus_ten)):
+                                # v = self.fix_template.copy()
+                                # v['entity'] = scope_node
+                                # v['score'] = self.attr_wt
+                                # meta.append(v['entity'])
                                 meta.append(scope_node)
 
-        self.score = self.attr_wt*int(len(meta) > 0)
+        self.score = self.attr_wt * int(len(meta) > 0)
         if len(meta) > 0:
             self.meta = meta
 
-        return
-
     def compute_openapiv3(self):
         """
         Description
 
         Params
         ------
         p1 : float
@@ -112,45 +109,47 @@
             Result desc
         """
         meta = []
 
         all_scopes = set()
         # Collect all defined scopes
         secschms_node = '%s->components->securitySchemes' % self.qspec.ROOT_NODE
-        for secschm_node in self.qspec.G.neighbors(secschms_node):
-            type_oauth2_node = '%s->type->oauth2' % secschm_node
-            if not self.qspec.G.has_node(type_oauth2_node):
+        if secschms_node not in self.qspec.node_id_mapping:
+            return
+
+        for secschm_node in self.qspec.G.iterNeighbors(self.qspec.node_id_mapping[secschms_node]):
+            type_oauth2_node = '%s->type->oauth2' % self.qspec.node_attributes['node_name_sp'][secschm_node]
+            if not self.qspec.G.hasNode(
+                    self.qspec.node_id_mapping.get(type_oauth2_node, self.qspec.total_node_plus_ten)):
                 continue
 
-            oauth_flows_node = '%s->flows' % secschm_node
-            for oauth_flow_node in self.qspec.G.neighbors(oauth_flows_node):
-                scopes_node = '%s->scopes' % oauth_flow_node
-                for scope in self.qspec.G.neighbors(scopes_node):
-                    all_scopes.add(self.qspec.G.nodes[scope]['nodenameraw'])
+            oauth_flows_node = '%s->flows' % self.qspec.node_attributes['node_name_sp'][secschm_node]
+            for oauth_flow_node in self.qspec.G.iterNeighbors(self.qspec.node_id_mapping[oauth_flows_node]):
+                scopes_node = '%s->scopes' % self.qspec.node_attributes['node_name_sp'][oauth_flow_node]
+                for scope in self.qspec.G.iterNeighbors(self.qspec.node_id_mapping[scopes_node]):
+                    all_scopes.add(self.qspec.node_attributes['node_name_raw'][scope])
 
         for security_node in self.qspec.get_security_objs():
-            for security_idx_node in self.qspec.G.neighbors(security_node):
-                for secschm_name_node in self.qspec.G.neighbors(security_idx_node):
-                    for scope_node_idx in self.qspec.G.neighbors(secschm_name_node):
-                        for scope_node in self.qspec.G.neighbors(scope_node_idx):
+            for security_idx_node in self.qspec.G.iterNeighbors(self.qspec.node_id_mapping[security_node]):
+                for secschm_name_node in self.qspec.G.iterNeighbors(security_idx_node):
+                    for scope_node_idx in self.qspec.G.iterNeighbors(secschm_name_node):
+                        for scope_node in self.qspec.G.iterNeighbors(scope_node_idx):
 
-                            scope_name = self.qspec.G.nodes[scope_node]['nodenameraw']
+                            scope_name = self.qspec.node_attributes['node_name_raw'][scope_node]
 
                             if scope_name not in all_scopes:
-                                #v = self.fix_template.copy()
-                                #v['v_entity'] = scope_node
-                                #v['v_score'] = self.attr_wt
+                                # v = self.fix_template.copy()
+                                # v['v_entity'] = scope_node
+                                # v['v_score'] = self.attr_wt
                                 meta.append(scope_node)
 
-        self.score = self.attr_wt*int(len(meta) > 0)
+        self.score = self.attr_wt * int(len(meta) > 0)
         if len(meta) > 0:
             self.meta = meta
 
-        return
-
     @check_meta
     def compute(self):
         """
         Description
 
         Params
         ------
@@ -164,8 +163,7 @@
         result: int
             Result desc
         """
         if self.openapi_ver == 'v2':
             self.compute_openapiv2()
         else:
             self.compute_openapiv3()
-        return
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/python
 
 import re
 
-
 RISK_CTGS = {
-            'Security': 0,
-            'Data': 1,
-            'Format': 2
-            }
+    'Security': 0,
+    'Data': 1,
+    'Format': 2
+}
 RISK_SUBCTGS = {
-            'Security': {
-                        'Authentication': 0,
-                        'Authorization': 1,
-                        'Transport': 2
-                        },
-            'Data': {},
-            'Format': {}
-            }
+    'Security': {
+        'Authentication': 0,
+        'Authorization': 1,
+        'Transport': 2
+    },
+    'Data': {},
+    'Format': {}
+}
 SEVERITY_CTGS = {
-                'Critical': 0,
-                'High': 1,
-                'Medium': 2,
-                'Low': 3,
-                'NoRisk': 4
-                }
+    'Critical': 0,
+    'High': 1,
+    'Medium': 2,
+    'Low': 3,
+    'NoRisk': 4
+}
 
 
 def init_rules_ds(rule_exps):
-    #print(rule_exps)
+    # print(rule_exps)
     RISK_CTGS = {}
     RISK_SUBCTGS = {}
     for rule in rule_exps.values():
         ctg = rule['category']
         sub_ctg = rule['sub_category']
 
         # Categories
@@ -46,15 +45,14 @@
             idx = len(RISK_SUBCTGS[ctg])
             RISK_SUBCTGS[ctg][sub_ctg] = idx
 
     return RISK_CTGS, RISK_SUBCTGS
 
 
 def isvalid_url(url):
-
     if not (url.startswith('http://') or url.startswith('https://')):
         return False
 
     return True
 
 
 def get_severity(score):
@@ -82,17 +80,17 @@
     elif specrisk_code == 'S0':
         risk_ctg, risk_subctg = 'Security', 'Authentication'
     elif specrisk_code == 'S1':
         risk_ctg, risk_subctg = 'Security', 'Authorization'
     elif specrisk_code == 'S2':
         risk_ctg, risk_subctg = 'Security', 'Transport'
     else:
-        raise(ValueError('Invalid code'))
+        raise (ValueError('Invalid code'))
 
-    return (risk_ctg, risk_subctg)
+    return risk_ctg, risk_subctg
 
 
 def get_api(remed_clue):
     fields = remed_clue.split(' ')
     if fields[3] == 'paths':
         api = fields[5]
         return api
@@ -115,15 +113,18 @@
         api_param = fields[11]
         return api_param.strip(']:')
 
     return None
 
 
 def get_api2(remed_clue):
-    matches = re.findall('\((.*?)\)', remed_clue)
+    if isinstance(remed_clue, str):
+        matches = re.findall('\((.*?)\)', remed_clue)
+    else:
+        matches = re.findall('\((.*?)\)', remed_clue['reference_path'])
     # print(matches)
     for match in matches:
         identifier = match.split(' ')[0]
         if identifier.startswith('#->paths->'):
             api = identifier.split('->')[2]
             return api
 
@@ -151,22 +152,27 @@
         if identifier.startswith('#->paths->') and len(fields) > 5 and fields[4] == 'parameters':
             api_op = fields[5]
             return api_op
 
     return None
 
 
-def parse_cvlrange(linenum_mapping, target_node, ret_cvlrangeds=False):
+# gets line number for the voilation
+def parse_cvlrange(linenum_mapping, target_node, ret_cvlrangeds=False, abs_path=None):
 
     if linenum_mapping is None:
         return ''
 
+    yaml_flag = False
+    if abs_path is not None and abs_path.endswith('.yaml'):
+        yaml_flag = True
+    line_no = ''
     try:
         target_node = re.sub(r'__key__$', '', target_node)
-        cvlrange_ds = None      # cvlrange data structure
+        cvlrange_ds = None  # cvlrange data structure
         nodes = target_node.split('->')
         level = 0
 
         while level < len(nodes):
 
             node = nodes[level]
 
@@ -176,39 +182,54 @@
 
             if level == 0:
                 cvlrange_ds = linenum_mapping
                 level += 1
                 continue
 
             try:
-                if type(cvlrange_ds) == list:
-                    cvlrange_ds = cvlrange_ds[int(node)]
+                if yaml_flag:
+                    if type(cvlrange_ds) == list:
+                        cvlrange_ds, line_no = cvlrange_ds[int(node)], line_no
+                    else:
+                        cvlrange_ds, line_no = cvlrange_ds[node], cvlrange_ds[f'__line__{node}']
                 else:
-                    cvlrange_ds = cvlrange_ds[node]
+                    if type(cvlrange_ds) == list:
+                        cvlrange_ds = cvlrange_ds[int(node)]
+                    else:
+                        cvlrange_ds = cvlrange_ds[node]
             except KeyError:
                 if '$ref' in cvlrange_ds:
                     # The key error could be because the spec points to another
                     # ref
-                    ref_str = cvlrange_ds['$ref'][0].replace('/', '->')
-                    cvlrange_ds = parse_cvlrange(linenum_mapping, ref_str,
-                                                 ret_cvlrangeds=True)
+                    if yaml_flag:
+                        ref_str = cvlrange_ds['$ref'].replace('/', '->')
+                    else:
+                        ref_str = cvlrange_ds['$ref'][0].replace('/', '->')
+                    cvlrange_ds, line_no = parse_cvlrange(linenum_mapping, ref_str,
+                                                 ret_cvlrangeds=True, abs_path=abs_path)
                     continue
                 else:
                     # If node not present, pass so that the line num of
                     # parent gets returned
                     pass
 
             level += 1
 
         if ret_cvlrangeds:
-            return cvlrange_ds
+            return cvlrange_ds, line_no
 
-        if type(cvlrange_ds) == dict:
-            line_num = cvlrange_ds['cvlrange26uel7Ao'][0]
+        if yaml_flag:
+            try:
+                line_num = '[%d]' % cvlrange_ds[f'__line__{nodes[-1]}']
+            except:
+                line_num = line_no
         else:
-            line_num = cvlrange_ds[-1]['cvlrange26uel7Ao'][0]
+            if type(cvlrange_ds) == dict:
+                line_num = cvlrange_ds['cvlrange26uel7Ao'][0]
+            else:
+                line_num = cvlrange_ds[-1]['cvlrange26uel7Ao'][0]
 
         linenum_idstr = '[%d]' % line_num
     except:
         linenum_idstr = ''
 
     return linenum_idstr
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/python
 
 import json
+import sys
 
-from openapi_spec_validator import validate_v2_spec, validate_v3_spec
-from openapi_spec_validator.exceptions import OpenAPIValidationError
+from openapi_spec_validator import validate_spec
+from openapi_spec_validator import validate_spec, openapi_v2_spec_validator, \
+    openapi_v30_spec_validator
+from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 from prance import ResolvingParser
 from prance.util.formats import ParseError
 
 from cvsvc_apirisk.score.base import ScoreNode
 from cvsvc_apirisk.score.spec_security.sps_spec_util import QuerySpec
 from cvsvc_apirisk.score.spec_security.security_attrs.sps_sec_attr07 import SpecSecSecurityAttr07
 
@@ -43,36 +46,36 @@
         super().__init__()
 
         self.target_obj = target_obj
 
         # Check for spec validity first
         try:
             if openapi_ver == 'v2':
-                validate_v2_spec(self.target_obj['raw_spec'])
+                validate_spec(self.target_obj['raw_spec'], validator=openapi_v2_spec_validator)
             elif openapi_ver == 'v3':
-                validate_v3_spec(self.target_obj['raw_spec'])
+                validate_spec(self.target_obj['raw_spec'], validator=openapi_v30_spec_validator)
 
-            parse = ResolvingParser(target_filename, recursion_limit_handler=reclimit_handler)
+            parse = ResolvingParser(
+                url=target_filename,
+                recursion_limit_handler=reclimit_handler)
 
         except OpenAPIValidationError as e:
             print(str(e))
-            raise
+            sys.exit(1)
         except ParseError:
             # Try again because prance's __parse_json() gets messed up because
             # of six.text_type(). Provide it a string rather than dict
             parse = ResolvingParser(spec_string=json.dumps(self.target_obj['raw_spec']),
                                     content_type='application/json', recursion_limit_handler=reclimit_handler)
 
         self.target_obj['spec_obj'] = parse.specification
         self.qspec = QuerySpec(spec_obj=self.target_obj['spec_obj'])
 
         self.add_child(SpecSecSecurityAttr07(self.qspec, openapi_ver))
 
-        return
-
     def __repr__(self):
         """
         Description
 
         Params
         ------
         p1 : float
```

### Comparing `impsparc-2.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,24 @@
 # - also check that "parameters.*" should be same rather than only "parameters"
 
 
 import sys
 from argparse import ArgumentParser
 import json
 import re
-#import ipdb
-#import faulthandler
 
-from networkx.exception import NetworkXError
 from parsimonious.grammar import Grammar
 from parsimonious.nodes import NodeVisitor
 
 from cvsvc_apirisk.score.spec_security.sps_main import SpecSecMain
 from cvsvc_apirisk.score.spec_security.sps_common import get_severity, \
-                                            parse_cvlrange
-
+    parse_cvlrange
 
 BNF_GRAMMAR = \
-        """
+    """
         rule = (expr)+
         expr = identifier " " condition " " value conj
         identifier = ~r"[a-zA-Z0-9\.\/\#]+"
         condition = ~r"[a-z\-<>=!]+"
         value = ~r"[a-zA-Z0-9]+"
         conj = " AND " / " OR " / ""
         """
@@ -69,16 +65,14 @@
         """
         self.spec_main = SpecSecMain(target_obj=target_obj,
                                      target_filename=target_filename,
                                      openapi_ver=openapi_ver)
         self.num_evaluations = 0
         self.linenum_mapping = linenum_mapping
 
-        return
-
     def read_rules_raw(self, rules_path):
         """
         Description
 
         Params
         ------
         p1 : float
@@ -92,15 +86,15 @@
             Result desc
         """
         self.grammar = Grammar(BNF_GRAMMAR)
         rules = []
         with open(rules_path) as inf:
             for line in inf:
                 name, score, rule = line.strip().split(',')
-                print('-'*50)
+                print('-' * 50)
                 grammar_tree = self.grammar.parse(rule)
                 sr_visitor = SpecRuleVisitor()
                 rule = sr_visitor.visit(grammar_tree)
                 print(rule)
                 rules.append(rule)
 
         return rules
@@ -123,15 +117,15 @@
         """
         with open(rules_path) as inf:
             rules_dict = json.load(inf)
 
         rules = {}
         for rule_dict in rules_dict['rules']:
             rule_id = rule_dict['ruleid']
-            rule_flt = []   # Flattened rule exp
+            rule_flt = []  # Flattened rule exp
             for rule in rule_dict['rule']:
                 if type(rule) == dict:
                     rule_flt.append('%s %s %s' % (rule['identifier'],
                                                   rule['condition'],
                                                   rule['value']))
                 else:
                     # should be str
@@ -213,15 +207,15 @@
             Param description
 
         Returns
         -------
         result: int
             Result desc
         """
-        #ipdb.set_trace()
+        # ipdb.set_trace()
 
         # Keyword prefixes, if any, should be the same.
         all_keywords = set()
         self.determine_keywords_in_rule(rule, all_keywords)
 
         if len(all_keywords) > 1:
             print(all_keywords)
@@ -261,64 +255,65 @@
             Param description
 
         Returns
         -------
         result: int
             Result desc
         """
-        identifier = node   #.replace('->', '.')
-        #ipdb.set_trace()
+        identifier = node  # .replace('->', '.')
+        # ipdb.set_trace()
 
         if condition in {'<', '>', '<=', '>=', '==', '!='}:
             try:
                 if str(node).lower() in {'true', 'false'}:
                     id_value = node
                 else:
                     id_value = int(self.spec_main.qspec.get_node_value(node))
                     value = int(value)
-            except NetworkXError:
+            except Exception:
                 raise ValueError('[%s] Unknown identifier' % identifier)
 
             return '(%s %s %s)' % (id_value, condition, value)
 
         elif condition in {'eq', 'ne'}:
             t_cond = '==' if condition == 'eq' else '!='
             try:
                 id_value = self.spec_main.qspec.get_node_value(node)
-            except NetworkXError:
+            except Exception:
                 raise ValueError('[%s] Unknown identifier' % identifier)
 
             return '("%s" %s "%s")' % (id_value, t_cond, value)
 
         elif condition == 'pattern-match':
-            #ipdb.set_trace()
             try:
                 id_value = self.spec_main.qspec.get_node_value(node)
-            except NetworkXError:
+            except Exception:
                 raise ValueError('[%s] Unknown identifier' % identifier)
 
             return '(bool(re.search("%s", "%s")))' % (value, id_value)
 
         elif condition == 'is-missing':
-            has_node = not self.spec_main.qspec.G.has_node(node)
+            has_node = not self.spec_main.qspec.G.hasNode(self.spec_main.qspec.node_id_mapping.get(
+                node, self.spec_main.qspec.total_node_plus_ten))
 
             return '(%s == %s)' % (has_node, value)
 
         elif condition == 'is-empty':
-            #ipdb.set_trace()
+            # ipdb.set_trace()
             try:
-                num_nbrs = len(list(self.spec_main.qspec.G.neighbors(node)))
-            except NetworkXError:
+                num_nbrs = len([x for x in self.spec_main.qspec.G.iterNeighbors(
+                    self.spec_main.qspec.node_id_mapping[node])
+                                ]
+                               )
+            except Exception:
                 raise ValueError('[%s] Unknown identifier' % identifier)
             has_no_nbrs = (num_nbrs == 0)
 
             return '(%s == %s)' % (has_no_nbrs, value)
 
-        return
-
     def identifier2nodes(self, identifier, is_identifier_a_keyword,
                          is_identifier_nestedref, rule_dict):
         """
         Description
 
         Params
         ------
@@ -330,22 +325,22 @@
         Returns
         -------
         result: int
             Result desc
         """
 
         # When the identifier is a rule itself; return the boolean outcomes as
-        # nodes 
+        # nodes
         if is_identifier_nestedref:
             rule_id = identifier[len('__rule__'):]
             rule_dict = self.rules[rule_id]
             _, _, nested_pernode_outcome, nested_pernode_raw_rule = \
-                    self.analyze_rule(rule_dict, list_node_outcomes=True)
+                self.analyze_rule(rule_dict, list_node_outcomes=True)
             nodes = nested_pernode_outcome
-            return (nodes, nested_pernode_raw_rule)
+            return nodes, nested_pernode_raw_rule
 
         key_enabled = False
         if re.search('__key__$', identifier):
             key_enabled = True
             identifier = re.sub(r'__key__$', '', identifier)
 
         for idx, field in enumerate(identifier.split('->')):
@@ -359,17 +354,18 @@
 
             elif field == '*':
                 # NOTE: We raise the exception here for "*" but for other
                 # invalid nodes, we raise the exception in get_expr()
                 new_nodes = []
                 for node in nodes:
                     try:
-                        for nbr_node in self.spec_main.qspec.G.neighbors(node):
-                            new_nodes.append(nbr_node)
-                    except NetworkXError:
+                        for nbr_node in self.spec_main.qspec.G.iterNeighbors(
+                                self.spec_main.qspec.node_id_mapping[node]):
+                            new_nodes.append(self.spec_main.qspec.node_attributes['node_name_sp'][nbr_node])
+                    except Exception:
                         if is_identifier_a_keyword:
                             pass
                         else:
                             raise ValueError('[%s] Unknown identifier' % identifier)
 
                 nodes = new_nodes
 
@@ -407,15 +403,15 @@
                 meta = self.spec_main.children[identifier].meta
 
                 return True, (meta is not None), meta
 
         # In every other case, return False
         return False, None, None
 
-    def analyze_rule(self, rule_dict, list_node_outcomes=False):
+    def analyze_rule(self, rule_dict, list_node_outcomes=False, abs_path=None):
         """
         Description
 
         Params
         ------
         p1 : float
             Param description
@@ -425,15 +421,15 @@
         Returns
         -------
         result: int
             Result desc
         """
         rule = rule_dict['rule_flt']
 
-        #ipdb.set_trace()
+        # ipdb.set_trace()
         # Check if the rule is hard-coded
         ran_embdr, has_violation, violating_rules = self.check_embd_rule(rule)
         if ran_embdr:
             # Return False because the check_embd_rule() will add the
             # violation to meta
 
             return has_violation, violating_rules, None, None
@@ -446,24 +442,25 @@
 
         # TWO issues:
         # - the returned rule_nodes can be [] ; soln is assume false
         # - how to evaluate expr first before going to next
 
         # E.g. node_cache: [['#->security', '#->api'], None, ['#->parameters->0', '#->parameters->1']]
 
-        violating_rules = []        # List of all checks violating the rule
-        pernode_procd_rule = []     # per node processed rule. E.g. 200 < 400
-        pernode_raw_rule = []       # per node raw rule. E.g. response.200 < 400
-        evaled_part_rule = None     # Array; for this rule, holds the state of
-                                    # evaluations done for the concat exprs
-        num_node_iterations = 0     # Changes based on how many node does the
-                                    # expr resolve to
+        violating_rules = []  # List of all checks violating the rule
+        pernode_procd_rule = []  # per node processed rule. E.g. 200 < 400
+        pernode_raw_rule = []  # per node raw rule. E.g. response.200 < 400
+        evaled_part_rule = None  # Array; for this rule, holds the state of
+        # evaluations done for the concat exprs
+        num_node_iterations = 0  # Changes based on how many node does the
+        # expr resolve to
 
-        #faulthandler.enable()
+        # faulthandler.enable()
 
+        #import pdb;pdb.set_trace()
         for rule_idx, raw_expr in enumerate(rule):
 
             if raw_expr in RULE_OPS:
                 pernode_procd_rule.append(raw_expr)
                 pernode_raw_rule.append(raw_expr)
                 continue
 
@@ -473,18 +470,18 @@
 
             is_identifier_a_keyword = self.is_keyword(identifier)
 
             # Resolve the identifier to corresponding nodes;
             # "nested_pernode_raw_rule" gets populated if the identifier is a
             # rule.
             id_nodes, nested_pernode_raw_rule = \
-                    self.identifier2nodes(identifier, is_identifier_a_keyword,
-                                          is_identifier_nestedref, rule_dict)
+                self.identifier2nodes(identifier, is_identifier_a_keyword,
+                                      is_identifier_nestedref, rule_dict)
             if len(id_nodes) == 0:
-                #print('DEBUG: No nodes associated with identifier: %s' %
+                # print('DEBUG: No nodes associated with identifier: %s' %
                 #      identifier)
                 pass
 
             num_node_iterations = max(num_node_iterations, len(id_nodes))
 
             # Each element in either of these lists represents data for the
             # node encountered for this expression within the rule
@@ -499,19 +496,14 @@
                 try:
                     # IndexError possible when id_nodes is empty. In which case
                     # we assume the expression evaluated to False only in case
                     # of keyword-based identifiers
                     target_node = id_nodes[node_idx]
                     expr = self.get_expr(target_node, condition, value)
 
-                    '''
-                    if rule_dict['ruleid'] == 'CVSPS002':
-                        print(expr)
-                    '''
-
                     # evaled_expr used for operator precedence
                     evaled_expr = eval(expr)
                 except Exception as e:
                     if not is_identifier_a_keyword:
                         if type(e) == IndexError:
                             # Raise ValueError to maintain consistency with
                             # unidentified nodes in get_expr()
@@ -521,58 +513,75 @@
                             raise
                     # In case of keyword-based identifiers, silently ignore
                     # the missing nodes. This is unlike the absolute identifier
                     expr = str(False)
                     evaled_expr = False
 
                 procd_rule = expr
+                line_num, int_line_num = None, None
                 if is_identifier_nestedref:
                     raw_rule = '(%s %s %s)' % \
-                        (nested_pernode_raw_rule[node_idx], condition, value)
+                               (nested_pernode_raw_rule[node_idx], condition, value)
                 else:
-                    raw_rule = '(%s %s %s)%s' % \
-                        (target_node, condition, value,
-                                parse_cvlrange(self.linenum_mapping,
-                                                  target_node))
+                    line_num = parse_cvlrange(
+                        self.linenum_mapping,
+                        target_node,
+                        abs_path=abs_path)
+
+                    raw_rule = '(%s %s %s)%s' % (
+                        target_node, condition, value,
+                        line_num)
+
+                    if line_num not in {'', None}:
+                        int_line_num = json.loads(line_num)
+                        int_line_num = int_line_num[0]
 
                 # To support expressions such as "True or undefined-var", we
                 # need to evaluate every local expression
                 # NOTE: With the implementation below, we evaluate all
                 # operators from left to right and the operators AND/OR have
                 # the same precedence
                 if rule_idx == 0:
                     evaled_intm_expr = evaled_expr
                     intm_procd_rule = procd_rule
-                    intm_raw_rule = raw_rule
+                    intm_raw_rule = {'reference_path': raw_rule}
+                    if int_line_num is not None:
+                        intm_raw_rule['element_line_num'] = [int_line_num]
                 else:
                     # part rule column idx; 0 if the previous expression was an
                     # absolute identifier
                     part_rule_cidx = min(len(evaled_part_rule) - 1, itr_idx)
                     part_rule_bool = evaled_part_rule[part_rule_cidx]
+                    intm_raw_rule = pernode_raw_rule[part_rule_cidx]
 
                     # Get the intermediate expr using the previously evaluated
                     # sub-rule and the operator preceding this expression
                     intm_expr = '%s %s %s' % \
-                        (part_rule_bool, rule[rule_idx - 1], evaled_expr)
+                                (part_rule_bool, rule[rule_idx - 1], evaled_expr)
                     evaled_intm_expr = eval(intm_expr)
 
                     # Get the intermediate procd/raw rules
                     intm_procd_rule = '%s %s %s' % \
-                        (pernode_procd_rule[part_rule_cidx], rule[rule_idx - 1],
-                         procd_rule)
-                    intm_raw_rule = '%s %s %s' % \
-                        (pernode_raw_rule[part_rule_cidx], rule[rule_idx - 1],
-                         raw_rule)
+                                      (pernode_procd_rule[part_rule_cidx], rule[rule_idx - 1],
+                                       procd_rule)
+                    intm_raw_rule_path = '%s %s %s' % (
+                        pernode_raw_rule[part_rule_cidx]['reference_path'],
+                        rule[rule_idx - 1],
+                        raw_rule)
+
+                    intm_raw_rule['reference_path'] = intm_raw_rule_path
+                    if int_line_num is not None:
+                        intm_raw_rule['element_line_num'].append(int_line_num)
 
                 evaled_part_rule_stg.append(evaled_intm_expr)
                 pernode_procd_rule_stg.append(intm_procd_rule)
                 pernode_raw_rule_stg.append(intm_raw_rule)
 
                 if (evaled_intm_expr and ((rule_idx + 1 == len(rule)) or
-                        (rule[rule_idx + 1] == 'or'))):
+                                          (rule[rule_idx + 1] == 'or'))):
                     # Break out if there is just one rule or if the next
                     # operator is an "or". Because "True or ...." makes it
                     # True.
                     # Else, keep evaluating the next expression.
                     violating_rules.append(intm_raw_rule)
 
             evaled_part_rule = evaled_part_rule_stg
@@ -595,15 +604,15 @@
 
         self.num_evaluations += num_node_iterations
 
         # Evaluate the final expression
         if len(pernode_procd_rule) != 0:
             intm_outcome = False
             for i in range(0, len(pernode_procd_rule), 100):
-                expanded_rule = ' or '.join(pernode_procd_rule[i:i+100])
+                expanded_rule = ' or '.join(pernode_procd_rule[i:i + 100])
                 intm_outcome = eval('%s or %s' % (intm_outcome, expanded_rule))
             outcome = intm_outcome
         else:
             outcome = False
 
         nested_pernode_outcome, nested_pernode_raw_rule = [], []
         if list_node_outcomes:
@@ -617,15 +626,15 @@
             for vr in violating_rules:
                 print('\t%s' % vr)
         '''
 
         return (outcome, violating_rules,
                 nested_pernode_outcome, nested_pernode_raw_rule)
 
-    def analyze_rules(self, rules):
+    def analyze_rules(self, rules, abs_path=None):
         """
         Description
 
         Params
         ------
         p1 : float
             Param description
@@ -639,18 +648,19 @@
         """
         self.rules = rules
         self.spec_main.meta = []
 
         for _, rule_dict in self.rules.items():
             if not rule_dict.get('enabled', True):
                 continue
-            #print('-'*50)
-            #print('Analyzing rule: [%s] %s' % (rule_dict['ruleid'],
+            # print('-'*50)
+            # print('Analyzing rule: [%s] %s' % (rule_dict['ruleid'],
             #                                   rule_dict['rule_flt']))
-            has_violation, violating_rules, _, _ = self.analyze_rule(rule_dict)
+
+            has_violation, violating_rules, _, _ = self.analyze_rule(rule_dict, abs_path=abs_path)
 
             if has_violation:
                 for vr in violating_rules:
                     violation = {}
                     violation['v_ruleid'] = rule_dict['ruleid']
                     violation['v_description'] = rule_dict['description']
                     violation['v_score'] = rule_dict['score']
@@ -662,16 +672,14 @@
 
                     self.spec_main.meta.append(violation)
 
         # Set the max score
         self.spec_main.score = max([v['v_score'] for v in self.spec_main.meta],
                                    default=0)
 
-        return
-
 
 class SpecRuleVisitor(NodeVisitor):
 
     def __init__(self):
         """
         Description
```

### Comparing `impsparc-2.0.1/impsparc.egg-info/PKG-INFO` & `impsparc-2.0.2/impsparc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.1
+Version: 2.0.2
 Summary: API Specification Analysis for Risks and Compliance
-Home-page: UNKNOWN
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
-License: UNKNOWN
-Description: # ImpSpARC
-        API Specification Analysis for Risks and Compliance
-        
-        ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
-        
-        API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
-        
-        ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# ImpSpARC
+
+API Specification Analysis for Risks and Compliance
+
+ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
+
+API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
+
+ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
+
```

### Comparing `impsparc-2.0.1/impsparc.egg-info/SOURCES.txt` & `impsparc-2.0.2/impsparc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
 cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
 cvsvc_apirisk/score/spec_security/json_line.py
 cvsvc_apirisk/score/spec_security/sps_common.py
 cvsvc_apirisk/score/spec_security/sps_main.py
 cvsvc_apirisk/score/spec_security/sps_main_cr.py
 cvsvc_apirisk/score/spec_security/sps_spec_util.py
+cvsvc_apirisk/score/spec_security/yaml_line.py
 cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
 cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
```

### Comparing `impsparc-2.0.1/setup.py` & `impsparc-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "2.0.1"),
+    version=os.environ.get("VER", "2.0.2"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -21,19 +21,19 @@
     entry_points = {
         'console_scripts':
         ['impsparc=cvsvc_apirisk.score.spec_security.cv_apirisk_assessment:main',
          'impsparcserver=cvsvc_apirisk.score.spec_security.cv_apirisk_server:main']
     },
     install_requires = [
         "MarkupSafe==2.0.1",
-        "openapi-spec-validator==0.2.9",
+        "openapi-spec-validator==0.5.6",
         "openapi3==1.0.0",
-        "prance==0.21.8.0",
+        "prance==0.22.11.4.0",
         "numpy==1.22.3",
-        "networkx==2.4",
+        "networkit==10.1",
         "parsimonious==0.8.1",
         "sanic==20.3.0",
         "jinja2==3.0.3",
         "idna==2.10",
         "PyYAML==6.0",
     ],
     include_package_data=True,
```

