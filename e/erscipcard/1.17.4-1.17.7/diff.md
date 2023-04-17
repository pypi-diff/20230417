# Comparing `tmp/erscipcard-1.17.4.tar.gz` & `tmp/erscipcard-1.17.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.17.4.tar", last modified: Sun Apr 16 12:22:26 2023, max compression
+gzip compressed data, was "erscipcard-1.17.7.tar", last modified: Mon Apr 17 10:51:29 2023, max compression
```

## Comparing `erscipcard-1.17.4.tar` & `erscipcard-1.17.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.128060 erscipcard-1.17.4/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-16 12:22:18.000000 erscipcard-1.17.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-16 12:22:18.000000 erscipcard-1.17.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-16 12:22:26.129060 erscipcard-1.17.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2023-04-16 12:22:18.000000 erscipcard-1.17.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.118059 erscipcard-1.17.4/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      290 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.119059 erscipcard-1.17.4/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.121060 erscipcard-1.17.4/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    19616 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    14825 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.116059 erscipcard-1.17.4/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.122059 erscipcard-1.17.4/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.123060 erscipcard-1.17.4/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.124060 erscipcard-1.17.4/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.124060 erscipcard-1.17.4/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.128060 erscipcard-1.17.4/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/static/spinners.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.128060 erscipcard-1.17.4/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      296 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.128060 erscipcard-1.17.4/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    11686 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templates/erscipcard/ou.html
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templates/replace_re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.128060 erscipcard-1.17.4/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    10280 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-04-16 12:22:18.000000 erscipcard-1.17.4/erscipcard/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:22:26.119059 erscipcard-1.17.4/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-16 12:22:25.000000 erscipcard-1.17.4/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-16 12:22:25.000000 erscipcard-1.17.4/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:22:25.000000 erscipcard-1.17.4/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-16 12:22:25.000000 erscipcard-1.17.4/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 12:22:25.000000 erscipcard-1.17.4/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-16 12:22:26.129060 erscipcard-1.17.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-16 12:22:18.000000 erscipcard-1.17.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.096574 erscipcard-1.17.7/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 10:51:11.000000 erscipcard-1.17.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 10:51:11.000000 erscipcard-1.17.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-17 10:51:29.096574 erscipcard-1.17.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 10:51:11.000000 erscipcard-1.17.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.083573 erscipcard-1.17.7/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      313 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.084573 erscipcard-1.17.7/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.086573 erscipcard-1.17.7/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    19616 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    14825 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.080573 erscipcard-1.17.7/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.087574 erscipcard-1.17.7/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-04-17 10:51:11.000000 erscipcard-1.17.7/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.089574 erscipcard-1.17.7/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.090574 erscipcard-1.17.7/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.090574 erscipcard-1.17.7/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.095574 erscipcard-1.17.7/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/static/spinners.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.095574 erscipcard-1.17.7/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.095574 erscipcard-1.17.7/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12524 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templates/erscipcard/ou.html
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templates/replace_re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.096574 erscipcard-1.17.7/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-04-17 10:51:12.000000 erscipcard-1.17.7/erscipcard/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:51:29.084573 erscipcard-1.17.7/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-17 10:51:28.000000 erscipcard-1.17.7/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-04-17 10:51:28.000000 erscipcard-1.17.7/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:51:28.000000 erscipcard-1.17.7/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-17 10:51:28.000000 erscipcard-1.17.7/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 10:51:28.000000 erscipcard-1.17.7/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-17 10:51:29.099574 erscipcard-1.17.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-17 10:51:12.000000 erscipcard-1.17.7/setup.py
```

### Comparing `erscipcard-1.17.4/LICENSE` & `erscipcard-1.17.7/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/PKG-INFO` & `erscipcard-1.17.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.17.4
+Version: 1.17.7
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -26,29 +26,29 @@
 ```
 INSTALLED_APPS = [
 ...,
 'erscipcard',
 ]
 ```
 
