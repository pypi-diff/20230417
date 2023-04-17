# Comparing `tmp/borb-2.1.8.tar.gz` & `tmp/borb-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borb-2.1.8.tar", last modified: Wed Jan 18 19:42:30 2023, max compression
+gzip compressed data, was "borb-2.1.9.tar", last modified: Fri Feb 17 17:20:27 2023, max compression
```

## Comparing `borb-2.1.8.tar` & `borb-2.1.9.tar`

### file list

```diff
@@ -1,1495 +1,1496 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)      866 2023-01-18 19:42:20.000000 borb-2.1.8/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-01-18 19:42:20.000000 borb-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-18 19:42:30.139444 borb-2.1.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3897 2023-01-18 19:42:20.000000 borb-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/datastructure/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/datastructure/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2805 2023-01-18 19:42:20.000000 borb-2.1.8/borb/datastructure/disjoint_set.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-01-18 19:42:20.000000 borb-2.1.8/borb/datastructure/str_trie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/filter/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/ascii85_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5721 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/flate_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/lzw_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2546 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/run_length_decode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2930 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/filter/stream_decode_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4415 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/any_object_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/encryption/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/encryption/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/encryption/rc4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22670 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/encryption/standard_security_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/font/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/font/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4323 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/font/font_dictionary_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/function/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/function/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/function/function_dictionary_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/ccitt_fax_image_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3072 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/compressed_jpeg_image_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/grayscale_image_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2627 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/jbig2_image_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/jpeg_2000_image_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2937 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/image/jpeg_image_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb/io/read/metadata/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/metadata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4198 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/metadata/xmp_metadata_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/object/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/object/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/object/array_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1805 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/object/dictionary_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2531 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/object/stream_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/page/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/page/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4112 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/page/page_dictionary_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3448 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/page/root_dictionary_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/postfix/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/postfix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19956 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/postfix/postfix_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/primitive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/primitive/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/primitive/number_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/primitive/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/reference/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/reference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4581 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/reference/reference_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10719 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/reference/xref_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/read/tokenize/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/tokenize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11312 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/tokenize/high_level_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8476 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/tokenize/low_level_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4820 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29281 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/read/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3788 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/any_object_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/conformance_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/document/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/document/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3759 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/document/catalog_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4131 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/document/document_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12257 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/document/information_dictionary_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/document/resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/document/resources/sRGB_CS_profile.icm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/font/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/font/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/font/character_set_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2448 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/font/copy_command_operator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4113 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/font/subset_show_text_with_glyph_positioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6131 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/font/subsetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/image/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/image/image_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/object/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/object/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/object/array_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/object/dictionary_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4280 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/object/stream_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/page/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/page/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/page/page_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2104 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/page/pages_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.007444 borb-2.1.8/borb/io/write/primitive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/primitive/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/primitive/boolean_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/primitive/name_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/primitive/number_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/primitive/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/io/write/reference/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/reference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/reference/reference_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5883 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/reference/xref_transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9032 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/io/write/version/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/version/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/version/version_as_comment_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/io/write/xmp/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/xmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2505 2023-01-18 19:42:20.000000 borb-2.1.8/borb/io/write/xmp/xmp_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/license/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/anonymous_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/geo_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/machine_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/usage_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/license/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4686 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/canvas/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4475 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/canvas_graphics_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12190 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/canvas_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/canvas/color/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/color/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24747 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/color/color.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/color/farrow_and_ball.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    79103 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/color/pantone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/canvas/event/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/begin_page_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/begin_text_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7922 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/chunk_of_text_render_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/end_page_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/end_text_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      615 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/event_listener.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/image_render_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/event/line_render_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/canvas/font/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2582 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/adobe_standard_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.011443 borb-2.1.8/borb/pdf/canvas/font/composite_font/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4410 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cid_font_type_0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cid_font_type_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.039444 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14796 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    14673 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    14827 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3198 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    16500 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     7080 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/83pv-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6070 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     6001 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     4212 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     7815 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3715 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    14854 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    15038 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3793 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     4002 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-1
--rwxr-xr-x   0 runner    (1001) docker     (123)     4022 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4122 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-3
--rwxr-xr-x   0 runner    (1001) docker     (123)     4142 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-4
--rwxr-xr-x   0 runner    (1001) docker     (123)     4142 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-5
--rwxr-xr-x   0 runner    (1001) docker     (123)     4142 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-6
--rwxr-xr-x   0 runner    (1001) docker     (123)     4118 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-7
--rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     3446 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-1
--rwxr-xr-x   0 runner    (1001) docker     (123)     4400 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4399 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-3
--rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-4
--rwxr-xr-x   0 runner    (1001) docker     (123)     5051 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-5
--rwxr-xr-x   0 runner    (1001) docker     (123)     7820 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity
--rwxr-xr-x   0 runner    (1001) docker     (123)     7820 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2619 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3380 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3390 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-3
--rwxr-xr-x   0 runner    (1001) docker     (123)     3868 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-4
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-5
--rwxr-xr-x   0 runner    (1001) docker     (123)     4468 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-6
--rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-7
--rwxr-xr-x   0 runner    (1001) docker     (123)     3168 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan2-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     3012 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3512 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-3
--rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-4
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-5
--rwxr-xr-x   0 runner    (1001) docker     (123)     3732 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-6
--rwxr-xr-x   0 runner    (1001) docker     (123)     4092 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-7
--rwxr-xr-x   0 runner    (1001) docker     (123)     4372 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-8
--rwxr-xr-x   0 runner    (1001) docker     (123)     4412 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-9
--rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-0
--rwxr-xr-x   0 runner    (1001) docker     (123)     4089 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-1
--rwxr-xr-x   0 runner    (1001) docker     (123)     4088 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-2
--rwxr-xr-x   0 runner    (1001) docker     (123)     7493 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2924 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     7547 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5pc-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5pc-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    12246 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    13278 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     5611 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS1-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2932 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS1-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    23202 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     7703 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3041 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     5075 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3223 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    15424 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    15607 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3481 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4427 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3100 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3076 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    83102 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3089 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    90926 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3482 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    83083 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3095 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    46773 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3108 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    46668 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3084 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    46803 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4455 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3112 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4941 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/H
--rwxr-xr-x   0 runner    (1001) docker     (123)    23268 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2941 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    20928 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2941 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    13724 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2947 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    13537 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2947 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    16507 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2947 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    23253 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     2821 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hankaku
--rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hiragana
--rwxr-xr-x   0 runner    (1001) docker     (123)     4626 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2709 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     4276 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2685 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    11728 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    11637 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    84250 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3050 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3012 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    15940 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)    15936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3050 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    12555 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3048 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     2711 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Katakana
--rwxr-xr-x   0 runner    (1001) docker     (123)    17298 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/NWP-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3603 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/NWP-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     5124 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     2688 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Roman
--rwxr-xr-x   0 runner    (1001) docker     (123)   186553 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)   250494 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)   220008 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)   326349 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2971 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   253253 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   324657 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3040 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   290056 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   274383 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   199981 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3061 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   267909 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   237834 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3115 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    83592 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2714 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    62948 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    84821 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)    73701 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2716 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   168597 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     2820 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6591 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     6509 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   188173 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     5771 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   245393 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   216408 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6296 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   188254 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   245474 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6827 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   216486 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6318 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-HW-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     6618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   245383 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6769 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   245463 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     6793 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   166009 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3076 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   122938 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3030 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   165010 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-V
--rwxr-xr-x   0 runner    (1001) docker     (123)   145845 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-H
--rwxr-xr-x   0 runner    (1001) docker     (123)     3076 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3199 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/V
--rwxr-xr-x   0 runner    (1001) docker     (123)     3093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/WP-Symbol
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11806 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/composite_font/font_type_0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18455 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/font.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9082 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/glyph_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.039444 borb-2.1.8/borb/pdf/canvas/font/simple_font/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.039444 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15397 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-bold-oblique.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    15331 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-bold.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    15439 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-oblique.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    15333 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    69363 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-bold-oblique.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    69267 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-bold.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    74390 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-oblique.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    74290 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)     9738 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/symbol.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    59640 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-bold-italic.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    64249 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-bold.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    66326 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-italic.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    60458 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-roman.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/zapfdingbats.afm
--rwxr-xr-x   0 runner    (1001) docker     (123)    23290 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/font_type_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3051 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/font_type_3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2312 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/simple_font.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14325 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/simple_font/true_type_font.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/font/symbol_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.039444 borb-2.1.8/borb/pdf/canvas/geometry/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/geometry/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/geometry/line_segment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4959 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/geometry/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/geometry/rectangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.039444 borb-2.1.8/borb/pdf/canvas/layout/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.043444 borb-2.1.8/borb/pdf/canvas/layout/annotation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7317 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/caret_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4174 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/circle_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/file_attachment_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5427 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/free_text_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/highlight_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/ink_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3757 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/line_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5479 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/link_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/movie_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/polygon_annotion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3966 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/polyline_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/popup_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/printer_mark_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7041 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/redact_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2623 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/remote_go_to_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3374 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/rubber_stamp_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/screen_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/sound_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4222 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/square_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/squiggly_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/strike_out_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3008 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/text_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/three_d_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/trap_net_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3065 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/underline_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/watermark_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/annotation/widget_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.043444 borb-2.1.8/borb/pdf/canvas/layout/emoji/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    66284 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.119444 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2116 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/a.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2491 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ab.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2672 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/abc.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/abcd.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1696 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aerial_tramway.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2822 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/airplane.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3866 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/alarm_clock.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4131 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/alien.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ambulance.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3060 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anchor.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/angel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2687 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anger.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/angry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anguished.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ant.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4043 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/apple.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aquarius.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aries.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_backward.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_double_down.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_double_up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2030 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down_hook.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_forward.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2088 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left_hook.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1721 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1637 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_lower_left.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_lower_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_right_hook.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1690 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_down.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_hook.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1276 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_upper_left.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_upper_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_clockwise.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2845 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_counterclockwise.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3329 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_right_twisted.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5329 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/art.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1946 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/articulated_lorry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3387 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/astonished.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3411 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/atm.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1955 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/b.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2668 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_bottle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_chick.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2932 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_symbol.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bagage_claim.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/balloon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2404 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ballot_box_with_check.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2865 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bamboo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3663 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/banana.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bang_bang.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bank.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bar_chart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/barber.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baseball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3638 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/basketball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bath.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bathtub.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      928 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/battery.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3146 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bear.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3234 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4309 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beers.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beetle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beginner.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2498 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bell.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5962 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bento.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5698 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bicyclist.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3473 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bike.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3381 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bikini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3740 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bird.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4463 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/birthday.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_circle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2747 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_joker.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_nib.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_square_button.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4031 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blossom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blowfish.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_book.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2687 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_circle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_diamond.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2913 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blush.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3856 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boar.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bomb.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2817 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/book.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bookmark.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bookmark_tabs.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/books.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3998 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boot.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5390 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bouquet.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bow.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bowling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2724 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bowtie.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3745 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2854 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bread.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5170 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bride_with_veil.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4693 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bridge_at_night.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1510 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/briefcase.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3474 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/broken_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3745 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bug.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3095 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bulb.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bullettrain_front.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bullettrain_side.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/busstop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bust_in_silhouette.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2367 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/busts_in_silhouette.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cactus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4220 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cake.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/calendar.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/calling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4236 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/camel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2243 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/camera.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4312 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cancer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/candy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3191 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/capital_abcd.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3517 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/capricorn.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1975 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/card_index.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4686 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/carousel_horse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3776 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4525 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cat_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cd.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2190 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart_with_downwards_trend.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2229 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart_with_upwards_trend.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/checkered_flag.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4296 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cherries.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4494 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cherry_blossom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4032 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chestnut.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3136 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chicken.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/children_crossing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chocolate_bar.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/christmas_tree.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5030 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/church.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cinema.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4225 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/circus_tent.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3232 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/city_sunrise.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2433 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/city_sunset.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cl.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3498 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clap.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clapper.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1661 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clipboard.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2327 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_10.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2441 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_10_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_11.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_11_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_12.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2314 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_12_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2372 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_1_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2314 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_2_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_3.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_3_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_4.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2433 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_4_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_5.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_5_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_6.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2301 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_6_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_7.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2360 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_7_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_8.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2450 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_8_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_9.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2301 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_9_30.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_book.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2468 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_lock_with_key.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3108 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_umbrella.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cloud.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clubs.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cn.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cocktail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/coffee.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3998 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/collision.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/computer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4223 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confetti_ball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confounded.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2338 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confused.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2157 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/construction.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5682 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/construction_worker.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1753 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/convenience_store.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3797 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cookie.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2647 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cool.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2787 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/copyright.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4643 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/corn.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4653 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couple.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4203 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couple_with_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5150 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couplekiss.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cow.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3589 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cow_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/credit_card.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4285 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crocodile.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crossed_flags.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crown.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3497 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crying_cat_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crystal_ball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3427 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cupid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2640 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/curly_loop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/currency_exchange.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4003 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/curry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4165 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/custard.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/customs.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3453 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cyclone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3937 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dancer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6305 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dancers.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dango.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3999 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3068 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dash.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/date.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/de.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/deciduous_tree.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2420 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/department_store.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2888 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/diamond_shape_with_dot_inside.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/diamonds.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2190 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/disappointed.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/disappointed_relieved.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dizzy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dizzy_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4208 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/do_not_litter.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3483 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dog.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dog_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dollar.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4006 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dolls.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4155 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dolphin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/door.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4452 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/doughnut.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dragon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5493 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dragon_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dress.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4163 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dromedary_camel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/droplet.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2732 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dvd.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/e_mail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ear.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5354 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ear_of_rice.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5364 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_africa.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4906 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_americas.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_asia.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2889 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/egg.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eggplant.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2139 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight_pointed_black_star.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3525 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight_pointed_blue_star.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/electric_plug.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/elephant.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/email.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/end.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/envelope.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/es.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1851 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/euro.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4491 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/european_castle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/european_post_office.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2317 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/evergreen_tree.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/exclamation.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/expressionless.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1846 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eyeglasses.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2803 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/facepunch.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3752 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/factory.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fallen_leaf.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5579 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/family.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fast_forward.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fax.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fearful.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/feelsgood.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/feet.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ferris_wheel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/file_folder.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/finnadie.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3103 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fire.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2596 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fire_engine.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4864 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fireworks.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3509 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3153 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon_with_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2527 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fish.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3945 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fish_cake.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4449 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fishing_pole_and_fish.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fist.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2968 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/five.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flags.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2977 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flashlight.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/floppy_disk.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flower_playing_cards.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3881 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flushed.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3349 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/foggy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4180 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/football.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5309 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fountain.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2538 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/four.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3457 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/four_leaf_clover.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1882 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fr.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2153 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/free.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5341 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fried_shrimp.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fries.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3297 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/frog.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2264 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/frowning.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fu.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fuelpump.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3622 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/full_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4385 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/full_moon_with_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/game_die.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gb.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3117 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gem.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gemini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2934 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ghost.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gift.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gift_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4284 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/girl.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4058 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/globe_with_meridians.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3412 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/goat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/goberserk.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/godmode.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1882 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/golf.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5025 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grapes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4112 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_apple.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_book.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2731 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      666 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grey_exclamation.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grey_question.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2587 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grimacing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grinning.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/guardsman.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3142 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/guitar.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gun.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5410 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/haircut.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hamburger.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hammer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4108 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hamster.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hand.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2983 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/handbag.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hankey.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3132 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hash.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2789 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hatched_chick.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3544 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hatching_chick.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3441 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/headphones.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4375 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hear_no_evil.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2694 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2313 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_decoration.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3788 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_eyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4499 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_eyes_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heartbeat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4696 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heartpulse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1955 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hearts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2315 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_check_mark.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_division_sign.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_dollar_sign.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_exclamation_mark.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_minus_sign.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2623 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_multiplication.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_plus_sign.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2867 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/helicopter.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/herb.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4687 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hibiscus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/high_brightness.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/high_heel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hocho.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4961 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/honey_pot.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3574 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/honeybee.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/horse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5467 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/horse_racing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hospital.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2564 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hotel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hotsprings.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hourglass.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2641 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hourglass_flowing_sand.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/house.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/house_with_garden.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4103 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hundred.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1375 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hurtrealbad.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2434 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hushed.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5541 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ice_cream.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/icecream.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/id.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2817 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/imp.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1674 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/inbox_tray.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/incoming_envelope.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4413 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/information_desk_person.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/information_source.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3646 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/innocent.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2619 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/interrobang.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/iphone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/it.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/izakaya_lantern.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3726 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jack_o_lantern.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japan.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4543 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_castle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3945 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_goblin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4434 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_ogre.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2390 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jeans.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3461 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/joy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4143 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/joy_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jp.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/key.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3165 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/keycap_ten.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3426 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kimono.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3695 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kiss.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2143 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3578 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_closed_eyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3518 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_smiling_eyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/knife_and_fork.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2833 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/koala.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/koko.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2460 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kr.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3278 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon_with_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3282 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/laughing.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3517 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leaves.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ledger.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2274 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/left_luggage.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lemon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3669 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leopard.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/libra.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/light_rail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1584 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/link.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2486 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lips.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lipstick.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lock.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2229 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lock_with_ink_pen.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lollipop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3419 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/loop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2484 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/loudspeaker.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3488 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/love_hotel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2682 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/love_letter.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2384 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/low_brightness.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4470 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/m.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3598 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mag.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mag_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3350 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/magic_8_ball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mahjong.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_closed.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_with_mail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_with_no_mail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3301 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man_with_gua_pi_mao.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3312 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man_with_turban.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mans_shoe.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/maple_leaf.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2822 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mask.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4834 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/massage.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3981 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/meat_on_bone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2983 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mega.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5528 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/melon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2496 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/memo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mens.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/metal.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3028 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/microphone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/microscope.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4769 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/milky_way.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minibus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1623 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minidisc.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minus_1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mobile_phone_off.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/money_with_wings.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2946 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moneybag.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4666 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monkey.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monkey_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monorail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4007 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mortar_board.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5321 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mount_fuji.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6540 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_bicyclist.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_cableway.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1467 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_railway.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3013 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mouse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3189 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mouse_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3338 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/movie_camera.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3297 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moyai.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2432 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/muscle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3919 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mushroom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_keyboard.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2012 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_note.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_score.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mute.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4023 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nail_care.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3231 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/name_badge.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3204 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/neckbeard.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3419 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/necktie.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2734 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/negative_squared_cross_mark.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/neutral_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2046 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2664 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new_moon_with_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/newspaper.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2834 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ng.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nine.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4568 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_bell.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4561 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_bicycles.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3661 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_entry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5149 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_good.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3931 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_mobile_phones.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_mouth.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4203 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_pedestrians.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_smoking.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4088 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/non_potable_water.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nose.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      403 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/notebook.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/notebook_with_decorative_cover.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2280 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/notes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nut_and_bolt.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2848 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/o.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4333 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ocean.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2468 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/octocat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5203 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/octopus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3118 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oden.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/office.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok_hand.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4257 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok_woman.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/older_man.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3942 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/older_woman.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3126 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/on.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_automobile.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1606 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_bus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2257 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_police_car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_taxi.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/one.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2887 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/one_two_three_four.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_file_folder.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_hands.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_mouth.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ophiuchus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/orange_book.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/orange_diamond.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/outbox_tray.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ox.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/page_facing_up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/page_with_curl.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pager.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4534 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/palm_tree.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3013 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/panda_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/paperclip.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1721 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/parking.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/part_alternation_mark.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3586 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/partly_sunny.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2799 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/passport_control.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/paw_prints.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4423 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/peach.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3303 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pear.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2496 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pencil.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pencil_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2622 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/penguin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pensive.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4427 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/performing_arts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2640 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/persevere.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/phone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2594 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig_nose.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pill.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pineapple.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3500 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pisces.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4062 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pizza.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/plus_1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1822 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_down.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_left.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1692 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_right.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2676 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1744 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_up_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1972 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/police_car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3377 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poodle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2850 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/post_office.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3586 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/postal_horn.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/postbox.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/potable_water.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2678 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pouch.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3233 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poultry_leg.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pound.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3410 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pouting_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2660 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pray.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/princess.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2803 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/punch.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2599 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/purple_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3300 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/purse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2662 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pushpin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/put_litter_in_its_place.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/question.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3178 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rabbit.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3248 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rabbit_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4356 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/racehorse.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2876 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/radio.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4416 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/radio_button.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2455 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_3.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1196 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_4.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1467 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/railway_car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rainbow.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raised_hand.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3689 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raised_hands.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4980 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raising_hand.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ram.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6109 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ramen.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3710 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3454 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/recycle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1975 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/red_car.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1736 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/red_circle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/registered.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3389 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/relaxed.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2620 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/relieved.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2543 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/repeat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3003 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/repeat_once.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3423 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/restroom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/revolving_hearts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rewind.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4245 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ribbon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3634 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3562 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_ball.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3427 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_cracker.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3037 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_scene.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3237 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ring.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2984 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rocket.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/roller_coaster.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rooster.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3055 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rose.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2058 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rotating_light.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/round_pushpin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3481 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rowboat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ru.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3418 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rugby_football.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3426 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/runner.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3426 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/running.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2774 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/running_shirt_with_sash.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sagittarius.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sailboat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sake.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sandal.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3115 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/santa.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/satelite.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3282 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/satisfied.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3115 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/saxophone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/school.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/school_satchel.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3615 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scissors.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3368 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scorpius.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scream.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scream_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2150 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scroll.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/see_no_evil.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seedling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2511 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seven.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4544 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shaved_ice.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3580 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sheep.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shell.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2104 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ship.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4612 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shipit.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shirt.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shit.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shoe.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2897 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shower.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/signal_strength.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3052 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/six.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3103 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/six_pointed_star.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4040 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ski.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1341 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/skull.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2671 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sleeping.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2807 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sleepy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/slot_machine.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_blue_diamond.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_orange_diamond.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_down.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3064 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smile.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3845 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smile_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3170 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiley.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3799 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiley_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2811 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiling_imp.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smirk.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3253 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smirk_cat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smoking.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3579 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snail.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4975 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snake.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowboarder.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4584 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowflake.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3566 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowman.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3735 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sob.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3134 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/soccer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3445 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/soon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sos.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sound.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/space_invader.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/spades.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6019 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/spaghetti.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4155 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkler.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2167 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkles.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3881 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkling_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3840 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speak_no_evil.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1934 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speaker.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speech_balloon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2675 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speedboat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/star.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/star_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stars.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3162 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/station.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3958 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/statue_of_liberty.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2592 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/steam_locomotive.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4962 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stew.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/straight_ruler.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4928 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/strawberry.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2787 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_closed_eyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_winking_eye.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3657 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sun_with_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4760 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunflower.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2547 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunglasses.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunny.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3307 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunrise.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4700 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunrise_over_mountains.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5892 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/surfer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4926 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sushi.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/suspect.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1927 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/suspension_railway.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2719 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat_drops.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3425 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat_smile.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3503 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweet_potato.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/swimmer.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3114 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/symbols.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2835 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/syringe.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tada.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4088 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tanabata_tree.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3805 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tangerine.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3620 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/taurus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2303 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/taxi.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tea.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telephone.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telephone_receiver.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4243 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telescope.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     5057 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tennis.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3488 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tent.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thought_balloon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/three.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thumbsdown.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thumbsup.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ticket.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tiger.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4624 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tiger_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tired_face.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1291 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tm.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/toilet.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1792 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tokyo_tower.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tomato.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tongue.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2563 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/top.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2466 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tophat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3663 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tractor.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/traffic_light.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/train.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2620 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/train_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2375 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tram.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triangular_flag_on_post.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triangular_ruler.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2993 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trident.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3768 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triumph.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trolleybus.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trollface.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trophy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2675 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tropical_drink.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tropical_fish.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1831 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/truck.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3818 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trumpet.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tshirt.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3017 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tulip.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3914 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/turtle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4451 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tv.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_hearts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4393 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_men_holding_hands.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4573 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_women_holding_hands.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/uk.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3455 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/umbrella.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2437 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/unamused.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4420 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/underage.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/unlock.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/us.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/v.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1836 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vertical_traffic_light.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vhs.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vibration_mode.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2772 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/video_camera.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/video_game.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4357 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/violin.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3830 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/virgo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4563 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/volcano.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3057 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vs.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2406 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/walking.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waning_cresent_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3874 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waning_gibbous_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1906 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/warning.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/watch.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/water_buffalo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3256 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/watermelon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wave.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wavy_dash.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3922 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waxing_cresent_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4007 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waxing_gibbous_moon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3048 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wc.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2927 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/weary.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4787 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wedding.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3858 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/whale.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/whale_2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/white_circle.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3393 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/white_flower.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/white_square_button.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wind_chime.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wine_glass.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wink.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2293 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wolf.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3449 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/woman.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2986 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womans_clothes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2998 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womans_hat.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womens.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/worried.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wrench.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2786 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yellow_heart.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1769 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yen.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2812 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yum.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1895 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zap.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2893 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zero.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2743 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zzz.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.119444 borb-2.1.8/borb/pdf/canvas/layout/forms/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9888 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/check_box.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7142 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/country_drop_down_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9793 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/drop_down_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/form_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13136 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/push_button.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9601 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/text_area.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8315 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/forms/text_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7043 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/free_space_finder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/horizontal_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.123444 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/hyphenation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.123444 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)   174033 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/af.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/as.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    57726 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/be.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   123484 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/bg.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/bn.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ca.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   103675 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/cy.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    16472 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/da.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   340992 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/de.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   131733 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/en-gb.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    76272 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/en-us.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    54781 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/es.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    56508 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/et.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/fi.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    19269 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/fr.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    22354 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/lt.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   198747 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/nl.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     9285 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ro.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   131354 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ru.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.123444 borb-2.1.8/borb/pdf/canvas/layout/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/image/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6162 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/image/barcode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/image/chart.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5367 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/image/image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/image/unsplash.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22768 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/layout_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/list/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7752 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/list/list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/list/ordered_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1570 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/list/roman_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3354 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/list/unordered_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/page_layout/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3953 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/block_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/header_footer_multi_column_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3948 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/inline_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8682 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/multi_column_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/page_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5821 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/page_layout/single_column_layout_with_overflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/shape/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/shape/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8128 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/shape/connected_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7228 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/shape/disconnected_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6937 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/shape/gradient_colored_disconnected_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5912 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/shape/progressbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/smart_art/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/smart_art/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48671 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/smart_art/smart_art.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/table/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/table/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/table/fixed_column_width_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13210 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/table/flexible_column_width_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18570 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/table/table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3443 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/table/table_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/layout/text/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9618 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/chunk_of_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4543 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/codeblock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/heading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/heterogeneous_paragraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7624 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/line_of_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16509 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/layout/text/paragraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/line_art/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/line_art/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3702 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/line_art/blob_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56858 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/line_art/line_art_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6341 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/line_art/rectangular_hitomezashi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5201 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/line_art/rectangular_maze_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.127444 borb-2.1.8/borb/pdf/canvas/lipsum/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7831 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/lipsum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.131445 borb-2.1.8/borb/pdf/canvas/lipsum/resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)   314156 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_agatha_christie.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    97075 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_alan_alexander_milne.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   326591 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_arthur_conan_doyle.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   577242 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_emily_bronte.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   554298 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_jane_austen.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   118929 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_lewis_carroll.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    64293 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_lipsum.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   440228 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_mary_shelley.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     9374 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/lipsum/text_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.131445 borb-2.1.8/borb/pdf/canvas/operator/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/canvas_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.131445 borb-2.1.8/borb/pdf/canvas/operator/color/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_cmyk_non_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_cmyk_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3892 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_color_non_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4135 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_color_space_non_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7044 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_color_space_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4697 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_color_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_gray_non_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1385 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_gray_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1346 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_rgb_non_stroking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/color/set_rgb_stroking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.131445 borb-2.1.8/borb/pdf/canvas/operator/compatibility/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/compatibility/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/compatibility/begin_compatibility_section.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/compatibility/end_compatibility_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/marked_content/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/marked_content/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1143 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/marked_content/begin_marked_content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/marked_content/begin_marked_content_with_property_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/marked_content/end_marked_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/path_construction/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6862 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_cubic_bezier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_line_segment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_rectangle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1745 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/begin_subpath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_construction/close_subpath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/path_painting/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_painting/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_painting/close_and_stroke_path.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_painting/fill_path_even_odd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_painting/fill_path_nonzero_winding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/path_painting/stroke_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/state/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/state/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/state/modify_transformation_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/state/pop_graphics_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/state/push_graphics_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/state/set_line_width.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/text/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1412 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/begin_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1021 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/end_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1869 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/move_text_position.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2111 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/move_text_position_set_leading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1805 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/move_to_next_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/move_to_next_line_show_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_character_spacing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_font_and_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_horizontal_text_scaling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_spacing_move_to_next_line_show_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_text_leading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1948 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_text_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      855 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_text_rendering_mode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_text_rise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/set_word_spacing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1684 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/show_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/text/show_text_with_glyph_positioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/canvas/operator/xobject/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/xobject/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/operator/xobject/do.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13534 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/canvas/redacted_canvas_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/document/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/document/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17412 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/document/document.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6733 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/document/name_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/page/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/page/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11035 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/page/page.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/page/page_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/page/page_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3551 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.135444 borb-2.1.8/borb/pdf/trailer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/trailer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16344 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/trailer/document_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/pdf/xref/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/xref/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5746 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/xref/plaintext_xref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6137 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/xref/rebuilt_xref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8979 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/xref/stream_xref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8873 2023-01-18 19:42:20.000000 borb-2.1.8/borb/pdf/xref/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/color/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/color/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8029 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/color/color_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/export/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/export/html_to_pdf/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/html_to_pdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36107 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/html_to_pdf/html_to_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/export/markdown_to_pdf/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/markdown_to_pdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/markdown_to_pdf/markdown_to_pdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/pdf_to_jpg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6007 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/pdf_to_mp3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8131 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/export/pdf_to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/image/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3089 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/image/image_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/image/image_format_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/location/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/location/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2366 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/location/location_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/ocr/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/ocr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6767 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/ocr/ocr_as_optional_content_group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12822 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/ocr/ocr_image_render_event_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/redact/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/redact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/redact/common_regular_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/table/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/table/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14061 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/table/table_detection_by_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.139444 borb-2.1.8/borb/toolkit/text/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/font_color_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2147 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/font_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/font_name_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14916 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/regular_expression_text_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/simple_find_replace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/simple_line_of_text_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3683 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/simple_non_ligature_text_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6996 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/simple_paragraph_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5092 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/simple_text_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11000 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/stop_words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6480 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/text_rank_keyword_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6924 2023-01-18 19:42:20.000000 borb-2.1.8/borb/toolkit/text/tf_idf_keyword_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:42:30.003444 borb-2.1.8/borb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-18 19:42:29.000000 borb-2.1.8/borb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    71967 2023-01-18 19:42:29.000000 borb-2.1.8/borb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 19:42:29.000000 borb-2.1.8/borb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-18 19:42:29.000000 borb-2.1.8/borb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-18 19:42:29.000000 borb-2.1.8/borb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 19:42:30.139444 borb-2.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1140 2023-01-18 19:42:20.000000 borb-2.1.8/setup.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.160677 borb-2.1.9/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      866 2021-09-20 10:49:37.000000 borb-2.1.9/LICENSE.md
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      357 2022-09-23 11:44:00.000000 borb-2.1.9/MANIFEST.in
+-rw-rw-r--   0 joris     (1000) joris     (1000)     4283 2023-02-17 17:20:27.160677 borb-2.1.9/PKG-INFO
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3897 2023-01-16 14:35:13.000000 borb-2.1.9/README.md
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.824676 borb-2.1.9/borb/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.824676 borb-2.1.9/borb/datastructure/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/datastructure/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2805 2022-09-09 13:04:21.000000 borb-2.1.9/borb/datastructure/disjoint_set.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1784 2022-04-06 21:53:10.000000 borb-2.1.9/borb/datastructure/str_trie.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.824676 borb-2.1.9/borb/io/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.824676 borb-2.1.9/borb/io/filter/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/filter/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1251 2021-08-01 19:20:26.000000 borb-2.1.9/borb/io/filter/ascii85_decode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5721 2022-04-06 21:17:27.000000 borb-2.1.9/borb/io/filter/flate_decode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3477 2022-09-04 14:44:22.000000 borb-2.1.9/borb/io/filter/lzw_decode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2546 2022-09-03 08:17:18.000000 borb-2.1.9/borb/io/filter/run_length_decode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2930 2022-05-13 22:58:40.000000 borb-2.1.9/borb/io/filter/stream_decode_util.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.828676 borb-2.1.9/borb/io/read/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4415 2022-06-18 22:06:41.000000 borb-2.1.9/borb/io/read/any_object_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.828676 borb-2.1.9/borb/io/read/encryption/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/encryption/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3124 2021-11-01 15:53:44.000000 borb-2.1.9/borb/io/read/encryption/rc4.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    22670 2022-07-31 20:25:41.000000 borb-2.1.9/borb/io/read/encryption/standard_security_handler.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.828676 borb-2.1.9/borb/io/read/font/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/font/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4323 2022-01-22 13:38:39.000000 borb-2.1.9/borb/io/read/font/font_dictionary_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.828676 borb-2.1.9/borb/io/read/function/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/function/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3618 2022-04-06 20:59:39.000000 borb-2.1.9/borb/io/read/function/function_dictionary_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.832676 borb-2.1.9/borb/io/read/image/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/image/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2633 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/ccitt_fax_image_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3072 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/compressed_jpeg_image_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3442 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/grayscale_image_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2627 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/jbig2_image_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2638 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/jpeg_2000_image_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2937 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/read/image/jpeg_image_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.832676 borb-2.1.9/borb/io/read/metadata/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/metadata/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4198 2021-09-04 19:37:51.000000 borb-2.1.9/borb/io/read/metadata/xmp_metadata_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.832676 borb-2.1.9/borb/io/read/object/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/object/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1681 2022-04-06 21:03:58.000000 borb-2.1.9/borb/io/read/object/array_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1805 2022-04-06 21:03:58.000000 borb-2.1.9/borb/io/read/object/dictionary_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2531 2022-04-06 20:59:39.000000 borb-2.1.9/borb/io/read/object/stream_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.832676 borb-2.1.9/borb/io/read/page/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/page/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4112 2022-04-06 21:08:17.000000 borb-2.1.9/borb/io/read/page/page_dictionary_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3448 2022-04-06 21:08:17.000000 borb-2.1.9/borb/io/read/page/root_dictionary_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.836676 borb-2.1.9/borb/io/read/postfix/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/postfix/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    19956 2022-09-26 20:27:11.000000 borb-2.1.9/borb/io/read/postfix/postfix_eval.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.836676 borb-2.1.9/borb/io/read/primitive/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/primitive/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1413 2022-04-06 21:23:44.000000 borb-2.1.9/borb/io/read/primitive/number_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1494 2021-11-09 18:48:38.000000 borb-2.1.9/borb/io/read/primitive/string_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.836676 borb-2.1.9/borb/io/read/reference/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/reference/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4581 2022-04-06 21:26:07.000000 borb-2.1.9/borb/io/read/reference/reference_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    10719 2022-09-26 20:27:11.000000 borb-2.1.9/borb/io/read/reference/xref_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.836676 borb-2.1.9/borb/io/read/tokenize/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/read/tokenize/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11312 2022-04-08 23:04:41.000000 borb-2.1.9/borb/io/read/tokenize/high_level_tokenizer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8476 2022-09-04 01:31:13.000000 borb-2.1.9/borb/io/read/tokenize/low_level_tokenizer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4820 2022-06-18 22:06:05.000000 borb-2.1.9/borb/io/read/transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    29281 2022-11-27 23:45:56.000000 borb-2.1.9/borb/io/read/types.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.840676 borb-2.1.9/borb/io/write/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3788 2022-10-17 13:35:37.000000 borb-2.1.9/borb/io/write/any_object_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2103 2022-03-16 10:15:30.000000 borb-2.1.9/borb/io/write/conformance_level.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.840676 borb-2.1.9/borb/io/write/document/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/io/write/document/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3759 2022-11-28 08:36:27.000000 borb-2.1.9/borb/io/write/document/catalog_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4131 2022-08-30 16:54:07.000000 borb-2.1.9/borb/io/write/document/document_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12257 2022-10-17 13:35:37.000000 borb-2.1.9/borb/io/write/document/information_dictionary_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.840676 borb-2.1.9/borb/io/write/document/resources/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3144 2022-01-22 00:24:03.000000 borb-2.1.9/borb/io/write/document/resources/sRGB_CS_profile.icm
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.840676 borb-2.1.9/borb/io/write/font/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/font/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1664 2022-07-10 07:15:21.000000 borb-2.1.9/borb/io/write/font/character_set_listener.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2448 2022-07-23 09:29:57.000000 borb-2.1.9/borb/io/write/font/copy_command_operator.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4113 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/write/font/subset_show_text_with_glyph_positioning.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6131 2022-11-28 08:40:22.000000 borb-2.1.9/borb/io/write/font/subsetter.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.840676 borb-2.1.9/borb/io/write/image/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/image/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4640 2022-09-05 20:03:21.000000 borb-2.1.9/borb/io/write/image/image_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.844676 borb-2.1.9/borb/io/write/object/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/io/write/object/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3698 2022-04-06 22:39:18.000000 borb-2.1.9/borb/io/write/object/array_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4067 2022-11-21 14:03:36.000000 borb-2.1.9/borb/io/write/object/dictionary_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4280 2022-04-06 21:33:19.000000 borb-2.1.9/borb/io/write/object/stream_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.844676 borb-2.1.9/borb/io/write/page/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/page/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2339 2022-07-16 23:24:13.000000 borb-2.1.9/borb/io/write/page/page_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2104 2022-08-01 19:03:57.000000 borb-2.1.9/borb/io/write/page/pages_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.844676 borb-2.1.9/borb/io/write/primitive/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/primitive/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1367 2022-04-06 21:41:20.000000 borb-2.1.9/borb/io/write/primitive/boolean_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1067 2021-11-09 18:48:38.000000 borb-2.1.9/borb/io/write/primitive/name_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1330 2021-11-09 18:48:38.000000 borb-2.1.9/borb/io/write/primitive/number_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1579 2021-11-09 18:48:38.000000 borb-2.1.9/borb/io/write/primitive/string_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.844676 borb-2.1.9/borb/io/write/reference/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/reference/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1454 2021-11-09 18:48:39.000000 borb-2.1.9/borb/io/write/reference/reference_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5883 2022-09-16 01:12:07.000000 borb-2.1.9/borb/io/write/reference/xref_transformer.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9032 2022-10-06 18:06:55.000000 borb-2.1.9/borb/io/write/transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.848676 borb-2.1.9/borb/io/write/version/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/version/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2055 2022-10-17 14:42:05.000000 borb-2.1.9/borb/io/write/version/version_as_comment_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.848676 borb-2.1.9/borb/io/write/xmp/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/io/write/xmp/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2505 2022-08-01 19:14:44.000000 borb-2.1.9/borb/io/write/xmp/xmp_transformer.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.848676 borb-2.1.9/borb/license/
+-rw-rw-r--   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/license/__init__.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     4540 2022-11-03 15:19:36.000000 borb-2.1.9/borb/license/anonymous_user_id.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     1511 2022-10-19 15:59:59.000000 borb-2.1.9/borb/license/machine_id.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     3184 2023-02-08 07:36:39.000000 borb-2.1.9/borb/license/usage_statistics.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     1527 2022-10-19 16:01:07.000000 borb-2.1.9/borb/license/uuid.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)      936 2023-02-17 11:59:59.000000 borb-2.1.9/borb/license/version.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.848676 borb-2.1.9/borb/pdf/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4686 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.848676 borb-2.1.9/borb/pdf/canvas/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1108 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/canvas.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4475 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/canvas_graphics_state.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12190 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/canvas_stream_processor.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.852676 borb-2.1.9/borb/pdf/canvas/color/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/color/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    24973 2023-01-29 21:58:14.000000 borb-2.1.9/borb/pdf/canvas/color/color.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     3318 2023-02-08 11:12:17.000000 borb-2.1.9/borb/pdf/canvas/color/color_palette_from_image.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6442 2022-09-04 14:36:29.000000 borb-2.1.9/borb/pdf/canvas/color/farrow_and_ball.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    79103 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/color/pantone.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.852676 borb-2.1.9/borb/pdf/canvas/event/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/event/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      599 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/begin_page_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      345 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/begin_text_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7922 2022-08-30 16:54:08.000000 borb-2.1.9/borb/pdf/canvas/event/chunk_of_text_render_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      595 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/end_page_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      344 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/end_text_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      615 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/event_listener.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1868 2022-09-05 20:03:21.000000 borb-2.1.9/borb/pdf/canvas/event/image_render_event.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      931 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/event/line_render_event.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.856676 borb-2.1.9/borb/pdf/canvas/font/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/font/__init__.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)   377414 2023-02-17 11:53:08.000000 borb-2.1.9/borb/pdf/canvas/font/adobe_glyph_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2582 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/adobe_standard_encoding.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.856676 borb-2.1.9/borb/pdf/canvas/font/composite_font/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4410 2022-01-22 13:52:13.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cid_font_type_0.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1733 2022-01-22 13:52:13.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cid_font_type_2.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.912676 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14796 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3222 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14673 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14827 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3228 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3198 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    16500 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4209 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7080 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/83pv-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6070 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4229 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6001 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4212 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7815 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3715 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14854 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15038 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3823 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3793 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3829 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4002 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-1
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4022 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-2
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4122 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-3
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4142 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-4
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4142 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-5
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4142 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-6
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4118 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-7
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3292 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3446 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-1
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4400 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-2
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4399 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-3
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4951 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-4
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5051 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-5
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7820 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7820 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2619 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3341 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3342 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-1
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3380 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-2
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3390 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-3
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3868 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-4
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4248 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-5
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4468 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-6
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4444 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-7
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3168 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan2-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2879 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3012 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-1
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3512 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-2
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3532 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-3
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3552 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-4
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3572 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-5
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3732 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-6
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4092 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-7
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4372 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-8
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4412 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-9
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3433 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-0
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4089 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-1
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4088 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-2
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7493 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2924 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7547 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5pc-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2936 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5pc-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12246 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13278 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5611 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS1-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2932 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS1-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4275 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2683 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    23202 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2955 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7703 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2974 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2729 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3041 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5075 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3223 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15424 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15607 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3481 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3451 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4427 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3100 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4322 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3076 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    83102 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3089 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    90926 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3482 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    83083 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3095 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    46773 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3108 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    46668 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3084 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    46803 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3120 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4455 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3112 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4941 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    23268 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2941 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    20928 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2941 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13724 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2947 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13537 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2947 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    16507 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2947 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    23253 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2961 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2821 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hankaku
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2795 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hiragana
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4626 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2709 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4276 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2685 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11728 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3036 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11637 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    84250 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3050 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3012 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15940 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15936 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3049 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3050 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12555 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3048 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2711 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Katakana
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    17298 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/NWP-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3603 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/NWP-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5124 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3229 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2688 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Roman
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   186553 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   250494 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   220008 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   326349 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2971 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   253253 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2960 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   324657 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3040 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   290056 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2996 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   274383 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3167 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   199981 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3061 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   267909 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3177 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   237834 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3115 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    83592 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2714 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    62948 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2720 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    84821 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2720 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    73701 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2716 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   168597 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2820 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6591 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6509 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   188173 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5771 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   245393 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6803 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   216408 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6296 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   188254 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5795 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   245474 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6827 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   216486 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6318 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6729 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-HW-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6618 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7467 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   245383 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6769 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   245463 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6793 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   166009 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3076 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   122938 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3030 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   165010 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3130 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   145845 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-H
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3076 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3199 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/V
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3093 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/WP-Symbol
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11806 2022-04-06 20:46:37.000000 borb-2.1.9/borb/pdf/canvas/font/composite_font/font_type_0.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    18455 2022-03-20 15:28:05.000000 borb-2.1.9/borb/pdf/canvas/font/font.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9082 2022-06-18 22:56:52.000000 borb-2.1.9/borb/pdf/canvas/font/glyph_line.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.916677 borb-2.1.9/borb/pdf/canvas/font/simple_font/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.920677 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15397 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-bold-oblique.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15331 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-bold.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15439 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-oblique.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    15333 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    69363 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-bold-oblique.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    69267 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-bold.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    74390 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-oblique.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    74290 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9738 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/symbol.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    59640 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-bold-italic.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    64249 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-bold.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    66326 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-italic.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    60458 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-roman.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9525 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/zapfdingbats.afm
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    23504 2023-02-17 11:50:24.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/font_type_1.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3051 2022-01-22 13:52:13.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/font_type_3.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2312 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/simple_font.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14325 2022-07-18 11:36:32.000000 borb-2.1.9/borb/pdf/canvas/font/simple_font/true_type_font.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4958 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/font/symbol_encoding.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.920677 borb-2.1.9/borb/pdf/canvas/geometry/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/geometry/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1423 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/geometry/line_segment.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4959 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/geometry/matrix.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/geometry/rectangle.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.920677 borb-2.1.9/borb/pdf/canvas/layout/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/pdf/canvas/layout/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.928676 borb-2.1.9/borb/pdf/canvas/layout/annotation/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7317 2022-03-20 15:28:05.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      572 2022-02-12 01:39:09.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/caret_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4174 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/circle_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      618 2022-02-12 01:39:02.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/file_attachment_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5427 2022-04-06 22:47:57.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/free_text_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3083 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/highlight_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      836 2022-02-12 01:38:52.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/ink_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3757 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/line_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5479 2022-09-02 07:45:16.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/link_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      922 2022-02-12 01:40:15.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/movie_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2936 2022-04-06 22:09:26.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/polygon_annotion.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3966 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/polyline_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1254 2022-02-12 01:40:44.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/popup_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      992 2022-02-12 01:41:31.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/printer_mark_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7041 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/redact_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2623 2022-04-06 22:17:47.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/remote_go_to_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3374 2022-09-02 10:44:51.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/rubber_stamp_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1004 2022-02-12 01:50:33.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/screen_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3709 2022-02-21 21:16:48.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/sound_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4222 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/square_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3549 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/squiggly_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3292 2022-03-20 15:33:22.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/strike_out_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3008 2022-04-24 18:26:01.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/text_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1400 2022-02-12 01:51:00.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/three_d_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      510 2022-02-12 01:50:54.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/trap_net_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3065 2022-02-12 01:51:49.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/underline_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1028 2022-02-12 01:51:44.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/watermark_annotation.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1172 2022-02-12 01:51:38.000000 borb-2.1.9/borb/pdf/canvas/layout/annotation/widget_annotation.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.928676 borb-2.1.9/borb/pdf/canvas/layout/emoji/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    66284 2022-08-30 16:54:10.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/emoji.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.104677 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2116 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/a.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2491 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ab.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2672 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/abc.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3087 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/abcd.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1696 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aerial_tramway.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2822 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/airplane.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3866 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/alarm_clock.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4131 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/alien.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1961 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ambulance.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3060 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anchor.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4775 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/angel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2687 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anger.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2695 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/angry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2391 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anguished.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2537 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ant.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4043 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/apple.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3087 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aquarius.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3274 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aries.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1309 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_backward.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1728 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_double_down.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1709 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_double_up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1333 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2030 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down_hook.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1324 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down_small.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1301 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_forward.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1324 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2088 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left_hook.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1721 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1637 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_lower_left.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1741 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_lower_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1330 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2108 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_right_hook.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1292 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1690 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_down.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2006 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_hook.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1276 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_small.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_upper_left.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1682 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_upper_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2752 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_clockwise.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2845 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_counterclockwise.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3329 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_right_twisted.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5329 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/art.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1946 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/articulated_lorry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3387 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/astonished.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3411 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/atm.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1955 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/b.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2668 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3397 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_bottle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2800 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_chick.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2932 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_symbol.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1961 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bagage_claim.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2349 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/balloon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2404 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ballot_box_with_check.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2865 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bamboo.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3663 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/banana.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1121 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bang_bang.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2401 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bank.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1559 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bar_chart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1853 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/barber.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3802 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baseball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3638 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/basketball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2113 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bath.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      990 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bathtub.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      928 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/battery.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3146 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bear.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3234 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4309 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beers.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3618 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beetle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1908 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beginner.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2498 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bell.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5962 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bento.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5698 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bicyclist.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3473 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bike.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3381 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bikini.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3740 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bird.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4463 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/birthday.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1147 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_circle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2747 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_joker.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2377 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_nib.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      496 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_square_button.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4031 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blossom.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4052 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blowfish.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      990 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_book.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2687 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1969 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_circle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1361 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_diamond.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2913 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3275 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blush.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3856 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boar.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2737 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2982 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bomb.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2817 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/book.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2641 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bookmark.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1540 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bookmark_tabs.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3778 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/books.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3998 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boom.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2126 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boot.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5390 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bouquet.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4389 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bow.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4322 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bowling.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2724 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bowtie.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3745 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2854 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bread.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5170 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bride_with_veil.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4693 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bridge_at_night.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1510 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/briefcase.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3474 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/broken_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3745 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bug.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3095 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bulb.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1597 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bullettrain_front.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1638 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bullettrain_side.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1272 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1723 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/busstop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1923 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bust_in_silhouette.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2367 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/busts_in_silhouette.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3560 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cactus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4220 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cake.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2638 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/calendar.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1833 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/calling.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4236 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/camel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2243 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/camera.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4312 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cancer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4119 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/candy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3191 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/capital_abcd.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3517 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/capricorn.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1975 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1862 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/card_index.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4686 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/carousel_horse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3776 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4525 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cat_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1814 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cd.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2636 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2190 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart_with_downwards_trend.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2229 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart_with_upwards_trend.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1603 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/checkered_flag.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4296 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cherries.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4494 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cherry_blossom.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4032 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chestnut.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3136 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chicken.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3704 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/children_crossing.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2948 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chocolate_bar.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2974 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/christmas_tree.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5030 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/church.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2195 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cinema.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4225 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/circus_tent.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3232 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/city_sunrise.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2433 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/city_sunset.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2050 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cl.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3498 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clap.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3083 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clapper.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1661 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clipboard.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2304 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_1.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2327 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_10.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2441 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_10_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2381 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_11.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2443 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_11_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2275 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_12.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2314 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_12_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2372 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_1_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2314 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2424 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_2_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2215 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_3.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2329 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_3_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2320 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_4.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2433 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_4_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2331 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_5.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2340 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_5_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2334 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_6.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2301 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_6_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2346 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_7.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2360 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_7_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2425 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_8.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2450 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_8_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2339 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_9.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2301 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_9_30.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1220 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_book.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2468 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_lock_with_key.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3108 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_umbrella.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2699 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cloud.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1442 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clubs.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2087 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cn.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2233 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cocktail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3398 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/coffee.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3998 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/collision.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      774 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/computer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4223 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confetti_ball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2524 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confounded.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2338 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confused.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2157 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/construction.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5682 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/construction_worker.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1753 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/convenience_store.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3797 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cookie.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2647 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cool.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4744 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2787 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/copyright.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4643 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/corn.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4653 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couple.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4203 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couple_with_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5150 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couplekiss.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2891 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cow.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3589 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cow_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1067 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/credit_card.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4285 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crocodile.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2577 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crossed_flags.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3511 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crown.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2879 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3497 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crying_cat_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3600 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crystal_ball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3427 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cupid.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2640 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/curly_loop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3296 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/currency_exchange.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4003 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/curry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4165 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/custard.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2705 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/customs.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3453 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cyclone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3937 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dancer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6305 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dancers.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3541 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dango.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3999 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3068 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dash.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2131 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/date.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2004 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/de.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2690 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/deciduous_tree.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2420 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/department_store.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2888 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/diamond_shape_with_dot_inside.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1496 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/diamonds.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2190 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/disappointed.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2614 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/disappointed_relieved.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3477 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dizzy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3155 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dizzy_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4208 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/do_not_litter.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3483 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dog.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4840 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dog_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1965 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dollar.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4006 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dolls.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4155 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dolphin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      613 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/door.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4452 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/doughnut.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5986 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dragon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5493 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dragon_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2739 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dress.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4163 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dromedary_camel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2408 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/droplet.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2732 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dvd.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1855 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/e_mail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3167 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ear.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5354 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ear_of_rice.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5364 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_africa.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4906 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_americas.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5199 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_asia.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2889 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/egg.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3166 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eggplant.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3251 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2139 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight_pointed_black_star.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3525 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight_pointed_blue_star.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1055 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/electric_plug.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3891 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/elephant.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1542 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/email.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2618 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/end.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1542 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/envelope.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2185 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/es.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1851 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/euro.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4491 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/european_castle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3644 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/european_post_office.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2317 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/evergreen_tree.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      981 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/exclamation.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1881 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/expressionless.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1846 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eyeglasses.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1326 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eyes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2803 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/facepunch.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3752 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/factory.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3738 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fallen_leaf.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5579 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/family.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1819 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fast_forward.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2446 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fax.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2891 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fearful.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1135 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/feelsgood.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2463 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/feet.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5177 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ferris_wheel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1010 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/file_folder.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1151 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/finnadie.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3103 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fire.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2596 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fire_engine.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4864 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fireworks.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3509 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3153 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon_with_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2527 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fish.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3945 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fish_cake.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4449 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fishing_pole_and_fish.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3738 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fist.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2968 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/five.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3950 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flags.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2977 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flashlight.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1090 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/floppy_disk.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1313 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flower_playing_cards.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3881 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flushed.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3349 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/foggy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4180 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/football.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5309 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fountain.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2538 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/four.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3457 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/four_leaf_clover.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1882 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fr.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2153 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/free.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5341 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fried_shrimp.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3371 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fries.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3297 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/frog.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2264 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/frowning.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1666 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fu.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2568 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fuelpump.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3622 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/full_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4385 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/full_moon_with_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2402 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/game_die.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2603 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gb.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3117 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gem.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3067 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gemini.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2934 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ghost.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2566 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gift.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4213 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gift_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4284 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/girl.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4058 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/globe_with_meridians.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3412 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/goat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1266 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/goberserk.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1027 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/godmode.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1882 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/golf.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5025 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grapes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4112 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_apple.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      982 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_book.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2731 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      666 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grey_exclamation.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1132 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grey_question.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2587 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grimacing.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3046 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2985 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grinning.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2754 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/guardsman.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3142 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/guitar.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2237 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gun.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5410 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/haircut.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4084 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hamburger.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1186 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hammer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4108 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hamster.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2577 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hand.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2983 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/handbag.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hankey.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3132 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hash.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2789 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hatched_chick.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3544 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hatching_chick.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3441 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/headphones.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4375 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hear_no_evil.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2694 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2313 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_decoration.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3788 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_eyes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4499 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_eyes_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3138 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heartbeat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4696 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heartpulse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1955 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hearts.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2315 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_check_mark.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1424 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_division_sign.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2282 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_dollar_sign.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      981 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_exclamation_mark.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      282 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_minus_sign.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2623 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_multiplication.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      603 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_plus_sign.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2867 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/helicopter.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4732 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/herb.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4687 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hibiscus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2750 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/high_brightness.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2464 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/high_heel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1801 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hocho.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4961 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/honey_pot.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3574 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/honeybee.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3480 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/horse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5467 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/horse_racing.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1357 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hospital.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2564 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hotel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3789 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hotsprings.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2403 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hourglass.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2641 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hourglass_flowing_sand.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3739 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/house.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4766 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/house_with_garden.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4103 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hundred.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1375 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hurtrealbad.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2434 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hushed.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5541 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ice_cream.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3214 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/icecream.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1858 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/id.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2817 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/imp.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1674 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/inbox_tray.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1662 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/incoming_envelope.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4413 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/information_desk_person.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1109 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/information_source.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3646 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/innocent.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2619 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/interrobang.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1250 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/iphone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1873 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/it.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2402 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/izakaya_lantern.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3726 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jack_o_lantern.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2852 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japan.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4543 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_castle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3945 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_goblin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4434 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_ogre.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2390 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jeans.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3461 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/joy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4143 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/joy_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2213 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jp.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2233 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/key.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3165 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/keycap_ten.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3426 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kimono.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3695 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kiss.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2143 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4259 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3578 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_closed_eyes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3518 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2261 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_smiling_eyes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1338 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/knife_and_fork.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2833 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/koala.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1531 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/koko.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2460 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kr.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3278 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3123 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon_with_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3282 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/laughing.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3517 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leaves.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1591 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ledger.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2274 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/left_luggage.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3569 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lemon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3669 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leo.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4680 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leopard.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3258 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/libra.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1338 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/light_rail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1584 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/link.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2486 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lips.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1459 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lipstick.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1050 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lock.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2229 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lock_with_ink_pen.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3930 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lollipop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3419 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/loop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2484 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/loudspeaker.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3488 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/love_hotel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2682 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/love_letter.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2384 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/low_brightness.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4470 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/m.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3598 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mag.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3543 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mag_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3350 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/magic_8_ball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1904 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mahjong.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1725 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1655 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_closed.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2085 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_with_mail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1604 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_with_no_mail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3301 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3704 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man_with_gua_pi_mao.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3312 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man_with_turban.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1962 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mans_shoe.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3777 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/maple_leaf.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2822 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mask.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4834 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/massage.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3981 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/meat_on_bone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2983 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mega.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5528 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/melon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2496 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/memo.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2039 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mens.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2885 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/metal.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3028 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/microphone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3442 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/microscope.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4769 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/milky_way.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1865 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minibus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1623 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minidisc.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2890 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minus_1.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3000 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mobile_phone_off.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3862 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/money_with_wings.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2946 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moneybag.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4666 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monkey.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3343 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monkey_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1526 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monorail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4007 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1700 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mortar_board.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5321 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mount_fuji.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6540 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_bicyclist.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1746 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_cableway.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1467 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_railway.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3013 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mouse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3189 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mouse_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3338 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/movie_camera.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3297 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moyai.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2432 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/muscle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3919 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mushroom.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      995 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_keyboard.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2012 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_note.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1827 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_score.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4551 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mute.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4023 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nail_care.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3231 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/name_badge.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3204 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/neckbeard.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3419 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/necktie.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2734 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/negative_squared_cross_mark.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2087 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/neutral_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2435 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2046 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2664 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new_moon_with_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1964 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/newspaper.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2834 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ng.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3054 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nine.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4568 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_bell.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4561 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_bicycles.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3661 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_entry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5149 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_good.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3931 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_mobile_phones.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2008 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_mouth.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4203 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_pedestrians.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3756 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_smoking.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4088 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/non_potable_water.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2065 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nose.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      403 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/notebook.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1587 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/notebook_with_decorative_cover.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2280 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/notes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1204 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nut_and_bolt.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2848 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/o.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4333 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ocean.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2468 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/octocat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5203 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/octopus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3118 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oden.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1791 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/office.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2978 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2737 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok_hand.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4257 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok_woman.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3364 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/older_man.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3942 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/older_woman.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3126 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/on.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2765 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_automobile.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1606 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_bus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2257 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_police_car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3563 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_taxi.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2061 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/one.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2887 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/one_two_three_four.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1255 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_file_folder.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2690 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_hands.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2236 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_mouth.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3549 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ophiuchus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      817 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/orange_book.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1268 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/orange_diamond.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1666 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/outbox_tray.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3749 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ox.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      832 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/page_facing_up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      841 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/page_with_curl.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2423 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pager.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4534 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/palm_tree.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3013 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/panda_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1395 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/paperclip.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1721 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/parking.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2459 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/part_alternation_mark.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3586 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/partly_sunny.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2799 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/passport_control.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2463 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/paw_prints.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4423 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/peach.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3303 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pear.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2496 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pencil.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2855 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pencil_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2622 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/penguin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2320 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pensive.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4427 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/performing_arts.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2640 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/persevere.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2016 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/phone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2594 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3188 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2451 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig_nose.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2896 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pill.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5237 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pineapple.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3500 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pisces.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4062 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pizza.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2936 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/plus_1.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1822 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_down.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1681 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_left.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1692 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_right.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2676 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1744 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_up_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1972 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/police_car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3377 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poodle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poop.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2850 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/post_office.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3586 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/postal_horn.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1488 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/postbox.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2597 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/potable_water.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2678 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pouch.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3233 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poultry_leg.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1731 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pound.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3410 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pouting_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2660 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pray.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4076 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/princess.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2803 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/punch.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2599 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/purple_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3300 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/purse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2662 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pushpin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3164 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/put_litter_in_its_place.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1834 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/question.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3178 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rabbit.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3248 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rabbit_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4356 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/racehorse.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2876 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/radio.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4416 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/radio_button.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2455 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1067 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_1.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1066 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1093 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_3.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1196 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_4.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1467 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/railway_car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2633 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rainbow.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2577 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raised_hand.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3689 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raised_hands.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4980 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raising_hand.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4414 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ram.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6109 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ramen.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3710 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3454 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/recycle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1975 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/red_car.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1736 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/red_circle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2735 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/registered.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3389 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/relaxed.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2620 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/relieved.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2543 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/repeat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3003 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/repeat_once.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3423 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/restroom.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3658 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/revolving_hearts.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1787 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rewind.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4245 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ribbon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3634 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3562 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_ball.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3427 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_cracker.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3037 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_scene.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3237 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ring.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2984 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rocket.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4442 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/roller_coaster.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4421 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rooster.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3055 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rose.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2058 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rotating_light.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1581 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/round_pushpin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3481 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rowboat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2085 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ru.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3418 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rugby_football.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3426 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/runner.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3426 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/running.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2774 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/running_shirt_with_sash.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3083 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sagittarius.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2737 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sailboat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1761 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sake.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2072 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sandal.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3115 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/santa.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3935 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/satelite.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3282 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/satisfied.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3115 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/saxophone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3947 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/school.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2504 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/school_satchel.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3615 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scissors.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3368 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scorpius.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3650 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scream.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4217 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scream_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2150 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scroll.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2128 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4564 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/see_no_evil.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2920 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seedling.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2511 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seven.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4544 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shaved_ice.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3580 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sheep.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3739 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shell.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2104 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ship.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4612 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shipit.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1832 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shirt.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shit.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1962 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shoe.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2897 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shower.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1303 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/signal_strength.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3052 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/six.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3103 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/six_pointed_star.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4040 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ski.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1341 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/skull.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2671 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sleeping.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2807 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sleepy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2656 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/slot_machine.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      687 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_blue_diamond.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      660 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_orange_diamond.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      798 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_down.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      795 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3064 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smile.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3845 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smile_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3170 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiley.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3799 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiley_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2811 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiling_imp.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2469 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smirk.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3253 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smirk_cat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1806 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smoking.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3579 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snail.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4975 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snake.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4541 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowboarder.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4584 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowflake.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3566 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowman.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3735 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sob.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3134 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/soccer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3445 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/soon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3567 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sos.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3000 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sound.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1490 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/space_invader.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1545 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/spades.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6019 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/spaghetti.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4155 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkler.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2167 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkles.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3881 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkling_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3840 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speak_no_evil.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1934 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speaker.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1168 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speech_balloon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2675 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speedboat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2800 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/star.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3291 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/star_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3645 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stars.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3162 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/station.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3958 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/statue_of_liberty.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2592 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/steam_locomotive.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4962 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stew.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1406 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/straight_ruler.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4928 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/strawberry.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2787 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2963 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_closed_eyes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3399 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_winking_eye.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3657 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sun_with_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4760 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunflower.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2547 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunglasses.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3063 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunny.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3307 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunrise.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4700 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunrise_over_mountains.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5892 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/surfer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4926 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sushi.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1004 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/suspect.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1927 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/suspension_railway.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2719 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3577 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat_drops.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3425 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat_smile.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3503 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweet_potato.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3221 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/swimmer.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3114 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/symbols.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2835 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/syringe.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3258 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tada.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4088 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tanabata_tree.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3805 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tangerine.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3620 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/taurus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2303 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/taxi.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3391 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tea.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2016 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telephone.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1321 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telephone_receiver.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4243 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telescope.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5057 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tennis.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3488 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tent.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1718 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thought_balloon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3172 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/three.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2890 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thumbsdown.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2936 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thumbsup.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1483 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ticket.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3606 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tiger.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4624 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tiger_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2910 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tired_face.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1291 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tm.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1951 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/toilet.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1792 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tokyo_tower.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3722 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tomato.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2879 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tongue.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2563 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/top.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2466 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tophat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3663 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tractor.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1762 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/traffic_light.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1765 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/train.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2620 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/train_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2375 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tram.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1158 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triangular_flag_on_post.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1659 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triangular_ruler.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2993 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trident.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3768 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triumph.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1884 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trolleybus.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2739 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trollface.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3756 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trophy.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2675 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tropical_drink.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4442 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tropical_fish.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1831 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/truck.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3818 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trumpet.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1832 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tshirt.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3017 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tulip.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3914 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/turtle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4451 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tv.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2929 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3155 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_hearts.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4393 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_men_holding_hands.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4573 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_women_holding_hands.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2603 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/uk.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3455 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/umbrella.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2437 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/unamused.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4420 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/underage.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1090 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/unlock.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2507 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/up.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2699 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/us.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3155 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/v.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1836 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vertical_traffic_light.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2125 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vhs.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2818 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vibration_mode.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2772 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/video_camera.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2695 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/video_game.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4357 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/violin.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3830 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/virgo.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4563 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/volcano.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3057 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vs.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2406 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/walking.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3802 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waning_cresent_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3874 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waning_gibbous_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1906 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/warning.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2818 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/watch.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3480 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/water_buffalo.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3256 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/watermelon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3409 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wave.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      949 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wavy_dash.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3922 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waxing_cresent_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4007 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waxing_gibbous_moon.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3048 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wc.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2927 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/weary.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4787 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wedding.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3858 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/whale.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3545 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/whale_2.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1099 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/white_circle.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3393 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/white_flower.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      479 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/white_square_button.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3438 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wind_chime.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2334 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wine_glass.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2442 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wink.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2293 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wolf.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3449 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/woman.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2986 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womans_clothes.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2998 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womans_hat.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2154 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womens.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2453 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/worried.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1123 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wrench.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2370 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/x.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2786 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yellow_heart.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1769 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yen.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2812 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yum.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1895 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zap.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2893 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zero.png
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2743 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zzz.png
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.108677 borb-2.1.9/borb/pdf/canvas/layout/forms/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9888 2022-11-27 23:45:56.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/check_box.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7142 2022-10-06 18:22:46.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/country_drop_down_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9793 2022-10-06 18:22:46.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/drop_down_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2395 2022-11-21 13:50:20.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/form_field.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13136 2022-09-14 21:34:56.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/push_button.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9601 2022-10-06 17:23:24.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/text_area.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8315 2022-10-04 05:08:13.000000 borb-2.1.9/borb/pdf/canvas/layout/forms/text_field.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7043 2022-08-30 16:54:08.000000 borb-2.1.9/borb/pdf/canvas/layout/free_space_finder.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2290 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/horizontal_rule.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.108677 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6112 2022-04-06 21:39:43.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/hyphenation.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.116677 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   174033 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/af.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      894 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/as.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    57726 2021-12-11 21:07:39.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/be.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   123484 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/bg.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1009 2021-12-11 21:09:27.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/bn.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13523 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ca.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   103675 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/cy.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    16472 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/da.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   340992 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/de.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   131733 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/en-gb.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    76272 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/en-us.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    54781 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/es.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    56508 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/et.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4144 2021-12-11 21:15:22.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/fi.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    19269 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/fr.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    22354 2021-12-11 21:18:46.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/lt.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   198747 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/nl.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9285 2021-12-11 21:32:33.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ro.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   131354 2021-12-11 21:06:35.000000 borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ru.json
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.116677 borb-2.1.9/borb/pdf/canvas/layout/image/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/image/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6162 2022-09-05 20:03:21.000000 borb-2.1.9/borb/pdf/canvas/layout/image/barcode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3034 2022-09-02 07:45:16.000000 borb-2.1.9/borb/pdf/canvas/layout/image/chart.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5367 2023-01-18 18:17:17.000000 borb-2.1.9/borb/pdf/canvas/layout/image/image.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2985 2022-10-17 13:35:37.000000 borb-2.1.9/borb/pdf/canvas/layout/image/unsplash.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    22768 2022-10-04 04:47:44.000000 borb-2.1.9/borb/pdf/canvas/layout/layout_element.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.116677 borb-2.1.9/borb/pdf/canvas/layout/list/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/list/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7752 2022-09-04 00:50:52.000000 borb-2.1.9/borb/pdf/canvas/layout/list/list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2860 2022-03-30 11:06:17.000000 borb-2.1.9/borb/pdf/canvas/layout/list/ordered_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1570 2022-04-06 20:40:41.000000 borb-2.1.9/borb/pdf/canvas/layout/list/roman_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3354 2022-03-30 11:06:17.000000 borb-2.1.9/borb/pdf/canvas/layout/list/unordered_list.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.120677 borb-2.1.9/borb/pdf/canvas/layout/page_layout/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3953 2022-09-09 11:24:00.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/block_flow.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4437 2022-11-28 08:43:39.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/header_footer_multi_column_layout.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3948 2022-12-01 16:04:11.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/inline_flow.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8682 2022-09-26 09:56:11.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/multi_column_layout.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1239 2022-06-18 22:06:05.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/page_layout.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5821 2022-11-28 08:53:11.000000 borb-2.1.9/borb/pdf/canvas/layout/page_layout/single_column_layout_with_overflow.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.120677 borb-2.1.9/borb/pdf/canvas/layout/shape/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/shape/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8128 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/shape/connected_shape.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7228 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/shape/disconnected_shape.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6937 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/shape/gradient_colored_disconnected_shape.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5912 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/shape/progressbar.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.120677 borb-2.1.9/borb/pdf/canvas/layout/smart_art/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/smart_art/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    48671 2022-10-17 14:44:50.000000 borb-2.1.9/borb/pdf/canvas/layout/smart_art/smart_art.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.124677 borb-2.1.9/borb/pdf/canvas/layout/table/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/table/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7275 2022-09-05 20:03:21.000000 borb-2.1.9/borb/pdf/canvas/layout/table/fixed_column_width_table.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13210 2023-01-18 18:17:17.000000 borb-2.1.9/borb/pdf/canvas/layout/table/flexible_column_width_table.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    18570 2022-09-29 14:15:52.000000 borb-2.1.9/borb/pdf/canvas/layout/table/table.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3443 2022-09-02 07:45:16.000000 borb-2.1.9/borb/pdf/canvas/layout/table/table_util.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.128677 borb-2.1.9/borb/pdf/canvas/layout/text/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/layout/text/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9618 2022-09-17 00:46:45.000000 borb-2.1.9/borb/pdf/canvas/layout/text/chunk_of_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4543 2022-09-05 20:03:21.000000 borb-2.1.9/borb/pdf/canvas/layout/text/codeblock.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5777 2022-09-02 16:42:40.000000 borb-2.1.9/borb/pdf/canvas/layout/text/heading.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12275 2022-11-28 08:39:12.000000 borb-2.1.9/borb/pdf/canvas/layout/text/heterogeneous_paragraph.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7624 2022-09-05 20:03:21.000000 borb-2.1.9/borb/pdf/canvas/layout/text/line_of_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    16509 2022-11-06 12:57:31.000000 borb-2.1.9/borb/pdf/canvas/layout/text/paragraph.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.128677 borb-2.1.9/borb/pdf/canvas/line_art/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/line_art/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3702 2022-04-06 13:09:41.000000 borb-2.1.9/borb/pdf/canvas/line_art/blob_factory.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    56858 2022-08-01 18:58:23.000000 borb-2.1.9/borb/pdf/canvas/line_art/line_art_factory.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6341 2022-03-06 09:58:24.000000 borb-2.1.9/borb/pdf/canvas/line_art/rectangular_hitomezashi.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5201 2022-04-06 22:39:18.000000 borb-2.1.9/borb/pdf/canvas/line_art/rectangular_maze_factory.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.128677 borb-2.1.9/borb/pdf/canvas/lipsum/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/lipsum/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7831 2022-09-26 20:27:11.000000 borb-2.1.9/borb/pdf/canvas/lipsum/lipsum.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.132677 borb-2.1.9/borb/pdf/canvas/lipsum/resources/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   314156 2022-09-22 22:10:50.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_agatha_christie.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    97075 2022-09-22 22:10:57.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_alan_alexander_milne.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   326591 2022-09-22 22:10:56.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_arthur_conan_doyle.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   577242 2022-09-22 22:10:53.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_emily_bronte.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   554298 2022-09-22 22:10:48.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_jane_austen.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   118929 2022-09-22 22:10:59.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_lewis_carroll.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    64293 2022-09-22 22:10:42.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_lipsum.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)   440228 2022-09-22 22:10:44.000000 borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_mary_shelley.json
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     9374 2022-09-26 20:27:11.000000 borb-2.1.9/borb/pdf/canvas/lipsum/text_generator.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.136677 borb-2.1.9/borb/pdf/canvas/operator/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1650 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/canvas_operator.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.136677 borb-2.1.9/borb/pdf/canvas/operator/color/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/color/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1396 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_cmyk_non_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2101 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_cmyk_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3892 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_color_non_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4135 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_color_space_non_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7044 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_color_space_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     4697 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_color_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1012 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_gray_non_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1385 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_gray_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1346 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_rgb_non_stroking.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1765 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/color/set_rgb_stroking.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.140677 borb-2.1.9/borb/pdf/canvas/operator/compatibility/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/compatibility/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1067 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/compatibility/begin_compatibility_section.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1066 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/compatibility/end_compatibility_section.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.140677 borb-2.1.9/borb/pdf/canvas/operator/marked_content/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/marked_content/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1143 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/marked_content/begin_marked_content.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1671 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/marked_content/begin_marked_content_with_property_list.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      907 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/marked_content/end_marked_content.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.140677 borb-2.1.9/borb/pdf/canvas/operator/path_construction/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6862 2022-08-30 16:54:09.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_cubic_bezier.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1535 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_line_segment.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2720 2021-11-04 18:40:55.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_rectangle.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1745 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/begin_subpath.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1743 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/path_construction/close_subpath.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.144677 borb-2.1.9/borb/pdf/canvas/operator/path_painting/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/path_painting/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1275 2021-10-06 10:31:32.000000 borb-2.1.9/borb/pdf/canvas/operator/path_painting/close_and_stroke_path.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      160 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/operator/path_painting/fill_path_even_odd.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      263 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/canvas/operator/path_painting/fill_path_nonzero_winding.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1038 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/path_painting/stroke_path.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.144677 borb-2.1.9/borb/pdf/canvas/operator/state/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/state/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2033 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/state/modify_transformation_matrix.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1203 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/state/pop_graphics_state.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      974 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/state/push_graphics_state.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      985 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/state/set_line_width.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.148677 borb-2.1.9/borb/pdf/canvas/operator/text/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/text/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1412 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/begin_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1021 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/end_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1869 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/move_text_position.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2111 2022-01-22 13:52:13.000000 borb-2.1.9/borb/pdf/canvas/operator/text/move_text_position_set_leading.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1805 2022-01-22 13:52:13.000000 borb-2.1.9/borb/pdf/canvas/operator/text/move_to_next_line.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1488 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/move_to_next_line_show_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1254 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_character_spacing.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2034 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_font_and_size.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1188 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_horizontal_text_scaling.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2342 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_spacing_move_to_next_line_show_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1188 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_text_leading.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1948 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_text_matrix.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)      855 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_text_rendering_mode.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1051 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_text_rise.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1189 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/text/set_word_spacing.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1684 2022-04-07 12:44:28.000000 borb-2.1.9/borb/pdf/canvas/operator/text/show_text.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3363 2021-11-09 18:48:52.000000 borb-2.1.9/borb/pdf/canvas/operator/text/show_text_with_glyph_positioning.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.148677 borb-2.1.9/borb/pdf/canvas/operator/xobject/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/canvas/operator/xobject/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2840 2021-09-24 22:18:59.000000 borb-2.1.9/borb/pdf/canvas/operator/xobject/do.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    13534 2022-09-29 11:33:14.000000 borb-2.1.9/borb/pdf/canvas/redacted_canvas_stream_processor.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.148677 borb-2.1.9/borb/pdf/document/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/document/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    17412 2022-10-04 05:08:13.000000 borb-2.1.9/borb/pdf/document/document.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6733 2022-08-30 16:54:10.000000 borb-2.1.9/borb/pdf/document/name_tree.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.148677 borb-2.1.9/borb/pdf/page/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/page/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11035 2022-11-03 15:24:12.000000 borb-2.1.9/borb/pdf/page/page.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6577 2022-09-04 13:48:08.000000 borb-2.1.9/borb/pdf/page/page_info.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2974 2021-08-01 19:20:26.000000 borb-2.1.9/borb/pdf/page/page_size.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3551 2023-01-18 09:11:41.000000 borb-2.1.9/borb/pdf/pdf.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.148677 borb-2.1.9/borb/pdf/trailer/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/trailer/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    16344 2022-10-04 04:49:32.000000 borb-2.1.9/borb/pdf/trailer/document_info.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/pdf/xref/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/pdf/xref/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5746 2022-06-18 22:29:21.000000 borb-2.1.9/borb/pdf/xref/plaintext_xref.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6137 2022-09-04 19:06:36.000000 borb-2.1.9/borb/pdf/xref/rebuilt_xref.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8979 2022-06-18 22:55:05.000000 borb-2.1.9/borb/pdf/xref/stream_xref.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8881 2023-01-30 10:37:38.000000 borb-2.1.9/borb/pdf/xref/xref.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3862 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/color/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/color/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8029 2022-11-30 15:03:46.000000 borb-2.1.9/borb/toolkit/color/color_extraction.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/export/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/toolkit/export/__init__.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/export/html_to_pdf/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/toolkit/export/html_to_pdf/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    36107 2022-11-28 08:39:24.000000 borb-2.1.9/borb/toolkit/export/html_to_pdf/html_to_pdf.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/export/markdown_to_pdf/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/toolkit/export/markdown_to_pdf/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     7592 2022-09-17 22:52:52.000000 borb-2.1.9/borb/toolkit/export/markdown_to_pdf/markdown_to_pdf.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6770 2022-11-28 08:40:12.000000 borb-2.1.9/borb/toolkit/export/pdf_to_jpg.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6007 2022-11-28 08:36:27.000000 borb-2.1.9/borb/toolkit/export/pdf_to_mp3.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     8131 2022-11-28 08:36:27.000000 borb-2.1.9/borb/toolkit/export/pdf_to_svg.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/image/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/image/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3089 2022-11-30 15:03:46.000000 borb-2.1.9/borb/toolkit/image/image_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2570 2022-09-26 15:39:31.000000 borb-2.1.9/borb/toolkit/image/image_format_optimization.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.152677 borb-2.1.9/borb/toolkit/location/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/location/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2366 2022-08-30 10:25:09.000000 borb-2.1.9/borb/toolkit/location/location_filter.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.156677 borb-2.1.9/borb/toolkit/ocr/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/toolkit/ocr/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6767 2022-09-14 20:13:39.000000 borb-2.1.9/borb/toolkit/ocr/ocr_as_optional_content_group.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    12822 2022-09-14 21:34:57.000000 borb-2.1.9/borb/toolkit/ocr/ocr_image_render_event_listener.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.156677 borb-2.1.9/borb/toolkit/redact/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:40.000000 borb-2.1.9/borb/toolkit/redact/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6224 2021-08-01 19:20:26.000000 borb-2.1.9/borb/toolkit/redact/common_regular_expressions.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.156677 borb-2.1.9/borb/toolkit/table/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/table/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14061 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/table/table_detection_by_lines.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:27.160677 borb-2.1.9/borb/toolkit/text/
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2093 2022-12-09 14:35:39.000000 borb-2.1.9/borb/toolkit/text/__init__.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2072 2022-06-18 22:06:05.000000 borb-2.1.9/borb/toolkit/text/font_color_filter.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     2147 2022-12-02 09:06:17.000000 borb-2.1.9/borb/toolkit/text/font_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1500 2022-06-18 22:06:05.000000 borb-2.1.9/borb/toolkit/text/font_name_filter.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    14916 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/regular_expression_text_extraction.py
+-rw-rw-r--   0 joris     (1000) joris     (1000)     5106 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/simple_find_replace.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6355 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/simple_line_of_text_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     3683 2022-12-02 09:49:07.000000 borb-2.1.9/borb/toolkit/text/simple_non_ligature_text_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6996 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/simple_paragraph_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     5092 2022-12-02 09:49:07.000000 borb-2.1.9/borb/toolkit/text/simple_text_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)    11000 2021-08-01 19:20:26.000000 borb-2.1.9/borb/toolkit/text/stop_words.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6480 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/text_rank_keyword_extraction.py
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     6924 2022-12-02 23:11:49.000000 borb-2.1.9/borb/toolkit/text/tf_idf_keyword_extraction.py
+drwxrwxr-x   0 joris     (1000) joris     (1000)        0 2023-02-17 17:20:26.824676 borb-2.1.9/borb.egg-info/
+-rw-rw-r--   0 joris     (1000) joris     (1000)     4283 2023-02-17 17:20:26.000000 borb-2.1.9/borb.egg-info/PKG-INFO
+-rw-rw-r--   0 joris     (1000) joris     (1000)    72026 2023-02-17 17:20:26.000000 borb-2.1.9/borb.egg-info/SOURCES.txt
+-rw-rw-r--   0 joris     (1000) joris     (1000)        1 2023-02-17 17:20:26.000000 borb-2.1.9/borb.egg-info/dependency_links.txt
+-rw-rw-r--   0 joris     (1000) joris     (1000)      108 2023-02-17 17:20:26.000000 borb-2.1.9/borb.egg-info/requires.txt
+-rw-rw-r--   0 joris     (1000) joris     (1000)        5 2023-02-17 17:20:26.000000 borb-2.1.9/borb.egg-info/top_level.txt
+-rw-rw-r--   0 joris     (1000) joris     (1000)       38 2023-02-17 17:20:27.160677 borb-2.1.9/setup.cfg
+-rwxrwxrwx   0 joris     (1000) joris     (1000)     1140 2022-12-06 20:25:28.000000 borb-2.1.9/setup.py
```

### Comparing `borb-2.1.8/LICENSE.md` & `borb-2.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/PKG-INFO` & `borb-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: borb
-Version: 2.1.8
+Version: 2.1.9
 Summary: borb is a library for reading, creating and manipulating PDF files in python.
 Home-page: https://github.com/jorisschellekens/borb
 Author: Joris Schellekens
 Author-email: joris.schellekens.1989@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # ![borb logo](https://github.com/jorisschellekens/borb/raw/master/logo/borb_64.png) borb
 
