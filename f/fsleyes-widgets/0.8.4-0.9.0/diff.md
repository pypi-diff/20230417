# Comparing `tmp/fsleyes-widgets-0.8.4.tar.gz` & `tmp/fsleyes-widgets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fsleyes-widgets-0.8.4.tar", last modified: Wed Oct  9 11:32:32 2019, max compression
+gzip compressed data, was "dist/fsleyes-widgets-0.9.0.tar", last modified: Thu Jun  4 22:25:08 2020, max compression
```

## Comparing `fsleyes-widgets-0.8.4.tar` & `fsleyes-widgets-0.9.0.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2327 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       56 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/requirements-dev.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     3729 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       16 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    28888 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      244 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2441 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_colourbutton.py
--rw-rw-rw-   0 root         (0) root         (0)     8078 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_layout.py
--rw-rw-rw-   0 root         (0) root         (0)    11418 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_colourbarbitmap.py
--rw-rw-rw-   0 root         (0) root         (0)     9246 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_runwindow.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_importall.py
--rw-rw-rw-   0 root         (0) root         (0)     6327 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_webpage.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_textbitmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_typedict.py
--rw-rw-rw-   0 root         (0) root         (0)     7814 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_floatspin.py
--rw-rw-rw-   0 root         (0) root         (0)     4882 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_autotextctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_bitmaptoggle.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_elistbox.py
--rw-rw-rw-   0 root         (0) root         (0)    10179 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_floatslider.py
--rw-rw-rw-   0 root         (0) root         (0)     2294 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_togglepanel.py
--rw-rw-rw-   0 root         (0) root         (0)    10660 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_rangeslider.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2019-10-09 11:13:13.000000 fsleyes-widgets-0.8.4/tests/test_status.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_textpanel.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_imagepanel.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_overlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2794 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_numberdialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7315 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_widgetgrid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/tests/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/tests/testdata/bitmapbuttons/
--rw-rw-rw-   0 root         (0) root         (0)     1289 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/bitmapbuttons/false.png
--rw-rw-rw-   0 root         (0) root         (0)     3608 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/bitmapbuttons/true.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/
--rw-rw-rw-   0 root         (0) root         (0)      478 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      684 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      616 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      465 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      856 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      320 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      852 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      868 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      420 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      358 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      381 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      587 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      312 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      388 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      432 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      564 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      574 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)     1261 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      366 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      470 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      909 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      366 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      858 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)     1237 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      907 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      480 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      465 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      370 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      313 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      378 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      359 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      586 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      461 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      778 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      477 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      534 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      447 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      381 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      525 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      461 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      428 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      421 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      587 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      328 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1009 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      437 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      439 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      853 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      466 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      573 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      507 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      653 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      768 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      366 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_1_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      617 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      353 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      489 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      461 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      482 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      867 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      417 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      426 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      909 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      620 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      618 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      395 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      471 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      575 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      321 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      528 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      327 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_1_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      367 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      463 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      323 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      313 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_1_1_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      549 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)      447 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_1_0_0_1_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      385 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_10_0_0_0_0_0_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      318 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_0_0_0_0_1_0_0_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      316 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_6_1_0_0_1_0_0_0_1_0.5.png
--rw-rw-rw-   0 root         (0) root         (0)     1037 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      928 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_0.5.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/
--rw-rw-rw-   0 root         (0) root         (0)      338 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      652 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)     2035 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2079 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      379 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1590 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      687 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_horizontal.png
--rw-rw-rw-   0 root         (0) root         (0)     2141 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      521 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2076 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      398 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     1935 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2035 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      331 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)      320 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     1527 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2195 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_rrrrr.png
--rw-rw-rw-   0 root         (0) root         (0)      374 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     3186 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_rrrrr.png
--rw-rw-rw-   0 root         (0) root         (0)     2197 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_rrrrr.png
--rw-rw-rw-   0 root         (0) root         (0)      394 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     1536 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      356 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      352 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     4361 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_16.png
--rw-rw-rw-   0 root         (0) root         (0)      345 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      309 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2103 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1527 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     3945 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     4724 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     4216 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_horizontal_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)      330 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)      700 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)     2612 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     3411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1935 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3408 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      361 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1938 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3032 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_10.png
--rw-rw-rw-   0 root         (0) root         (0)     2262 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      557 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)      451 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_False_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     6064 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_vertical_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)     2124 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1597 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1938 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      261 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      479 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_True_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     2184 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lllll.png
--rw-rw-rw-   0 root         (0) root         (0)      604 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)     2206 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_ccccc.png
--rw-rw-rw-   0 root         (0) root         (0)     1956 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3879 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1406 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1167 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_vertical_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)      434 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2052 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      264 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     6755 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.25_0.5_0.75_1.png
--rw-rw-rw-   0 root         (0) root         (0)      544 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2593 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1530 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      334 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2357 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2946 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      500 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)     1407 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1683 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2515 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1533 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2315 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_10.png
--rw-rw-rw-   0 root         (0) root         (0)     2240 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      333 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     5368 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.5_1.png
--rw-rw-rw-   0 root         (0) root         (0)      966 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_horizontal_top.png
--rw-rw-rw-   0 root         (0) root         (0)     2515 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2656 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      326 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2263 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2686 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_6.png
--rw-rw-rw-   0 root         (0) root         (0)     2069 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_horizontal_top.png
--rw-rw-rw-   0 root         (0) root         (0)      325 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3898 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     6563 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_horizontal_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)     3058 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_ccccc.png
--rw-rw-rw-   0 root         (0) root         (0)      301 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      412 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_False_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2245 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      430 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     3945 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2040 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      341 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3879 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1881 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      285 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      422 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      501 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)      539 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     6189 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_vertical_top.png
--rw-rw-rw-   0 root         (0) root         (0)     3222 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_16.png
--rw-rw-rw-   0 root         (0) root         (0)     2141 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     3220 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_16.png
--rw-rw-rw-   0 root         (0) root         (0)      556 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)     1667 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     9469 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_vertical_top.png
--rw-rw-rw-   0 root         (0) root         (0)      419 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2910 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_lllll.png
--rw-rw-rw-   0 root         (0) root         (0)      437 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     6563 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_horizontal_top.png
--rw-rw-rw-   0 root         (0) root         (0)     2870 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2084 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     3370 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2217 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lcccr.png
--rw-rw-rw-   0 root         (0) root         (0)     1595 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1791 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2650 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_vertical_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)     2696 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_vertical_top.png
--rw-rw-rw-   0 root         (0) root         (0)     2040 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1674 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2540 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      809 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_vertical.png
--rw-rw-rw-   0 root         (0) root         (0)     1881 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2347 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      458 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      357 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2245 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1409 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     4222 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_horizontal_top.png
--rw-rw-rw-   0 root         (0) root         (0)     3919 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2263 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1956 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2103 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1530 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      661 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_vertical.png
--rw-rw-rw-   0 root         (0) root         (0)     2540 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      516 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2041 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2079 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2946 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2052 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2161 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      341 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2656 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1406 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2990 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_ccccc.png
--rw-rw-rw-   0 root         (0) root         (0)     1951 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2218 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lcccr.png
--rw-rw-rw-   0 root         (0) root         (0)      265 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      337 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1801 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      645 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     1791 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      648 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2084 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2041 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      533 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     2357 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1533 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      947 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_horizontal_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)     2161 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      320 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      687 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)      407 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_True_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     1886 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1858 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2205 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_ccccc.png
--rw-rw-rw-   0 root         (0) root         (0)      276 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      531 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     2526 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1675 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      397 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2909 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2070 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_horizontal_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)      529 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     2526 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1536 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2124 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2549 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      515 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_10.png
--rw-rw-rw-   0 root         (0) root         (0)     1595 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      351 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     1801 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2309 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_10.png
--rw-rw-rw-   0 root         (0) root         (0)      269 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      512 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     3411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1864 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     3370 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     2076 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      700 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_horizontal.png
--rw-rw-rw-   0 root         (0) root         (0)      407 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)      354 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      343 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2914 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      528 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_horizontal.png
--rw-rw-rw-   0 root         (0) root         (0)     3182 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_lcccr.png
--rw-rw-rw-   0 root         (0) root         (0)     2643 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     4236 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_16.png
--rw-rw-rw-   0 root         (0) root         (0)     2621 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3919 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1667 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2840 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lllll.png
--rw-rw-rw-   0 root         (0) root         (0)     2240 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      575 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      725 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)     2347 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1674 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     9346 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_vertical_bottom.png
--rw-rw-rw-   0 root         (0) root         (0)      556 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_Greys.png
--rw-rw-rw-   0 root         (0) root         (0)     2909 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1606 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2080 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2677 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2606 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2593 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_6.png
--rw-rw-rw-   0 root         (0) root         (0)      260 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1951 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      398 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2914 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      528 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)      614 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)     1597 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1816 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3108 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lcccr.png
--rw-rw-rw-   0 root         (0) root         (0)     1825 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1683 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2643 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      285 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2080 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1407 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1838 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_6.png
--rw-rw-rw-   0 root         (0) root         (0)     1411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2612 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     1832 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_6.png
--rw-rw-rw-   0 root         (0) root         (0)     1675 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2870 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2593 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     6202 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.49_0.51_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3408 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1606 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_10_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2621 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_16_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1816 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_6_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      728 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)      867 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_vertical.png
--rw-rw-rw-   0 root         (0) root         (0)      544 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_horizontal.png
--rw-rw-rw-   0 root         (0) root         (0)     1148 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_vertical_top.png
--rw-rw-rw-   0 root         (0) root         (0)      269 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1590 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     1864 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1825 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2606 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2184 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lllll.png
--rw-rw-rw-   0 root         (0) root         (0)      335 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3455 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1886 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      664 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_vertical.png
--rw-rw-rw-   0 root         (0) root         (0)     3898 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     2380 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)     3092 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_rrrrr.png
--rw-rw-rw-   0 root         (0) root         (0)     2380 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png
--rw-rw-rw-   0 root         (0) root         (0)      405 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     3455 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      318 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_0_0_0_0.png
--rw-rw-rw-   0 root         (0) root         (0)     2677 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_16_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)      645 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_Blues.png
--rw-rw-rw-   0 root         (0) root         (0)      356 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_1_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2549 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      523 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_None.png
--rw-rw-rw-   0 root         (0) root         (0)     2262 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)     1858 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.25_0.75.png
--rw-rw-rw-   0 root         (0) root         (0)      411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_None.png
--rw-rw-rw-   0 root         (0) root         (0)     1409 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_6_0_0_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)     2736 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_bitmapradio.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_progress.py
--rw-rw-rw-   0 root         (0) root         (0)    11967 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_texttag.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/tests/test_placeholder_textctrl.py
--rw-rw-rw-   0 root         (0) root         (0)     3249 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/doc/
--rw-rw-rw-   0 root         (0) root         (0)    11165 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.bitmaptoggle.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/doc/images/
--rw-rw-rw-   0 root         (0) root         (0)    39219 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/widgetgrid.png
--rw-rw-rw-   0 root         (0) root         (0)     6684 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/bitmapradiobox.png
--rw-rw-rw-   0 root         (0) root         (0)     4152 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/colourbarbitmap.png
--rw-rw-rw-   0 root         (0) root         (0)    10674 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/simplemessagedialog.png
--rw-rw-rw-   0 root         (0) root         (0)    48181 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/fsldirdialog.png
--rw-rw-rw-   0 root         (0) root         (0)   104782 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/widgetlist.png
--rw-rw-rw-   0 root         (0) root         (0)   220800 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/texteditdialog.png
--rw-rw-rw-   0 root         (0) root         (0)    14080 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/texttagpanel.png
--rw-rw-rw-   0 root         (0) root         (0)    13017 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/images/rangesliderspinpanel.png
--rw-rw-rw-   0 root         (0) root         (0)      193 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.placeholder_textctrl.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.numberdialog.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.imagepanel.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.progress.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.floatslider.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.bitmapradio.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.layout.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.elistbox.rst
--rw-rw-rw-   0 root         (0) root         (0)      518 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      178 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.runwindow.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.webpage.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.typedict.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.rangeslider.rst
--rw-rw-rw-   0 root         (0) root         (0)      196 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.colourbarbitmap.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.floatspin.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.textpanel.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.autotextctrl.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/mock_classes.txt
--rw-rw-rw-   0 root         (0) root         (0)      172 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.overlay.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.widgetgrid.rst
--rw-rw-rw-   0 root         (0) root         (0)      103 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.status.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.colourbutton.rst
--rw-rw-rw-   0 root         (0) root         (0)      706 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.textbitmap.rst
--rw-rw-rw-   0 root         (0) root         (0)      151 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.dialog.rst
--rw-rw-rw-   0 root         (0) root         (0)       92 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/mock_modules.txt
--rw-rw-rw-   0 root         (0) root         (0)      154 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.texttag.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.notebook.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.togglepanel.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.b64icon.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/doc/fsleyes_widgets.widgetlist.rst
--rw-rw-rw-   0 root         (0) root         (0)       53 2019-10-09 11:13:13.000000 fsleyes-widgets-0.8.4/COPYRIGHT
--rw-rw-rw-   0 root         (0) root         (0)      239 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3729 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/
--rw-rw-rw-   0 root         (0) root         (0)     5038 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/bitmapradio.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2019-10-09 11:23:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/textpanel.py
--rw-rw-rw-   0 root         (0) root         (0)     5804 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/numberdialog.py
--rw-rw-rw-   0 root         (0) root         (0)    19981 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/floatslider.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/placeholder_textctrl.py
--rw-rw-rw-   0 root         (0) root         (0)    19483 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/widgetlist.py
--rw-rw-rw-   0 root         (0) root         (0)    17299 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/floatspin.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/colourbutton.py
--rw-rw-rw-   0 root         (0) root         (0)    14187 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)    30062 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7270 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/togglepanel.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/bitmaptoggle.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/imagepanel.py
--rw-rw-rw-   0 root         (0) root         (0)    21631 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/texttag.py
--rw-rw-rw-   0 root         (0) root         (0)    26916 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/rangeslider.py
--rw-rw-rw-   0 root         (0) root         (0)    49617 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/elistbox.py
--rw-rw-rw-   0 root         (0) root         (0)    50430 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/widgetgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    20153 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/autotextctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-09 11:32:32.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7459 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/progress.py
--rw-rw-rw-   0 root         (0) root         (0)    17742 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/layout.py
--rw-rw-rw-   0 root         (0) root         (0)     8400 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/colourbarbitmap.py
--rw-rw-rw-   0 root         (0) root         (0)     7565 2019-10-09 11:13:13.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/status.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/webpage.py
--rw-rw-rw-   0 root         (0) root         (0)    10665 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/typedict.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/overlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/textbitmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8857 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/runwindow.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2019-10-04 13:33:24.000000 fsleyes-widgets-0.8.4/fsleyes_widgets/utils/b64icon.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2019-10-09 11:13:13.000000 fsleyes-widgets-0.8.4/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       44 2020-06-04 22:25:07.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2020-06-04 22:25:07.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-06-04 22:25:07.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     3729 2020-06-04 22:25:07.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28888 2020-06-04 22:25:07.000000 fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      244 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.textpanel.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.notebook.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.numberdialog.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.bitmaptoggle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      518 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      193 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.placeholder_textctrl.rst
+-rw-rw-rw-   0 root         (0) root         (0)      160 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.floatspin.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.webpage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.progress.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.floatslider.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.status.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.widgetlist.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.imagepanel.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.colourbutton.rst
+-rw-rw-rw-   0 root         (0) root         (0)      196 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.colourbarbitmap.rst
+-rw-rw-rw-   0 root         (0) root         (0)       92 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/mock_modules.txt
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.b64icon.rst
+-rw-rw-rw-   0 root         (0) root         (0)      151 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.dialog.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.textbitmap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.widgetgrid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.texttag.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.autotextctrl.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.bitmapradio.rst
+-rw-rw-rw-   0 root         (0) root         (0)      103 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/mock_classes.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.elistbox.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)     4152 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/colourbarbitmap.png
+-rw-rw-rw-   0 root         (0) root         (0)   104782 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/widgetlist.png
+-rw-rw-rw-   0 root         (0) root         (0)    39219 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/widgetgrid.png
+-rw-rw-rw-   0 root         (0) root         (0)    10674 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/simplemessagedialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    48181 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/fsldirdialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    13017 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/rangesliderspinpanel.png
+-rw-rw-rw-   0 root         (0) root         (0)   220800 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/texteditdialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/bitmapradiobox.png
+-rw-rw-rw-   0 root         (0) root         (0)    14080 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/images/texttagpanel.png
+-rw-rw-rw-   0 root         (0) root         (0)      172 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.overlay.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.rangeslider.rst
+-rw-rw-rw-   0 root         (0) root         (0)      178 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.runwindow.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.typedict.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.togglepanel.rst
+-rw-rw-rw-   0 root         (0) root         (0)      706 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/doc/fsleyes_widgets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      608 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3729 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/textpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    49617 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/elistbox.py
+-rw-rw-rw-   0 root         (0) root         (0)    26916 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/rangeslider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/bitmaptoggle.py
+-rw-rw-rw-   0 root         (0) root         (0)    14187 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/
+-rw-rw-rw-   0 root         (0) root         (0)    17742 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/layout.py
+-rw-rw-rw-   0 root         (0) root         (0)     8857 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/runwindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     7459 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     7565 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/overlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10665 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/typedict.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/textbitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/b64icon.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/webpage.py
+-rw-rw-rw-   0 root         (0) root         (0)     8400 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/utils/colourbarbitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2020-06-04 20:50:14.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20047 2020-06-04 19:50:19.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/floatslider.py
+-rw-rw-rw-   0 root         (0) root         (0)    50430 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/widgetgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/bitmapradio.py
+-rw-rw-rw-   0 root         (0) root         (0)    19483 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/widgetlist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5804 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/numberdialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2020-06-04 19:50:19.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/floatspin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/imagepanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    30062 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7270 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/togglepanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    21631 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/texttag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/placeholder_textctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/colourbutton.py
+-rw-rw-rw-   0 root         (0) root         (0)    20889 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/fsleyes_widgets/autotextctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_bitmaptoggle.py
+-rw-rw-rw-   0 root         (0) root         (0)    11418 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_colourbarbitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_importall.py
+-rw-rw-rw-   0 root         (0) root         (0)     7814 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_floatspin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_runwindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8078 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_imagepanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)    11967 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_texttag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_elistbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     7315 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_widgetgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     9246 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_textpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_colourbutton.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    10238 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_floatslider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10698 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_rangeslider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_togglepanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_typedict.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_bitmapradio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/tests/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/tests/testdata/bitmapbuttons/
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/bitmapbuttons/false.png
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/bitmapbuttons/true.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/
+-rw-rw-rw-   0 root         (0) root         (0)      398 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_rrrrr.png
+-rw-rw-rw-   0 root         (0) root         (0)      544 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      533 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2245 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_horizontal_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_vertical_top.png
+-rw-rw-rw-   0 root         (0) root         (0)      285 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      341 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)      867 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_vertical.png
+-rw-rw-rw-   0 root         (0) root         (0)      528 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      337 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      330 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lcccr.png
+-rw-rw-rw-   0 root         (0) root         (0)      556 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      412 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_False_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      645 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)      575 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      419 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      479 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_True_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      652 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1667 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3092 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_rrrrr.png
+-rw-rw-rw-   0 root         (0) root         (0)      398 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      458 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_lllll.png
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      379 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     6563 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_horizontal_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)      269 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_ccccc.png
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_6.png
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      947 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_horizontal_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)     3182 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_lcccr.png
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     4724 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1667 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      320 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)      557 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     5368 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.5_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      352 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      343 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_10.png
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_horizontal_top.png
+-rw-rw-rw-   0 root         (0) root         (0)      966 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_horizontal_top.png
+-rw-rw-rw-   0 root         (0) root         (0)      331 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_16.png
+-rw-rw-rw-   0 root         (0) root         (0)      397 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     2161 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      687 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_horizontal.png
+-rw-rw-rw-   0 root         (0) root         (0)      407 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_True_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      374 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      528 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_horizontal.png
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      521 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      531 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)      529 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)      430 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2643 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      512 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_10.png
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      523 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      516 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      326 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)      354 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      265 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_ccccc.png
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_6.png
+-rw-rw-rw-   0 root         (0) root         (0)     9346 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_vertical_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)     2621 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      451 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_False_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_rrrrr.png
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      664 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_vertical.png
+-rw-rw-rw-   0 root         (0) root         (0)      361 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      335 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_vertical_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2621 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      515 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      318 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      309 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      261 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_16.png
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lllll.png
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lllll.png
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      556 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      405 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_vertical_top.png
+-rw-rw-rw-   0 root         (0) root         (0)     6563 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_horizontal_top.png
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2643 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      285 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      422 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      276 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.25_0.5_0.75_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     4222 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_horizontal_top.png
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      356 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3919 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2240 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      260 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lcccr.png
+-rw-rw-rw-   0 root         (0) root         (0)      434 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      356 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3945 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      325 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      357 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)      687 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2240 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_10_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     6202 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.49_0.51_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      700 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      301 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_vertical_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_horizontal_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)      728 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lllll.png
+-rw-rw-rw-   0 root         (0) root         (0)      614 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_6.png
+-rw-rw-rw-   0 root         (0) root         (0)      407 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      500 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)      320 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     6189 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_vertical_top.png
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      394 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     3945 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      333 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      345 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      809 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_vertical.png
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_vertical_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)      341 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_horizontal_1.0_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      539 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      501 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      648 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     2161 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_6_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_16_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_6_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_vertical_bottom.png
+-rw-rw-rw-   0 root         (0) root         (0)      351 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_vertical_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_10.png
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_ccccc.png
+-rw-rw-rw-   0 root         (0) root         (0)     3058 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_ccccc.png
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_10.png
+-rw-rw-rw-   0 root         (0) root         (0)      661 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_vertical.png
+-rw-rw-rw-   0 root         (0) root         (0)      725 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_6.png
+-rw-rw-rw-   0 root         (0) root         (0)      544 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_horizontal.png
+-rw-rw-rw-   0 root         (0) root         (0)      700 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_horizontal.png
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     4236 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_16.png
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      269 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      264 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_6_horizontal_0.25_0_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_vertical_top.png
+-rw-rw-rw-   0 root         (0) root         (0)      645 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lcccr.png
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_rrrrr.png
+-rw-rw-rw-   0 root         (0) root         (0)      338 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Greys_256_vertical_0.25_1_0_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)      334 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_6_horizontal_0.25_0_0_0_0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     2245 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.25_0.75.png
+-rw-rw-rw-   0 root         (0) root         (0)      437 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_None.png
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_16.png
+-rw-rw-rw-   0 root         (0) root         (0)      604 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)     3919 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      432 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      617 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      366 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      482 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      684 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      437 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      366 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      465 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      461 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      463 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      528 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      573 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      461 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      328 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      313 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      439 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      378 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      575 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      323 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      489 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      470 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      318 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      447 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      316 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      370 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      618 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      421 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      466 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      420 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      653 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      534 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      395 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      525 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      868 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      620 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      768 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      574 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      853 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      587 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      358 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      909 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      852 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      426 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      909 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      867 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      385 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      778 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      471 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      507 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      477 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      478 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      447 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      461 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      417 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      381 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      858 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      312 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      856 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      327 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      367 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      907 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      320 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      928 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      586 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      359 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      366 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      587 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      616 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      388 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_1_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      321 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_0_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      428 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      549 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      564 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      353 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_1_1_1_1_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      381 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_10_0_0_0_0_1_0_0_1_1.0.png
+-rw-rw-rw-   0 root         (0) root         (0)      480 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_0_0_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)      313 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_6_0_0_0_1_1_0_0_1_0.5.png
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_autotextctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_overlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_textbitmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_webpage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_placeholder_textctrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/tests/test_numberdialog.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/COPYRIGHT
+-rw-rw-rw-   0 root         (0) root         (0)      313 2020-06-04 22:25:08.000000 fsleyes-widgets-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       44 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       51 2020-06-04 18:48:37.000000 fsleyes-widgets-0.9.0/requirements-dev.txt
```

### Comparing `fsleyes-widgets-0.8.4/README.rst` & `fsleyes-widgets-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/PKG-INFO` & `fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-widgets
-Version: 0.8.4
+Version: 0.9.0
 Summary: A collection of wxPython widgets used by FSLeyes
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsleyes/widgets
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Description: fsleyes-widgets
         ===============
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets.egg-info/SOURCES.txt` & `fsleyes-widgets-0.9.0/fsleyes_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_colourbutton.py` & `fsleyes-widgets-0.9.0/tests/test_colourbutton.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_layout.py` & `fsleyes-widgets-0.9.0/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_colourbarbitmap.py` & `fsleyes-widgets-0.9.0/tests/test_colourbarbitmap.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/__init__.py` & `fsleyes-widgets-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_runwindow.py` & `fsleyes-widgets-0.9.0/tests/test_runwindow.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_importall.py` & `fsleyes-widgets-0.9.0/tests/test_importall.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_notebook.py` & `fsleyes-widgets-0.9.0/tests/test_notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,18 @@
     notebook.AdvanceSelection(False)
     assert notebook.GetSelection() == 0
     notebook.ShowPage(1)
     notebook.AdvanceSelection()
     assert notebook.GetSelection() == 1
 
 
