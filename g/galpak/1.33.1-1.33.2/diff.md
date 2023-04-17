# Comparing `tmp/galpak-1.33.1.tar.gz` & `tmp/galpak-1.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galpak-1.33.1.tar", last modified: Fri Dec 16 15:53:03 2022, max compression
+gzip compressed data, was "galpak-1.33.2.tar", last modified: Mon Apr 17 09:57:22 2023, max compression
```

## Comparing `galpak-1.33.1.tar` & `galpak-1.33.2.tar`

### file list

```diff
@@ -1,150 +1,131 @@
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      215 2022-11-09 20:19:35.000000 galpak-1.33.1/.gitignore
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      999 2022-12-16 15:21:25.000000 galpak-1.33.1/.gitlab-ci.yml
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    10352 2022-11-09 20:47:52.000000 galpak-1.33.1/CHANGELOG.md
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      454 2022-11-09 20:19:35.000000 galpak-1.33.1/INSTALL
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      254 2020-03-31 09:29:29.000000 galpak-1.33.1/LICENCE
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      332 2022-11-09 20:19:35.000000 galpak-1.33.1/MANIFEST.in
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     5605 2022-12-16 15:53:03.000000 galpak-1.33.1/PKG-INFO
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3928 2022-11-09 20:19:35.000000 galpak-1.33.1/README.md
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)       16 2022-11-09 20:19:35.000000 galpak-1.33.1/TODO
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   607680 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ALMA_Freq_test1.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   518400 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ALMA_Freq_test2.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   184320 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ALMA_Freq_test3.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/GalPaK_cube_1101_from_paper.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2019-07-23 08:10:03.000000 galpak-1.33.1/data/input/GalPaK_cube_1101_from_paper.fits~
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)      359 2021-07-27 10:23:39.000000 galpak-1.33.1/data/input/alma_instrument.txt
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/cube/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/GalPaK_cube_1101_size4.08_flux1e-16_incl60_vmax199_disp80_seeing1.0.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   296640 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/MUSE_subcube.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   141120 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/MUSE_subcube_mpdaf.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/MUSE_testcube_noheader.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)       94 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/README
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   296640 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/subcube_MUSE.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   141120 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/subcube_mpdaf.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2018-06-17 17:25:57.000000 galpak-1.33.1/data/input/cube/test_cube.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   190080 2022-01-30 15:52:47.000000 galpak-1.33.1/data/input/cube/zoomVariance_oii_subcube_3Dcontinuum_subtracted.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   190080 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/cube/zoom_oii_subcube_3Dcontinuum_subtracted.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/galfit_125_seeing1.0_flux1e-16.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/galpak_125_seeing1.0_flux1e-16.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      147 2021-07-27 10:23:39.000000 galpak-1.33.1/data/input/myinstrument.txt
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/pymulti/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   207685 2022-01-01 00:36:50.000000 galpak-1.33.1/data/input/pymulti/out.txt
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    89600 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outIS.iterinfo
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)  1282932 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outIS.points
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   237600 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outIS.ptprob
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   962000 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outev.dat
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    67400 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outlive.points
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    68200 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outphys_live.points
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      337 2022-01-01 00:36:50.000000 galpak-1.33.1/data/input/pymulti/outpost_equal_weights.dat
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      225 2022-01-01 00:37:32.000000 galpak-1.33.1/data/input/pymulti/outresume.dat
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1745 2022-01-01 00:36:50.000000 galpak-1.33.1/data/input/pymulti/outstats.dat
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     2634 2022-01-01 00:36:50.000000 galpak-1.33.1/data/input/pymulti/outsummary.txt
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/ref/
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2022-11-09 20:19:35.000000 galpak-1.33.1/data/input/ref/GalPaK_cube_1101_from_v191.fits
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2022-11-09 20:19:35.000000 galpak-1.33.1/data/input/ref/GalPaK_cube_1101_from_v191_noised.fits
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   146880 2022-11-09 20:19:35.000000 galpak-1.33.1/data/input/ref/cubeclean_current_pair-2.fits
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   146880 2022-11-09 20:19:35.000000 galpak-1.33.1/data/input/ref/psf3d_current_pair_Seeing08.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ref/ref_cube_clean.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ref/ref_cube_clean_gpk188.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ref/ref_cube_conv_gpk188.fits
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      249 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ref/ref_instrument.dat
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      240 2020-04-22 22:09:40.000000 galpak-1.33.1/data/input/ref/ref_parameters.dat
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/ultranest/
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/ultranest/out/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1138 2021-12-31 23:32:17.000000 galpak-1.33.1/data/input/ultranest/out/debug.log
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/data/input/ultranest/out/results/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    61472 2022-01-01 00:27:52.000000 galpak-1.33.1/data/input/ultranest/out/results/points.hdf5
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/doc/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     5966 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/Makefile
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     5105 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/make.bat
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/doc/source/
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/doc/source/_static/
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     4286 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/_static/favicon.ico
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      313 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/acknowledgments.rst
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      337 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/api.rst
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      371 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/bug.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)      137 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/common.rst
--rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     8247 2022-11-09 20:19:35.000000 galpak-1.33.1/doc/source/conf.py
--rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     1143 2022-11-09 20:19:35.000000 galpak-1.33.1/doc/source/dependencies.rst
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1560 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/disk_model.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     4997 2020-02-11 16:59:36.000000 galpak-1.33.1/doc/source/galaxy_parameters.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)      462 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/hyperspectral_cube.rst
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/doc/source/images/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   141936 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/GalPaK_MCMC.png
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    53225 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/GalPak_flow.odp
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   203423 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/GalPak_flow.png
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/doc/source/images/deconvolution_example/
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)   110332 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/125_velocity_seeing10.png
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   139184 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig2.png
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    45016 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig4.png
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)   118803 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig5.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)   148127 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/bad_chain_not_scaled.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)   173957 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/good_chain_scaled.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    48403 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/plot_images.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)   121698 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/plot_mcmc.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    94385 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/deconvolution_example/plot_mcmc_sorted.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    48878 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/instrument_chart.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    12956 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/images/logo_galpak.png
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    76134 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/images/plot_geweke.png
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     2033 2019-12-12 13:29:14.000000 galpak-1.33.1/doc/source/index.rst
--rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      641 2022-11-09 20:19:35.000000 galpak-1.33.1/doc/source/install.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     2937 2020-02-11 16:59:36.000000 galpak-1.33.1/doc/source/instruments.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     1201 2018-04-15 07:02:15.000000 galpak-1.33.1/doc/source/line_spread_functions.rst
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1856 2020-04-22 22:09:40.000000 galpak-1.33.1/doc/source/mcmc.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)     3518 2020-02-11 16:59:36.000000 galpak-1.33.1/doc/source/overview.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)      782 2019-04-10 14:30:51.000000 galpak-1.33.1/doc/source/point_spread_functions.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)      117 2016-08-03 10:31:41.000000 galpak-1.33.1/doc/source/table_of_contents.rst
--rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    31035 2022-11-09 20:19:35.000000 galpak-1.33.1/doc/source/tutorials.rst
--rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    32016 2018-03-20 20:27:07.000000 galpak-1.33.1/doc/source/tutorials.rst.orig
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      291 2022-11-09 20:19:35.000000 galpak-1.33.1/doc/source/under_the_hood.rst
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     5567 2022-11-09 20:19:35.000000 galpak-1.33.1/dodo.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)       90 2022-12-16 15:53:03.000000 galpak-1.33.1/setup.cfg
--rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     1624 2022-11-09 20:19:35.000000 galpak-1.33.1/setup.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/src/
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/src/galpak/
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      458 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/__init__.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      460 2022-11-09 20:47:52.000000 galpak-1.33.1/src/galpak/__version__.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      265 2022-01-30 15:52:47.000000 galpak-1.33.1/src/galpak/ansi_colors.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     7287 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/api.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     5667 2022-01-31 09:00:16.000000 galpak-1.33.1/src/galpak/convolution.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     2636 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/fits_sanitizer.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     1865 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/galaxy_parameter.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    18207 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/galaxy_parameters.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    68512 2022-11-09 20:23:23.000000 galpak-1.33.1/src/galpak/galpak3d.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     7260 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/galpak3d_utils.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    33770 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/hyperspectral_cube.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    21586 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/instruments.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     4138 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/math_utils.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    22336 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/mcmc.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    28247 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/model_class.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    13508 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/model_sersic3d.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    11134 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/model_utilities.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    48756 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/plot_utilities.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    31112 2022-11-09 20:19:35.000000 galpak-1.33.1/src/galpak/spread_functions.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      246 2022-01-30 15:52:47.000000 galpak-1.33.1/src/galpak/string_stdout.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/src/galpak.egg-info/
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     4161 2022-12-16 15:53:03.000000 galpak-1.33.1/src/galpak.egg-info/SOURCES.txt
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/tests/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)        0 2020-10-05 10:41:42.000000 galpak-1.33.1/tests/__init__.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/tests/benchmarks/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     3497 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/benchmarks/galpak_speed.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1133 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/benchmarks/nan_to_num.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1249 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/benchmarks/power_of_three.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1235 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/benchmarks/power_of_two.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/tests/other/
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3799 2022-11-09 20:19:35.000000 galpak-1.33.1/tests/other/galpak3d_quantuum_test.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/tests/suite/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)        0 2021-07-27 10:23:40.000000 galpak-1.33.1/tests/suite/__init__.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3924 2022-11-09 20:19:35.000000 galpak-1.33.1/tests/suite/galaxy_parameters_test.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    26323 2022-11-09 20:19:35.000000 galpak-1.33.1/tests/suite/galpak3d_test.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)    14682 2021-07-27 10:23:40.000000 galpak-1.33.1/tests/suite/hyperspectral_cube_test.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      857 2021-07-27 10:23:40.000000 galpak-1.33.1/tests/suite/math_utils_test.py
-drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2022-12-16 15:53:03.000000 galpak-1.33.1/tests/tools/
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)        0 2020-10-05 10:41:49.000000 galpak-1.33.1/tests/tools/__init__.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      618 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/tools/make_animation.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)      940 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/tools/numeric_assertions.py
--rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1739 2020-04-22 22:09:40.000000 galpak-1.33.1/tests/tools/numpy_ndarray_assertions.py
--rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      844 2022-11-09 20:32:50.000000 galpak-1.33.1/tox.ini
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.062587 galpak-1.33.2/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      454 2023-04-17 09:21:12.000000 galpak-1.33.2/INSTALL
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      254 2023-03-10 10:57:09.000000 galpak-1.33.2/LICENCE
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      332 2023-04-17 09:21:12.000000 galpak-1.33.2/MANIFEST.in
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     4328 2023-04-17 09:57:22.062587 galpak-1.33.2/PKG-INFO
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3928 2023-04-17 09:21:12.000000 galpak-1.33.2/README.md
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.042587 galpak-1.33.2/data/
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.046587 galpak-1.33.2/data/input/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   607680 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ALMA_Freq_test1.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   518400 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ALMA_Freq_test2.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   184320 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ALMA_Freq_test3.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/GalPaK_cube_1101_from_paper.fits
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2019-07-23 08:10:03.000000 galpak-1.33.2/data/input/GalPaK_cube_1101_from_paper.fits~
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      359 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/alma_instrument.txt
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.050587 galpak-1.33.2/data/input/cube/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/GalPaK_cube_1101_size4.08_flux1e-16_incl60_vmax199_disp80_seeing1.0.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   296640 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/MUSE_subcube.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   141120 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/MUSE_subcube_mpdaf.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/MUSE_testcube_noheader.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)       94 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/README
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   296640 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/subcube_MUSE.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   141120 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/subcube_mpdaf.fits
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)   218880 2018-06-17 17:25:57.000000 galpak-1.33.2/data/input/cube/test_cube.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   190080 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/zoomVariance_oii_subcube_3Dcontinuum_subtracted.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   190080 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/cube/zoom_oii_subcube_3Dcontinuum_subtracted.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/galfit_125_seeing1.0_flux1e-16.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/galpak_125_seeing1.0_flux1e-16.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      147 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/myinstrument.txt
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.054587 galpak-1.33.2/data/input/pymulti/
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)   207685 2022-01-01 00:36:50.000000 galpak-1.33.2/data/input/pymulti/out.txt
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)    89600 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outIS.iterinfo
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)  1282932 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outIS.points
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)   237600 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outIS.ptprob
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)   962000 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outev.dat
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)    67400 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outlive.points
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)    68200 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outphys_live.points
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)      337 2022-01-01 00:36:50.000000 galpak-1.33.2/data/input/pymulti/outpost_equal_weights.dat
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)      225 2022-01-01 00:37:32.000000 galpak-1.33.2/data/input/pymulti/outresume.dat
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1745 2022-01-01 00:36:50.000000 galpak-1.33.2/data/input/pymulti/outstats.dat
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)     2634 2022-01-01 00:36:50.000000 galpak-1.33.2/data/input/pymulti/outsummary.txt
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.054587 galpak-1.33.2/data/input/ref/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-04-17 09:21:12.000000 galpak-1.33.2/data/input/ref/GalPaK_cube_1101_from_v191.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-04-17 09:21:12.000000 galpak-1.33.2/data/input/ref/GalPaK_cube_1101_from_v191_noised.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   146880 2023-04-17 09:21:12.000000 galpak-1.33.2/data/input/ref/cubeclean_current_pair-2.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   146880 2023-04-17 09:21:12.000000 galpak-1.33.2/data/input/ref/psf3d_current_pair_Seeing08.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ref/ref_cube_clean.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ref/ref_cube_clean_gpk188.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   218880 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ref/ref_cube_conv_gpk188.fits
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      249 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ref/ref_instrument.dat
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      240 2023-03-10 10:57:09.000000 galpak-1.33.2/data/input/ref/ref_parameters.dat
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.042587 galpak-1.33.2/data/input/ultranest/
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.054587 galpak-1.33.2/data/input/ultranest/out/
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)     1138 2021-12-31 23:32:17.000000 galpak-1.33.2/data/input/ultranest/out/debug.log
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.054587 galpak-1.33.2/data/input/ultranest/out/results/
+-rw-r--r--   0 nbouche   (1000) nbouche   (1000)    61472 2022-01-01 00:27:52.000000 galpak-1.33.2/data/input/ultranest/out/results/points.hdf5
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.054587 galpak-1.33.2/doc/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     5966 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/Makefile
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     5105 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/make.bat
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.058587 galpak-1.33.2/doc/source/
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.058587 galpak-1.33.2/doc/source/_static/
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     4286 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/_static/favicon.ico
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      313 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/acknowledgments.rst
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      337 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/api.rst
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      371 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/bug.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      137 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/common.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     8247 2023-04-17 09:21:12.000000 galpak-1.33.2/doc/source/conf.py
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     1143 2023-04-17 09:21:12.000000 galpak-1.33.2/doc/source/dependencies.rst
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     1560 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/disk_model.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     4997 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/galaxy_parameters.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      462 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/hyperspectral_cube.rst
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.058587 galpak-1.33.2/doc/source/images/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   141936 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/GalPaK_MCMC.png
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    53225 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/GalPak_flow.odp
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   203423 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/GalPak_flow.png
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.058587 galpak-1.33.2/doc/source/images/deconvolution_example/
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)   110332 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/125_velocity_seeing10.png
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   139184 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig2.png
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    45016 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig4.png
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)   118803 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig5.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)   148127 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/bad_chain_not_scaled.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)   173957 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/good_chain_scaled.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    48403 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/plot_images.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)   121698 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/plot_mcmc.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    94385 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/deconvolution_example/plot_mcmc_sorted.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    48878 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/instrument_chart.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    12956 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/logo_galpak.png
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    76134 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/images/plot_geweke.png
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     2033 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/index.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      641 2023-04-17 09:21:12.000000 galpak-1.33.2/doc/source/install.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     2937 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/instruments.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     1201 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/line_spread_functions.rst
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     1856 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/mcmc.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     3518 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/overview.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      782 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/point_spread_functions.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)      117 2023-03-10 10:57:09.000000 galpak-1.33.2/doc/source/table_of_contents.rst
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)    31035 2023-04-17 09:21:12.000000 galpak-1.33.2/doc/source/tutorials.rst
+-rwxr-xr-x   0 nbouche   (1000) nbouche   (1000)    32016 2018-03-20 20:27:07.000000 galpak-1.33.2/doc/source/tutorials.rst.orig
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      291 2023-04-17 09:21:12.000000 galpak-1.33.2/doc/source/under_the_hood.rst
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)       90 2023-04-17 09:57:22.062587 galpak-1.33.2/setup.cfg
+-rwxrwxr-x   0 nbouche   (1000) nbouche   (1000)     1624 2023-04-17 09:21:12.000000 galpak-1.33.2/setup.py
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.046587 galpak-1.33.2/src/
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.062587 galpak-1.33.2/src/galpak/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      458 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/__init__.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      460 2023-04-17 09:56:28.000000 galpak-1.33.2/src/galpak/__version__.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      265 2023-03-10 10:57:09.000000 galpak-1.33.2/src/galpak/ansi_colors.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     7287 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/api.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     5667 2023-03-10 10:57:09.000000 galpak-1.33.2/src/galpak/convolution.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     2636 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/fits_sanitizer.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     1865 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/galaxy_parameter.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    18207 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/galaxy_parameters.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    68504 2023-04-17 09:28:46.000000 galpak-1.33.2/src/galpak/galpak3d.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     7260 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/galpak3d_utils.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    33770 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/hyperspectral_cube.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    21586 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/instruments.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     4138 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/math_utils.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    22336 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/mcmc.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    28385 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/model_class.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    13508 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/model_sersic3d.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    11134 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/model_utilities.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    48756 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/plot_utilities.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    31112 2023-04-17 09:21:12.000000 galpak-1.33.2/src/galpak/spread_functions.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      246 2023-03-10 10:57:09.000000 galpak-1.33.2/src/galpak/string_stdout.py
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.062587 galpak-1.33.2/src/galpak.egg-info/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3785 2023-04-17 09:57:22.000000 galpak-1.33.2/src/galpak.egg-info/SOURCES.txt
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.046587 galpak-1.33.2/tests/
+drwxrwxr-x   0 nbouche   (1000) nbouche   (1000)        0 2023-04-17 09:57:22.062587 galpak-1.33.2/tests/suite/
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)        0 2023-03-10 10:57:09.000000 galpak-1.33.2/tests/suite/__init__.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)     3924 2023-04-17 09:21:12.000000 galpak-1.33.2/tests/suite/galaxy_parameters_test.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    26323 2023-04-17 09:21:12.000000 galpak-1.33.2/tests/suite/galpak3d_test.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)    14682 2023-03-10 10:57:09.000000 galpak-1.33.2/tests/suite/hyperspectral_cube_test.py
+-rw-rw-r--   0 nbouche   (1000) nbouche   (1000)      857 2023-03-10 10:57:09.000000 galpak-1.33.2/tests/suite/math_utils_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galpak-1.33.1/README.md` & `galpak-1.33.2/README.md`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ALMA_Freq_test1.fits` & `galpak-1.33.2/data/input/ALMA_Freq_test1.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ALMA_Freq_test2.fits` & `galpak-1.33.2/data/input/ALMA_Freq_test2.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ALMA_Freq_test3.fits` & `galpak-1.33.2/data/input/ALMA_Freq_test3.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/GalPaK_cube_1101_from_paper.fits` & `galpak-1.33.2/data/input/GalPaK_cube_1101_from_paper.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/GalPaK_cube_1101_from_paper.fits~` & `galpak-1.33.2/data/input/GalPaK_cube_1101_from_paper.fits~`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/GalPaK_cube_1101_size4.08_flux1e-16_incl60_vmax199_disp80_seeing1.0.fits` & `galpak-1.33.2/data/input/cube/GalPaK_cube_1101_size4.08_flux1e-16_incl60_vmax199_disp80_seeing1.0.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/MUSE_subcube.fits` & `galpak-1.33.2/data/input/cube/MUSE_subcube.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/MUSE_subcube_mpdaf.fits` & `galpak-1.33.2/data/input/cube/MUSE_subcube_mpdaf.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/MUSE_testcube_noheader.fits` & `galpak-1.33.2/data/input/cube/MUSE_testcube_noheader.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/subcube_MUSE.fits` & `galpak-1.33.2/data/input/cube/subcube_MUSE.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/subcube_mpdaf.fits` & `galpak-1.33.2/data/input/cube/subcube_mpdaf.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/test_cube.fits` & `galpak-1.33.2/data/input/cube/test_cube.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/zoomVariance_oii_subcube_3Dcontinuum_subtracted.fits` & `galpak-1.33.2/data/input/cube/zoomVariance_oii_subcube_3Dcontinuum_subtracted.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/cube/zoom_oii_subcube_3Dcontinuum_subtracted.fits` & `galpak-1.33.2/data/input/cube/zoom_oii_subcube_3Dcontinuum_subtracted.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/galfit_125_seeing1.0_flux1e-16.fits` & `galpak-1.33.2/data/input/galfit_125_seeing1.0_flux1e-16.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/galpak_125_seeing1.0_flux1e-16.fits` & `galpak-1.33.2/data/input/galpak_125_seeing1.0_flux1e-16.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/out.txt` & `galpak-1.33.2/data/input/pymulti/out.txt`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outIS.iterinfo` & `galpak-1.33.2/data/input/pymulti/outIS.iterinfo`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outIS.points` & `galpak-1.33.2/data/input/pymulti/outIS.points`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outIS.ptprob` & `galpak-1.33.2/data/input/pymulti/outIS.ptprob`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outev.dat` & `galpak-1.33.2/data/input/pymulti/outev.dat`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outlive.points` & `galpak-1.33.2/data/input/pymulti/outlive.points`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outphys_live.points` & `galpak-1.33.2/data/input/pymulti/outphys_live.points`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outstats.dat` & `galpak-1.33.2/data/input/pymulti/outstats.dat`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/pymulti/outsummary.txt` & `galpak-1.33.2/data/input/pymulti/outsummary.txt`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/GalPaK_cube_1101_from_v191.fits` & `galpak-1.33.2/data/input/ref/GalPaK_cube_1101_from_v191.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/GalPaK_cube_1101_from_v191_noised.fits` & `galpak-1.33.2/data/input/ref/GalPaK_cube_1101_from_v191_noised.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/cubeclean_current_pair-2.fits` & `galpak-1.33.2/data/input/ref/cubeclean_current_pair-2.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/psf3d_current_pair_Seeing08.fits` & `galpak-1.33.2/data/input/ref/psf3d_current_pair_Seeing08.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/ref_cube_clean.fits` & `galpak-1.33.2/data/input/ref/ref_cube_clean.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/ref_cube_clean_gpk188.fits` & `galpak-1.33.2/data/input/ref/ref_cube_clean_gpk188.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ref/ref_cube_conv_gpk188.fits` & `galpak-1.33.2/data/input/ref/ref_cube_conv_gpk188.fits`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ultranest/out/debug.log` & `galpak-1.33.2/data/input/ultranest/out/debug.log`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/data/input/ultranest/out/results/points.hdf5` & `galpak-1.33.2/data/input/ultranest/out/results/points.hdf5`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/Makefile` & `galpak-1.33.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/make.bat` & `galpak-1.33.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/_static/favicon.ico` & `galpak-1.33.2/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/conf.py` & `galpak-1.33.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/dependencies.rst` & `galpak-1.33.2/doc/source/dependencies.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/disk_model.rst` & `galpak-1.33.2/doc/source/disk_model.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/galaxy_parameters.rst` & `galpak-1.33.2/doc/source/galaxy_parameters.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/GalPaK_MCMC.png` & `galpak-1.33.2/doc/source/images/GalPaK_MCMC.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/GalPak_flow.odp` & `galpak-1.33.2/doc/source/images/GalPak_flow.odp`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/GalPak_flow.png` & `galpak-1.33.2/doc/source/images/GalPak_flow.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/125_velocity_seeing10.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/125_velocity_seeing10.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig2.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig2.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig4.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig4.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig5.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/GalPaK_cube_1101_from_paper_fig5.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/bad_chain_not_scaled.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/bad_chain_not_scaled.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/good_chain_scaled.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/good_chain_scaled.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/plot_images.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/plot_images.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/plot_mcmc.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/plot_mcmc.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/deconvolution_example/plot_mcmc_sorted.png` & `galpak-1.33.2/doc/source/images/deconvolution_example/plot_mcmc_sorted.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/instrument_chart.png` & `galpak-1.33.2/doc/source/images/instrument_chart.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/logo_galpak.png` & `galpak-1.33.2/doc/source/images/logo_galpak.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/images/plot_geweke.png` & `galpak-1.33.2/doc/source/images/plot_geweke.png`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/index.rst` & `galpak-1.33.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/install.rst` & `galpak-1.33.2/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/instruments.rst` & `galpak-1.33.2/doc/source/instruments.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/line_spread_functions.rst` & `galpak-1.33.2/doc/source/line_spread_functions.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/mcmc.rst` & `galpak-1.33.2/doc/source/mcmc.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/overview.rst` & `galpak-1.33.2/doc/source/overview.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/point_spread_functions.rst` & `galpak-1.33.2/doc/source/point_spread_functions.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/tutorials.rst` & `galpak-1.33.2/doc/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/doc/source/tutorials.rst.orig` & `galpak-1.33.2/doc/source/tutorials.rst.orig`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/setup.py` & `galpak-1.33.2/setup.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/api.py` & `galpak-1.33.2/src/galpak/api.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/convolution.py` & `galpak-1.33.2/src/galpak/convolution.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/fits_sanitizer.py` & `galpak-1.33.2/src/galpak/fits_sanitizer.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/galaxy_parameter.py` & `galpak-1.33.2/src/galpak/galaxy_parameter.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/galaxy_parameters.py` & `galpak-1.33.2/src/galpak/galaxy_parameters.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/galpak3d.py` & `galpak-1.33.2/src/galpak/galpak3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,18 +246,18 @@
                 variance_cube = variance
                 if variance_cube.data is None:
                     self.logger.warning("Provided variance cube is empty.")
                 else:
                     self.logger.info("Saving variance into varianceCube")
                 if variance_cube.filename == None:
                     variance_cube.filename = 'Variance_cube_from_user'
-            elif isinstance(variance, np.float):
+            elif isinstance(variance, float):
                 variance_cube = HyperCube(variance)
                 variance_cube.filename = 'Variance_float_from_user={:.2e}'.format(variance)
-            elif not (isinstance(variance,np.float) or  isinstance(variance, HyperCube) or isinstance(variance, basestring)):
+            elif not (isinstance(variance, float) or  isinstance(variance, HyperCube) or isinstance(variance, basestring)):
                 raise TypeError("Provided variance is not a string nor HyperCube nor a float")
         else:
             variance_cube = HyperCube(self.cube.var, filename='Variance_from_cube_extension')
 
 
         # Set up the instrument's context
         if instrument is None:
@@ -1006,15 +1006,15 @@
                  ]
         chain_full = self.chain.copy()
         chain_full.add_columns(list(cols))
 
 
         #extract subchain
         chain_size = np.size(chain_full)
-        n = np.int(chain_size * last_fraction / 100.)  # number of samples (last_fraction(%) of total)
+        n = int(chain_size * last_fraction / 100.)  # number of samples (last_fraction(%) of total)
 
         idx = chain_full.argsort('reduced_chi')
         self.chain.idxsorted = idx
 
         if method_chain == 'chi_min' or method_chain == 'MAP':
             min_chi_index = self._get_min_chi_index()
             xmin = np.max([0, min_chi_index - n // 2])
```