-2.Add below line to STATICFILES_DIRS in your project setting.py file:
+2.(optional) (for show pic in edit personel box) Add below line to STATICFILES_DIRS in your project setting.py file:
 
 ```
 STATICFILES_DIRS = [
 ...,
 BASE_DIR / "images",
 ]
 ```
 
 3.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('erscipcard/', include('erscipcard.urls')),
 ```
 
-4.Run ``python manage.py makemigrations`` and ``python manage.py migrate``  to create the erscipcard models.
+4.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
 
 then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
 
 5.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
 
 first download card template , edit it and uplaod your custom template , then print cards.
```

### Comparing `erscipcard-1.17.4/README.md` & `erscipcard-1.17.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 ```
 INSTALLED_APPS = [
 ...,
 'erscipcard',
 ]
 ```
 
-2.Add below line to STATICFILES_DIRS in your project setting.py file:
+2.(optional) (for show pic in edit personel box) Add below line to STATICFILES_DIRS in your project setting.py file:
 
 ```
 STATICFILES_DIRS = [
 ...,
 BASE_DIR / "images",
 ]
 ```
 
 3.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('erscipcard/', include('erscipcard.urls')),
 ```
 
-4.Run ``python manage.py makemigrations`` and ``python manage.py migrate``  to create the erscipcard models.
+4.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
 
 then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
 
 5.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
 
 first download card template , edit it and uplaod your custom template , then print cards.