-def test_event():
-    nb_run_with_wx(_test_event)
-def _test_event(side, ornt):
+@pytest.mark.dodgy
+def test_notebook_events():
+    nb_run_with_wx(_test_notebook_events)
+def _test_notebook_events(side, ornt):
     sim      = wx.UIActionSimulator()
     frame    = wx.GetApp().GetTopWindow()
     sizer    = wx.BoxSizer(wx.VERTICAL)
     notebook = nb.Notebook(frame, style=side | ornt)
     page1    = wx.Panel(notebook)
     page2    = wx.Panel(notebook)
     page3    = wx.Panel(notebook)
```

### Comparing `fsleyes-widgets-0.8.4/tests/test_webpage.py` & `fsleyes-widgets-0.9.0/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_textbitmap.py` & `fsleyes-widgets-0.9.0/tests/test_textbitmap.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_typedict.py` & `fsleyes-widgets-0.9.0/tests/test_typedict.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_floatspin.py` & `fsleyes-widgets-0.9.0/tests/test_floatspin.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_autotextctrl.py` & `fsleyes-widgets-0.9.0/tests/test_autotextctrl.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_bitmaptoggle.py` & `fsleyes-widgets-0.9.0/tests/test_bitmaptoggle.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_elistbox.py` & `fsleyes-widgets-0.9.0/tests/test_elistbox.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_floatslider.py` & `fsleyes-widgets-0.9.0/tests/test_floatslider.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,19 +136,23 @@
     run_with_wx(_test_FloatSlider_changeRange)
 def _test_FloatSlider_changeRange():
     frame  = wx.GetApp().GetTopWindow()
     slider = floatslider.FloatSlider(frame)
     _test_widget_changeRange(slider)
 
 
