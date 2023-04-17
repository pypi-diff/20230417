# Comparing `tmp/Pandora-ChatGPT-1.0.1.tar.gz` & `tmp/Pandora-ChatGPT-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-va_65r8b/Pandora-ChatGPT-1.0.1.tar", last modified: Thu Apr 13 11:18:02 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-o8manuz6/Pandora-ChatGPT-1.0.2.tar", last modified: Mon Apr 17 04:16:36 2023, max compression
```

## Comparing `Pandora-ChatGPT-1.0.1.tar` & `Pandora-ChatGPT-1.0.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:18:02.000000 Pandora-ChatGPT-1.0.1/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-13 11:17:53.000000 Pandora-ChatGPT-1.0.1/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-17 04:16:24.000000 Pandora-ChatGPT-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 04:16:24.000000 Pandora-ChatGPT-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-17 04:16:24.000000 Pandora-ChatGPT-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:16:36.000000 Pandora-ChatGPT-1.0.2/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-17 04:16:25.000000 Pandora-ChatGPT-1.0.2/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-1.0.1/LICENSE` & `Pandora-ChatGPT-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/PKG-INFO` & `Pandora-ChatGPT-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -142,27 +142,25 @@
 ## 程序参数
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
 * `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
 
 ## 关于 Access Token
 
 * 使用`Access Token`方式登录，可以无代理直连。
```

### Comparing `Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -142,27 +142,25 @@
 ## 程序参数
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
 * `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
 
 ## 关于 Access Token
 
 * 使用`Access Token`方式登录，可以无代理直连。
```

### Comparing `Pandora-ChatGPT-1.0.1/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.0.2/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/README.md` & `Pandora-ChatGPT-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -105,27 +105,25 @@
 ## 程序参数
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
 * `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
-* `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
 
 ## 关于 Access Token
 
 * 使用`Access Token`方式登录，可以无代理直连。
```

### Comparing `Pandora-ChatGPT-1.0.1/setup.py` & `Pandora-ChatGPT-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.0.2/src/pandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.0.2/src/pandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.0.2/src/pandora/cloud_launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,20 +37,14 @@
         '--server',
         help='Specific server bind. Format: ip:port, default: 127.0.0.1:8018',
         required=False,
         type=str,
         default='127.0.0.1:8018',
     )
     parser.add_argument(
-        '-l',
-        '--local',
-        help='Login locally. Pay attention to the risk control of the login ip!',
-        action='store_true',
-    )
-    parser.add_argument(
         '--sentry',
         help='Enable sentry to send error reports when errors occur.',
         action='store_true',
     )
     parser.add_argument(
         '-v',
         '--verbose',
@@ -62,15 +56,15 @@
 
     if args.sentry:
         sentry.init(args.proxy)
 
     try:
         from pandora_cloud.server import ChatBot as CloudServer
 
-        return CloudServer(args.proxy, args.verbose, args.sentry, args.local).run(args.server)
+        return CloudServer(args.proxy, args.verbose, args.sentry, True).run(args.server)
     except (ImportError, ModuleNotFoundError):
         Console.error_bh('### You need `pip install Pandora-ChatGPT[cloud]` to support cloud mode.')
 
 
 def run():
     hook_except_handle()
```

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.0.2/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.0.2/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.0.2/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/launcher.py` & `Pandora-ChatGPT-1.0.2/src/pandora/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     return valid_tokens
 
 
 def main():
     global __show_verbose
 
     api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
-    prefix_changed = 'https://chat.gateway.do' != api_prefix
 
     Console.debug_b(
         '''
             Pandora - A command-line interface to ChatGPT
             Github: https://github.com/pengzhile/pandora
             Get access token: {}/auth
             Version: {}'''.format(api_prefix, __version__), end=''
@@ -157,20 +156,14 @@
     parser.add_argument(
         '-a',
         '--api',
         help='Use gpt-3.5-turbo chat api. Note: OpenAI will bill you.',
         action='store_true',
     )
     parser.add_argument(
-        '-l',
-        '--local',
-        help='Login locally. Pay attention to the risk control of the login ip!',
-        action='store_true',
-    )
-    parser.add_argument(
         '--sentry',
         help='Enable sentry to send error reports when errors occur.',
         action='store_true',
     )
     parser.add_argument(
         '-v',
         '--verbose',
@@ -198,21 +191,18 @@
 
     access_tokens = parse_access_tokens(args.tokens_file, args.api) if args.tokens_file else None
 
     if not access_tokens:
         access_token, need_save = confirm_access_token(args.token_file, args.server, args.api)
         if not access_token:
             Console.info_b('Please enter your email and password to log in ChatGPT!')
-            if not args.local:
-                Console.warn('We login via {}{}'.format(
-                    api_prefix, '' if prefix_changed else ', but it doesn\'t retain your data.'))
             email = getenv('OPENAI_EMAIL') or Prompt.ask('  Email')
             password = getenv('OPENAI_PASSWORD') or Prompt.ask('  Password', password=True)
             Console.warn('### Do login, please wait...')
-            access_token = Auth0(email, password, args.proxy).auth(args.local)
+            access_token = Auth0(email, password, args.proxy).auth(True)
 
         if not check_access_token_out(access_token, args.api):
             return
 
         if need_save:
             if args.server or Confirm.ask('Do you want to save your access token for the next login?', default=True):
                 save_access_token(access_token)
```

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.0.2/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.0.2/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.0.2/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.0.2/src/pandora/openai/api.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.0.2/src/pandora/openai/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
 
     @staticmethod
     def __check_email(email: str):
         regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
         return re.fullmatch(regex, email)
 
-    def auth(self, login_local=False) -> str:
+    def auth(self, login_local=True) -> str:
         if self.use_cache and self.access_token and self.expires and self.expires > dt.now():
             return self.access_token
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception('invalid email or password.')
 
         return self.__part_two() if login_local else self.get_access_token_proxy()
```

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.0.2/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.0.2/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.1/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.0.2/src/pandora/turbo/chat.py`

 * *Files identical despite different names*

