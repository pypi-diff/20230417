# Comparing `tmp/xj_dictionary-1.0.7.tar.gz` & `tmp/xj_dictionary-1.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_dictionary-1.0.7.tar", last modified: Fri Mar  3 07:17:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

