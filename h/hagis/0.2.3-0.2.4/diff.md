# Comparing `tmp/hagis-0.2.3.tar.gz` & `tmp/hagis-0.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.3.tar", last modified: Mon Apr 17 13:03:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