@@ -115,7 +117,9 @@
 
 ## 3. Acknowledgements
 
 I would like to thank the following people, for their contributions / advice with regards to developing `borb`:
 - Aleksander Banasik
 - Benoît Lagae
 - Michael Klink
+
+
```

### Comparing `borb-2.1.8/README.md` & `borb-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/__init__.py` & `borb-2.1.9/borb/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/datastructure/__init__.py` & `borb-2.1.9/borb/datastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/datastructure/disjoint_set.py` & `borb-2.1.9/borb/datastructure/disjoint_set.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/datastructure/str_trie.py` & `borb-2.1.9/borb/datastructure/str_trie.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/__init__.py` & `borb-2.1.9/borb/io/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/__init__.py` & `borb-2.1.9/borb/io/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/ascii85_decode.py` & `borb-2.1.9/borb/io/filter/ascii85_decode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/flate_decode.py` & `borb-2.1.9/borb/io/filter/flate_decode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/lzw_decode.py` & `borb-2.1.9/borb/io/filter/lzw_decode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/run_length_decode.py` & `borb-2.1.9/borb/io/filter/run_length_decode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/filter/stream_decode_util.py` & `borb-2.1.9/borb/io/filter/stream_decode_util.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/__init__.py` & `borb-2.1.9/borb/io/read/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/any_object_transformer.py` & `borb-2.1.9/borb/io/read/any_object_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/encryption/__init__.py` & `borb-2.1.9/borb/io/read/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/encryption/rc4.py` & `borb-2.1.9/borb/io/read/encryption/rc4.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/encryption/standard_security_handler.py` & `borb-2.1.9/borb/io/read/encryption/standard_security_handler.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/font/__init__.py` & `borb-2.1.9/borb/io/read/font/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/font/font_dictionary_transformer.py` & `borb-2.1.9/borb/io/read/font/font_dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/function/__init__.py` & `borb-2.1.9/borb/io/read/function/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/function/function_dictionary_transformer.py` & `borb-2.1.9/borb/io/read/function/function_dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/__init__.py` & `borb-2.1.9/borb/io/read/image/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/ccitt_fax_image_transformer.py` & `borb-2.1.9/borb/io/read/image/ccitt_fax_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/compressed_jpeg_image_transformer.py` & `borb-2.1.9/borb/io/read/image/compressed_jpeg_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/grayscale_image_transformer.py` & `borb-2.1.9/borb/io/read/image/grayscale_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/jbig2_image_transformer.py` & `borb-2.1.9/borb/io/read/image/jbig2_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/jpeg_2000_image_transformer.py` & `borb-2.1.9/borb/io/read/image/jpeg_2000_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/image/jpeg_image_transformer.py` & `borb-2.1.9/borb/io/read/image/jpeg_image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/metadata/__init__.py` & `borb-2.1.9/borb/io/read/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/metadata/xmp_metadata_transformer.py` & `borb-2.1.9/borb/io/read/metadata/xmp_metadata_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/object/__init__.py` & `borb-2.1.9/borb/io/read/object/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/object/array_transformer.py` & `borb-2.1.9/borb/io/read/object/array_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/object/dictionary_transformer.py` & `borb-2.1.9/borb/io/read/object/dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/object/stream_transformer.py` & `borb-2.1.9/borb/io/read/object/stream_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/page/__init__.py` & `borb-2.1.9/borb/io/read/page/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/page/page_dictionary_transformer.py` & `borb-2.1.9/borb/io/read/page/page_dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/page/root_dictionary_transformer.py` & `borb-2.1.9/borb/io/read/page/root_dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/postfix/__init__.py` & `borb-2.1.9/borb/io/read/postfix/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/postfix/postfix_eval.py` & `borb-2.1.9/borb/io/read/postfix/postfix_eval.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/primitive/__init__.py` & `borb-2.1.9/borb/io/read/primitive/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/primitive/number_transformer.py` & `borb-2.1.9/borb/io/read/primitive/number_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/primitive/string_transformer.py` & `borb-2.1.9/borb/io/read/primitive/string_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/reference/__init__.py` & `borb-2.1.9/borb/io/read/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/reference/reference_transformer.py` & `borb-2.1.9/borb/io/read/reference/reference_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/reference/xref_transformer.py` & `borb-2.1.9/borb/io/read/reference/xref_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/tokenize/__init__.py` & `borb-2.1.9/borb/io/read/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/tokenize/high_level_tokenizer.py` & `borb-2.1.9/borb/io/read/tokenize/high_level_tokenizer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/tokenize/low_level_tokenizer.py` & `borb-2.1.9/borb/io/read/tokenize/low_level_tokenizer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/transformer.py` & `borb-2.1.9/borb/io/read/transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/read/types.py` & `borb-2.1.9/borb/io/read/types.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/__init__.py` & `borb-2.1.9/borb/io/write/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/any_object_transformer.py` & `borb-2.1.9/borb/io/write/any_object_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/conformance_level.py` & `borb-2.1.9/borb/io/write/conformance_level.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/document/__init__.py` & `borb-2.1.9/borb/io/write/document/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/document/catalog_transformer.py` & `borb-2.1.9/borb/io/write/document/catalog_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/document/document_transformer.py` & `borb-2.1.9/borb/io/write/document/document_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/document/information_dictionary_transformer.py` & `borb-2.1.9/borb/io/write/document/information_dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/document/resources/sRGB_CS_profile.icm` & `borb-2.1.9/borb/io/write/document/resources/sRGB_CS_profile.icm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/font/__init__.py` & `borb-2.1.9/borb/io/write/font/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/font/character_set_listener.py` & `borb-2.1.9/borb/io/write/font/character_set_listener.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/font/copy_command_operator.py` & `borb-2.1.9/borb/io/write/font/copy_command_operator.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/font/subset_show_text_with_glyph_positioning.py` & `borb-2.1.9/borb/io/write/font/subset_show_text_with_glyph_positioning.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/font/subsetter.py` & `borb-2.1.9/borb/io/write/font/subsetter.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/image/__init__.py` & `borb-2.1.9/borb/io/write/image/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/image/image_transformer.py` & `borb-2.1.9/borb/io/write/image/image_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/object/__init__.py` & `borb-2.1.9/borb/io/write/object/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/object/array_transformer.py` & `borb-2.1.9/borb/io/write/object/array_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/object/dictionary_transformer.py` & `borb-2.1.9/borb/io/write/object/dictionary_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/object/stream_transformer.py` & `borb-2.1.9/borb/io/write/object/stream_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/page/__init__.py` & `borb-2.1.9/borb/io/write/page/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/page/page_transformer.py` & `borb-2.1.9/borb/io/write/page/page_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/page/pages_transformer.py` & `borb-2.1.9/borb/io/write/page/pages_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/primitive/__init__.py` & `borb-2.1.9/borb/io/write/primitive/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/primitive/boolean_transformer.py` & `borb-2.1.9/borb/io/write/primitive/boolean_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/primitive/name_transformer.py` & `borb-2.1.9/borb/io/write/primitive/name_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/primitive/number_transformer.py` & `borb-2.1.9/borb/io/write/primitive/number_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/primitive/string_transformer.py` & `borb-2.1.9/borb/io/write/primitive/string_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/reference/__init__.py` & `borb-2.1.9/borb/io/write/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/reference/reference_transformer.py` & `borb-2.1.9/borb/io/write/reference/reference_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/reference/xref_transformer.py` & `borb-2.1.9/borb/io/write/reference/xref_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/transformer.py` & `borb-2.1.9/borb/io/write/transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/version/__init__.py` & `borb-2.1.9/borb/io/write/version/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/version/version_as_comment_transformer.py` & `borb-2.1.9/borb/io/write/version/version_as_comment_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/xmp/__init__.py` & `borb-2.1.9/borb/io/write/xmp/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/io/write/xmp/xmp_transformer.py` & `borb-2.1.9/borb/io/write/xmp/xmp_transformer.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/license/__init__.py` & `borb-2.1.9/borb/license/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/license/anonymous_user_id.py` & `borb-2.1.9/borb/license/anonymous_user_id.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/license/machine_id.py` & `borb-2.1.9/borb/license/machine_id.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/license/usage_statistics.py` & `borb-2.1.9/borb/license/usage_statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import sys
 import threading
 from datetime import datetime, timezone
 import typing
 
 import requests
 from borb.license.anonymous_user_id import AnonymousUserID
