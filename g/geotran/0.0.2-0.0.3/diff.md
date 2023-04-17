# Comparing `tmp/geotran-0.0.2.tar.gz` & `tmp/geotran-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotran-0.0.2.tar", last modified: Sat Apr 15 01:29:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

