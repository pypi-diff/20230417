# Comparing `tmp/rapidfuzz-2.9.0.tar.gz` & `tmp/rapidfuzz-3.0.0-cp37-cp37m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-2.9.0.tar", last modified: Fri Sep 16 01:00:42 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