### Comparing `galpak-1.33.1/src/galpak/galpak3d_utils.py` & `galpak-1.33.2/src/galpak/galpak3d_utils.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/hyperspectral_cube.py` & `galpak-1.33.2/src/galpak/hyperspectral_cube.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/instruments.py` & `galpak-1.33.2/src/galpak/instruments.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/math_utils.py` & `galpak-1.33.2/src/galpak/math_utils.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/mcmc.py` & `galpak-1.33.2/src/galpak/mcmc.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/model_class.py` & `galpak-1.33.2/src/galpak/model_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,65 +42,69 @@
 
     def set_cosmology(self, cosmo_string='planck15'):
         try:
             from colossus.cosmology import cosmology
             from colossus import halo
             from colossus.halo import mass_defs, mass_adv, mass_so, concentration
             self.logger.info("setting cosmology with colossus package")
-            if cosmo_string is cosmology.cosmologies.keys():
+            if cosmo_string in cosmology.cosmologies.keys():
                 cosmo=cosmology.setCosmology(cosmo_string)
             else:
                 self.logger.info("colossus: cosmology %s is not available\n "
                                  "Please use one of %s \n"
-                                 "Will be uing cosmology Planck15 as default" \
+                                 "Will be using cosmology Planck15 as default" \
                                  % (cosmo_string, cosmology.cosmologies.keys()) )
                 cosmo=cosmology.setCosmology('planck15')