```

### Comparing `erscipcard-1.17.4/erscipcard/migrations/0001_initial.py` & `erscipcard-1.17.7/erscipcard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/models.py` & `erscipcard-1.17.7/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/1.docx` & `erscipcard-1.17.7/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/2.docx` & `erscipcard-1.17.7/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.17.7/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/BTITR.TTF` & `erscipcard-1.17.7/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/style.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/css/util.css` & `erscipcard-1.17.7/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.17.7/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.17.7/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.17.7/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.17.7/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.17.7/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.17.7/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.17.7/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.17.7/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.17.7/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.17.7/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.17.7/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/favicon.ico` & `erscipcard-1.17.7/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/logo.png` & `erscipcard-1.17.7/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/main.css` & `erscipcard-1.17.7/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/atebits.css` & `erscipcard-1.17.7/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/ball.css` & `erscipcard-1.17.7/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/circles.css` & `erscipcard-1.17.7/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/dots.css` & `erscipcard-1.17.7/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/echo.css` & `erscipcard-1.17.7/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/flower.css` & `erscipcard-1.17.7/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/gauge.css` & `erscipcard-1.17.7/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.17.7/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.17.7/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.17.7/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.17.7/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.17.7/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/plus.css` & `erscipcard-1.17.7/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/pong.css` & `erscipcard-1.17.7/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/pulse.css` & `erscipcard-1.17.7/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.17.7/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/spinner.css` & `erscipcard-1.17.7/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.17.7/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.17.7/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/throbber.css` & `erscipcard-1.17.7/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/timer.css` & `erscipcard-1.17.7/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/whirly.css` & `erscipcard-1.17.7/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.17.7/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/static/spinners.css` & `erscipcard-1.17.7/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.17.7/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.17.7/erscipcard/templates/erscipcard/ou.html`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 					    <li> <a class="dropdown-item " href="#" onclick="loadershow();window.open('https://colab.research.google.com/drive/19WCN9Di6q8sf2-WkSI7wtDIkB6JdF8Rl?usp=sharing','_self');"> ریموت Colab</a>	    </li>
 					  </ul>
 					</li>
 				</ul>
 				<ul class="navbar-nav me-auto ">
 					<li class="nav-item dropdown">
 					  <a class="nav-link dropdown-toggle" href="#" id="navbarScrollingDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
-						کاربر  <i class="fa fa-user"></i>
+						{{request.user.last_name}} <i class="fa fa-user"></i>
 						</a>
 						<ul class="dropdown-menu" aria-labelledby="navbarScrollingDropdown2">
 						<li><a class="dropdown-item" href="#" onclick="loadershow();window.open('/erscipcard/changepass','_self');" > تغییر رمز عبور  </a></li>
 						<li><hr class="dropdown-divider"></li>
 						<li><a href="/erscipcard/logout" class="dropdown-item " > خروج  </a></li>
 					  </ul>
 					</li>
@@ -136,15 +136,15 @@
 						</tr>
 						{% for i in userlist %}
 						<tr>
 						<td>{{i.name}}</td>
 						<td>{{i.personeli}}</td>
 						<td>{{i.number}}</td>
 						<td>{{i.etebar}}</td>
-						<td><a href="/static/{{i.pic.name | basepath }}"><i class="fa fa-picture-o" aria-hidden="true"></i></a></td>
+						<td><a href="#" onclick="showpic({{i.id}});" ><i class="fa fa-picture-o" aria-hidden="true"></i></a></td>
 						<td><a class="btn btn-primary" href="#" onclick="loadershow();window.open('/erscipcard/edituser?id={{i.id}}','_self');">ویرایش</a></td>
 						<td><a class="btn btn-danger" href="#" onclick="loadershow();window.open('/erscipcard/deluser?id={{i.id}}','_self');">پاک شود</a></td>
 						</tr>
 						{% endfor %}
 					</table>
 				</div>
 					
@@ -207,14 +207,24 @@
     </div>
     <!-- Modal 2  {backdrop:'static', keyboard: false , show: true } -->
     <div class="modal bottom fade" tabindex="-1"  id="loader" data-backdrop="static" data-keyboard="false">
         <div class="modal-dialog modal-frame modal-bottom text-center">
             <span class="ball-loader"></span>
         </div>
     </div>
+	<!-- Modal 3 -->
+    <div class="modal modal-dialog-scrollable  bottom fade" id="canvasshowpic" tabindex="-1" data-backdrop="static" data-keyboard="false">
+      <div class="modal-dialog modal-frame modal-bottom ">
+        <div class="modal-content">
+          <div class="modal-body">
+			<img id="showpicimg" width="150px" src="" />
+		  </div>
+        </div>
+      </div>
+    </div>
 	{% endif %}
 
     <!--Bootstrap core JavaScript -->
 	<script src="{% static 'bt/js/jquery.min.js' %}"></script>
     <script src="{% static 'bt/js/bootstrap.bundle.min.js' %}"></script>
 	{{ form.media }}
       
@@ -223,16 +233,31 @@
     document.querySelectorAll('form').forEach(form => form.addEventListener('submit', loadershow));
     window.addEventListener("unload", loaderhide);
     document.addEventListener("DOMContentLoaded", loaderhide);
     function loadershow () {
         $('#loader').modal('show');
     }
     function loaderhide () {
-        $('#loader').modal('hide');    }
-	
+        $('#loader').modal('hide');    
+	}		
+	function showpic(picid){
+		let request = new XMLHttpRequest();
+		let method = 'GET';
+		//let query = document.getElementById("searchText").value;
+		let url = '/erscipcard/showpic/' + picid;
+		request.open(method, url);
+		request.onload = function () {
+			let html = request.response;
+			document.getElementById("showpicimg").src = html;
+			//window.open(html,'_self');
+			$("#canvasshowpic").modal('show'); 
+		};
+		request.send();			
+	}
+
 	function sortTable(z) {
 	  var table, rows, switching, i, x, y, shouldSwitch;
 	  table = document.getElementById("userTable");
 	  switching = true;
 	  /*Make a loop that will continue until
 	  no switching has been done:*/
 	  while (switching) {
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
           o ===================================================================
           o دانلود_فایل_نمونه_پرینت_کارت
           o دانلود_فایل_نمونه_کاربران
           o آپلود_فایل_نمونه
           o ===================================================================
           o دانلود_از_یوتیوب
           o ریموت_Colab
-    * کاربر
+    * {{request.user.last_name}}
           o تغییر_رمز_عبور
           o ===================================================================
           o خروج
 {% endif %}
 
 {% if request.user.is_authenticated %} {% if var1 == 1 %}
 {{ memo }}
@@ -57,9 +57,10 @@
  {% if request.user.is_authenticated %}
 ** چاپ یک یا چند کارت **
 {% csrf_token %}
 [Unknown INPUT type]
 [Unknown INPUT type]
 o فایل Word o فایل Pdf
 [ارسال] بستن
+[Image]
 {% endif %}
  {{ form.media }}
```

