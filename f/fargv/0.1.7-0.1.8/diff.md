# Comparing `tmp/fargv-0.1.7.tar.gz` & `tmp/fargv-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fargv-0.1.7.tar", last modified: Tue Aug  9 11:31:22 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