+                cosmo_string = cosmo.name
             #put h in
             self.h = cosmo.h
             self.Ez = cosmo.Ez(self.redshift)
             DA = cosmo.angularDiameterDistance(self.redshift) / self.h  ####!!
             self.DeltaVir = halo.mass_so.deltaVir(self.redshift)
             self.halo = halo #Diemer Halo module for NFW halo models
         except ImportError:
             try:
-                from astLib import astCalc
-                #using  astLib for cosmology
-                self.logger.info("Using AstLib for a 737 cosmology, h,OM, OL= (0.7, 0.3, 0.7)")
-                self.h = astCalc.H0 / 100.
-                self.Ez = astCalc.Ez(self.redshift)
-                DA = astCalc.da(self.redshift)#for h=0.7
-                self.DeltaVir = astCalc.DeltaVz(self.redshift)
-                self.halo = None
-                #self.logger.warning('Best to use colossus package from Diemer& Kratsov for this module')
-            except ImportError:
-                #using astropy
+                # using astropy
                 import astropy
                 from astropy import cosmology
-                if astropy.__version__ < '5.0':
+                if astropy.__version__ < LooseVersion('5.1'):
                     cosmo_available = cosmology.parameters.available
                     cosmo_get = cosmology.default_cosmology.get_cosmology_from_string
                 else:
