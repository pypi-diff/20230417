# Comparing `tmp/PartehDB-1.0.2.tar.gz` & `tmp/PartehDB-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PartehDB-1.0.2.tar", last modified: Mon Apr 17 01:18:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

