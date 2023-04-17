# Comparing `tmp/fiduswriter-books-3.9.4.tar.gz` & `tmp/fiduswriter-books-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiduswriter-books-3.9.4.tar", last modified: Thu Apr 15 19:45:14 2021, max compression
+gzip compressed data, was "dist/fiduswriter-books-3.9.5.tar", last modified: Fri Apr 16 14:52:05 2021, max compression
```

## Comparing `fiduswriter-books-3.9.4.tar` & `fiduswriter-books-3.9.5.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    34500 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/LICENSE
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      297 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/MANIFEST.in
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1578 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/PKG-INFO
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      581 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/README.rst
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       47 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      605 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/admin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.166258 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    34478 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/initial_book_data.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.166258 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   191484 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Bold.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   153060 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Italic.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   223616 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Regular.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    44512 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Bold.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    39280 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-BoldItalic.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    55548 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Italic.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    95500 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Roman.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    26424 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Lobster-1.4.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_crtDjCs.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_yO6HqH2.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_9HCH4bJ.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_rB1dJdY.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_OL1vKDc.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_ZMVQrVq.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_mqEfVcK.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_t56TEHe.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    91484 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Bold.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    94044 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Regular.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    63256 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold.woff
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    63256 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold_kmw0DlW.woff
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      446 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      513 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8216 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    14932 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      380 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      447 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6454 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13170 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      398 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      465 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6550 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13266 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      392 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      459 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6662 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13378 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      385 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      470 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6492 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13208 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      405 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      472 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6584 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13328 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/migrations/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3415 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0001_initial.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      434 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0002_auto_20151226_1110.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      436 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0003_auto_20160515_1007.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      946 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0004_auto_20160515_1008.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      441 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0005_auto_20160515_1013.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      646 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0006_auto_20190622_2126.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2161 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/0007_bookstyle_bookstylefile.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/migrations/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3124 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/models.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/static/css/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      615 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/css/book.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.170258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/accessrights/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6926 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/accessrights/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3276 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/accessrights/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    16932 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/actions.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/epub/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12475 2021-04-15 19:42:58.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/epub/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7072 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/epub/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/html/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8996 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/html/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2438 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/html/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/latex/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3667 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/latex/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      590 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/latex/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/print/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5507 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/print/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      625 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/print/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1136 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/tools.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10647 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6783 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    14597 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.162258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/app/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      351 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/app/book.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/books_overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       42 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/books_overview/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/menu/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      381 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/static/js/plugins/menu/book.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter/book/tests/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/tests/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    18254 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/tests/test_book.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      392 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    14223 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.4/fiduswriter/book/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/fiduswriter_books.egg-info/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1578 2021-04-15 19:45:14.000000 fiduswriter-books-3.9.4/fiduswriter_books.egg-info/PKG-INFO
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5004 2021-04-15 19:45:14.000000 fiduswriter-books-3.9.4/fiduswriter_books.egg-info/SOURCES.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        1 2021-04-15 19:45:14.000000 fiduswriter-books-3.9.4/fiduswriter_books.egg-info/dependency_links.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       15 2021-04-15 19:45:14.000000 fiduswriter-books-3.9.4/fiduswriter_books.egg-info/top_level.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2021-04-15 19:45:14.174258 fiduswriter-books-3.9.4/setup.cfg
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2052 2021-04-15 19:44:29.000000 fiduswriter-books-3.9.4/setup.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    34500 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/LICENSE
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      297 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/MANIFEST.in
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1578 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/PKG-INFO
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      581 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/README.rst
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.279147 fiduswriter-books-3.9.5/fiduswriter/book/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       47 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      605 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/admin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.279147 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    34478 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/initial_book_data.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   191484 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Bold.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   153060 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Italic.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   223616 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Regular.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    44512 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Bold.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    39280 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-BoldItalic.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    55548 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Italic.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    95500 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Roman.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    26424 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Lobster-1.4.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_crtDjCs.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37520 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_yO6HqH2.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_9HCH4bJ.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41084 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_rB1dJdY.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_OL1vKDc.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    37404 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_ZMVQrVq.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_mqEfVcK.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41604 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_t56TEHe.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    91484 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Bold.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    94044 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Regular.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    63256 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold.woff
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    63256 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold_kmw0DlW.woff
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      446 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      513 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8216 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    14932 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      380 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      447 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6454 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13170 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      398 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      465 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6550 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13266 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      392 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      459 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6662 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13378 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.283147 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      385 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      470 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6492 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13208 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      405 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      472 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6584 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13328 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/migrations/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3415 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0001_initial.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      434 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0002_auto_20151226_1110.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      436 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0003_auto_20160515_1007.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      946 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0004_auto_20160515_1008.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      441 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0005_auto_20160515_1013.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      646 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0006_auto_20190622_2126.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2161 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/0007_bookstyle_bookstylefile.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/migrations/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3124 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/models.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/static/css/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      615 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/css/book.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/accessrights/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6926 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/accessrights/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3276 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/accessrights/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    16932 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/actions.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.287147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/epub/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12475 2021-04-15 19:42:58.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/epub/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7072 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/epub/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/html/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8768 2021-04-16 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/html/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2717 2021-04-16 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/html/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/latex/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3667 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/latex/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      590 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/latex/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/print/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5507 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/print/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      625 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/print/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1136 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/tools.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10647 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6783 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    14597 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.275147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/app/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      351 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/app/book.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/books_overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       42 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/books_overview/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/menu/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      381 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/static/js/plugins/menu/book.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter/book/tests/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/tests/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    18254 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/tests/test_book.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      392 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    14223 2021-03-23 14:51:36.000000 fiduswriter-books-3.9.5/fiduswriter/book/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/fiduswriter_books.egg-info/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1578 2021-04-16 14:52:05.000000 fiduswriter-books-3.9.5/fiduswriter_books.egg-info/PKG-INFO
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5004 2021-04-16 14:52:05.000000 fiduswriter-books-3.9.5/fiduswriter_books.egg-info/SOURCES.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        1 2021-04-16 14:52:05.000000 fiduswriter-books-3.9.5/fiduswriter_books.egg-info/dependency_links.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       20 2021-04-16 14:52:05.000000 fiduswriter-books-3.9.5/fiduswriter_books.egg-info/top_level.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2021-04-16 14:52:05.291147 fiduswriter-books-3.9.5/setup.cfg
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2052 2021-04-16 14:51:44.000000 fiduswriter-books-3.9.5/setup.py
```

### Comparing `fiduswriter-books-3.9.4/LICENSE` & `fiduswriter-books-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/PKG-INFO` & `fiduswriter-books-3.9.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fiduswriter-books
-Version: 3.9.4
+Version: 3.9.5
 Summary: A Fidus Writer plugin to allow creation of books and article collections
 Home-page: https://www.github.org/fiduswriter/fiduswriter-books
 Author: Johannes Wilm
 Author-email: johannes@fiduswriter.org
 License: AGPL License
 Description: FidusWriter-Books
         =================
