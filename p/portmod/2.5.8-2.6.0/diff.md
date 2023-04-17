# Comparing `tmp/portmod-2.5.8.tar.gz` & `tmp/portmod-2.6.0-cp37-abi3-macosx_11_0_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/portmod-2.5.8.tar", last modified: Tue Mar  7 03:30:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

