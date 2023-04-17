# Comparing `tmp/compoundwidgets-0.2.0.tar.gz` & `tmp/compoundwidgets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.2.0.tar", last modified: Wed Apr 12 14:10:19 2023, max compression
+gzip compressed data, was "compoundwidgets-0.2.1.tar", last modified: Sun Apr 16 17:39:11 2023, max compression
```

## Comparing `compoundwidgets-0.2.0.tar` & `compoundwidgets-0.2.1.tar`

### file list

```diff
@@ -1,1002 +1,1002 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      673 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.419089 compoundwidgets-0.2.0/compoundwidgets/
--rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    51971 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    16269 2023-04-07 22:03:31.000000 compoundwidgets-0.2.0/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.498763 compoundwidgets-0.2.0/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.0/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.0/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.0/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1843 2023-04-12 10:28:05.000000 compoundwidgets-0.2.0/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.451516 compoundwidgets-0.2.0/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    49571 2023-04-12 14:10:10.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 14:10:09.000000 compoundwidgets-0.2.0/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-04-05 20:13:41.000000 compoundwidgets-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.578957 compoundwidgets-0.2.0/test/
--rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.0/test/autocomplete_widget_test.py
--rw-rw-rw-   0        0        0    10106 2023-04-07 11:48:52.000000 compoundwidgets-0.2.0/test/compound_widgets_test_1.py
--rw-rw-rw-   0        0        0     7285 2023-04-07 19:05:00.000000 compoundwidgets-0.2.0/test/compound_widgets_test_2.py
--rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.0/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.0/test/custom_frames_test_1.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.0/test/custom_frames_test_2.py
--rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.0/test/custom_frames_test_3.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.0/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.0/test/message_box_test.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.344025 compoundwidgets-0.2.0/venv/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.271765 compoundwidgets-0.2.0/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:10.593930 compoundwidgets-0.2.0/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.609021 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/
--rw-rw-rw-   0        0        0     3359 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BdfFontFile.py
--rw-rw-rw-   0        0        0    16483 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BlpImagePlugin.py
--rw-rw-rw-   0        0        0    18138 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BmpImagePlugin.py
--rw-rw-rw-   0        0        0     1629 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
--rw-rw-rw-   0        0        0     3003 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ContainerIO.py
--rw-rw-rw-   0        0        0     1796 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/CurImagePlugin.py
--rw-rw-rw-   0        0        0     2037 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DcxImagePlugin.py
--rw-rw-rw-   0        0        0     9637 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DdsImagePlugin.py
--rw-rw-rw-   0        0        0    15413 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/EpsImagePlugin.py
--rw-rw-rw-   0        0        0    10098 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ExifTags.py
--rw-rw-rw-   0        0        0     2132 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsImagePlugin.py
--rw-rw-rw-   0        0        0     1749 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py
--rw-rw-rw-   0        0        0     4614 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FliImagePlugin.py
--rw-rw-rw-   0        0        0     2874 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FontFile.py
--rw-rw-rw-   0        0        0     7214 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FpxImagePlugin.py
--rw-rw-rw-   0        0        0     3980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FtexImagePlugin.py
--rw-rw-rw-   0        0        0     3010 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GbrImagePlugin.py
--rw-rw-rw-   0        0        0     2704 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GdImageFile.py
--rw-rw-rw-   0        0        0    36797 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GifImagePlugin.py
--rw-rw-rw-   0        0        0     3533 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpGradientFile.py
--rw-rw-rw-   0        0        0     1401 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpPaletteFile.py
--rw-rw-rw-   0        0        0     1623 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
--rw-rw-rw-   0        0        0     1626 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
--rw-rw-rw-   0        0        0    12329 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
--rw-rw-rw-   0        0        0    11980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcoImagePlugin.py
--rw-rw-rw-   0        0        0    11238 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImImagePlugin.py
--rw-rw-rw-   0        0        0   137510 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Image.py
--rw-rw-rw-   0        0        0     7306 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageChops.py
--rw-rw-rw-   0        0        0    38772 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageCms.py
--rw-rw-rw-   0        0        0     9097 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageColor.py
--rw-rw-rw-   0        0        0    39813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw.py
--rw-rw-rw-   0        0        0     6210 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw2.py
--rw-rw-rw-   0        0        0     3293 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageEnhance.py
--rw-rw-rw-   0        0        0    24312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFile.py
--rw-rw-rw-   0        0        0    17019 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFilter.py
--rw-rw-rw-   0        0        0    51659 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFont.py
--rw-rw-rw-   0        0        0     4834 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageGrab.py
--rw-rw-rw-   0        0        0     7620 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMath.py
--rw-rw-rw-   0        0        0     3004 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMode.py
--rw-rw-rw-   0        0        0     8231 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMorph.py
--rw-rw-rw-   0        0        0    21590 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageOps.py
--rw-rw-rw-   0        0        0     8421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImagePalette.py
--rw-rw-rw-   0        0        0      355 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImagePath.py
--rw-rw-rw-   0        0        0     7119 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageQt.py
--rw-rw-rw-   0        0        0     1948 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageSequence.py
--rw-rw-rw-   0        0        0    11813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageShow.py
--rw-rw-rw-   0        0        0     4072 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageStat.py
--rw-rw-rw-   0        0        0     8988 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTk.py
--rw-rw-rw-   0        0        0     2985 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTransform.py
--rw-rw-rw-   0        0        0     7421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageWin.py
--rw-rw-rw-   0        0        0     2680 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImtImagePlugin.py
--rw-rw-rw-   0        0        0     6007 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IptcImagePlugin.py
--rw-rw-rw-   0        0        0    11982 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
--rw-rw-rw-   0        0        0    30012 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegImagePlugin.py
--rw-rw-rw-   0        0        0    12583 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegPresets.py
--rw-rw-rw-   0        0        0     1871 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
--rw-rw-rw-   0        0        0     2699 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MicImagePlugin.py
--rw-rw-rw-   0        0        0     1905 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpegImagePlugin.py
--rw-rw-rw-   0        0        0     6486 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpoImagePlugin.py
--rw-rw-rw-   0        0        0     5806 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MspImagePlugin.py
--rw-rw-rw-   0        0        0     6754 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PSDraw.py
--rw-rw-rw-   0        0        0     1179 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PaletteFile.py
--rw-rw-rw-   0        0        0     9369 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PalmImagePlugin.py
--rw-rw-rw-   0        0        0     1558 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcdImagePlugin.py
--rw-rw-rw-   0        0        0     7013 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcfFontFile.py
--rw-rw-rw-   0        0        0     6242 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcxImagePlugin.py
--rw-rw-rw-   0        0        0     9264 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfImagePlugin.py
--rw-rw-rw-   0        0        0    35563 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfParser.py
--rw-rw-rw-   0        0        0     1720 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PixarImagePlugin.py
--rw-rw-rw-   0        0        0    48199 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PngImagePlugin.py
--rw-rw-rw-   0        0        0    11746 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PpmImagePlugin.py
--rw-rw-rw-   0        0        0     7838 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PsdImagePlugin.py
--rw-rw-rw-   0        0        0    10189 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PyAccess.py
--rw-rw-rw-   0        0        0     3722 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/QoiImagePlugin.py
--rw-rw-rw-   0        0        0     6409 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SgiImagePlugin.py
--rw-rw-rw-   0        0        0     9792 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
--rw-rw-rw-   0        0        0     4537 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SunImagePlugin.py
--rw-rw-rw-   0        0        0     1557 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TarIO.py
--rw-rw-rw-   0        0        0     6830 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TgaImagePlugin.py
--rw-rw-rw-   0        0        0    79211 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffImagePlugin.py
--rw-rw-rw-   0        0        0    17374 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffTags.py
--rw-rw-rw-   0        0        0     5642 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WalImageFile.py
--rw-rw-rw-   0        0        0    11732 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WebPImagePlugin.py
--rw-rw-rw-   0        0        0     4867 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WmfImagePlugin.py
--rw-rw-rw-   0        0        0     2064 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
--rw-rw-rw-   0        0        0     2581 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XbmImagePlugin.py
--rw-rw-rw-   0        0        0     3312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XpmImagePlugin.py
--rw-rw-rw-   0        0        0     2091 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/__init__.py
--rw-rw-rw-   0        0        0       44 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/__main__.py
--rw-rw-rw-   0        0        0     2145 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_binary.py
--rw-rw-rw-   0        0        0     2071 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_deprecate.py
--rw-rw-rw-   0        0        0      691 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_tkinter_finder.py
--rw-rw-rw-   0        0        0      388 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_util.py
--rw-rw-rw-   0        0        0       52 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_version.py
--rw-rw-rw-   0        0        0     9949 2023-04-07 11:46:18.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/features.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.625652 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/override.py
--rw-rw-rw-   0        0        0     5770 2023-04-07 11:44:14.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/_virtualenv.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.673007 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.755008 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0    10734 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:11.880531 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     7842 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    29497 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2472 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10817 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18172 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.070182 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1685 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4129 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5289 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4793 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3188 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    32389 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12343 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3886 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     7396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13529 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.117629 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6494 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    24244 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.149931 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16504 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37873 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.197270 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    15365 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6100 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7680 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2556 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.247967 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4280 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25277 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.295480 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      107 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7457 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0     9773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.410268 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     6626 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2617 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    18602 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.490791 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.522600 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.599169 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1422 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1474 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1075 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9784 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.630510 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0     4105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-rw-   0        0        0    27407 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    25091 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     6987 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.708947 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2807 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17646 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    35763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     2858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24045 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.724575 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.724575 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:12.823294 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18963 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    27878 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9914 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     2526 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5455 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    11533 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8167 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.106217 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     5764 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     1115 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-rw-   0        0        0     2118 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     4831 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    22253 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     5662 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7702 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3456 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.169236 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3519 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18116 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5238 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    13079 2023-04-07 11:44:45.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.202489 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4966 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.315895 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      465 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1379 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     5033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1535 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.348855 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      778 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    16416 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     3946 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4154 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.377966 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.821486 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     4797 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0    10032 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3915 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     5420 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.837614 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3732 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0      542 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-rw-   0        0        0     1860 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1683 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     4006 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3934 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    14537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1752 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    27055 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5380 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     6077 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-rw-   0        0        0     3715 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.849574 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0      402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-rw-   0        0        0     6400 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4137 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     4007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    14848 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8505 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2812 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      244 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.900821 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      266 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    11128 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     3325 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:13.964020 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/
--rw-rw-rw-   0        0        0       75 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-rw-   0        0        0    10678 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-rw-   0        0        0     6741 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-rw-   0        0        0     1866 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-rw-   0        0        0     1079 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-rw-   0        0        0     3709 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-rw-   0        0        0     6181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     7134 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.120653 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.152296 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    49330 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.249930 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.282126 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6080 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.396538 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.427996 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   108287 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.523467 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0      160 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.697254 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2999 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.697254 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.850582 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     4810 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35441 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     5871 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    32005 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.888897 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    11174 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    70232 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     4630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:14.888897 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.015125 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9171 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213344 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.030673 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.051041 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-rw-   0        0        0      491 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-rw-   0        0        0    11920 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.062621 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-rw-   0        0        0      546 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-rw-   0        0        0    10927 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.251459 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5178 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33240 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.282668 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:15.301380 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5872 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    17592 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4794 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.052673 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     6090 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8478 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0     9695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     1643 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6819 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9842 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4503 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    18015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    97992 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     7954 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1616 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9585 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5053 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14172 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11903 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    37414 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59836 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4436 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2843 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24224 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    26332 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    34995 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39684 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45686 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3627 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    26070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.138889 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    18364 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     1944 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1496 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     1908 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     7550 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     2790 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8011 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.170688 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    80114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.281865 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39095 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.331805 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.364259 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11036 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.383790 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.383790 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30641 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.525568 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14298 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.588990 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-04-07 11:44:47.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.605334 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   109315 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.620338 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.715142 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.762660 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.778300 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.828811 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0      148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   133344 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    22975 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.955254 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:16.986632 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12806 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0      160 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-rw-rw-   0        0        0    80078 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.002940 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2442 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.301892 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     9170 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.655795 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      359 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     5300 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0       43 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_log.py
--rw-rw-rw-   0        0        0      239 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    19616 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8572 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14721 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    48643 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17861 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.920236 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      430 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5408 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4665 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    22013 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     5584 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7684 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31503 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16537 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5604 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4872 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2594 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13077 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2762 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2788 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1180 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8409 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1932 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11817 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7491 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9397 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    11924 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3414 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8072 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50174 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10270 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17899 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8212 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13715 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1201 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30188 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23577 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      217 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3495 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18928 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12085 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15601 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18099 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12951 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5205 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     2282 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0     3722 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_normalization.py
--rw-rw-rw-   0        0        0     1056 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      882 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:17.956185 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.046759 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    26498 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1859 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1165 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     1098 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-rw-rw-   0        0        0     2166 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.093020 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.108775 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.124312 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.156522 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.234813 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.259929 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    19612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.527830 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     6589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4423 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    15821 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    14115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     6963 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     4074 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    31903 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-rw-rw-   0        0        0    28176 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2123 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2714 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     7071 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8102 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7470 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.575295 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13816 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.657358 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   274907 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     9161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16319 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19598 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    21087 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45710 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5591 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.670677 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2527 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     5063 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     4697 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    47115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    39682 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      134 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8608 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2023-04-07 11:44:56.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.843071 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/
--rw-rw-rw-   0        0        0      396 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/__init__.py
--rw-rw-rw-   0        0        0     8926 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/__main__.py
--rw-rw-rw-   0        0        0     5255 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/colorutils.py
--rw-rw-rw-   0        0        0      775 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.894710 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/
--rw-rw-rw-   0        0        0       42 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/__init__.py
--rw-rw-rw-   0        0        0    22700 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py
--rw-rw-rw-   0        0        0     6885 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py
--rw-rw-rw-   0        0        0    64245 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py
--rw-rw-rw-   0        0        0   118811 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/icons.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.925957 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/
--rw-rw-rw-   0        0        0      675 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/__init__.py
--rw-rw-rw-   0        0        0     5594 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py
--rw-rw-rw-   0        0        0    15106 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgs.py
--rw-rw-rw-   0        0        0     2879 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/publisher.py
--rw-rw-rw-   0        0        0    15839 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/scrolled.py
--rw-rw-rw-   0        0        0   172335 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/style.py
--rw-rw-rw-   0        0        0    92575 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tableview.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.942245 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/__init__.py
--rw-rw-rw-   0        0        0    11286 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/standard.py
--rw-rw-rw-   0        0        0       14 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/user.py
--rw-rw-rw-   0        0        0     8389 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/toast.py
--rw-rw-rw-   0        0        0     5139 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tooltip.py
--rw-rw-rw-   0        0        0     3555 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/utility.py
--rw-rw-rw-   0        0        0    10200 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/validation.py
--rw-rw-rw-   0        0        0    40690 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/widgets.py
--rw-rw-rw-   0        0        0    18186 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/window.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:18.957748 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/__init__.py
--rw-rw-rw-   0        0        0    17276 2023-04-07 11:46:20.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.020532 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/
--rw-rw-rw-   0        0        0       59 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/__init__.py
--rw-rw-rw-   0        0        0      455 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/__main__.py
--rw-rw-rw-   0        0        0      746 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/_setuptools_logging.py
--rw-rw-rw-   0        0        0    19868 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/bdist_wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.084426 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/
--rw-rw-rw-   0        0        0     3932 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-rw-rw-   0        0        0     9427 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/convert.py
--rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/pack.py
--rw-rw-rw-   0        0        0     5124 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/tags.py
--rw-rw-rw-   0        0        0     1021 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-rw-rw-   0        0        0    16143 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-rw-rw-   0        0        0     5889 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/metadata.py
--rw-rw-rw-   0        0        0      621 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.084426 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.158208 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/
--rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_elffile.py
--rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_parser.py
--rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_structures.py
--rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/markers.py
--rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/requirements.py
--rw-rw-rw-   0        0        0    39047 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/specifiers.py
--rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/utils.py
--rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/version.py
--rw-rw-rw-   0        0        0     7674 2023-04-07 11:44:41.000000 compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/wheelfile.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:10:19.164003 compoundwidgets-0.2.0/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:20.000000 compoundwidgets-0.2.0/venv/Scripts/activate_this.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.354898 compoundwidgets-0.2.1/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-16 17:39:11.339336 compoundwidgets-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.174351 compoundwidgets-0.2.1/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.1/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    52425 2023-04-16 17:38:57.000000 compoundwidgets-0.2.1/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.1/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16404 2023-04-16 17:35:39.000000 compoundwidgets-0.2.1/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.252866 compoundwidgets-0.2.1/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.1/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.1/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.1/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.1/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-16 17:38:57.000000 compoundwidgets-0.2.1/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.206061 compoundwidgets-0.2.1/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-16 17:39:01.000000 compoundwidgets-0.2.1/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    49571 2023-04-16 17:39:02.000000 compoundwidgets-0.2.1/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 17:39:01.000000 compoundwidgets-0.2.1/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 17:39:01.000000 compoundwidgets-0.2.1/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-16 17:39:01.000000 compoundwidgets-0.2.1/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 17:39:11.354898 compoundwidgets-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-16 17:38:57.000000 compoundwidgets-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.316103 compoundwidgets-0.2.1/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.1/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10106 2023-04-07 11:48:52.000000 compoundwidgets-0.2.1/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7285 2023-04-07 19:05:00.000000 compoundwidgets-0.2.1/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.1/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.1/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.1/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.1/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.1/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.1/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.125886 compoundwidgets-0.2.1/venv/
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.061901 compoundwidgets-0.2.1/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:02.332538 compoundwidgets-0.2.1/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.440589 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/
+-rw-rw-rw-   0        0        0     3359 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BdfFontFile.py
+-rw-rw-rw-   0        0        0    16483 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BlpImagePlugin.py
+-rw-rw-rw-   0        0        0    18138 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BmpImagePlugin.py
+-rw-rw-rw-   0        0        0     1629 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
+-rw-rw-rw-   0        0        0     3003 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ContainerIO.py
+-rw-rw-rw-   0        0        0     1796 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/CurImagePlugin.py
+-rw-rw-rw-   0        0        0     2037 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/DcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9637 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/DdsImagePlugin.py
+-rw-rw-rw-   0        0        0    15413 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/EpsImagePlugin.py
+-rw-rw-rw-   0        0        0    10098 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ExifTags.py
+-rw-rw-rw-   0        0        0     2132 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FitsImagePlugin.py
+-rw-rw-rw-   0        0        0     1749 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py
+-rw-rw-rw-   0        0        0     4614 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FliImagePlugin.py
+-rw-rw-rw-   0        0        0     2874 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FontFile.py
+-rw-rw-rw-   0        0        0     7214 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FpxImagePlugin.py
+-rw-rw-rw-   0        0        0     3980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FtexImagePlugin.py
+-rw-rw-rw-   0        0        0     3010 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GbrImagePlugin.py
+-rw-rw-rw-   0        0        0     2704 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GdImageFile.py
+-rw-rw-rw-   0        0        0    36797 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GifImagePlugin.py
+-rw-rw-rw-   0        0        0     3533 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GimpGradientFile.py
+-rw-rw-rw-   0        0        0     1401 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GimpPaletteFile.py
+-rw-rw-rw-   0        0        0     1623 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
+-rw-rw-rw-   0        0        0     1626 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
+-rw-rw-rw-   0        0        0    12329 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
+-rw-rw-rw-   0        0        0    11980 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IcoImagePlugin.py
+-rw-rw-rw-   0        0        0    11238 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImImagePlugin.py
+-rw-rw-rw-   0        0        0   137510 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Image.py
+-rw-rw-rw-   0        0        0     7306 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageChops.py
+-rw-rw-rw-   0        0        0    38772 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageCms.py
+-rw-rw-rw-   0        0        0     9097 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageColor.py
+-rw-rw-rw-   0        0        0    39813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageDraw.py
+-rw-rw-rw-   0        0        0     6210 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageDraw2.py
+-rw-rw-rw-   0        0        0     3293 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageEnhance.py
+-rw-rw-rw-   0        0        0    24312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFile.py
+-rw-rw-rw-   0        0        0    17019 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFilter.py
+-rw-rw-rw-   0        0        0    51659 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFont.py
+-rw-rw-rw-   0        0        0     4834 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageGrab.py
+-rw-rw-rw-   0        0        0     7620 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMath.py
+-rw-rw-rw-   0        0        0     3004 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMode.py
+-rw-rw-rw-   0        0        0     8231 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMorph.py
+-rw-rw-rw-   0        0        0    21590 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageOps.py
+-rw-rw-rw-   0        0        0     8421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImagePalette.py
+-rw-rw-rw-   0        0        0      355 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImagePath.py
+-rw-rw-rw-   0        0        0     7119 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageQt.py
+-rw-rw-rw-   0        0        0     1948 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageSequence.py
+-rw-rw-rw-   0        0        0    11813 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageShow.py
+-rw-rw-rw-   0        0        0     4072 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageStat.py
+-rw-rw-rw-   0        0        0     8988 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageTk.py
+-rw-rw-rw-   0        0        0     2985 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageTransform.py
+-rw-rw-rw-   0        0        0     7421 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageWin.py
+-rw-rw-rw-   0        0        0     2680 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImtImagePlugin.py
+-rw-rw-rw-   0        0        0     6007 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IptcImagePlugin.py
+-rw-rw-rw-   0        0        0    11982 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
+-rw-rw-rw-   0        0        0    30012 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/JpegImagePlugin.py
+-rw-rw-rw-   0        0        0    12583 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/JpegPresets.py
+-rw-rw-rw-   0        0        0     1871 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
+-rw-rw-rw-   0        0        0     2699 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MicImagePlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MpegImagePlugin.py
+-rw-rw-rw-   0        0        0     6486 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MpoImagePlugin.py
+-rw-rw-rw-   0        0        0     5806 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MspImagePlugin.py
+-rw-rw-rw-   0        0        0     6754 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PSDraw.py
+-rw-rw-rw-   0        0        0     1179 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PaletteFile.py
+-rw-rw-rw-   0        0        0     9369 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PalmImagePlugin.py
+-rw-rw-rw-   0        0        0     1558 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcdImagePlugin.py
+-rw-rw-rw-   0        0        0     7013 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcfFontFile.py
+-rw-rw-rw-   0        0        0     6242 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9264 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PdfImagePlugin.py
+-rw-rw-rw-   0        0        0    35563 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PdfParser.py
+-rw-rw-rw-   0        0        0     1720 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PixarImagePlugin.py
+-rw-rw-rw-   0        0        0    48199 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PngImagePlugin.py
+-rw-rw-rw-   0        0        0    11746 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PpmImagePlugin.py
+-rw-rw-rw-   0        0        0     7838 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PsdImagePlugin.py
+-rw-rw-rw-   0        0        0    10189 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PyAccess.py
+-rw-rw-rw-   0        0        0     3722 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/QoiImagePlugin.py
+-rw-rw-rw-   0        0        0     6409 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SgiImagePlugin.py
+-rw-rw-rw-   0        0        0     9792 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
+-rw-rw-rw-   0        0        0     4537 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SunImagePlugin.py
+-rw-rw-rw-   0        0        0     1557 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TarIO.py
+-rw-rw-rw-   0        0        0     6830 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TgaImagePlugin.py
+-rw-rw-rw-   0        0        0    79211 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TiffImagePlugin.py
+-rw-rw-rw-   0        0        0    17374 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TiffTags.py
+-rw-rw-rw-   0        0        0     5642 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WalImageFile.py
+-rw-rw-rw-   0        0        0    11732 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WebPImagePlugin.py
+-rw-rw-rw-   0        0        0     4867 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WmfImagePlugin.py
+-rw-rw-rw-   0        0        0     2064 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
+-rw-rw-rw-   0        0        0     2581 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XbmImagePlugin.py
+-rw-rw-rw-   0        0        0     3312 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XpmImagePlugin.py
+-rw-rw-rw-   0        0        0     2091 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/__main__.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_binary.py
+-rw-rw-rw-   0        0        0     2071 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_deprecate.py
+-rw-rw-rw-   0        0        0      691 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_tkinter_finder.py
+-rw-rw-rw-   0        0        0      388 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_util.py
+-rw-rw-rw-   0        0        0       52 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_version.py
+-rw-rw-rw-   0        0        0     9949 2023-04-07 11:46:18.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/features.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.455687 compoundwidgets-0.2.1/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-rw-rw-   0        0        0     5770 2023-04-07 11:44:14.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/_virtualenv.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.487223 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.590937 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0    10734 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.716454 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     7842 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    29497 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18172 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.889594 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1685 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5289 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4793 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    32389 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     7396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:03.952902 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    24244 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.000469 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16504 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37873 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.055895 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.087080 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.121022 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.229081 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6626 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2617 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18602 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.322885 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    16507 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.369823 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.432659 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9784 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.463911 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0     4105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-rw-   0        0        0    27407 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    25091 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     6987 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.527046 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2807 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17646 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    35763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24045 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.542591 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.562188 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.629924 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18963 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27878 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9914 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     2526 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5455 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11533 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8167 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.898477 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     5764 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     1115 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-rw-   0        0        0     2118 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     4831 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    22253 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     5662 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.961607 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    13079 2023-04-07 11:44:45.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:04.994096 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.125419 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.156846 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.189432 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.674987 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.684512 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.700145 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.747647 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.811402 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.937212 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:05.975614 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.063838 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.120292 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6080 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34557 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.213947 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.245202 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108287 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.340244 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1176 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.501751 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.514771 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.673431 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4810 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35441 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     5871 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32005 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.698696 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11174 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    70232 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     4630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.713907 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.840030 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.840030 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.876879 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:06.887402 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:07.076810 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:07.129588 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:07.130983 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5872 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1583 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    17592 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4794 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:07.958738 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0     9695 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1643 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6819 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4503 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18015 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    97992 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     7954 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1616 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9585 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5053 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14172 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    37414 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59836 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4436 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4773 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24224 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4374 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    26332 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    34995 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45686 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3627 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    26070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.084840 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    18364 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     1944 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1496 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1376 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     1908 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     7550 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     2790 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2145 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8011 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.132588 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    80114 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.250783 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20070 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39095 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.330001 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.408301 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.423900 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.439619 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.612297 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10003 2023-04-07 11:44:46.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14298 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.668559 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-04-07 11:44:47.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.685564 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   109315 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.700574 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.794709 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.826548 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.843068 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:08.905548 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0      148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   133344 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    22975 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:09.046569 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:09.094228 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12806 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-rw-rw-   0        0        0    80078 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:09.110520 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2442 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:09.380467 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     9170 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:09.758580 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      359 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0       43 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_log.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19616 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8572 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14721 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    48643 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17861 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.089715 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5408 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4665 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22013 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5584 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7684 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31503 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16537 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5604 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4872 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2594 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13077 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2762 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2788 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1180 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8409 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1932 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11817 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7491 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4911 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9397 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    11924 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3414 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8072 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50174 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17899 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8212 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13715 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1201 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30188 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23577 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3495 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18928 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12085 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15601 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18099 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12951 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5205 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     2282 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0     3722 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_normalization.py
+-rw-rw-rw-   0        0        0     1056 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      882 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.151892 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.239687 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    26498 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1859 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1165 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     1098 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-rw-rw-   0        0        0     2166 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.286479 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.286479 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.318603 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.333550 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.428749 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39046 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.460993 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.696999 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16596 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6589 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4423 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     6963 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4074 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31903 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    28176 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2123 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2714 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7470 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.752158 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13816 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.831426 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   274907 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     9161 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19598 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25431 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    21087 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45710 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:10.847680 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2527 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     5063 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1232 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4697 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47115 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    39682 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      134 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8608 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-04-07 11:44:56.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.051438 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/
+-rw-rw-rw-   0        0        0      396 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/__init__.py
+-rw-rw-rw-   0        0        0     8926 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/__main__.py
+-rw-rw-rw-   0        0        0     5255 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/colorutils.py
+-rw-rw-rw-   0        0        0      775 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.082577 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/
+-rw-rw-rw-   0        0        0       42 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/__init__.py
+-rw-rw-rw-   0        0        0    22700 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py
+-rw-rw-rw-   0        0        0     6885 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py
+-rw-rw-rw-   0        0        0    64245 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py
+-rw-rw-rw-   0        0        0   118811 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/icons.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.113830 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/
+-rw-rw-rw-   0        0        0      675 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/__init__.py
+-rw-rw-rw-   0        0        0     5594 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py
+-rw-rw-rw-   0        0        0    15106 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/msgs.py
+-rw-rw-rw-   0        0        0     2879 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/publisher.py
+-rw-rw-rw-   0        0        0    15839 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/scrolled.py
+-rw-rw-rw-   0        0        0   172335 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/style.py
+-rw-rw-rw-   0        0        0    92575 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/tableview.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.145931 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/themes/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/themes/__init__.py
+-rw-rw-rw-   0        0        0    11286 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/themes/standard.py
+-rw-rw-rw-   0        0        0       14 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/themes/user.py
+-rw-rw-rw-   0        0        0     8389 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/toast.py
+-rw-rw-rw-   0        0        0     5139 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/tooltip.py
+-rw-rw-rw-   0        0        0     3555 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/utility.py
+-rw-rw-rw-   0        0        0    10200 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/validation.py
+-rw-rw-rw-   0        0        0    40690 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/widgets.py
+-rw-rw-rw-   0        0        0    18186 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/window.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.145931 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkcreator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkcreator/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-04-07 11:46:20.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/ttkcreator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.224417 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/
+-rw-rw-rw-   0        0        0       59 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/__main__.py
+-rw-rw-rw-   0        0        0      746 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/_setuptools_logging.py
+-rw-rw-rw-   0        0        0    19868 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/bdist_wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.261135 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/
+-rw-rw-rw-   0        0        0     3932 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-rw-rw-   0        0        0     9427 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-rw-rw-   0        0        0     4338 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-rw-rw-   0        0        0     5124 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/tags.py
+-rw-rw-rw-   0        0        0     1021 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-rw-rw-   0        0        0    16143 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-rw-rw-   0        0        0     5889 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/metadata.py
+-rw-rw-rw-   0        0        0      621 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/util.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.261135 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.339336 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/
+-rw-rw-rw-   0        0        0        0 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8813 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     9399 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5148 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8161 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/markers.py
+-rw-rw-rw-   0        0        0     3264 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39047 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18065 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/utils.py
+-rw-rw-rw-   0        0        0    16295 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/version.py
+-rw-rw-rw-   0        0        0     7674 2023-04-07 11:44:41.000000 compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/wheelfile.py
+drwxrwxrwx   0        0        0        0 2023-04-16 17:39:11.339336 compoundwidgets-0.2.1/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-04-07 11:44:20.000000 compoundwidgets-0.2.1/venv/Scripts/activate_this.py
```

### Comparing `compoundwidgets-0.2.0/LICENSE.txt` & `compoundwidgets-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/MANIFEST.in` & `compoundwidgets-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/README.md` & `compoundwidgets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.2.1/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.1/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         font: font to be used for the label
     Methods for the user:
         set(value): sets a value to the combobox widget
         get(): gets the current value from the combobox widget
         disable(): turns the whole widget 'off'
         enable(): turns the whole widget 'on'
         readonly(): turn the whole widget 'readonly' (non-editable)
