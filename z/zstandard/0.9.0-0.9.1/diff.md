# Comparing `tmp/zstandard-0.9.0.tar.gz` & `tmp/zstandard-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zstandard-0.9.0.tar", last modified: Mon Apr  9 01:03:29 2018, max compression
+gzip compressed data, was "dist/zstandard-0.9.1.tar", last modified: Tue Jun  5 05:39:01 2018, max compression
```

## Comparing `zstandard-0.9.0.tar` & `zstandard-0.9.1.tar`

### file list

```diff
@@ -1,119 +1,127 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/c-ext/
--rw-r--r--   0 travis    (2000) travis    (2000)    23793 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/bufferutil.c
--rw-r--r--   0 travis    (2000) travis    (2000)    11971 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressiondict.c
--rw-r--r--   0 travis    (2000) travis    (2000)    15835 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressionparams.c
--rw-r--r--   0 travis    (2000) travis    (2000)     9836 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressionreader.c
--rw-r--r--   0 travis    (2000) travis    (2000)     8720 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressionwriter.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7241 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressobj.c
--rw-r--r--   0 travis    (2000) travis    (2000)    43526 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressor.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7048 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/compressoriterator.c
--rw-r--r--   0 travis    (2000) travis    (2000)     4259 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/constants.c
--rw-r--r--   0 travis    (2000) travis    (2000)    11162 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/decompressionreader.c
--rw-r--r--   0 travis    (2000) travis    (2000)     5663 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/decompressionwriter.c
--rw-r--r--   0 travis    (2000) travis    (2000)     4829 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/decompressobj.c
--rw-r--r--   0 travis    (2000) travis    (2000)    51152 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/decompressor.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7384 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/decompressoriterator.c
--rw-r--r--   0 travis    (2000) travis    (2000)     4285 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/frameparams.c
--rw-r--r--   0 travis    (2000) travis    (2000)     8466 2018-04-09 01:03:08.000000 zstandard-0.9.0/c-ext/python-zstandard.h
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/tests/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4497 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/common.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4102 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_buffer_util.py
--rw-r--r--   0 travis    (2000) travis    (2000)    45441 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_compressor.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7781 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_compressor_fuzzing.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8455 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_data_structures.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3590 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_data_structures_fuzzing.py
--rw-r--r--   0 travis    (2000) travis    (2000)    38877 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_decompressor.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9948 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_decompressor_fuzzing.py
--rw-r--r--   0 travis    (2000) travis    (2000)      271 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_estimate_sizes.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1647 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_module_attributes.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2828 2018-04-09 01:03:08.000000 zstandard-0.9.0/tests/test_train_dictionary.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard/
--rw-r--r--   0 travis    (2000) travis    (2000)     2386 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstandard/__init__.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    67426 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     5193 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       11 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       26 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstandard.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/common/
--rw-r--r--   0 travis    (2000) travis    (2000)    18395 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/bitstream.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3846 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/compiler.h
--rw-r--r--   0 travis    (2000) travis    (2000)     4444 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/cpu.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8807 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/entropy_common.c
--rw-r--r--   0 travis    (2000) travis    (2000)     2695 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/error_private.c
--rw-r--r--   0 travis    (2000) travis    (2000)     2305 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/error_private.h
--rw-r--r--   0 travis    (2000) travis    (2000)    32738 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/fse.h
--rw-r--r--   0 travis    (2000) travis    (2000)    11205 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/fse_decompress.c
--rw-r--r--   0 travis    (2000) travis    (2000)    19067 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/huf.h
--rw-r--r--   0 travis    (2000) travis    (2000)    11394 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/mem.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8910 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/pool.c
--rw-r--r--   0 travis    (2000) travis    (2000)     2137 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/pool.h
--rw-r--r--   0 travis    (2000) travis    (2000)     1839 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/threading.c
--rw-r--r--   0 travis    (2000) travis    (2000)     4049 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/threading.h
--rw-r--r--   0 travis    (2000) travis    (2000)    28905 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/xxhash.c
--rw-r--r--   0 travis    (2000) travis    (2000)    12781 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/xxhash.h
--rw-r--r--   0 travis    (2000) travis    (2000)     2721 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/zstd_common.c
--rw-r--r--   0 travis    (2000) travis    (2000)     3715 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/zstd_errors.h
--rw-r--r--   0 travis    (2000) travis    (2000)    10369 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/common/zstd_internal.h
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/compress/
--rw-r--r--   0 travis    (2000) travis    (2000)    32724 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/fse_compress.c
--rw-r--r--   0 travis    (2000) travis    (2000)    32367 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/huf_compress.c
--rw-r--r--   0 travis    (2000) travis    (2000)   153726 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_compress.c
--rw-r--r--   0 travis    (2000) travis    (2000)    29578 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_compress_internal.h
--rw-r--r--   0 travis    (2000) travis    (2000)    15241 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_double_fast.c
--rw-r--r--   0 travis    (2000) travis    (2000)     1238 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_double_fast.h
--rw-r--r--   0 travis    (2000) travis    (2000)    11127 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_fast.c
--rw-r--r--   0 travis    (2000) travis    (2000)     1158 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_fast.h
--rw-r--r--   0 travis    (2000) travis    (2000)    36596 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_lazy.c
--rw-r--r--   0 travis    (2000) travis    (2000)     2483 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_lazy.h
--rw-r--r--   0 travis    (2000) travis    (2000)    25365 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_ldm.c
--rw-r--r--   0 travis    (2000) travis    (2000)     4057 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_ldm.h
--rw-r--r--   0 travis    (2000) travis    (2000)    39866 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_opt.c
--rw-r--r--   0 travis    (2000) travis    (2000)     1554 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstd_opt.h
--rw-r--r--   0 travis    (2000) travis    (2000)    81101 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstdmt_compress.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7565 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/compress/zstdmt_compress.h
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/decompress/
--rw-r--r--   0 travis    (2000) travis    (2000)    45932 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/decompress/huf_decompress.c
--rw-r--r--   0 travis    (2000) travis    (2000)   124664 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/decompress/zstd_decompress.c
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/deprecated/
--rw-r--r--   0 travis    (2000) travis    (2000)    11474 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/deprecated/zbuff.h
--rw-r--r--   0 travis    (2000) travis    (2000)     1003 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/deprecated/zbuff_common.c
--rw-r--r--   0 travis    (2000) travis    (2000)     5334 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/deprecated/zbuff_compress.c
--rw-r--r--   0 travis    (2000) travis    (2000)     1919 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/dictBuilder/
--rw-r--r--   0 travis    (2000) travis    (2000)    34007 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/dictBuilder/cover.c
--rw-r--r--   0 travis    (2000) travis    (2000)    54592 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/dictBuilder/divsufsort.c
--rw-r--r--   0 travis    (2000) travis    (2000)     2419 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/dictBuilder/divsufsort.h
--rw-r--r--   0 travis    (2000) travis    (2000)    43582 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/dictBuilder/zdict.c
--rw-r--r--   0 travis    (2000) travis    (2000)    11175 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/dictBuilder/zdict.h
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-09 01:03:29.000000 zstandard-0.9.0/zstd/legacy/
--rw-r--r--   0 travis    (2000) travis    (2000)    12579 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_legacy.h
--rw-r--r--   0 travis    (2000) travis    (2000)    70278 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v01.c
--rw-r--r--   0 travis    (2000) travis    (2000)     3432 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v01.h
--rw-r--r--   0 travis    (2000) travis    (2000)   127088 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v02.c
--rw-r--r--   0 travis    (2000) travis    (2000)     3342 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v02.h
--rw-r--r--   0 travis    (2000) travis    (2000)   113189 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v03.c
--rw-r--r--   0 travis    (2000) travis    (2000)     3352 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v03.h
--rw-r--r--   0 travis    (2000) travis    (2000)   136412 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v04.c
--rw-r--r--   0 travis    (2000) travis    (2000)     6070 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v04.h
--rw-r--r--   0 travis    (2000) travis    (2000)   155065 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v05.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7131 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v05.h
--rw-r--r--   0 travis    (2000) travis    (2000)   165199 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v06.c
--rw-r--r--   0 travis    (2000) travis    (2000)     7687 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v06.h
--rw-r--r--   0 travis    (2000) travis    (2000)   184041 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v07.c
--rw-r--r--   0 travis    (2000) travis    (2000)     8330 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/legacy/zstd_v07.h
--rw-r--r--   0 travis    (2000) travis    (2000)    18091 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/COPYING
--rw-r--r--   0 travis    (2000) travis    (2000)     1530 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)    86878 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd/zstd.h
--rw-r--r--   0 travis    (2000) travis    (2000)     1484 2018-04-09 01:03:08.000000 zstandard-0.9.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)      109 2018-04-09 01:03:08.000000 zstandard-0.9.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)    55366 2018-04-09 01:03:08.000000 zstandard-0.9.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     6039 2018-04-09 01:03:08.000000 zstandard-0.9.0/make_cffi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2721 2018-04-09 01:03:08.000000 zstandard-0.9.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4388 2018-04-09 01:03:08.000000 zstandard-0.9.0/setup_zstd.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9809 2018-04-09 01:03:08.000000 zstandard-0.9.0/zstd.c
--rw-r--r--   0 travis    (2000) travis    (2000)    67426 2018-04-09 01:03:29.000000 zstandard-0.9.0/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-04-09 01:03:29.000000 zstandard-0.9.0/setup.cfg
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:01.000000 zstandard-0.9.1/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/c-ext/
+-rw-r--r--   0 travis    (2000) travis    (2000)    23793 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/bufferutil.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    11971 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressiondict.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    15835 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressionparams.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     9836 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressionreader.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     8720 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressionwriter.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7241 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressobj.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    43526 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressor.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7048 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/compressoriterator.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     4259 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/constants.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    11162 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/decompressionreader.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     5663 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/decompressionwriter.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     4829 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/decompressobj.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    51152 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/decompressor.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7384 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/decompressoriterator.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     4285 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/frameparams.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     8466 2018-06-05 05:38:51.000000 zstandard-0.9.1/c-ext/python-zstandard.h
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/debian/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/debian/source/
+-rw-r--r--   0 travis    (2000) travis    (2000)       12 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/source/format
+-rw-r--r--   0 travis    (2000) travis    (2000)       33 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/source/options
+-rw-r--r--   0 travis    (2000) travis    (2000)      169 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/changelog
+-rw-r--r--   0 travis    (2000) travis    (2000)        2 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/compat
+-rw-r--r--   0 travis    (2000) travis    (2000)     1044 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/control
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      253 2018-06-05 05:38:51.000000 zstandard-0.9.1/debian/rules
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4497 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/common.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4102 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_buffer_util.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    45441 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_compressor.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7781 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_compressor_fuzzing.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8455 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_data_structures.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3590 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_data_structures_fuzzing.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    38877 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_decompressor.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9948 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_decompressor_fuzzing.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      271 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_estimate_sizes.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1647 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_module_attributes.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2828 2018-06-05 05:38:51.000000 zstandard-0.9.1/tests/test_train_dictionary.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard/
+-rw-r--r--   0 travis    (2000) travis    (2000)     2386 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstandard/__init__.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)    67426 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)     5295 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       11 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       26 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstandard.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstd/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstd/common/
+-rw-r--r--   0 travis    (2000) travis    (2000)    18395 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/bitstream.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3846 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/compiler.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     4444 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/cpu.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8807 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/entropy_common.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     2695 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/error_private.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     2305 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/error_private.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    32738 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/fse.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    11205 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/fse_decompress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    19067 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/huf.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    11394 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/mem.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8910 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/pool.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     2137 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/pool.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     1839 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/threading.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     4049 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/threading.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    28905 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/xxhash.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    12781 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/xxhash.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     2721 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/zstd_common.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     3715 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/zstd_errors.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    10369 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/common/zstd_internal.h
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstd/compress/
+-rw-r--r--   0 travis    (2000) travis    (2000)    32724 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/fse_compress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    32367 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/huf_compress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)   153726 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_compress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    29578 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_compress_internal.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    15241 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_double_fast.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     1238 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_double_fast.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    11127 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_fast.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     1158 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_fast.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    36596 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_lazy.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     2483 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_lazy.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    25365 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_ldm.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     4057 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_ldm.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    39866 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_opt.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     1554 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstd_opt.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    81101 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstdmt_compress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7565 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/compress/zstdmt_compress.h
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:00.000000 zstandard-0.9.1/zstd/decompress/
+-rw-r--r--   0 travis    (2000) travis    (2000)    45932 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/decompress/huf_decompress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)   124664 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/decompress/zstd_decompress.c
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:01.000000 zstandard-0.9.1/zstd/deprecated/
+-rw-r--r--   0 travis    (2000) travis    (2000)    11474 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/deprecated/zbuff.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     1003 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/deprecated/zbuff_common.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     5334 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/deprecated/zbuff_compress.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     1919 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:01.000000 zstandard-0.9.1/zstd/dictBuilder/
+-rw-r--r--   0 travis    (2000) travis    (2000)    34007 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/dictBuilder/cover.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    54592 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/dictBuilder/divsufsort.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     2419 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/dictBuilder/divsufsort.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    43582 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/dictBuilder/zdict.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    11175 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/dictBuilder/zdict.h
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-05 05:39:01.000000 zstandard-0.9.1/zstd/legacy/
+-rw-r--r--   0 travis    (2000) travis    (2000)    12579 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_legacy.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    70278 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v01.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     3432 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v01.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   127088 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v02.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     3342 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v02.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   113189 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v03.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     3352 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v03.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   136412 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v04.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     6070 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v04.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   155065 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v05.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7131 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v05.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   165199 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v06.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     7687 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v06.h
+-rw-r--r--   0 travis    (2000) travis    (2000)   184041 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v07.c
+-rw-r--r--   0 travis    (2000) travis    (2000)     8330 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/legacy/zstd_v07.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    18091 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/COPYING
+-rw-r--r--   0 travis    (2000) travis    (2000)     1530 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)    86878 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd/zstd.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     1484 2018-06-05 05:38:51.000000 zstandard-0.9.1/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)      122 2018-06-05 05:38:51.000000 zstandard-0.9.1/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)    55366 2018-06-05 05:38:51.000000 zstandard-0.9.1/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     6039 2018-06-05 05:38:51.000000 zstandard-0.9.1/make_cffi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2721 2018-06-05 05:38:51.000000 zstandard-0.9.1/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4481 2018-06-05 05:38:51.000000 zstandard-0.9.1/setup_zstd.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9809 2018-06-05 05:38:51.000000 zstandard-0.9.1/zstd.c
+-rw-r--r--   0 travis    (2000) travis    (2000)    67426 2018-06-05 05:39:01.000000 zstandard-0.9.1/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-06-05 05:39:01.000000 zstandard-0.9.1/setup.cfg
```

### Comparing `zstandard-0.9.0/c-ext/bufferutil.c` & `zstandard-0.9.1/c-ext/bufferutil.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressiondict.c` & `zstandard-0.9.1/c-ext/compressiondict.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressionparams.c` & `zstandard-0.9.1/c-ext/compressionparams.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressionreader.c` & `zstandard-0.9.1/c-ext/compressionreader.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressionwriter.c` & `zstandard-0.9.1/c-ext/compressionwriter.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressobj.c` & `zstandard-0.9.1/c-ext/compressobj.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressor.c` & `zstandard-0.9.1/c-ext/compressor.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/compressoriterator.c` & `zstandard-0.9.1/c-ext/compressoriterator.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/constants.c` & `zstandard-0.9.1/c-ext/constants.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/decompressionreader.c` & `zstandard-0.9.1/c-ext/decompressionreader.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/decompressionwriter.c` & `zstandard-0.9.1/c-ext/decompressionwriter.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/decompressobj.c` & `zstandard-0.9.1/c-ext/decompressobj.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/decompressor.c` & `zstandard-0.9.1/c-ext/decompressor.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/decompressoriterator.c` & `zstandard-0.9.1/c-ext/decompressoriterator.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/frameparams.c` & `zstandard-0.9.1/c-ext/frameparams.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/c-ext/python-zstandard.h` & `zstandard-0.9.1/c-ext/python-zstandard.h`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include "structmember.h"
 
 #define ZSTD_STATIC_LINKING_ONLY
 #define ZDICT_STATIC_LINKING_ONLY
 #include <zstd.h>
 #include <zdict.h>
 
-#define PYTHON_ZSTANDARD_VERSION "0.9.0"
+#define PYTHON_ZSTANDARD_VERSION "0.9.1"
 
 typedef enum {
 	compressorobj_flush_finish,
 	compressorobj_flush_block,
 } CompressorObj_Flush;
 
 /*
```