```

### Comparing `fiduswriter-books-3.9.4/README.rst` & `fiduswriter-books-3.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/admin.py` & `fiduswriter-books-3.9.5/fiduswriter/book/admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/initial_book_data.json` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/initial_book_data.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Bold.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Italic.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Cardo-Regular.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Cardo-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Bold.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-BoldItalic.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Italic.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Roman.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/CrimsonText-Roman.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/Lobster-1.4.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/Lobster-1.4.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_crtDjCs.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_crtDjCs.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_yO6HqH2.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-BoldItalic_yO6HqH2.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_9HCH4bJ.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_9HCH4bJ.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_rB1dJdY.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Bold_rB1dJdY.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_OL1vKDc.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_OL1vKDc.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_ZMVQrVq.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Italic_ZMVQrVq.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_mqEfVcK.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_mqEfVcK.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_t56TEHe.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/NoticiaText-Regular_t56TEHe.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Bold.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Regular.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/OpenSans-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold_kmw0DlW.woff` & `fiduswriter-books-3.9.5/fiduswriter/book/fixtures/media/book-style-files/SourceSansPro-Bold_kmw0DlW.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/django.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.po` & `fiduswriter-books-3.9.5/fiduswriter/book/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/migrations/0001_initial.py` & `fiduswriter-books-3.9.5/fiduswriter/book/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/migrations/0004_auto_20160515_1008.py` & `fiduswriter-books-3.9.5/fiduswriter/book/migrations/0004_auto_20160515_1008.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/migrations/0006_auto_20190622_2126.py` & `fiduswriter-books-3.9.5/fiduswriter/book/migrations/0006_auto_20190622_2126.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/migrations/0007_bookstyle_bookstylefile.py` & `fiduswriter-books-3.9.5/fiduswriter/book/migrations/0007_bookstyle_bookstylefile.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/models.py` & `fiduswriter-books-3.9.5/fiduswriter/book/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/css/book.css` & `fiduswriter-books-3.9.5/fiduswriter/book/static/css/book.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/accessrights/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/accessrights/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/accessrights/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/accessrights/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/actions.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/actions.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/epub/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/epub/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/epub/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/epub/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/html/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/html/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -191,23 +191,14 @@
                     id: 0,
                     level: -1,
                     subItems: []
                 })
                 currentPart = this.book.chapters[index].part
             }
 
-            contentItems.push({
-                link: `document-${this.book.chapters[index].number}.html`,
-                title,
-                docNum: this.book.chapters[index].number,
-                id: 0,
-                level: 0,
-                subItems: []
-            })
-
             // Make links to all H1-3 and create a TOC list of them
             contentItems.push(...setLinks(contents, this.book.chapters[index].number))
 
             const contentsCode = this.replaceImgSrc(contents.innerHTML)
 
             const htmlCode = this.chapterTemplate({
                 part: this.book.chapters[index].part,
@@ -232,14 +223,17 @@
 
         this.outputList.push({
             filename: 'index.html',
             contents: pretty(htmlBookIndexTemplate({
                 contentItems,
                 book: this.book,
                 creator: this.user.name,
+                styleSheets: [{
+                    filename: bookStyle
+                }],
                 // TODO: specify a book language rather than using the current users UI language
                 language: gettext('English')
             }), {
                 ocd: true
             })
         })
```

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/html/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/html/templates.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
         <link type="text/css" rel="stylesheet" href="css/document.css" />
         ${
     styleSheets.map(sheet =>
         `<link type="text/css" rel="stylesheet" href="${sheet.filename}" />`
     ).join('')
 }
     </head>
