# Comparing `tmp/fastapi_allauth-0.1.1.tar.gz` & `tmp/fastapi_allauth-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_allauth-0.1.1.tar", last modified: Mon Feb  6 15:09:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