-                    cosmo_available = cosmology.realizations.available
+                    cosmo_available = cosmology.available
                     cosmo_get = cosmology.default_cosmology.get_cosmology_from_string
 
                 if cosmo_string in cosmo_available:
                     cosmo = cosmo_get(cosmo_string)
                 else:
                     self.logger.info("Astropy: Parameter %s is not available\n "
                                      "Please use one of %s \n"
                                      "Will be uing astropy.cosmology Planck15 as default" \
                                      % (cosmo_string, cosmo_available))
                     cosmo = cosmo_get('Planck15')
+                    cosmo_string = cosmo.name
                 self.h = cosmo.h
-                DA = cosmo.angular_diameter_distance(self.redshift).value #in Mpc
-                self.Ez = cosmo.H(self.redshift).value/cosmo.H0
-                x = cosmo.Om(self.redshift) - 1.0 #Omega_M(z) - 1.0
-                self.DeltaVir = 18 * np.pi**2 + 82 *x - 39 * x**2
+                DA = cosmo.angular_diameter_distance(self.redshift).value  # in Mpc
+                Ez = cosmo.H(self.redshift) / cosmo.H0
+                self.Ez = Ez.to_value()
+                x = cosmo.Om(self.redshift) - 1.0  # Omega_M(z) - 1.0
+                self.DeltaVir = 18 * np.pi ** 2 + 82 * x - 39 * x ** 2
                 self.halo = None