-
-from borb.license.geo_information import GeoInformation
 from borb.license.version import Version
 
 
 class UsageStatistics:
     """
     This class implements the basics for sending usage statistics to the borb server(s).
     These kinds of checks are useful to get an idea of which functionality is most often used,
@@ -86,22 +84,16 @@
                 )
         except:
             pass
 
         # set payload
         json_payload: typing.Dict[str, typing.Any] = {
             "anonymous_user_id": anonymous_user_id,
-            "city": GeoInformation.get_city(),
-            "country_code": GeoInformation.get_country_code(),
-            "country_name": GeoInformation.get_country_name(),
             "event": event,
-            "latitude": GeoInformation.get_latitude(),
-            "longitude": GeoInformation.get_longitude(),
             "number_of_pages": number_of_pages,
-            "state": GeoInformation.get_state(),
             "sys_platform": sys.platform,
             "utc_time_in_ms": int(datetime.now(timezone.utc).timestamp() * 1000),
             "version": Version.get_version(),
         }
 
         # set headers
         headers = {"Content-type": "application/json", "Accept": "text/plain"}
```

### Comparing `borb-2.1.8/borb/license/uuid.py` & `borb-2.1.9/borb/license/uuid.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/license/version.py` & `borb-2.1.9/borb/license/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     @staticmethod
     def get_version() -> str:
         """
         This function returns the current borb version
         :return:    the current borb version
         """
-        return "2.1.8"
+        return "2.1.9"
 
     @staticmethod
     def get_author() -> str:
         """
         This function returns the author of the borb library
         :return:    the author of the borb library
         """
```

### Comparing `borb-2.1.8/borb/pdf/__init__.py` & `borb-2.1.9/borb/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/__init__.py` & `borb-2.1.9/borb/pdf/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/canvas.py` & `borb-2.1.9/borb/pdf/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/canvas_graphics_state.py` & `borb-2.1.9/borb/pdf/canvas/canvas_graphics_state.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/canvas_stream_processor.py` & `borb-2.1.9/borb/pdf/canvas/canvas_stream_processor.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/color/__init__.py` & `borb-2.1.9/borb/pdf/canvas/color/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/color/color.py` & `borb-2.1.9/borb/pdf/canvas/color/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,23 @@
         g /= 255
         b /= 255
         super(HexColor, self).__init__(Decimal(r), Decimal(g), Decimal(b))
 
     def __deepcopy__(self, memodict={}):
         return HexColor(self.to_hex_string())
 
+    def __hash__(self):
+        return hash(self.to_hex_string())
+
+    def __eq__(self, other):
+        return (
+            isinstance(other, HexColor)
+            and other.to_hex_string() == self.to_hex_string()
+        )
+
 
 class HSVColor(Color):
     """
     HSL (hue, saturation, lightness) and HSV (hue, saturation, value, also known as HSB or hue, saturation, brightness)
     are alternative representations of the RGB color model, designed in the 1970s by computer graphics researchers
     to more closely align with the way human vision perceives color-making attributes.
     In these models, colors of each hue are arranged in a radial slice,