### Comparing `zstandard-0.9.0/tests/common.py` & `zstandard-0.9.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_buffer_util.py` & `zstandard-0.9.1/tests/test_buffer_util.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_compressor.py` & `zstandard-0.9.1/tests/test_compressor.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_compressor_fuzzing.py` & `zstandard-0.9.1/tests/test_compressor_fuzzing.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_data_structures.py` & `zstandard-0.9.1/tests/test_data_structures.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_data_structures_fuzzing.py` & `zstandard-0.9.1/tests/test_data_structures_fuzzing.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_decompressor.py` & `zstandard-0.9.1/tests/test_decompressor.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_decompressor_fuzzing.py` & `zstandard-0.9.1/tests/test_decompressor_fuzzing.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_module_attributes.py` & `zstandard-0.9.1/tests/test_module_attributes.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/tests/test_train_dictionary.py` & `zstandard-0.9.1/tests/test_train_dictionary.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstandard/__init__.py` & `zstandard-0.9.1/zstandard/__init__.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstandard.egg-info/PKG-INFO` & `zstandard-0.9.1/zstandard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zstandard
-Version: 0.9.0
+Version: 0.9.1
 Summary: Zstandard bindings for Python
 Home-page: https://github.com/indygreg/python-zstandard
 Author: Gregory Szorc
 Author-email: gregory.szorc@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: ================