-                #self.logger.warning('Best to use colossus package from Diemer& Kratsov for this module')
+                # self.logger.warning('Best to use colossus package from Diemer& Kratsov for this module')
+            except ImportError:
+                from astLib import astCalc
+                # using  astLib for cosmology
+                self.logger.info("Using AstLib for a 737 cosmology, h,OM, OL= (0.7, 0.3, 0.7)")
+                self.h = astCalc.H0 / 100.
+                self.Ez = astCalc.Ez(self.redshift)
+                DA = astCalc.da(self.redshift)  # for h=0.7
+                self.DeltaVir = astCalc.DeltaVz(self.redshift)
+                self.halo = None
+                # self.logger.warning('Best to use colossus package from Diemer& Kratsov for this module')
+
 
         self.kpc = DA * 1e3 * np.radians(1./3600)# in unit kpc
         #self.hkpc = self.kpc * h
 
     def Parameters(self):
         """
         Returns `GalaxyParameters' instance
```

### Comparing `galpak-1.33.1/src/galpak/model_sersic3d.py` & `galpak-1.33.2/src/galpak/model_sersic3d.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/model_utilities.py` & `galpak-1.33.2/src/galpak/model_utilities.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/plot_utilities.py` & `galpak-1.33.2/src/galpak/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak/spread_functions.py` & `galpak-1.33.2/src/galpak/spread_functions.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/src/galpak.egg-info/SOURCES.txt` & `galpak-1.33.2/src/galpak.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-.gitignore
-.gitlab-ci.yml
-CHANGELOG.md
 INSTALL
 LICENCE
 MANIFEST.in
 README.md
-TODO
-dodo.py
 setup.cfg
 setup.py
-tox.ini
 data/input/ALMA_Freq_test1.fits
 data/input/ALMA_Freq_test2.fits
 data/input/ALMA_Freq_test3.fits
 data/input/GalPaK_cube_1101_from_paper.fits
 data/input/GalPaK_cube_1101_from_paper.fits~
 data/input/alma_instrument.txt
 data/input/galfit_125_seeing1.0_flux1e-16.fits
@@ -105,22 +99,12 @@
 src/galpak/mcmc.py
 src/galpak/model_class.py
 src/galpak/model_sersic3d.py
 src/galpak/model_utilities.py
 src/galpak/plot_utilities.py
 src/galpak/spread_functions.py
 src/galpak/string_stdout.py
-tests/__init__.py
-tests/benchmarks/galpak_speed.py
-tests/benchmarks/nan_to_num.py
-tests/benchmarks/power_of_three.py
-tests/benchmarks/power_of_two.py
-tests/other/galpak3d_quantuum_test.py
 tests/suite/__init__.py
 tests/suite/galaxy_parameters_test.py
 tests/suite/galpak3d_test.py
 tests/suite/hyperspectral_cube_test.py
-tests/suite/math_utils_test.py
-tests/tools/__init__.py
-tests/tools/make_animation.py
-tests/tools/numeric_assertions.py
-tests/tools/numpy_ndarray_assertions.py
+tests/suite/math_utils_test.py
```

### Comparing `galpak-1.33.1/tests/suite/galaxy_parameters_test.py` & `galpak-1.33.2/tests/suite/galaxy_parameters_test.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/tests/suite/galpak3d_test.py` & `galpak-1.33.2/tests/suite/galpak3d_test.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/tests/suite/hyperspectral_cube_test.py` & `galpak-1.33.2/tests/suite/hyperspectral_cube_test.py`

 * *Files identical despite different names*

### Comparing `galpak-1.33.1/tests/suite/math_utils_test.py` & `galpak-1.33.2/tests/suite/math_utils_test.py`

 * *Files identical despite different names*