+@pytest.mark.dodgy
 def test_FloatSlider_mouse_non_gtk():
     run_with_wx(_test_FloatSlider_mouse)
+
+@pytest.mark.dodgy
 def test_FloatSlider_mouse_gtk():
     with mock.patch('fsleyes_widgets.floatslider.wx.Platform', '__WXGTK__'):
         run_with_wx(_test_FloatSlider_mouse)
+
 def _test_FloatSlider_mouse():
 
     sim    = wx.UIActionSimulator()
     frame  = wx.GetApp().GetTopWindow()
     minval = 0
     init   = 50
     maxval = 100
@@ -319,14 +323,15 @@
             simclick(sim, btn)
             assert tuple(panel.GetRange()) == expected
 
             if shouldEv: assert result[0] == expected
             else:        assert result[0] is None
 
 
+@pytest.mark.dodgy
 def test_SliderSpinPanel_events():
     run_with_wx(_test_SliderSpinPanel_events)
 def _test_SliderSpinPanel_events():
 
     sim   = wx.UIActionSimulator()
     frame = wx.GetApp().GetTopWindow()
     panel = floatslider.SliderSpinPanel(frame, label='Value', style=0)
```

### Comparing `fsleyes-widgets-0.8.4/tests/test_togglepanel.py` & `fsleyes-widgets-0.9.0/tests/test_togglepanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_rangeslider.py` & `fsleyes-widgets-0.9.0/tests/test_rangeslider.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     sizer = wx.BoxSizer(wx.HORIZONTAL)
     sizer.Add(panel, flag=wx.EXPAND)
     frame.SetSizer(sizer)
     frame.Layout()
     _test_RangePanel_logic(panel)
 
 
