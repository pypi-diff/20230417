# Comparing `tmp/granslate-3.4.0.tar.gz` & `tmp/granslate-3.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granslate-3.4.0.tar", last modified: Tue Dec 27 10:07:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