@@ -256,36 +265,36 @@
     def darker(self) -> "HSVColor":
         """
         This function returns a darker shade of the current HSV color
         """
         return HSVColor(self.hue, self.saturation, self.value * Decimal(0.8))
 
     @staticmethod
-    def complementary(color: Color):
-        """
-        This function returns an HSV color whose hue is the complement of the current HSV color
-        """
-        c: HSVColor = HSVColor.from_rgb(color.to_rgb())
-        new_hue: int = int(float(c.hue) * 360.0) + 180 % 360
-        return HSVColor(Decimal(new_hue / 360), c.saturation, c.value)
-
-    @staticmethod
     def analogous(color: Color) -> typing.List[Color]:
         """
         This function returns an analogous color scheme.
         Analogous color schemes use colors that are next to each other on the color wheel. They usually match well and create serene and comfortable designs.
         Analogous color schemes are often found in nature and are harmonious and pleasing to the eye.
         """
         c: HSVColor = HSVColor.from_rgb(color.to_rgb())
         return [
             HSVColor(Decimal((int(c.hue * 360 + a) % 360) / 360), c.saturation, c.value)
             for a in [0, 15, 30]
         ]
 
     @staticmethod
+    def complementary(color: Color):
+        """
+        This function returns an HSV color whose hue is the complement of the current HSV color
+        """
+        c: HSVColor = HSVColor.from_rgb(color.to_rgb())
+        new_hue: int = int(float(c.hue) * 360.0) + 180 % 360
+        return HSVColor(Decimal(new_hue / 360), c.saturation, c.value)
+
+    @staticmethod
     def split_complementary(color: Color) -> typing.List[Color]:
         """
         This function returns a split complementary color scheme.
         A split complementary color scheme uses two colors plus the color that is opposite to them on the color wheel.
         For example blue and purple with yellow.
         :param color:       the complementary color
         :return:            3 colors (a split complementary color scheme)
```

### Comparing `borb-2.1.8/borb/pdf/canvas/color/farrow_and_ball.py` & `borb-2.1.9/borb/pdf/canvas/color/farrow_and_ball.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/color/pantone.py` & `borb-2.1.9/borb/pdf/canvas/color/pantone.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/__init__.py` & `borb-2.1.9/borb/pdf/canvas/event/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/begin_page_event.py` & `borb-2.1.9/borb/pdf/canvas/event/begin_page_event.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/chunk_of_text_render_event.py` & `borb-2.1.9/borb/pdf/canvas/event/chunk_of_text_render_event.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/end_page_event.py` & `borb-2.1.9/borb/pdf/canvas/event/end_page_event.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/event_listener.py` & `borb-2.1.9/borb/pdf/canvas/event/event_listener.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/image_render_event.py` & `borb-2.1.9/borb/pdf/canvas/event/image_render_event.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/event/line_render_event.py` & `borb-2.1.9/borb/pdf/canvas/event/line_render_event.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/__init__.py` & `borb-2.1.9/borb/pdf/canvas/font/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/adobe_standard_encoding.py` & `borb-2.1.9/borb/pdf/canvas/font/adobe_standard_encoding.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/__init__.py` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cid_font_type_0.py` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cid_font_type_0.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cid_font_type_2.py` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cid_font_type_2.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/78ms-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/83pv-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/83pv-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90ms-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90msp-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/90pv-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Add-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Add-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-1` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-1`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-2` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-2`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-3` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-3`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-4` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-4`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-5` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-5`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-6` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-6`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-7` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-CNS1-7`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-1` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-1`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-2` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-2`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-3` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-3`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-4` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-4`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-5` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-GB1-5`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Identity-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-1` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-1`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-2` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-2`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-3` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-3`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-4` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-4`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-5` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-5`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-6` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-6`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-7` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan1-7`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan2-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Japan2-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-1` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-1`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-2` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-2`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-3` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-3`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-4` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-4`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-5` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-5`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-6` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-6`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-7` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-7`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-8` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-8`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-9` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-KR-9`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-0` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-0`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-1` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-1`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-2` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Adobe-Korea1-2`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5pc-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5pc-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/B5pc-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/B5pc-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS1-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS1-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS1-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS1-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/CNS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/CNS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETHK-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETen-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/ETenms-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Ext-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Ext-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GB-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GB-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBK2K-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBKp-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBT-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBT-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBTpc-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/GBpc-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdla-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKdlb-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKgccs-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm314-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKm471-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/HKscs-B5-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hankaku` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hankaku`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hiragana` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hiragana`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Hojo-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Hojo-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-Johab-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-HW-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCms-UHC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/KSCpc-EUC-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Katakana` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Katakana`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/NWP-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/NWP-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/NWP-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/NWP-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/RKSJ-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/Roman` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/Roman`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniAKR-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniCNS-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniGB-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniHojo-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-HW-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJIS2004-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-HW-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-HW-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISPro-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX0213-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniJISX02132004-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UCS2-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF16-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF32-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-H` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-H`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/UniKS-UTF8-V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/V` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/V`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/WP-Symbol` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/WP-Symbol`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/cmaps/__init__.py` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/cmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/composite_font/font_type_0.py` & `borb-2.1.9/borb/pdf/canvas/font/composite_font/font_type_0.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/font.py` & `borb-2.1.9/borb/pdf/canvas/font/font.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/glyph_line.py` & `borb-2.1.9/borb/pdf/canvas/font/glyph_line.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/__init__.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/__init__.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-bold-oblique.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-bold-oblique.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-bold.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-bold.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier-oblique.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier-oblique.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/courier.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/courier.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-bold-oblique.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-bold-oblique.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-bold.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-bold.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica-oblique.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica-oblique.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/helvetica.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/helvetica.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/symbol.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/symbol.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-bold-italic.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-bold-italic.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-bold.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-bold.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-italic.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-italic.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/times-roman.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/times-roman.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/afm/zapfdingbats.afm` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/afm/zapfdingbats.afm`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/font_type_1.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/font_type_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from fontTools.afmLib import AFM  # type: ignore [import]
 from fontTools.agl import toUnicode  # type: ignore [import]
 from fontTools.cffLib import CFFFontSet, TopDict  # type: ignore [import]
 
 from borb.io.read.types import Decimal as bDecimal
 from borb.io.read.types import Dictionary, Name
+from borb.pdf.canvas.font.adobe_glyph_list import AdobeGlyphList
 from borb.pdf.canvas.font.adobe_standard_encoding import (
     adobe_standard_decode,
     adobe_standard_encode,
 )
 from borb.pdf.canvas.font.font import Font
 from borb.pdf.canvas.font.simple_font.simple_font import SimpleFont
 from borb.pdf.canvas.font.symbol_encoding import symbol_decode, zapfdingbats_decode
@@ -488,22 +489,24 @@
 
     def get_width(self, character_identifier: int) -> typing.Optional[bDecimal]:
         """
         This function returns the width (in text space) of a given character identifier.
         If this Font is unable to represent the glyph that corresponds to the character identifier,
         this function returns None
         """
-        widths: typing.List[bDecimal] = [
-            bDecimal(v[1])
-            for k, v in self._afm._chars.items()
-            if v[0] == character_identifier
-        ]
-        if len(widths) == 1:
-            return widths[0]
-        return bDecimal(0)
+        default_tuple: typing.Tuple[int, int, typing.Tuple[int, int, int, int]] = (
+            0,
+            0,
+            (0, 0, 0, 0),
+        )
+        name: typing.Optional[str] = AdobeGlyphList.UNICODE_TO_NAME.get(
+            ord(self._character_identifier_to_unicode_lookup[character_identifier]),
+            None,
+        )
+        return bDecimal(self._afm._chars.get(name, default_tuple)[1])
 
     def get_ascent(self) -> bDecimal:
         """
         This function returns the maximum height above the baseline reached by glyphs in this font.
         The height of glyphs for accented characters shall be excluded.
         """
         if "Ascender" in self._afm._attrs:
```

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/font_type_3.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/font_type_3.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/simple_font.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/simple_font.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/simple_font/true_type_font.py` & `borb-2.1.9/borb/pdf/canvas/font/simple_font/true_type_font.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/font/symbol_encoding.py` & `borb-2.1.9/borb/pdf/canvas/font/symbol_encoding.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/geometry/__init__.py` & `borb-2.1.9/borb/pdf/canvas/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/geometry/line_segment.py` & `borb-2.1.9/borb/pdf/canvas/geometry/line_segment.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/geometry/matrix.py` & `borb-2.1.9/borb/pdf/canvas/geometry/matrix.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/geometry/rectangle.py` & `borb-2.1.9/borb/pdf/canvas/geometry/rectangle.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/caret_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/caret_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/circle_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/circle_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/file_attachment_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/file_attachment_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/free_text_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/free_text_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/highlight_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/highlight_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/ink_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/ink_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/line_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/line_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/link_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/link_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/movie_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/movie_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/polygon_annotion.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/polygon_annotion.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/polyline_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/polyline_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/popup_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/popup_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/printer_mark_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/printer_mark_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/redact_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/redact_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/remote_go_to_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/remote_go_to_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/rubber_stamp_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/rubber_stamp_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/screen_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/screen_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/sound_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/sound_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/square_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/square_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/squiggly_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/squiggly_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/strike_out_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/strike_out_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/text_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/text_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/three_d_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/three_d_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/underline_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/underline_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/watermark_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/watermark_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/annotation/widget_annotation.py` & `borb-2.1.9/borb/pdf/canvas/layout/annotation/widget_annotation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/emoji.py` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/emoji.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/a.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/a.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ab.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ab.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/abc.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/abc.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/abcd.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/abcd.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aerial_tramway.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aerial_tramway.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/airplane.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/airplane.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/alarm_clock.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/alarm_clock.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/alien.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/alien.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ambulance.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ambulance.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anchor.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anchor.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/angel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/angel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anger.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anger.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/angry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/angry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/anguished.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/anguished.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ant.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ant.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/apple.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/apple.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aquarius.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aquarius.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/aries.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/aries.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_backward.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_backward.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_double_down.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_double_down.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_double_up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_double_up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down_hook.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down_hook.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_down_small.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_down_small.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_forward.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_forward.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left_hook.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left_hook.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_left_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_left_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_lower_left.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_lower_left.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_lower_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_lower_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_right_hook.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_right_hook.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_down.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_down.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_hook.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_hook.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_up_small.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_up_small.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_upper_left.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_upper_left.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrow_upper_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrow_upper_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_clockwise.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_clockwise.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_counterclockwise.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_counterclockwise.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/arrows_right_twisted.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/arrows_right_twisted.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/art.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/art.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/articulated_lorry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/articulated_lorry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/astonished.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/astonished.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/atm.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/atm.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/b.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/b.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_bottle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_bottle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_chick.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_chick.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baby_symbol.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baby_symbol.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bagage_claim.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bagage_claim.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/balloon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/balloon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ballot_box_with_check.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ballot_box_with_check.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bamboo.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bamboo.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/banana.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/banana.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bang_bang.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bang_bang.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bank.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bank.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bar_chart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bar_chart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/barber.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/barber.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/baseball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/baseball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/basketball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/basketball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bath.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bath.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bathtub.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bathtub.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/battery.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/battery.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bear.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bear.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beers.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beers.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beetle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beetle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/beginner.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/beginner.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bell.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bell.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bento.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bento.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bicyclist.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bicyclist.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bike.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bike.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bikini.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bikini.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bird.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bird.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/birthday.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/birthday.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_circle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_circle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_joker.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_joker.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/black_nib.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/black_nib.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blossom.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blossom.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blowfish.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blowfish.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_book.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_book.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_circle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_circle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_diamond.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_diamond.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blue_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blue_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/blush.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/blush.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boar.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boar.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bomb.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bomb.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/book.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/book.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bookmark.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bookmark.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bookmark_tabs.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bookmark_tabs.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/books.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/books.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boom.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boom.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boot.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boot.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bouquet.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bouquet.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bow.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bow.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bowling.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bowling.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bowtie.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bowtie.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/boy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/boy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bread.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bread.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bride_with_veil.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bride_with_veil.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bridge_at_night.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bridge_at_night.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/briefcase.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/briefcase.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/broken_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/broken_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bug.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bug.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bulb.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bulb.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bullettrain_front.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bullettrain_front.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bullettrain_side.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bullettrain_side.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/busstop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/busstop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/bust_in_silhouette.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/bust_in_silhouette.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/busts_in_silhouette.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/busts_in_silhouette.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cactus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cactus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cake.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cake.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/calendar.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/calendar.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/calling.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/calling.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/camel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/camel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/camera.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/camera.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cancer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cancer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/candy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/candy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/capital_abcd.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/capital_abcd.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/capricorn.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/capricorn.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/card_index.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/card_index.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/carousel_horse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/carousel_horse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cat_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cat_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cd.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cd.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart_with_downwards_trend.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart_with_downwards_trend.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chart_with_upwards_trend.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chart_with_upwards_trend.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/checkered_flag.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/checkered_flag.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cherries.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cherries.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cherry_blossom.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cherry_blossom.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chestnut.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chestnut.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chicken.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chicken.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/children_crossing.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/children_crossing.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/chocolate_bar.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/chocolate_bar.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/christmas_tree.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/christmas_tree.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/church.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/church.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cinema.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cinema.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/circus_tent.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/circus_tent.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/city_sunrise.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/city_sunrise.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/city_sunset.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/city_sunset.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cl.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cl.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clap.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clap.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clapper.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clapper.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clipboard.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clipboard.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_1.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_1.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_10.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_10.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_10_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_10_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_11.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_11.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_11_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_11_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_12.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_12.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_12_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_12_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_1_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_1_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_2_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_2_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_3.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_3.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_3_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_3_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_4.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_4.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_4_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_4_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_5.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_5.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_5_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_5_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_6.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_6.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_6_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_6_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_7.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_7.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_7_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_7_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_8.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_8.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_8_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_8_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_9.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_9.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clock_9_30.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clock_9_30.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_book.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_book.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_lock_with_key.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_lock_with_key.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/closed_umbrella.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/closed_umbrella.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cloud.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cloud.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/clubs.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/clubs.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cn.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cn.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cocktail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cocktail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/coffee.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/coffee.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/collision.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/collision.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/computer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/computer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confetti_ball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confetti_ball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confounded.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confounded.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/confused.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/confused.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/construction.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/construction.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/construction_worker.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/construction_worker.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/convenience_store.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/convenience_store.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cookie.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cookie.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cool.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cool.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/copyright.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/copyright.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/corn.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/corn.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couple.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couple.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couple_with_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couple_with_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/couplekiss.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/couplekiss.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cow.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cow.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cow_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cow_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/credit_card.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/credit_card.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crocodile.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crocodile.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crossed_flags.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crossed_flags.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crown.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crown.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crying_cat_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crying_cat_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/crystal_ball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/crystal_ball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cupid.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cupid.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/curly_loop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/curly_loop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/currency_exchange.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/currency_exchange.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/curry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/curry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/custard.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/custard.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/customs.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/customs.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/cyclone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/cyclone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dancer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dancer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dancers.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dancers.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dango.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dango.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dash.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dash.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/date.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/date.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/de.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/de.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/deciduous_tree.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/deciduous_tree.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/department_store.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/department_store.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/diamond_shape_with_dot_inside.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/diamond_shape_with_dot_inside.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/diamonds.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/diamonds.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/disappointed.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/disappointed.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/disappointed_relieved.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/disappointed_relieved.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dizzy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dizzy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dizzy_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dizzy_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/do_not_litter.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/do_not_litter.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dog.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dog.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dog_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dog_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dollar.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dollar.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dolls.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dolls.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dolphin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dolphin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/door.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/door.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/doughnut.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/doughnut.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dragon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dragon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dragon_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dragon_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dress.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dress.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dromedary_camel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dromedary_camel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/droplet.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/droplet.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/dvd.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/dvd.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/e_mail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/e_mail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ear.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ear.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ear_of_rice.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ear_of_rice.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_africa.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_africa.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_americas.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_americas.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/earth_asia.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/earth_asia.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/egg.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/egg.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eggplant.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eggplant.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight_pointed_black_star.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight_pointed_black_star.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eight_pointed_blue_star.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eight_pointed_blue_star.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/electric_plug.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/electric_plug.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/elephant.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/elephant.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/email.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/email.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/end.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/end.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/envelope.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/envelope.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/es.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/es.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/euro.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/euro.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/european_castle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/european_castle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/european_post_office.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/european_post_office.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/evergreen_tree.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/evergreen_tree.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/exclamation.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/exclamation.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/expressionless.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/expressionless.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eyeglasses.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eyeglasses.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/eyes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/eyes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/facepunch.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/facepunch.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/factory.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/factory.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fallen_leaf.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fallen_leaf.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/family.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/family.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fast_forward.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fast_forward.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fax.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fax.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fearful.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fearful.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/feelsgood.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/feelsgood.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/feet.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/feet.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ferris_wheel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ferris_wheel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/file_folder.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/file_folder.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/finnadie.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/finnadie.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fire.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fire.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fire_engine.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fire_engine.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fireworks.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fireworks.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon_with_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/first_quarter_moon_with_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fish.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fish.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fish_cake.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fish_cake.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fishing_pole_and_fish.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fishing_pole_and_fish.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fist.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fist.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/five.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/five.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flags.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flags.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flashlight.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flashlight.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/floppy_disk.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/floppy_disk.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flower_playing_cards.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flower_playing_cards.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/flushed.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/flushed.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/foggy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/foggy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/football.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/football.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fountain.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fountain.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/four.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/four.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/four_leaf_clover.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/four_leaf_clover.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fr.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fr.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/free.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/free.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fried_shrimp.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fried_shrimp.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fries.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fries.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/frog.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/frog.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/frowning.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/frowning.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fu.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fu.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/fuelpump.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/fuelpump.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/full_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/full_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/full_moon_with_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/full_moon_with_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/game_die.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/game_die.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gb.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gb.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gem.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gem.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gemini.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gemini.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ghost.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ghost.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gift.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gift.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gift_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gift_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/girl.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/girl.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/globe_with_meridians.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/globe_with_meridians.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/goat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/goat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/goberserk.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/goberserk.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/godmode.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/godmode.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/golf.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/golf.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grapes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grapes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_apple.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_apple.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_book.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_book.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/green_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/green_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grey_exclamation.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grey_exclamation.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grey_question.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grey_question.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grimacing.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grimacing.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/grinning.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/grinning.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/guardsman.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/guardsman.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/guitar.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/guitar.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/gun.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/gun.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/haircut.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/haircut.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hamburger.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hamburger.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hammer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hammer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hamster.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hamster.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hand.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hand.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/handbag.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/handbag.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hankey.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hankey.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hash.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hash.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hatched_chick.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hatched_chick.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hatching_chick.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hatching_chick.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/headphones.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/headphones.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hear_no_evil.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hear_no_evil.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_decoration.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_decoration.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_eyes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_eyes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heart_eyes_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heart_eyes_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heartbeat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heartbeat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heartpulse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heartpulse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hearts.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hearts.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_check_mark.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_check_mark.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_division_sign.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_division_sign.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_dollar_sign.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_dollar_sign.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_exclamation_mark.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_exclamation_mark.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_multiplication.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_multiplication.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/heavy_plus_sign.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/heavy_plus_sign.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/helicopter.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/helicopter.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/herb.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/herb.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hibiscus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hibiscus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/high_brightness.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/high_brightness.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/high_heel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/high_heel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hocho.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hocho.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/honey_pot.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/honey_pot.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/honeybee.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/honeybee.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/horse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/horse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/horse_racing.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/horse_racing.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hospital.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hospital.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hotel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hotel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hotsprings.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hotsprings.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hourglass.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hourglass.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hourglass_flowing_sand.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hourglass_flowing_sand.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/house.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/house.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/house_with_garden.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/house_with_garden.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hundred.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hundred.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hurtrealbad.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hurtrealbad.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/hushed.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/hushed.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ice_cream.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ice_cream.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/icecream.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/icecream.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/id.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/id.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/imp.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/imp.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/inbox_tray.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/inbox_tray.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/incoming_envelope.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/incoming_envelope.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/information_desk_person.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/information_desk_person.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/information_source.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/information_source.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/innocent.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/innocent.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/interrobang.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/interrobang.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/iphone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/iphone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/it.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/it.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/izakaya_lantern.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/izakaya_lantern.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jack_o_lantern.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jack_o_lantern.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japan.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japan.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_castle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_castle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_goblin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_goblin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/japanese_ogre.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/japanese_ogre.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jeans.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jeans.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/joy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/joy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/joy_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/joy_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/jp.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/jp.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/key.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/key.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/keycap_ten.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/keycap_ten.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kimono.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kimono.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kiss.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kiss.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_closed_eyes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_closed_eyes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kissing_smiling_eyes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kissing_smiling_eyes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/knife_and_fork.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/knife_and_fork.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/koala.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/koala.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/koko.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/koko.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/kr.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/kr.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon_with_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/last_quarter_moon_with_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/laughing.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/laughing.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leaves.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leaves.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ledger.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ledger.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/left_luggage.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/left_luggage.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lemon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lemon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leo.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leo.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/leopard.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/leopard.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/libra.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/libra.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/light_rail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/light_rail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/link.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/link.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lips.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lips.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lipstick.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lipstick.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lock.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lock.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lock_with_ink_pen.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lock_with_ink_pen.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/lollipop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/lollipop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/loop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/loop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/loudspeaker.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/loudspeaker.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/love_hotel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/love_hotel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/love_letter.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/love_letter.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/low_brightness.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/low_brightness.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/m.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/m.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mag.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mag.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mag_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mag_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/magic_8_ball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/magic_8_ball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mahjong.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mahjong.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_closed.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_closed.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_with_mail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_with_mail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mailbox_with_no_mail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mailbox_with_no_mail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man_with_gua_pi_mao.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man_with_gua_pi_mao.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/man_with_turban.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/man_with_turban.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mans_shoe.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mans_shoe.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/maple_leaf.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/maple_leaf.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mask.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mask.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/massage.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/massage.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/meat_on_bone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/meat_on_bone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mega.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mega.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/melon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/melon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/memo.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/memo.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mens.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mens.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/metal.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/metal.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/microphone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/microphone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/microscope.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/microscope.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/milky_way.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/milky_way.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minibus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minibus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minidisc.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minidisc.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/minus_1.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/minus_1.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mobile_phone_off.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mobile_phone_off.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/money_with_wings.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/money_with_wings.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moneybag.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moneybag.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monkey.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monkey.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monkey_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monkey_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/monorail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/monorail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mortar_board.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mortar_board.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mount_fuji.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mount_fuji.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_bicyclist.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_bicyclist.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_cableway.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_cableway.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mountain_railway.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mountain_railway.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mouse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mouse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mouse_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mouse_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/movie_camera.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/movie_camera.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/moyai.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/moyai.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/muscle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/muscle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mushroom.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mushroom.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_keyboard.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_keyboard.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_note.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_note.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/musical_score.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/musical_score.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/mute.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/mute.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nail_care.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nail_care.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/name_badge.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/name_badge.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/neckbeard.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/neckbeard.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/necktie.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/necktie.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/negative_squared_cross_mark.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/negative_squared_cross_mark.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/neutral_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/neutral_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/new_moon_with_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/new_moon_with_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/newspaper.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/newspaper.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ng.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ng.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nine.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nine.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_bell.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_bell.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_bicycles.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_bicycles.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_entry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_entry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_good.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_good.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_mobile_phones.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_mobile_phones.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_mouth.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_mouth.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_pedestrians.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_pedestrians.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/no_smoking.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/no_smoking.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/non_potable_water.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/non_potable_water.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nose.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nose.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/notebook_with_decorative_cover.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/notebook_with_decorative_cover.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/notes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/notes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/nut_and_bolt.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/nut_and_bolt.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/o.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/o.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ocean.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ocean.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/octocat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/octocat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/octopus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/octopus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oden.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oden.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/office.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/office.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok_hand.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok_hand.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ok_woman.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ok_woman.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/older_man.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/older_man.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/older_woman.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/older_woman.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/on.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/on.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_automobile.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_automobile.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_bus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_bus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_police_car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_police_car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/oncoming_taxi.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/oncoming_taxi.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/one.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/one.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/one_two_three_four.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/one_two_three_four.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_file_folder.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_file_folder.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_hands.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_hands.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/open_mouth.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/open_mouth.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ophiuchus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ophiuchus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/orange_book.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/orange_book.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/orange_diamond.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/orange_diamond.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/outbox_tray.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/outbox_tray.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ox.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ox.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/page_facing_up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/page_facing_up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/page_with_curl.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/page_with_curl.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pager.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pager.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/palm_tree.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/palm_tree.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/panda_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/panda_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/paperclip.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/paperclip.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/parking.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/parking.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/part_alternation_mark.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/part_alternation_mark.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/partly_sunny.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/partly_sunny.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/passport_control.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/passport_control.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/paw_prints.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/paw_prints.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/peach.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/peach.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pear.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pear.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pencil.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pencil.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pencil_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pencil_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/penguin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/penguin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pensive.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pensive.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/performing_arts.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/performing_arts.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/persevere.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/persevere.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/phone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/phone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pig_nose.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pig_nose.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pill.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pill.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pineapple.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pineapple.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pisces.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pisces.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pizza.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pizza.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/plus_1.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/plus_1.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_down.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_down.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_left.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_left.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_right.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_right.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/point_up_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/point_up_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/police_car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/police_car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poodle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poodle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poop.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poop.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/post_office.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/post_office.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/postal_horn.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/postal_horn.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/postbox.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/postbox.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/potable_water.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/potable_water.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pouch.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pouch.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/poultry_leg.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/poultry_leg.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pound.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pound.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pouting_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pouting_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pray.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pray.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/princess.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/princess.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/punch.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/punch.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/purple_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/purple_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/purse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/purse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/pushpin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/pushpin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/put_litter_in_its_place.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/put_litter_in_its_place.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/question.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/question.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rabbit.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rabbit.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rabbit_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rabbit_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/racehorse.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/racehorse.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/radio.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/radio.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/radio_button.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/radio_button.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_1.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_1.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_3.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_3.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rage_4.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rage_4.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/railway_car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/railway_car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rainbow.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rainbow.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raised_hand.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raised_hand.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raised_hands.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raised_hands.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/raising_hand.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/raising_hand.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ram.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ram.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ramen.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ramen.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/recycle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/recycle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/red_car.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/red_car.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/red_circle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/red_circle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/registered.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/registered.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/relaxed.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/relaxed.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/relieved.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/relieved.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/repeat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/repeat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/repeat_once.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/repeat_once.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/restroom.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/restroom.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/revolving_hearts.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/revolving_hearts.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rewind.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rewind.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ribbon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ribbon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_ball.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_ball.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_cracker.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_cracker.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rice_scene.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rice_scene.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ring.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ring.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rocket.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rocket.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/roller_coaster.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/roller_coaster.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rooster.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rooster.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rose.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rose.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rotating_light.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rotating_light.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/round_pushpin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/round_pushpin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rowboat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rowboat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ru.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ru.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/rugby_football.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/rugby_football.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/runner.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/runner.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/running.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/running.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/running_shirt_with_sash.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/running_shirt_with_sash.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sagittarius.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sagittarius.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sailboat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sailboat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sake.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sake.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sandal.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sandal.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/santa.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/santa.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/satelite.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/satelite.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/satisfied.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/satisfied.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/saxophone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/saxophone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/school.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/school.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/school_satchel.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/school_satchel.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scissors.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scissors.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scorpius.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scorpius.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scream.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scream.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scream_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scream_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/scroll.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/scroll.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/see_no_evil.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/see_no_evil.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seedling.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seedling.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/seven.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/seven.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shaved_ice.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shaved_ice.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sheep.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sheep.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shell.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shell.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ship.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ship.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shipit.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shipit.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shirt.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shirt.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shit.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shit.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shoe.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shoe.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/shower.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/shower.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/signal_strength.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/signal_strength.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/six.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/six.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/six_pointed_star.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/six_pointed_star.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ski.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ski.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/skull.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/skull.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sleeping.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sleeping.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sleepy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sleepy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/slot_machine.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/slot_machine.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_blue_diamond.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_blue_diamond.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_orange_diamond.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_orange_diamond.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_down.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_down.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/small_red_triangle_up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smile.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smile.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smile_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smile_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiley.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiley.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiley_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiley_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smiling_imp.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smiling_imp.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smirk.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smirk.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smirk_cat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smirk_cat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/smoking.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/smoking.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snail.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snail.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snake.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snake.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowboarder.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowboarder.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowflake.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowflake.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/snowman.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/snowman.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sob.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sob.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/soccer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/soccer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/soon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/soon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sos.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sos.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sound.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sound.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/space_invader.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/space_invader.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/spades.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/spades.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/spaghetti.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/spaghetti.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkler.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkler.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkles.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkles.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sparkling_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sparkling_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speak_no_evil.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speak_no_evil.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speaker.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speaker.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speech_balloon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speech_balloon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/speedboat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/speedboat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/star.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/star.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/star_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/star_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stars.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stars.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/station.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/station.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/statue_of_liberty.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/statue_of_liberty.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/steam_locomotive.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/steam_locomotive.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stew.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stew.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/straight_ruler.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/straight_ruler.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/strawberry.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/strawberry.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_closed_eyes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_closed_eyes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_winking_eye.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/stuck_out_tongue_winking_eye.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sun_with_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sun_with_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunflower.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunflower.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunglasses.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunglasses.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunny.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunny.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunrise.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunrise.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sunrise_over_mountains.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sunrise_over_mountains.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/surfer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/surfer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sushi.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sushi.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/suspect.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/suspect.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/suspension_railway.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/suspension_railway.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat_drops.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat_drops.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweat_smile.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweat_smile.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/sweet_potato.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/sweet_potato.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/swimmer.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/swimmer.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/symbols.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/symbols.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/syringe.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/syringe.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tada.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tada.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tanabata_tree.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tanabata_tree.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tangerine.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tangerine.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/taurus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/taurus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/taxi.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/taxi.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tea.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tea.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telephone.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telephone.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telephone_receiver.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telephone_receiver.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/telescope.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/telescope.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tennis.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tennis.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tent.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tent.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thought_balloon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thought_balloon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/three.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/three.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thumbsdown.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thumbsdown.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/thumbsup.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/thumbsup.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/ticket.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/ticket.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tiger.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tiger.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tiger_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tiger_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tired_face.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tired_face.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tm.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tm.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/toilet.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/toilet.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tokyo_tower.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tokyo_tower.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tomato.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tomato.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tongue.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tongue.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/top.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/top.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tophat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tophat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tractor.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tractor.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/traffic_light.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/traffic_light.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/train.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/train.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/train_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/train_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tram.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tram.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triangular_flag_on_post.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triangular_flag_on_post.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triangular_ruler.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triangular_ruler.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trident.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trident.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/triumph.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/triumph.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trolleybus.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trolleybus.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trollface.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trollface.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trophy.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trophy.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tropical_drink.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tropical_drink.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tropical_fish.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tropical_fish.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/truck.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/truck.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/trumpet.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/trumpet.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tshirt.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tshirt.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tulip.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tulip.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/turtle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/turtle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/tv.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/tv.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_hearts.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_hearts.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_men_holding_hands.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_men_holding_hands.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/two_women_holding_hands.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/two_women_holding_hands.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/uk.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/uk.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/umbrella.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/umbrella.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/unamused.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/unamused.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/underage.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/underage.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/unlock.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/unlock.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/up.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/up.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/us.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/us.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/v.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/v.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vertical_traffic_light.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vertical_traffic_light.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vhs.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vhs.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vibration_mode.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vibration_mode.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/video_camera.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/video_camera.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/video_game.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/video_game.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/violin.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/violin.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/virgo.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/virgo.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/volcano.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/volcano.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/vs.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/vs.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/walking.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/walking.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waning_cresent_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waning_cresent_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waning_gibbous_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waning_gibbous_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/warning.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/warning.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/watch.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/watch.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/water_buffalo.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/water_buffalo.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/watermelon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/watermelon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wave.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wave.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wavy_dash.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wavy_dash.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waxing_cresent_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waxing_cresent_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/waxing_gibbous_moon.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/waxing_gibbous_moon.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wc.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wc.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/weary.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/weary.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wedding.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wedding.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/whale.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/whale.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/whale_2.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/whale_2.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/white_circle.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/white_circle.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/white_flower.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/white_flower.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wind_chime.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wind_chime.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wine_glass.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wine_glass.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wink.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wink.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wolf.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wolf.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/woman.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/woman.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womans_clothes.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womans_clothes.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womans_hat.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womans_hat.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/womens.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/womens.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/worried.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/worried.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/wrench.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/wrench.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/x.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/x.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yellow_heart.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yellow_heart.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yen.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yen.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/yum.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/yum.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zap.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zap.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zero.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zero.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/emoji/resources/zzz.png` & `borb-2.1.9/borb/pdf/canvas/layout/emoji/resources/zzz.png`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/check_box.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/check_box.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/country_drop_down_list.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/country_drop_down_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/drop_down_list.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/drop_down_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/form_field.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/form_field.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/push_button.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/push_button.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/text_area.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/text_area.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/forms/text_field.py` & `borb-2.1.9/borb/pdf/canvas/layout/forms/text_field.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/free_space_finder.py` & `borb-2.1.9/borb/pdf/canvas/layout/free_space_finder.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/horizontal_rule.py` & `borb-2.1.9/borb/pdf/canvas/layout/horizontal_rule.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/hyphenation.py` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/hyphenation.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/af.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/af.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/as.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/as.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/be.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/be.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/bg.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/bg.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/bn.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/bn.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ca.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ca.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/cy.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/cy.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/da.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/da.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/de.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/de.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/en-gb.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/en-gb.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/en-us.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/en-us.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/es.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/es.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/et.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/et.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/fi.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/fi.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/fr.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/fr.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/lt.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/lt.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/nl.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/nl.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ro.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ro.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/hyphenation/resources/ru.json` & `borb-2.1.9/borb/pdf/canvas/layout/hyphenation/resources/ru.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/image/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/image/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/image/barcode.py` & `borb-2.1.9/borb/pdf/canvas/layout/image/barcode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/image/chart.py` & `borb-2.1.9/borb/pdf/canvas/layout/image/chart.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/image/image.py` & `borb-2.1.9/borb/pdf/canvas/layout/image/image.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/image/unsplash.py` & `borb-2.1.9/borb/pdf/canvas/layout/image/unsplash.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/layout_element.py` & `borb-2.1.9/borb/pdf/canvas/layout/layout_element.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/list/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/list/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/list/list.py` & `borb-2.1.9/borb/pdf/canvas/layout/list/list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/list/ordered_list.py` & `borb-2.1.9/borb/pdf/canvas/layout/list/ordered_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/list/roman_list.py` & `borb-2.1.9/borb/pdf/canvas/layout/list/roman_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/list/unordered_list.py` & `borb-2.1.9/borb/pdf/canvas/layout/list/unordered_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/block_flow.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/block_flow.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/header_footer_multi_column_layout.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/header_footer_multi_column_layout.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/inline_flow.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/inline_flow.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/multi_column_layout.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/multi_column_layout.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/page_layout.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/page_layout.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/page_layout/single_column_layout_with_overflow.py` & `borb-2.1.9/borb/pdf/canvas/layout/page_layout/single_column_layout_with_overflow.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/shape/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/shape/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/shape/connected_shape.py` & `borb-2.1.9/borb/pdf/canvas/layout/shape/connected_shape.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/shape/disconnected_shape.py` & `borb-2.1.9/borb/pdf/canvas/layout/shape/disconnected_shape.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/shape/gradient_colored_disconnected_shape.py` & `borb-2.1.9/borb/pdf/canvas/layout/shape/gradient_colored_disconnected_shape.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/shape/progressbar.py` & `borb-2.1.9/borb/pdf/canvas/layout/shape/progressbar.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/smart_art/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/smart_art/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/smart_art/smart_art.py` & `borb-2.1.9/borb/pdf/canvas/layout/smart_art/smart_art.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/table/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/table/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/table/fixed_column_width_table.py` & `borb-2.1.9/borb/pdf/canvas/layout/table/fixed_column_width_table.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/table/flexible_column_width_table.py` & `borb-2.1.9/borb/pdf/canvas/layout/table/flexible_column_width_table.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/table/table.py` & `borb-2.1.9/borb/pdf/canvas/layout/table/table.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/table/table_util.py` & `borb-2.1.9/borb/pdf/canvas/layout/table/table_util.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/__init__.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/chunk_of_text.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/chunk_of_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/codeblock.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/codeblock.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/heading.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/heading.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/heterogeneous_paragraph.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/heterogeneous_paragraph.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/line_of_text.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/line_of_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/layout/text/paragraph.py` & `borb-2.1.9/borb/pdf/canvas/layout/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/line_art/__init__.py` & `borb-2.1.9/borb/pdf/canvas/line_art/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/line_art/blob_factory.py` & `borb-2.1.9/borb/pdf/canvas/line_art/blob_factory.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/line_art/line_art_factory.py` & `borb-2.1.9/borb/pdf/canvas/line_art/line_art_factory.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/line_art/rectangular_hitomezashi.py` & `borb-2.1.9/borb/pdf/canvas/line_art/rectangular_hitomezashi.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/line_art/rectangular_maze_factory.py` & `borb-2.1.9/borb/pdf/canvas/line_art/rectangular_maze_factory.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/__init__.py` & `borb-2.1.9/borb/pdf/canvas/lipsum/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/lipsum.py` & `borb-2.1.9/borb/pdf/canvas/lipsum/lipsum.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_agatha_christie.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_agatha_christie.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_alan_alexander_milne.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_alan_alexander_milne.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_arthur_conan_doyle.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_arthur_conan_doyle.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_emily_bronte.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_emily_bronte.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_jane_austen.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_jane_austen.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_lewis_carroll.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_lewis_carroll.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_lipsum.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_lipsum.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/resources/mm_mary_shelley.json` & `borb-2.1.9/borb/pdf/canvas/lipsum/resources/mm_mary_shelley.json`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/lipsum/text_generator.py` & `borb-2.1.9/borb/pdf/canvas/lipsum/text_generator.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/canvas_operator.py` & `borb-2.1.9/borb/pdf/canvas/operator/canvas_operator.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_cmyk_non_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_cmyk_non_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_cmyk_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_cmyk_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_color_non_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_color_non_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_color_space_non_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_color_space_non_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_color_space_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_color_space_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_color_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_color_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_gray_non_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_gray_non_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_gray_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_gray_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_rgb_non_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_rgb_non_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/color/set_rgb_stroking.py` & `borb-2.1.9/borb/pdf/canvas/operator/color/set_rgb_stroking.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/compatibility/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/compatibility/begin_compatibility_section.py` & `borb-2.1.9/borb/pdf/canvas/operator/compatibility/begin_compatibility_section.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/compatibility/end_compatibility_section.py` & `borb-2.1.9/borb/pdf/canvas/operator/compatibility/end_compatibility_section.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/marked_content/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/marked_content/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/marked_content/begin_marked_content.py` & `borb-2.1.9/borb/pdf/canvas/operator/marked_content/begin_marked_content.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/marked_content/begin_marked_content_with_property_list.py` & `borb-2.1.9/borb/pdf/canvas/operator/marked_content/begin_marked_content_with_property_list.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/marked_content/end_marked_content.py` & `borb-2.1.9/borb/pdf/canvas/operator/marked_content/end_marked_content.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_cubic_bezier.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_cubic_bezier.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_line_segment.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_line_segment.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/append_rectangle.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/append_rectangle.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/begin_subpath.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/begin_subpath.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_construction/close_subpath.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_construction/close_subpath.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_painting/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_painting/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_painting/close_and_stroke_path.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_painting/close_and_stroke_path.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/path_painting/stroke_path.py` & `borb-2.1.9/borb/pdf/canvas/operator/path_painting/stroke_path.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/state/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/state/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/state/modify_transformation_matrix.py` & `borb-2.1.9/borb/pdf/canvas/operator/state/modify_transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/state/pop_graphics_state.py` & `borb-2.1.9/borb/pdf/canvas/operator/state/pop_graphics_state.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/state/push_graphics_state.py` & `borb-2.1.9/borb/pdf/canvas/operator/state/push_graphics_state.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/state/set_line_width.py` & `borb-2.1.9/borb/pdf/canvas/operator/state/set_line_width.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/begin_text.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/begin_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/end_text.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/end_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/move_text_position.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/move_text_position.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/move_text_position_set_leading.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/move_text_position_set_leading.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/move_to_next_line.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/move_to_next_line.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/move_to_next_line_show_text.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/move_to_next_line_show_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_character_spacing.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_character_spacing.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_font_and_size.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_font_and_size.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_horizontal_text_scaling.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_horizontal_text_scaling.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_spacing_move_to_next_line_show_text.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_spacing_move_to_next_line_show_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_text_leading.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_text_leading.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_text_matrix.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_text_matrix.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_text_rendering_mode.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_text_rendering_mode.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_text_rise.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_text_rise.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/set_word_spacing.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/set_word_spacing.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/show_text.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/show_text.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/text/show_text_with_glyph_positioning.py` & `borb-2.1.9/borb/pdf/canvas/operator/text/show_text_with_glyph_positioning.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/xobject/__init__.py` & `borb-2.1.9/borb/pdf/canvas/operator/xobject/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/operator/xobject/do.py` & `borb-2.1.9/borb/pdf/canvas/operator/xobject/do.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/canvas/redacted_canvas_stream_processor.py` & `borb-2.1.9/borb/pdf/canvas/redacted_canvas_stream_processor.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/document/__init__.py` & `borb-2.1.9/borb/pdf/document/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/document/document.py` & `borb-2.1.9/borb/pdf/document/document.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/document/name_tree.py` & `borb-2.1.9/borb/pdf/document/name_tree.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/page/__init__.py` & `borb-2.1.9/borb/pdf/page/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/page/page.py` & `borb-2.1.9/borb/pdf/page/page.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/page/page_info.py` & `borb-2.1.9/borb/pdf/page/page_info.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/page/page_size.py` & `borb-2.1.9/borb/pdf/page/page_size.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/pdf.py` & `borb-2.1.9/borb/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/trailer/__init__.py` & `borb-2.1.9/borb/pdf/trailer/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/trailer/document_info.py` & `borb-2.1.9/borb/pdf/trailer/document_info.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/xref/__init__.py` & `borb-2.1.9/borb/pdf/xref/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/xref/plaintext_xref.py` & `borb-2.1.9/borb/pdf/xref/plaintext_xref.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/xref/rebuilt_xref.py` & `borb-2.1.9/borb/pdf/xref/rebuilt_xref.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/xref/stream_xref.py` & `borb-2.1.9/borb/pdf/xref/stream_xref.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/pdf/xref/xref.py` & `borb-2.1.9/borb/pdf/xref/xref.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         while pos > 0:
             # get bytes in window
             bytes_near_eof: bytes = b"".join([tok._next_byte() for _ in range(0, 1024)])
             idx = bytes_near_eof.find(b"startxref")
             if idx >= 0:
                 return pos + idx
             # next iteration
-            pos = pos - 1024
+            pos = max(pos - 1024, 0)
             tok.seek(pos)
 
         # not found
         return -1
 
     def _seek_to_xref_token(
         self,
```

### Comparing `borb-2.1.8/borb/toolkit/__init__.py` & `borb-2.1.9/borb/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/color/__init__.py` & `borb-2.1.9/borb/toolkit/color/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/color/color_extraction.py` & `borb-2.1.9/borb/toolkit/color/color_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/__init__.py` & `borb-2.1.9/borb/toolkit/export/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/html_to_pdf/__init__.py` & `borb-2.1.9/borb/toolkit/export/html_to_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/html_to_pdf/html_to_pdf.py` & `borb-2.1.9/borb/toolkit/export/html_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/markdown_to_pdf/__init__.py` & `borb-2.1.9/borb/toolkit/export/markdown_to_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/markdown_to_pdf/markdown_to_pdf.py` & `borb-2.1.9/borb/toolkit/export/markdown_to_pdf/markdown_to_pdf.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/pdf_to_jpg.py` & `borb-2.1.9/borb/toolkit/export/pdf_to_jpg.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/pdf_to_mp3.py` & `borb-2.1.9/borb/toolkit/export/pdf_to_mp3.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/export/pdf_to_svg.py` & `borb-2.1.9/borb/toolkit/export/pdf_to_svg.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/image/__init__.py` & `borb-2.1.9/borb/toolkit/image/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/image/image_extraction.py` & `borb-2.1.9/borb/toolkit/image/image_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/image/image_format_optimization.py` & `borb-2.1.9/borb/toolkit/image/image_format_optimization.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/location/__init__.py` & `borb-2.1.9/borb/toolkit/location/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/location/location_filter.py` & `borb-2.1.9/borb/toolkit/location/location_filter.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/ocr/__init__.py` & `borb-2.1.9/borb/toolkit/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/ocr/ocr_as_optional_content_group.py` & `borb-2.1.9/borb/toolkit/ocr/ocr_as_optional_content_group.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/ocr/ocr_image_render_event_listener.py` & `borb-2.1.9/borb/toolkit/ocr/ocr_image_render_event_listener.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/redact/__init__.py` & `borb-2.1.9/borb/toolkit/redact/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/redact/common_regular_expressions.py` & `borb-2.1.9/borb/toolkit/redact/common_regular_expressions.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/table/__init__.py` & `borb-2.1.9/borb/toolkit/table/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/table/table_detection_by_lines.py` & `borb-2.1.9/borb/toolkit/table/table_detection_by_lines.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/__init__.py` & `borb-2.1.9/borb/toolkit/text/__init__.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/font_color_filter.py` & `borb-2.1.9/borb/toolkit/text/font_color_filter.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/font_extraction.py` & `borb-2.1.9/borb/toolkit/text/font_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/font_name_filter.py` & `borb-2.1.9/borb/toolkit/text/font_name_filter.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/regular_expression_text_extraction.py` & `borb-2.1.9/borb/toolkit/text/regular_expression_text_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/simple_find_replace.py` & `borb-2.1.9/borb/toolkit/text/simple_find_replace.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/simple_line_of_text_extraction.py` & `borb-2.1.9/borb/toolkit/text/simple_line_of_text_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/simple_non_ligature_text_extraction.py` & `borb-2.1.9/borb/toolkit/text/simple_non_ligature_text_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/simple_paragraph_extraction.py` & `borb-2.1.9/borb/toolkit/text/simple_paragraph_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/simple_text_extraction.py` & `borb-2.1.9/borb/toolkit/text/simple_text_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/stop_words.py` & `borb-2.1.9/borb/toolkit/text/stop_words.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/text_rank_keyword_extraction.py` & `borb-2.1.9/borb/toolkit/text/text_rank_keyword_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb/toolkit/text/tf_idf_keyword_extraction.py` & `borb-2.1.9/borb/toolkit/text/tf_idf_keyword_extraction.py`

 * *Files identical despite different names*

### Comparing `borb-2.1.8/borb.egg-info/PKG-INFO` & `borb-2.1.9/borb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: borb
-Version: 2.1.8
+Version: 2.1.9
 Summary: borb is a library for reading, creating and manipulating PDF files in python.
 Home-page: https://github.com/jorisschellekens/borb
 Author: Joris Schellekens
 Author-email: joris.schellekens.1989@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # ![borb logo](https://github.com/jorisschellekens/borb/raw/master/logo/borb_64.png) borb
 
@@ -115,7 +117,9 @@
 
 ## 3. Acknowledgements
 
 I would like to thank the following people, for their contributions / advice with regards to developing `borb`:
 - Aleksander Banasik
 - Benoît Lagae
 - Michael Klink
+
+
```

### Comparing `borb-2.1.8/borb.egg-info/SOURCES.txt` & `borb-2.1.9/borb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -89,40 +89,41 @@
 borb/io/write/reference/xref_transformer.py
 borb/io/write/version/__init__.py
 borb/io/write/version/version_as_comment_transformer.py
 borb/io/write/xmp/__init__.py
 borb/io/write/xmp/xmp_transformer.py
 borb/license/__init__.py
 borb/license/anonymous_user_id.py
-borb/license/geo_information.py
 borb/license/machine_id.py
 borb/license/usage_statistics.py
 borb/license/uuid.py
 borb/license/version.py
 borb/pdf/__init__.py
 borb/pdf/pdf.py
 borb/pdf/canvas/__init__.py
 borb/pdf/canvas/canvas.py
 borb/pdf/canvas/canvas_graphics_state.py
 borb/pdf/canvas/canvas_stream_processor.py
 borb/pdf/canvas/redacted_canvas_stream_processor.py
 borb/pdf/canvas/color/__init__.py
 borb/pdf/canvas/color/color.py
+borb/pdf/canvas/color/color_palette_from_image.py
 borb/pdf/canvas/color/farrow_and_ball.py
 borb/pdf/canvas/color/pantone.py
 borb/pdf/canvas/event/__init__.py
 borb/pdf/canvas/event/begin_page_event.py
 borb/pdf/canvas/event/begin_text_event.py
 borb/pdf/canvas/event/chunk_of_text_render_event.py
 borb/pdf/canvas/event/end_page_event.py
 borb/pdf/canvas/event/end_text_event.py
 borb/pdf/canvas/event/event_listener.py
 borb/pdf/canvas/event/image_render_event.py
 borb/pdf/canvas/event/line_render_event.py
 borb/pdf/canvas/font/__init__.py
+borb/pdf/canvas/font/adobe_glyph_list.py
 borb/pdf/canvas/font/adobe_standard_encoding.py
 borb/pdf/canvas/font/font.py
 borb/pdf/canvas/font/glyph_line.py
 borb/pdf/canvas/font/symbol_encoding.py
 borb/pdf/canvas/font/composite_font/__init__.py
 borb/pdf/canvas/font/composite_font/cid_font_type_0.py
 borb/pdf/canvas/font/composite_font/cid_font_type_2.py
```

### Comparing `borb-2.1.8/setup.py` & `borb-2.1.9/setup.py`

 * *Files identical despite different names*