+@pytest.mark.dodgy
 def test_RangePanel_events_slider():
     run_with_wx(_test_RangePanel_events_slider)
 def _test_RangePanel_events_slider():
 
     sim   = wx.UIActionSimulator()
     frame = wx.GetApp().GetTopWindow()
     panel = rangeslider.RangePanel(frame, style=rangeslider.RP_SLIDER)
@@ -232,14 +233,15 @@
     sizer = wx.BoxSizer(wx.HORIZONTAL)
     sizer.Add(panel, flag=wx.EXPAND, proportion=1)
     frame.SetSizer(sizer)
     frame.Layout()
     _test_RangePanel_logic(panel)
 
 
+@pytest.mark.dodgy
 def test_RangeSliderSpinPanel_onchange():
     run_with_wx(_test_RangeSliderSpinPanel_onchange)
 def _test_RangeSliderSpinPanel_onchange():
 
     sim   = wx.UIActionSimulator()
     frame = wx.GetApp().GetTopWindow()
     frame.SetSize((600, 600))
```

### Comparing `fsleyes-widgets-0.8.4/tests/test_status.py` & `fsleyes-widgets-0.9.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_textpanel.py` & `fsleyes-widgets-0.9.0/tests/test_textpanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_imagepanel.py` & `fsleyes-widgets-0.9.0/tests/test_imagepanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_utils.py` & `fsleyes-widgets-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_numberdialog.py` & `fsleyes-widgets-0.9.0/tests/test_numberdialog.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_widgetgrid.py` & `fsleyes-widgets-0.9.0/tests/test_widgetgrid.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/bitmapbuttons/false.png` & `fsleyes-widgets-0.9.0/tests/testdata/bitmapbuttons/false.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/bitmapbuttons/true.png` & `fsleyes-widgets-0.9.0/tests/testdata/bitmapbuttons/true.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_0_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_1_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_1_1_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_1_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_0_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_0_0_0_0_1_0_0_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_10_1_0_0_1_0_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_6_0_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/R_16_0_0_0_1_1_1_1_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_1_0_0_1_1_1_1_1_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_0.5.png` & `fsleyes-widgets-0.9.0/tests/testdata/textbitmap/Label_16_0_0_0_0_0_0_0_1_0.5.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_horizontal.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_horizontal.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_rrrrr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_rrrrr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_rrrrr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_rrrrr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_rrrrr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_rrrrr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_16.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_16.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_horizontal_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_horizontal_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_10.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_10.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_vertical_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_vertical_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lllll.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lllll.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_False_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_ccccc.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_ccccc.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_vertical_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_vertical_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.25_0.5_0.75_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.25_0.5_0.75_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_10.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_10.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.5_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.5_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_horizontal_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_horizontal_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_6.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_6.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_horizontal_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_horizontal_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_horizontal_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_horizontal_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_ccccc.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_ccccc.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_vertical_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_vertical_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_16.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_16.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_16.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_16.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_vertical_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_vertical_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_lllll.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_lllll.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_horizontal_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_horizontal_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lcccr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_top_lcccr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_vertical_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_vertical_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_vertical_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_vertical_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_vertical.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_False_vertical.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_2.0_horizontal_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_2.0_horizontal_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_vertical.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_vertical.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_ccccc.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_ccccc.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lcccr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lcccr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_horizontal_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_horizontal_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_ccccc.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_ccccc.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_1.0_horizontal_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_1.0_horizontal_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_True_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_horizontal_1.0_0_0_0_0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_10.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_10.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_10.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_10.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_horizontal.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_horizontal.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_horizontal.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_top_lcccr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_top_lcccr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_16.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_bottom_16.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lllll.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lllll.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_16_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/standard_usage_Blues_256_vertical_1.0_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_False_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_6_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_3.0_vertical_bottom.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_3.0_vertical_bottom.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_Greys.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_True_Greys_Greys.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_right_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_right_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_6.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_vertical_top_6.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_1.0_False_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_False_horizontal.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_3.0_True_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lcccr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_lcccr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_left_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_6.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_bottom_6.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_left_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_top_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_6.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_and_ticks_horizontal_top_6.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_10_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.49_0.51_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_ticks_Reds_Blues_0_0.49_0.51_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_top_10_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_left_10_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_16_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_top_16_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_6_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_6_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_0.5_True_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_vertical.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_Blues_True_vertical.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_horizontal.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_horizontal.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/scale_0.5_vertical_top.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/scale_0.5_vertical_top.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_1_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_bottom_10_1_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_top_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_left_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lllll.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_horizontal_bottom_lllll.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_left_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_vertical.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/negCmap_invert_Reds_None_True_vertical.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_1_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_1_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_rrrrr.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/tickalign_vertical_bottom_rrrrr.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_left_6_0_0_0_1_0.0_0.25_0.75_1.0.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_bottom_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_right_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_vertical_bottom_16_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_vertical_bottom_16_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_Blues.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_Blues.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_vertical_top_10_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_None.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/gamma_2.0_False_Reds_None.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_top_16_0_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.25_0.75.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/ticks_horizontal_right_10_1_0_0_1_0.25_0.75.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/testdata/colourbarbitmap/label_horizontal_right_6_0_0_0_1.png` & `fsleyes-widgets-0.9.0/tests/testdata/colourbarbitmap/label_horizontal_right_6_0_0_0_1.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_bitmapradio.py` & `fsleyes-widgets-0.9.0/tests/test_bitmapradio.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_progress.py` & `fsleyes-widgets-0.9.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_texttag.py` & `fsleyes-widgets-0.9.0/tests/test_texttag.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/tests/test_placeholder_textctrl.py` & `fsleyes-widgets-0.9.0/tests/test_placeholder_textctrl.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/setup.py` & `fsleyes-widgets-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 basedir = op.dirname(__file__)
 
 # Dependencies are listed in requirements.txt
 with open(op.join(basedir, 'requirements.txt'), 'rt') as f:
     install_requires = [l.strip() for l in f.readlines()]
 