+        set_combo_values(values): sets the combobox values after it has been created
     """
 
     def __init__(self, parent,
                  label_text='Label:', label_anchor='e', label_width=None,
                  combo_value='', combo_list=('No values informed',), combo_width=None,
                  combo_method=None, font=None):
 
@@ -83,14 +84,18 @@
         if str(self.combobox.cget('state')) == 'disabled':
             return
         if value in self.combo_list:
             self.variable.set(value)
         else:
             self.variable.set('')
 
+    def set_combo_values(self, values):
+        self.combo_list = values
+        self.combobox.config(values=values)
+
 
 class LabelEntry (ttk.Frame):
     """
     Create a compound widget, with a label and an entry field within a frame.
     Parameters:
         parent: parent widget
         label_text: label text value
@@ -565,16 +570,16 @@
     Internal Classes:
         NoUnitCombo: ('-')
         TemperatureCombo: ('°C', '°F')
         LengthCombo: ('mm', 'cm', 'in')
         AreaCombo: ('mm²', 'cm²', 'in²')
         PressureCombo: ('kPa', 'bar', 'kgf/cm²', 'MPa', 'atmosphere', 'ksi', 'psi')
         StressCombo: ('MPa', 'GPa', 'x10³ ksi', 'psi', 'ksi')
-        ForceCombo: ('N', 'kgf', 'lbf')
-        MomentCombo: ('N.m', 'kgf.m', 'lbf.ft')
+        ForceCombo: ('N', 'kN', 'kgf', 'lbf')
+        MomentCombo: ('N.m', 'kN.m', 'kgf.m', 'lbf.ft')
         EnergyCombo: ('joule', 'ft-lbf')
         ToughnessCombo: ('MPa.√m', 'N/mm^(3/2)', 'ksi.√in')
         JIntegralCombo: ('joule/m²', 'ft-lbf/ft²')
     """
 
     class NoUnitCombo(ttk.Combobox):
         def __init__(self, parent, width):
@@ -637,26 +642,26 @@
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class ForceCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
-            self.values = ('N', 'kgf', 'lbf')
-            self.conversion_values = (1, 9.80665, 4.448222)
+            self.values = ('N', 'kN', 'kgf', 'lbf')
+            self.conversion_values = (1, 1000, 9.80665, 4.448222)
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class MomentCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
-            self.values = ('N.m', 'kgf.m', 'lbf.ft')
-            self.conversion_values = (1, 9.80665, 1.35582)
+            self.values = ('N.m', 'kN.m', 'kgf.m', 'lbf.ft')
+            self.conversion_values = (1, 1000, 9.80665, 1.35582)
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     class EnergyCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
@@ -1261,14 +1266,15 @@
         font: font to be used for the label, the entry and the button
     Methods for the user:
         set(value): sets a value to the entry widget
         get(): gets the current value from the entry widget
         disable(): turns the whole widget 'off'
         enable(): turns the whole widget 'on'
         readonly(): turn the whole widget 'readonly' (non-editable)
+        set_combo_values(values): sets the combobox values after it has been created
     """
 
     def __init__(self, parent,
                  label_text='Label:', label_anchor='e', label_width=None,
                  combo_value='', combo_list=('No values informed',), combo_width=None, combo_method=None,
                  button_text='', button_width=None, button_method=None,
                  font=None):
