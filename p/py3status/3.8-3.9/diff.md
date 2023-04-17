# Comparing `tmp/py3status-3.8.tar.gz` & `tmp/py3status-3.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3status-3.8.tar", last modified: Mon Apr  2 17:07:07 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

