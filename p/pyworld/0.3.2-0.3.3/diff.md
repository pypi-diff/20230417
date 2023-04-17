# Comparing `tmp/pyworld-0.3.2.tar.gz` & `tmp/pyworld-0.3.3-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyworld-0.3.2.tar", last modified: Wed Nov  2 00:58:13 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