@@ -1337,7 +1343,11 @@
     def set(self, value):
         if str(self.combobox.cget('state')) == 'disabled':
             return
         if value in self.combo_list:
             self.variable.set(value)
         else:
             self.variable.set('')
+
+    def set_combo_values(self, values):
+        self.combo_list = values
+        self.combobox.config(values=values)
```

### Comparing `compoundwidgets-0.2.0/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.1/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.2.1/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         for method in _methods:
             if "grid" in method:
                 # prefix content frame methods with 'content_'
                 setattr(self, f"content_{method}", getattr(self, method))
                 # overwrite content frame methods from container frame
                 setattr(self, method, getattr(self.container, method))
 
+        self.bind("<Configure>", lambda _: parent.yview())
+
         # Collapsed start adjust
         if not open_start:
             self.collapse_frame()
 
         # Status flag: disabled / enabled
         if disabled:
             self.collapse_frame()
@@ -285,27 +287,28 @@
 
 
 class ScrollableFrame(ttk.Frame):
     """
     Creates a frame with a vertical scrollbar.
     Parameters:
         parent: container for the frame
+        style: bootstyle (color style)
     """
 
-    def __init__(self, master=None, **kwargs):
+    def __init__(self, master=None, style='TFrame', **kwargs):
 
         # content frame container
         self.container = ttk.Frame(master)
         self.container.bind("<Configure>", lambda _: self.yview())
         self.container.rowconfigure(0, weight=1)
         self.container.columnconfigure(0, weight=1)
         self.container.columnconfigure(1, weight=0)
 
         # content frame