```

### Comparing `zstandard-0.9.0/zstandard.egg-info/SOURCES.txt` & `zstandard-0.9.1/zstandard.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 c-ext/decompressionreader.c
 c-ext/decompressionwriter.c
 c-ext/decompressobj.c
 c-ext/decompressor.c
 c-ext/decompressoriterator.c
 c-ext/frameparams.c
 c-ext/python-zstandard.h
+debian/changelog
+debian/compat
+debian/control
+debian/rules
+debian/source/format
+debian/source/options
 tests/__init__.py
 tests/common.py
 tests/test_buffer_util.py
 tests/test_compressor.py
 tests/test_compressor_fuzzing.py
 tests/test_data_structures.py
 tests/test_data_structures_fuzzing.py
```

### Comparing `zstandard-0.9.0/zstd/common/bitstream.h` & `zstandard-0.9.1/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/compiler.h` & `zstandard-0.9.1/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/cpu.h` & `zstandard-0.9.1/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/entropy_common.c` & `zstandard-0.9.1/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/error_private.c` & `zstandard-0.9.1/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/error_private.h` & `zstandard-0.9.1/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/fse.h` & `zstandard-0.9.1/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/fse_decompress.c` & `zstandard-0.9.1/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/huf.h` & `zstandard-0.9.1/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/mem.h` & `zstandard-0.9.1/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/pool.c` & `zstandard-0.9.1/zstd/common/pool.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/pool.h` & `zstandard-0.9.1/zstd/common/pool.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/threading.c` & `zstandard-0.9.1/zstd/common/threading.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/threading.h` & `zstandard-0.9.1/zstd/common/threading.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/xxhash.c` & `zstandard-0.9.1/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/xxhash.h` & `zstandard-0.9.1/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/zstd_common.c` & `zstandard-0.9.1/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/zstd_errors.h` & `zstandard-0.9.1/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/common/zstd_internal.h` & `zstandard-0.9.1/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/fse_compress.c` & `zstandard-0.9.1/zstd/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/huf_compress.c` & `zstandard-0.9.1/zstd/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_compress.c` & `zstandard-0.9.1/zstd/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_compress_internal.h` & `zstandard-0.9.1/zstd/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_double_fast.c` & `zstandard-0.9.1/zstd/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_double_fast.h` & `zstandard-0.9.1/zstd/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_fast.c` & `zstandard-0.9.1/zstd/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_fast.h` & `zstandard-0.9.1/zstd/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_lazy.c` & `zstandard-0.9.1/zstd/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_lazy.h` & `zstandard-0.9.1/zstd/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_ldm.c` & `zstandard-0.9.1/zstd/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_ldm.h` & `zstandard-0.9.1/zstd/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_opt.c` & `zstandard-0.9.1/zstd/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstd_opt.h` & `zstandard-0.9.1/zstd/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstdmt_compress.c` & `zstandard-0.9.1/zstd/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/compress/zstdmt_compress.h` & `zstandard-0.9.1/zstd/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/decompress/huf_decompress.c` & `zstandard-0.9.1/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/decompress/zstd_decompress.c` & `zstandard-0.9.1/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/deprecated/zbuff.h` & `zstandard-0.9.1/zstd/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/deprecated/zbuff_common.c` & `zstandard-0.9.1/zstd/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/deprecated/zbuff_compress.c` & `zstandard-0.9.1/zstd/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/deprecated/zbuff_decompress.c` & `zstandard-0.9.1/zstd/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/dictBuilder/cover.c` & `zstandard-0.9.1/zstd/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/dictBuilder/divsufsort.c` & `zstandard-0.9.1/zstd/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/dictBuilder/divsufsort.h` & `zstandard-0.9.1/zstd/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/dictBuilder/zdict.c` & `zstandard-0.9.1/zstd/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/dictBuilder/zdict.h` & `zstandard-0.9.1/zstd/dictBuilder/zdict.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_legacy.h` & `zstandard-0.9.1/zstd/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v01.c` & `zstandard-0.9.1/zstd/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v01.h` & `zstandard-0.9.1/zstd/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v02.c` & `zstandard-0.9.1/zstd/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v02.h` & `zstandard-0.9.1/zstd/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v03.c` & `zstandard-0.9.1/zstd/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v03.h` & `zstandard-0.9.1/zstd/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v04.c` & `zstandard-0.9.1/zstd/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v04.h` & `zstandard-0.9.1/zstd/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v05.c` & `zstandard-0.9.1/zstd/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v05.h` & `zstandard-0.9.1/zstd/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v06.c` & `zstandard-0.9.1/zstd/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v06.h` & `zstandard-0.9.1/zstd/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v07.c` & `zstandard-0.9.1/zstd/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/legacy/zstd_v07.h` & `zstandard-0.9.1/zstd/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/COPYING` & `zstandard-0.9.1/zstd/COPYING`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/LICENSE` & `zstandard-0.9.1/zstd/LICENSE`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/zstd/zstd.h` & `zstandard-0.9.1/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/LICENSE` & `zstandard-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/README.rst` & `zstandard-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/make_cffi.py` & `zstandard-0.9.1/make_cffi.py`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/setup.py` & `zstandard-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 if '--system-zstd' in sys.argv:
     SYSTEM_ZSTD = True
     sys.argv.remove('--system-zstd')
 
 if '--warnings-as-errors' in sys.argv:
     WARNINGS_AS_ERRORS = True
-    sys.argv.remote('--warning-as-errors')
+    sys.argv.remove('--warning-as-errors')
 
 # Code for obtaining the Extension instance is in its own module to
 # facilitate reuse in other projects.
 extensions = [
     setup_zstd.get_c_extension(name='zstd',
                                support_legacy=SUPPORT_LEGACY,
                                system_zstd=SYSTEM_ZSTD,
```