-    <body${currentPart && currentPart.length ? ` class="${currentPart.toLowerCase().replace(/[^a-z]/g, '')}"` : ''}>
+    <body class="book-chapter${currentPart && currentPart.length ? ` ${currentPart.toLowerCase().replace(/[^a-z]/g, '')}` : ''}">
         ${
     part && part.length ?
         `<h1 class="part">${escapeText(part)}</h1>` :
         ''
 }
         ${contents}
     </body>
@@ -60,41 +60,48 @@
     </li>`
 
 /** A template to create the book index. */
 export const htmlBookIndexTemplate = ({
         book,
         contentItems,
         language,
-        creator
+        creator,
+        styleSheets
     }) =>
     `<!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8"></meta>
         <title>${escapeText(book.title)}</title>
+        <link type="text/css" rel="stylesheet" href="css/document.css" />
+        ${
+    styleSheets.map(sheet =>
+        `<link type="text/css" rel="stylesheet" href="${sheet.filename}" />`
+    ).join('')
+}
     </head>
-    <body>
+    <body class="book-index">
         <h1>${escapeText(book.title)}</h1>
         ${
     book.metadata.subtitle.length ?
         `<h2>${escapeText(book.metadata.subtitle)}</h2>` :
         ''
 }
         ${
     book.metadata.author.length ?
         `<h3>${gettext('by')} ${escapeText(book.metadata.author)}</h3>` :
         ''
 }
-        <ol>
+        <nav role="doc-toc"><ol>
             ${
     contentItems.map(item =>
         htmlBookIndexItemTemplate({item})
     ).join('')
 }
-        </ol>
+        </ol></nav>
         ${
     book.metadata.publisher && book.metadata.publisher.length ?
         `<p>${gettext('Published by')}: ${escapeText(book.metadata.publisher)}</p>` :
         ''
 }
         <p>${gettext('Last Updated')}: ${book.updated}</p>
         <p>${gettext('Created')}: ${book.added}</p>
```

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/latex/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/latex/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/latex/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/latex/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/print/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/print/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/print/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/print/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/exporter/tools.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/exporter/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/index.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/menu.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/static/js/modules/books/templates.js` & `fiduswriter-books-3.9.5/fiduswriter/book/static/js/modules/books/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/tests/test_book.py` & `fiduswriter-books-3.9.5/fiduswriter/book/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter/book/views.py` & `fiduswriter-books-3.9.5/fiduswriter/book/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/fiduswriter_books.egg-info/PKG-INFO` & `fiduswriter-books-3.9.5/fiduswriter_books.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fiduswriter-books
-Version: 3.9.4
+Version: 3.9.5
 Summary: A Fidus Writer plugin to allow creation of books and article collections
 Home-page: https://www.github.org/fiduswriter/fiduswriter-books
 Author: Johannes Wilm
 Author-email: johannes@fiduswriter.org
 License: AGPL License
 Description: FidusWriter-Books
         =================
```

### Comparing `fiduswriter-books-3.9.4/fiduswriter_books.egg-info/SOURCES.txt` & `fiduswriter-books-3.9.5/fiduswriter_books.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-books-3.9.4/setup.py` & `fiduswriter-books-3.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='fiduswriter-books',
-    version='3.9.4',
+    version='3.9.5',
     packages=find_namespace_packages(),
     exclude_package_data={
         "": ["configuration.py", "django-admin.py", "build/*"]
     },
     include_package_data=True,
     license='AGPL License',
     description=(
```