-packages = find_packages(
-    exclude=('doc', 'tests', 'dist', 'build', 'fsleyes_widgets.egg-info'))
+packages = find_packages(include=('fsleyes_widgets', 'fsleyes_widgets.*'))
 
 # Extract the vesrion number from fsleyes_widgets/__init__.py
 version = {}
 with open(op.join(basedir, "fsleyes_widgets", "__init__.py"), 'rt') as f:
     for line in f:
         if line.startswith('__version__'):
             exec(line, version)
```

### Comparing `fsleyes-widgets-0.8.4/doc/conf.py` & `fsleyes-widgets-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/widgetgrid.png` & `fsleyes-widgets-0.9.0/doc/images/widgetgrid.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/bitmapradiobox.png` & `fsleyes-widgets-0.9.0/doc/images/bitmapradiobox.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/colourbarbitmap.png` & `fsleyes-widgets-0.9.0/doc/images/colourbarbitmap.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/simplemessagedialog.png` & `fsleyes-widgets-0.9.0/doc/images/simplemessagedialog.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/fsldirdialog.png` & `fsleyes-widgets-0.9.0/doc/images/fsldirdialog.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/widgetlist.png` & `fsleyes-widgets-0.9.0/doc/images/widgetlist.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/texteditdialog.png` & `fsleyes-widgets-0.9.0/doc/images/texteditdialog.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/texttagpanel.png` & `fsleyes-widgets-0.9.0/doc/images/texttagpanel.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/images/rangesliderspinpanel.png` & `fsleyes-widgets-0.9.0/doc/images/rangesliderspinpanel.png`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/fsleyes_widgets.utils.rst` & `fsleyes-widgets-0.9.0/doc/fsleyes_widgets.utils.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/doc/fsleyes_widgets.rst` & `fsleyes-widgets-0.9.0/doc/fsleyes_widgets.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/PKG-INFO` & `fsleyes-widgets-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-widgets
-Version: 0.8.4
+Version: 0.9.0
 Summary: A collection of wxPython widgets used by FSLeyes
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsleyes/widgets
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Description: fsleyes-widgets
         ===============
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/bitmapradio.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/bitmapradio.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/__init__.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 behaviour in the existing controls.
 
 
 This file is used to store the current ``fsleyes-widgets`` version.
 """
 
 
-__version__ = '0.8.4'
+__version__ = '0.9.0'
 
 
 from fsleyes_widgets.utils import (WX_PYTHON,  # noqa
                                    WX_PHOENIX,
                                    wxversion,
                                    isalive)
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/textpanel.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/textpanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/numberdialog.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/numberdialog.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/floatslider.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/floatslider.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,16 @@
     def __init__(self,
                  parent,
                  value=None,
                  minValue=None,
                  maxValue=None,
                  label=None,
                  style=None,
-                 spinWidth=None):
+                 spinWidth=None,
+                 precision=None):
         """Create a ``SliderSpinPanel``.
 
         The following style flags are available:
 
          .. autosummary::
             SSP_SHOW_LIMITS
             SSP_EDIT_LIMITS
@@ -409,15 +410,16 @@
         self.__spinbox = floatspin.FloatSpinCtrl(
             self,
             value=value,
             minValue=minValue,
             maxValue=maxValue,
             increment=increment,
             style=spinStyle,
-            width=spinWidth)
+            width=spinWidth,
+            precision=precision)
 
         self.__sizer = wx.BoxSizer(wx.HORIZONTAL)
         self.SetSizer(self.__sizer)
 
         if label is not None:
             self.__label = wx.StaticText(self, label=label)
             self.__sizer.Add(self.__label, flag=wx.EXPAND)
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/placeholder_textctrl.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/placeholder_textctrl.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/widgetlist.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/widgetlist.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/floatspin.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/floatspin.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
                  parent,
                  minValue=None,
                  maxValue=None,
                  increment=None,
                  value=None,
                  style=None,
                  width=None,
-                 evDelta=None):
+                 evDelta=None,
+                 precision=None):
         """Create a ``FloatSpinCtrl``.
 
         The following style flags are available:
           .. autosummary::
              FSC_MOUSEWHEEL
              FSC_INTEGER
              FSC_NO_LIMIT
@@ -87,14 +88,18 @@
                         from the spin button can be processed. This is
                         implemented in the :meth:`__onSpinDown` and
                         :meth:`__onSpinUp` methods.
 
                         This has the side effect that if the user clicks and
                         holds on the spin button, they have to wait <delta>
                         seconds between increments/decrements.
+
+        :arg precision: The desired precision to the right of the decimal
+                        value. Ignored if the :attr:`FSC_INTEGER` style is
+                        active.
         """
         FloatSpinBase.__init__(self, parent)
 
         if minValue  is None: minValue  = 0
         if maxValue  is None: maxValue  = 100
         if value     is None: value     = 0
         if increment is None: increment = 1
@@ -147,14 +152,18 @@
             width = self.__text.GetTextExtent('0' * width)[0]
             self.__text.SetMinSize((width + 10, -1))
             self.__text.SetMaxSize((width + 10, -1))
 
         if self.__integer: self.__format = '{:d}'
         else:              self.__format = '{:.7G}'
 
+        if   self.__integer:    self.__format = '{:d}'
+        elif precision is None: self.__format = '{:.7G}'
+        else:                   self.__format = '{:.' + str(precision) + 'f}'
+
         # Events on key down, enter, focus
         # lost, and on the spin control
         self.__text.Bind(wx.EVT_KEY_DOWN,   self.__onKeyDown)
         self.__text.Bind(wx.EVT_TEXT_ENTER, self.__onText)
         self.__text.Bind(wx.EVT_KILL_FOCUS, self.__onKillFocus)
         self.__spin.Bind(wx.EVT_SPIN_UP,    self.__onSpinUp)
         self.__spin.Bind(wx.EVT_SPIN_DOWN,  self.__onSpinDown)
@@ -376,15 +385,14 @@
 
         try:
             if self.__integer: val = int(  val)
             else:              val = float(val)
         except ValueError:
             self.SetValue(self.__value)
             return
-
         valset = self.SetValue(val)
 
         # Add a 'changed' attribute so
         # users can tell if the value
         # that was entered was not the
         # value that ended up getting
         # stored
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/colourbutton.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/colourbutton.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/notebook.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/notebook.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/dialog.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/togglepanel.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/togglepanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/bitmaptoggle.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/bitmaptoggle.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/imagepanel.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/imagepanel.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/texttag.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/texttag.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/rangeslider.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/rangeslider.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/elistbox.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/elistbox.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/widgetgrid.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/widgetgrid.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/autotextctrl.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/autotextctrl.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 
 import logging
 
 import wx
 import wx.lib.newevent as wxevent
 
+import fsleyes_widgets.utils as wutils
+
 
 log = logging.getLogger(__name__)
 
 
 class AutoTextCtrl(wx.Panel):
     """The ``AutoTextCtrl`` class is essentially a ``wx.TextCtrl`` which is able
     to dynamically show a list of options to the user, with a
@@ -305,14 +307,15 @@
                       pattern matching case sensitive.
         """
 
         wx.Dialog.__init__(self,
                           parent,
                           style=(wx.NO_BORDER | wx.STAY_ON_TOP))
 
+        self.__alive         = True
         self.__caseSensitive = style & ATC_CASE_SENSITIVE
         self.__atc           = atc
         self.__options       = options
         self.__textCtrl      = wx.TextCtrl(self,
                                            value=text,
                                            style=wx.TE_PROCESS_ENTER)
         self.__listBox       = wx.ListBox( self,
@@ -416,55 +419,70 @@
 
     def __destroy(self, genEnter=True, returnFocus=True):
         """Called by various event handlers. Copies the current value in
         this ``AutoCompletePopup`` to the owning :class:`AutoTextCtrl`,
         and then (asynchronously) destroys this ``AutoCompletePopup``.
         """
 
+        # destroy has already been
+        # called - don't run again
+        if not self.__alive:
+            return
+
+        self.__alive = False
+
         value = self.__textCtrl.GetValue()
         idx   = self.__textCtrl.GetInsertionPoint()
         atc   = self.__atc
 
         # Under wx/GTK, we might still receive focus
         # events, which will trigger another call to
         # __destroy. So we remove all callbacks to
         # prevent this from happening.
-        self           .Bind(wx.EVT_SET_FOCUS,  None)
-        self.__textCtrl.Bind(wx.EVT_SET_FOCUS,  None)
-        self.__listBox .Bind(wx.EVT_SET_FOCUS,  None)
-        self           .Bind(wx.EVT_KILL_FOCUS, None)
-        self.__textCtrl.Bind(wx.EVT_KILL_FOCUS, None)
-        self.__listBox .Bind(wx.EVT_KILL_FOCUS, None)
+        self.__textCtrl.Bind(wx.EVT_TEXT,           None)
+        self.__textCtrl.Bind(wx.EVT_TEXT_ENTER,     None)
+        self.__textCtrl.Bind(wx.EVT_CHAR_HOOK,      None)
+        self.__textCtrl.Bind(wx.EVT_KEY_DOWN,       None)
+        self.__listBox .Bind(wx.EVT_CHAR_HOOK,      None)
+        self.__listBox .Bind(wx.EVT_KEY_DOWN,       None)
+        self.__listBox .Bind(wx.EVT_LISTBOX_DCLICK, None)
+        self.__listBox .Bind(wx.EVT_LEFT_DOWN,      None)
+        self.__listBox .Bind(wx.EVT_RIGHT_DOWN,     None)
+        self           .Bind(wx.EVT_SET_FOCUS,      None)
+        self.__textCtrl.Bind(wx.EVT_SET_FOCUS,      None)
+        self.__listBox .Bind(wx.EVT_SET_FOCUS,      None)
+        self           .Bind(wx.EVT_KILL_FOCUS,     None)
+        self.__textCtrl.Bind(wx.EVT_KILL_FOCUS,     None)
+        self.__listBox .Bind(wx.EVT_KILL_FOCUS,     None)
 
         atc.ChangeValue(      value)
         atc.SetInsertionPoint(idx)
 
         # Tell the atc whether or not it
         # should take the focus when this
         # popup is destroyed.
         atc.SetTakeFocus(returnFocus)
 
         if genEnter:
             atc.GenEnterEvent()
 
         def destroy():
-            try:
-                if self.IsModal():
-                    self.EndModal(wx.ID_OK)
-                else:
-                    self.Close()
-                    self.Destroy()
 
-            except wx.PyDeadObjectError:
-                pass
+            if not wutils.isalive(self):
+                return
+
+            if self.IsModal():
+                self.EndModal(wx.ID_OK)
+            else:
+                self.Close()
+                self.Destroy()
 
         ev = ATCPopupDestroyEvent()
         ev.SetEventObject(self)
         wx.PostEvent(self, ev)
-
         wx.CallAfter(destroy)
 
 
     def __getMatches(self, prefix):
         """Returns a list of auto-completion options which match the given
         prefix.
         """
```

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/progress.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/progress.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/layout.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/layout.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/colourbarbitmap.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/colourbarbitmap.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/status.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/status.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/__init__.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/webpage.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/webpage.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/typedict.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/typedict.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/overlay.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/overlay.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/textbitmap.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/textbitmap.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/runwindow.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/runwindow.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/fsleyes_widgets/utils/b64icon.py` & `fsleyes-widgets-0.9.0/fsleyes_widgets/utils/b64icon.py`

 * *Files identical despite different names*

### Comparing `fsleyes-widgets-0.8.4/LICENSE` & `fsleyes-widgets-0.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The fsleyes-widgets library
 
-Copyright 2016-2019 University of Oxford, Oxford, UK.
+Copyright 2016-2020 University of Oxford, Oxford, UK.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

