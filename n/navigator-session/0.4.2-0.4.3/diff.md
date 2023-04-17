# Comparing `tmp/navigator-session-0.4.2.tar.gz` & `tmp/navigator_session-0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigator-session-0.4.2.tar", last modified: Wed Mar 22 18:03:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

