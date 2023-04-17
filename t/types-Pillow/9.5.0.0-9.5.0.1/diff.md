# Comparing `tmp/types-Pillow-9.5.0.0.tar.gz` & `tmp/types-Pillow-9.5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pillow-9.5.0.0.tar", last modified: Fri Apr 14 09:14:44 2023, max compression
+gzip compressed data, was "types-Pillow-9.5.0.1.tar", last modified: Mon Apr 17 12:30:45 2023, max compression
```

## Comparing `types-Pillow-9.5.0.0.tar` & `types-Pillow-9.5.0.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.250007 types-Pillow-9.5.0.0/PIL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BdfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BlpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BmpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BufrStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ContainerIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/CurImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/DcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/DdsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/EpsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ExifTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FitsStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FliImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FpxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FtexImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GbrImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GdImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GifImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GimpGradientFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GimpPaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GribStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Hdf5StubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IcnsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IcoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageChops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageCms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageColor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageDraw2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageEnhance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageGrab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMorph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageOps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImagePalette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImagePath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageQt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageSequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageShow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageStat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageTk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageTransform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageWin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImtImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IptcImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Jpeg2KImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/JpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/JpegPresets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/PIL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/McIdasImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MicImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MpoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MspImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PSDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PalmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PdfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PdfParser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PixarImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PngImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PsdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PyAccess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SgiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SpiderImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SunImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TarIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TgaImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TiffImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TiffTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WalImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WebPImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WmfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XVThumbImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XbmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_imaging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_tkinter_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/types_Pillow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/PIL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BdfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BlpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BmpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BufrStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ContainerIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/CurImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/DcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/DdsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/EpsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ExifTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FitsStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FliImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FpxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FtexImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GbrImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GdImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GifImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GimpGradientFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GimpPaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GribStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Hdf5StubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IcnsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IcoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageChops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageCms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageColor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageDraw2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageEnhance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageGrab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImagePalette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImagePath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageQt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageSequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageShow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageStat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageTk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageTransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageWin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImtImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IptcImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Jpeg2KImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/JpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/JpegPresets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/PIL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/McIdasImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MicImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MpoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MspImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PSDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PalmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PdfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PdfParser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PixarImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PngImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PsdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PyAccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SgiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SpiderImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SunImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TarIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TgaImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TiffImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TiffTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WalImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WebPImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WmfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XVThumbImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XbmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_imaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_tkinter_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/types_Pillow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/top_level.txt
```

### Comparing `types-Pillow-9.5.0.0/CHANGELOG.md` & `types-Pillow-9.5.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 9.5.0.1 (2023-04-17)
+
+[Pillow] Add Base and GPS enums in PIL.ExifTags (#10051)
+
 ## 9.5.0.0 (2023-04-14)
 
 Bump Pillow to 9.5.* (#10046)
 
 Release: https://pypi.org/pypi/Pillow/9.5.0
 Homepage: https://python-pillow.org
 Changelog: https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst
```

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/BlpImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/BlpImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/DdsImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/DdsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/EpsImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/EpsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/FpxImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/FpxImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/GifImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/GifImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/IcnsImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/IcnsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/IcoImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/IcoImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/Image.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/Image.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageChops.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageChops.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageCms.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageCms.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageDraw.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageDraw2.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageDraw2.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageEnhance.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageEnhance.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageFile.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageFile.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageFilter.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageFilter.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageFont.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageFont.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageMath.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageMath.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageMorph.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageMorph.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageOps.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageOps.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImagePalette.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImagePalette.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageQt.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageQt.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageShow.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageShow.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageTk.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageTk.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/ImageWin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/ImageWin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/JpegImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/JpegImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/MicImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/MicImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/PSDraw.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/PSDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/PdfParser.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/PdfParser.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/PngImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/PngImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/PyAccess.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/PyAccess.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/SpiderImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/SpiderImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/TiffImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/TiffImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/TiffTags.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/TiffTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/WmfImagePlugin.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/WmfImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PIL-stubs/features.pyi` & `types-Pillow-9.5.0.1/PIL-stubs/features.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.0/PKG-INFO` & `types-Pillow-9.5.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.0
+Version: 9.5.0.1
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
+This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
```

### Comparing `types-Pillow-9.5.0.0/setup.py` & `types-Pillow-9.5.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
+This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
 '''.lstrip()
 
 setup(name=name,
-      version="9.5.0.0",
+      version="9.5.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md",
```

### Comparing `types-Pillow-9.5.0.0/types_Pillow.egg-info/PKG-INFO` & `types-Pillow-9.5.0.1/types_Pillow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.0
+Version: 9.5.0.1
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
+This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
```

### Comparing `types-Pillow-9.5.0.0/types_Pillow.egg-info/SOURCES.txt` & `types-Pillow-9.5.0.1/types_Pillow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