### Comparing `zstandard-0.9.0/setup_zstd.py` & `zstandard-0.9.1/setup_zstd.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     if hasattr(compiler, 'initialize'):
         compiler.initialize()
 
     if compiler.compiler_type == 'unix':
         compiler_type = 'unix'
     elif compiler.compiler_type == 'msvc':
         compiler_type = 'msvc'
+    elif compiler.compiler_type == 'mingw32':
+        compiler_type = 'mingw32'
     else:
         raise Exception('unhandled compiler type: %s' %
                         compiler.compiler_type)
 
     extra_args = ['-DZSTD_MULTITHREAD']
 
     if not system_zstd:
@@ -137,15 +139,15 @@
         if compiler_type == 'unix':
             extra_args.append('-fvisibility=hidden')
 
     if not system_zstd and support_legacy:
         extra_args.append('-DZSTD_LEGACY_SUPPORT=1')
 
     if warnings_as_errors:
-        if compiler_type == 'unix':
+        if compiler_type in ('unix', 'mingw32'):
             extra_args.append('-Werror')
         elif compiler_type == 'msvc':
             extra_args.append('/WX')
         else:
             assert False
 
     libraries = ['zstd'] if system_zstd else []
```

### Comparing `zstandard-0.9.0/zstd.c` & `zstandard-0.9.1/zstd.c`

 * *Files identical despite different names*

### Comparing `zstandard-0.9.0/PKG-INFO` & `zstandard-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zstandard
-Version: 0.9.0
+Version: 0.9.1
 Summary: Zstandard bindings for Python
 Home-page: https://github.com/indygreg/python-zstandard
 Author: Gregory Szorc
 Author-email: gregory.szorc@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: ================
```