-        super().__init__(self.container, **kwargs)
+        super().__init__(self.container, bootstyle=style, **kwargs)
         self.place(rely=0.0, relwidth=1.0)
 
         # vertical scrollbar
         self.vscroll = ttk.Scrollbar(self.container, command=self.yview, orient='vertical')
         self.vscroll.pack(side='right', fill='y')
 
         # widget event binding
```

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.2.1/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.2.1/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.1/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.2.1/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/compoundwidgets/__init__.py` & `compoundwidgets-0.2.1/compoundwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.00"
+__version__ = "0.2.01"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.2.0/compoundwidgets.egg-info/SOURCES.txt` & `compoundwidgets-0.2.1/compoundwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/setup.py` & `compoundwidgets-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.2.00',
+    version='0.2.01',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.2.0/test/autocomplete_widget_test.py` & `compoundwidgets-0.2.1/test/autocomplete_widget_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/compound_widgets_test_1.py` & `compoundwidgets-0.2.1/test/compound_widgets_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/compound_widgets_test_2.py` & `compoundwidgets-0.2.1/test/compound_widgets_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/custom_buttons_test.py` & `compoundwidgets-0.2.1/test/custom_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/custom_frames_test_1.py` & `compoundwidgets-0.2.1/test/custom_frames_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/custom_frames_test_2.py` & `compoundwidgets-0.2.1/test/custom_frames_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/custom_frames_test_3.py` & `compoundwidgets-0.2.1/test/custom_frames_test_3.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/led_buttons_test.py` & `compoundwidgets-0.2.1/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/test/message_box_test.py` & `compoundwidgets-0.2.1/test/message_box_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BdfFontFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BdfFontFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BlpImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BlpImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BmpImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BmpImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ContainerIO.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ContainerIO.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/CurImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/CurImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DcxImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/DcxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/DdsImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/DdsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/EpsImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/EpsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ExifTags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ExifTags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FitsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FliImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FliImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FontFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FontFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FpxImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FpxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/FtexImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/FtexImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GbrImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GbrImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GdImageFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GdImageFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GifImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GifImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpGradientFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GimpGradientFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GimpPaletteFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GimpPaletteFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/GribStubImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/GribStubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcnsImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IcnsImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IcoImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IcoImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Image.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Image.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageChops.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageChops.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageCms.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageCms.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageColor.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageColor.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageDraw.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageDraw2.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageDraw2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageEnhance.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageEnhance.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFilter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFilter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageFont.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageFont.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageGrab.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageGrab.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMath.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMath.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMode.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMode.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageMorph.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageMorph.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageOps.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageOps.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImagePalette.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImagePalette.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageQt.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageQt.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageSequence.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageSequence.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageShow.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageShow.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageStat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageStat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTk.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageTk.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageTransform.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageTransform.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImageWin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImageWin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/ImtImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/ImtImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/IptcImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/IptcImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/JpegImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/JpegPresets.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/JpegPresets.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/McIdasImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/McIdasImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MicImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MicImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpegImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MpegImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MpoImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MpoImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/MspImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/MspImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PSDraw.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PSDraw.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PaletteFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PaletteFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PalmImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PalmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcdImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcdImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcfFontFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcfFontFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PcxImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PcxImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PdfImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PdfParser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PdfParser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PixarImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PixarImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PngImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PngImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PpmImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PpmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PsdImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PsdImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/PyAccess.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/PyAccess.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/QoiImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/QoiImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SgiImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SgiImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SpiderImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SpiderImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/SunImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/SunImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TarIO.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TarIO.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TgaImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TgaImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TiffImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/TiffTags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/TiffTags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WalImageFile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WalImageFile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WebPImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WebPImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/WmfImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/WmfImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XbmImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XbmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/XpmImagePlugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/XpmImagePlugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_binary.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_binary.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_deprecate.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_deprecate.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/_tkinter_finder.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/_tkinter_finder.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/PIL/features.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/PIL/features.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/_distutils_hack/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/_virtualenv.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/__pip-runner__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/build_env.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/check.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/download.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/help.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/index.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/install.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/list.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/search.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/show.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/configuration.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/collector.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/index/sources.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/locations/base.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/index.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/link.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/auth.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/download.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/session.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/check.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/pyproject.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/models.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/align.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/box.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/console.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/control.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/json.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/status.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/style.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/table.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/text.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/six.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/config.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/core.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/log.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_entry_points.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_imp.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_importlib.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_itertools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_normalization.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_path.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_reqs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/archive_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/build_meta.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/alias.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_clib.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_ext.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/build_py.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/develop.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/dist_info.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/easy_install.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/egg_info.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_lib.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/py36compat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/rotate.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/saveopts.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/sdist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/setopt.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/test.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/expand.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/config/setupcfg.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dep_util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/depends.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/discovery.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/dist.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/errors.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extension.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/extern/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/glob.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/installer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/launch.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/logging.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/monkey.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/msvc.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/namespaces.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/package_index.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/sandbox.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/unicode_utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/setuptools/windows_support.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/colorutils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/colorutils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/constants.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/constants.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/icons.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/icons.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/localization/msgs.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/localization/msgs.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/publisher.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/publisher.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/scrolled.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/scrolled.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/style.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/style.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tableview.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/tableview.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/themes/standard.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/themes/standard.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/toast.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/toast.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/tooltip.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/tooltip.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/utility.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/utility.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/validation.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/validation.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/widgets.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/widgets.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkbootstrap/window.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkbootstrap/window.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/ttkcreator/__main__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/ttkcreator/__main__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/_setuptools_logging.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/bdist_wheel.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/__init__.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/convert.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/pack.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/cli/unpack.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/macosx_libfile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/metadata.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/util.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_elffile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_parser.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_structures.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/_tokenizer.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/markers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/requirements.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/specifiers.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/utils.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/vendored/packaging/version.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Lib/site-packages/wheel/wheelfile.py` & `compoundwidgets-0.2.1/venv/Lib/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.0/venv/Scripts/activate_this.py` & `compoundwidgets-0.2.1/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