### Comparing `erscipcard-1.17.4/erscipcard/urls.py` & `erscipcard-1.17.7/erscipcard/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,10 +39,10 @@
 	path('userlist/', views.userlist),
 	path('edituser/', views.edituser),
 	path('deluser/', views.deluser),
 	path('signin/', views.signin),
 	path('logout/', views.logout_form),
 	path('uploadtpl/', views.uploadtpl),
 	path('printalluser/', views.printalluser),
-        
+        path('showpic/<int:picid>/', views.showpic , name = 'showpic'),        
 ]
```

### Comparing `erscipcard-1.17.4/erscipcard/views.py` & `erscipcard-1.17.7/erscipcard/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.http import HttpResponse,FileResponse,JsonResponse,Http404
 from django.db.models import Avg, Count, Min, Sum
 from django.conf import settings
 from django.contrib.auth.forms import PasswordChangeForm
 from django.contrib.auth import update_session_auth_hash
 from django.views.decorators.csrf import csrf_exempt
 from django.core import serializers
-import os,random,json
+import os,random,json,base64
 from .forms import User1form
 from .models import User1
 from docxtpl import DocxTemplate
 from docxtpl import InlineImage
 import platform
 from docx.shared import Mm
 from pathlib import Path
@@ -213,14 +213,28 @@
 		if request.method == 'GET':
 			idx = request.GET['id']
 			User1.objects.get(id = idx).delete()
 	except:
 		pass
 	return redirect("/erscipcard/userlist")
 ####################################################################
+def showpic(request,picid):
+	if not request.user.is_authenticated:
+		return render (request,'erscipcard/login.html' )
+	try:
+                picdata=User1.objects.get(id = picid)
+                img=open(picdata.pic.path, "rb")
+                image_data = base64.b64encode(img.read()).decode('utf-8')
+                imgdata = "data:image/png;base64,{}".format(image_data)
+                return HttpResponse(imgdata)
+
+	except:
+		pass
+	return redirect("/erscipcard/userlist")
+####################################################################
 def uploadtpl(request):
 	if not request.user.is_authenticated:
 		return render (request,'erscipcard/login.html')
 	try:
 		if request.method == 'POST':
 			f=request.FILES['file']
 			f2=request.FILES['file2']
```

### Comparing `erscipcard-1.17.4/erscipcard/widget.py` & `erscipcard-1.17.7/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.17.7/erscipcard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.17.4
+Version: 1.17.7
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -26,29 +26,29 @@
 ```
 INSTALLED_APPS = [
 ...,
 'erscipcard',
 ]
 ```
 
-2.Add below line to STATICFILES_DIRS in your project setting.py file:
+2.(optional) (for show pic in edit personel box) Add below line to STATICFILES_DIRS in your project setting.py file:
 
 ```
 STATICFILES_DIRS = [
 ...,
 BASE_DIR / "images",
 ]
 ```
 
 3.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('erscipcard/', include('erscipcard.urls')),
 ```
 
-4.Run ``python manage.py makemigrations`` and ``python manage.py migrate``  to create the erscipcard models.
+4.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
 
 then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
 
 5.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
 
 first download card template , edit it and uplaod your custom template , then print cards.
```

### Comparing `erscipcard-1.17.4/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.17.7/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.4/setup.cfg` & `erscipcard-1.17.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.17.4
+version = 1.17.7
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

