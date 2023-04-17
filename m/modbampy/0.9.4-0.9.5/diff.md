# Comparing `tmp/modbampy-0.9.4.tar.gz` & `tmp/modbampy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbampy-0.9.4.tar", last modified: Thu Mar 30 12:45:43 2023, max compression
+gzip compressed data, was "modbampy-0.9.5.tar", last modified: Mon Apr 17 11:25:14 2023, max compression
```

## Comparing `modbampy-0.9.4.tar` & `modbampy-0.9.5.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.272608 modbampy-0.9.4/
--rw-rw-rw-   0 root         (0) root         (0)    16725 2023-03-30 12:44:37.000000 modbampy-0.9.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-03-30 12:44:37.000000 modbampy-0.9.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3821 2023-03-30 12:44:37.000000 modbampy-0.9.4/Makefile
--rw-r--r--   0 root         (0) root         (0)    17924 2023-03-30 12:45:43.268608 modbampy-0.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-03-30 12:44:37.000000 modbampy-0.9.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-03-30 12:44:37.000000 modbampy-0.9.4/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.036589 modbampy-0.9.4/htslib/
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/.appveyor.yml
--rw-rw-rw-   0 root         (0) root         (0)     4756 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/.cirrus.yml
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-03-30 12:44:43.000000 modbampy-0.9.4/htslib/.git
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/.gitmodules
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/INSTALL
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    43947 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    79495 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/NEWS
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/README
--rw-rw-rw-   0 root         (0) root         (0)     7784 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/README.large_positions.md
--rw-rw-rw-   0 root         (0) root         (0)     4131 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/README.md
--rw-rw-rw-   0 root         (0) root         (0)    22986 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/bcf_sr_sort.c
--rw-rw-rw-   0 root         (0) root         (0)     3869 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/bcf_sr_sort.h
--rw-rw-rw-   0 root         (0) root         (0)    81695 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/bgzf.c
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/bgzip.1
--rw-rw-rw-   0 root         (0) root         (0)    15717 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/bgzip.c
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/builddir_vars.mk.in
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/config.mk.in
--rw-rw-rw-   0 root         (0) root         (0)    21655 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/configure.ac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.060591 modbampy-0.9.4/htslib/cram/
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram.h
--rw-rw-rw-   0 root         (0) root         (0)   121688 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_codecs.c
--rw-rw-rw-   0 root         (0) root         (0)     8507 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_codecs.h
--rw-rw-rw-   0 root         (0) root         (0)   126131 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_decode.c
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_decode.h
--rw-rw-rw-   0 root         (0) root         (0)   137752 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_encode.c
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_encode.h
--rw-rw-rw-   0 root         (0) root         (0)    13923 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_external.c
--rw-rw-rw-   0 root         (0) root         (0)    22787 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_index.c
--rw-rw-rw-   0 root         (0) root         (0)     3866 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_index.h
--rw-rw-rw-   0 root         (0) root         (0)   173012 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_io.c
--rw-rw-rw-   0 root         (0) root         (0)    18202 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_io.h
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_samtools.h
--rw-rw-rw-   0 root         (0) root         (0)     7036 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_stats.c
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_stats.h
--rw-rw-rw-   0 root         (0) root         (0)    29085 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/cram_structs.h
--rw-rw-rw-   0 root         (0) root         (0)    17233 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/mFILE.c
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/mFILE.h
--rw-rw-rw-   0 root         (0) root         (0)     3371 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/misc.h
--rw-rw-rw-   0 root         (0) root         (0)    13991 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/open_trace_file.c
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/open_trace_file.h
--rw-rw-rw-   0 root         (0) root         (0)     6816 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/os.h
--rw-rw-rw-   0 root         (0) root         (0)     5049 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/pooled_alloc.c
--rw-rw-rw-   0 root         (0) root         (0)     2185 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/pooled_alloc.h
--rw-rw-rw-   0 root         (0) root         (0)     4422 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/string_alloc.c
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/cram/string_alloc.h
--rw-rw-rw-   0 root         (0) root         (0)     6757 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/errmod.c
--rw-rw-rw-   0 root         (0) root         (0)     6262 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/faidx.5
--rw-rw-rw-   0 root         (0) root         (0)    27173 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/faidx.c
--rw-rw-rw-   0 root         (0) root         (0)    80191 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/header.c
--rw-rw-rw-   0 root         (0) root         (0)    10466 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/header.h
--rw-rw-rw-   0 root         (0) root         (0)    39701 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile.c
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile_gcs.c
--rw-rw-rw-   0 root         (0) root         (0)     8112 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile_internal.h
--rw-rw-rw-   0 root         (0) root         (0)    48933 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile_libcurl.c
--rw-rw-rw-   0 root         (0) root         (0)    39724 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile_s3.c
--rw-rw-rw-   0 root         (0) root         (0)    24154 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hfile_s3_write.c
--rw-rw-rw-   0 root         (0) root         (0)   155740 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts.c
--rw-rw-rw-   0 root         (0) root         (0)    28360 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts_expr.c
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts_internal.h
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts_os.c
--rwxrwxrwx   0 root         (0) root         (0)     3119 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts_probe_cc.sh
--rw-rw-rw-   0 root         (0) root         (0)     5886 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/hts_time_funcs.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.064591 modbampy-0.9.4/htslib/htscodecs/
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/.appveyor.yml
--rw-rw-rw-   0 root         (0) root         (0)     4089 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/.cirrus.yml
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/.git
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/BENCHMARKS.md
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/MAINTAINERS.md
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/Makefile.am
--rw-rw-rw-   0 root         (0) root         (0)     7339 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/NEWS.md
--rw-rw-rw-   0 root         (0) root         (0)     9728 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7327 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/configure.ac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.072592 modbampy-0.9.4/htslib/htscodecs/htscodecs/
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/Makefile.am
--rw-rw-rw-   0 root         (0) root         (0)    35772 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/arith_dynamic.c
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/arith_dynamic.h
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/c_range_coder.h
--rw-rw-rw-   0 root         (0) root         (0)     5742 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/c_simple_model.h
--rw-rw-rw-   0 root         (0) root         (0)    46411 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/fqzcomp_qual.c
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/fqzcomp_qual.h
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs.c
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs.h
--rw-rw-rw-   0 root         (0) root         (0)     3557 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs_endian.h
--rw-rw-rw-   0 root         (0) root         (0)    10630 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/pack.c
--rw-rw-rw-   0 root         (0) root         (0)     3292 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/pack.h
--rw-rw-rw-   0 root         (0) root         (0)    14270 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/permute.h
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/pooled_alloc.h
--rw-rw-rw-   0 root         (0) root         (0)    18584 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_byte.h
--rw-rw-rw-   0 root         (0) root         (0)    24824 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static.c
--rw-rw-rw-   0 root         (0) root         (0)     2079 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static.h
--rw-rw-rw-   0 root         (0) root         (0)    19473 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static16_int.h
--rw-rw-rw-   0 root         (0) root         (0)    24916 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr.c
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr.h
--rw-rw-rw-   0 root         (0) root         (0)    64565 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx2.c
--rw-rw-rw-   0 root         (0) root         (0)    38963 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx512.c
--rw-rw-rw-   0 root         (0) root         (0)    75051 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_neon.c
--rw-rw-rw-   0 root         (0) root         (0)    70432 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_sse4.c
--rw-rw-rw-   0 root         (0) root         (0)     4169 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static4x16.h
--rw-rw-rw-   0 root         (0) root         (0)    52031 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static4x16pr.c
--rw-rw-rw-   0 root         (0) root         (0)    16469 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_word.h
--rw-rw-rw-   0 root         (0) root         (0)     6760 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rle.c
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/rle.h
--rw-rw-rw-   0 root         (0) root         (0)    58271 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/tokenise_name3.c
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/tokenise_name3.h
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/utils.c
--rw-rw-rw-   0 root         (0) root         (0)    11661 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/utils.h
--rw-rw-rw-   0 root         (0) root         (0)    12439 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/varint.h
--rw-rw-rw-   0 root         (0) root         (0)     9715 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/htscodecs/varint2.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.076592 modbampy-0.9.4/htslib/htscodecs/javascript/
--rw-rw-rw-   0 root         (0) root         (0)     5655 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/README.md
--rw-rw-rw-   0 root         (0) root         (0)    16014 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/arith_gen.js
--rw-rw-rw-   0 root         (0) root         (0)     5054 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/arith_sh.js
--rw-rw-rw-   0 root         (0) root         (0)     3829 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/byte_model.js
--rw-rw-rw-   0 root         (0) root         (0)    22412 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/fqzcomp.js
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/index.js
--rw-rw-rw-   0 root         (0) root         (0)     6533 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/iostream.js
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/main_arith_gen.js
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/main_fqzcomp.js
--rw-rw-rw-   0 root         (0) root         (0)     3026 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/main_rans.js
--rw-rw-rw-   0 root         (0) root         (0)     3055 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/main_rans4x16.js
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/main_tok3.js
--rw-rw-rw-   0 root         (0) root         (0)    14143 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/rans.js
--rw-rw-rw-   0 root         (0) root         (0)    25671 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/rans4x16.js
--rw-rw-rw-   0 root         (0) root         (0)    10220 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/javascript/tok3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.076592 modbampy-0.9.4/htslib/htscodecs/m4/
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/m4/ax_check_compile_flag.m4
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/m4/ax_with_libdeflate.m4
--rw-rw-rw-   0 root         (0) root         (0)     5068 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/m4/vl_prog_warnings.m4
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/m4/zlib.m4
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.080592 modbampy-0.9.4/htslib/htscodecs/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/arith_dynamic_fuzz.c
--rw-rw-rw-   0 root         (0) root         (0)     8886 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/arith_dynamic_test.c
--rw-rw-rw-   0 root         (0) root         (0)     8400 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/entropy.c
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c
--rw-rw-rw-   0 root         (0) root         (0)    14190 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/fqzcomp_qual_test.c
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c
--rw-rw-rw-   0 root         (0) root         (0)    10395 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/rANS_static4x16pr_test.c
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/rANS_static_fuzz.c
--rw-rw-rw-   0 root         (0) root         (0)     8681 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/rANS_static_test.c
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/tokenise_name3_fuzz.c
--rw-rw-rw-   0 root         (0) root         (0)     6384 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/tokenise_name3_test.c
--rw-rw-rw-   0 root         (0) root         (0)    10245 2023-03-30 12:44:47.000000 modbampy-0.9.4/htslib/htscodecs/tests/varint_test.c
--rw-rw-rw-   0 root         (0) root         (0)     3775 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htscodecs_bundled.mk
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htscodecs_external.mk
--rw-rw-rw-   0 root         (0) root         (0)     3857 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htsfile.1
--rw-rw-rw-   0 root         (0) root         (0)     9617 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htsfile.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.104595 modbampy-0.9.4/htslib/htslib/
--rw-rw-rw-   0 root         (0) root         (0)    16453 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/bgzf.h
--rw-rw-rw-   0 root         (0) root         (0)    17961 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/cram.h
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/faidx.h
--rw-rw-rw-   0 root         (0) root         (0)    13351 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hfile.h
--rw-rw-rw-   0 root         (0) root         (0)    57362 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts.h
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts_defs.h
--rw-rw-rw-   0 root         (0) root         (0)    11708 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts_endian.h
--rw-rw-rw-   0 root         (0) root         (0)     5991 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts_expr.h
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts_log.h
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/hts_os.h
--rw-rw-rw-   0 root         (0) root         (0)     5605 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/kbitset.h
--rw-rw-rw-   0 root         (0) root         (0)     2828 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/kfunc.h
--rw-rw-rw-   0 root         (0) root         (0)    22899 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/khash.h
--rw-rw-rw-   0 root         (0) root         (0)     4050 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/khash_str2int.h
--rw-rw-rw-   0 root         (0) root         (0)     5135 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/klist.h
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/knetfile.h
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/kroundup.h
--rw-rw-rw-   0 root         (0) root         (0)     8916 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/kseq.h
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/ksort.h
--rw-rw-rw-   0 root         (0) root         (0)    11462 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/kstring.h
--rw-rw-rw-   0 root         (0) root         (0)     8881 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/regidx.h
--rw-rw-rw-   0 root         (0) root         (0)    87719 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/sam.h
--rw-rw-rw-   0 root         (0) root         (0)    16293 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/synced_bcf_reader.h
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/tbx.h
--rw-rw-rw-   0 root         (0) root         (0)    12747 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/thread_pool.h
--rw-rw-rw-   0 root         (0) root         (0)    66805 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/vcf.h
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/vcf_sweep.h
--rw-rw-rw-   0 root         (0) root         (0)     4919 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib/vcfutils.h
--rw-rw-rw-   0 root         (0) root         (0)     7338 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib-s3-plugin.7
--rw-rw-rw-   0 root         (0) root         (0)     6849 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib.mk
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib.pc.in
--rw-rw-rw-   0 root         (0) root         (0)     3333 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/htslib_vars.mk
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/kfunc.c
--rw-rw-rw-   0 root         (0) root         (0)    10570 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/kstring.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.108595 modbampy-0.9.4/htslib/m4/
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/m4/ax_check_compile_flag.m4
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/m4/hts_hide_dynamic_syms.m4
--rw-rw-rw-   0 root         (0) root         (0)     8273 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/m4/hts_prog_cc_warnings.m4
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/m4/pkg.m4
--rw-rw-rw-   0 root         (0) root         (0)    10656 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/md5.c
--rw-rw-rw-   0 root         (0) root         (0)     8488 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/multipart.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.108595 modbampy-0.9.4/htslib/os/
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/os/lzma_stub.h
--rw-rw-rw-   0 root         (0) root         (0)     2704 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/os/rand.c
--rw-rw-rw-   0 root         (0) root         (0)     6501 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/plugin.c
--rw-rw-rw-   0 root         (0) root         (0)    16107 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/probaln.c
--rw-rw-rw-   0 root         (0) root         (0)    12493 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/realn.c
--rw-rw-rw-   0 root         (0) root         (0)    19883 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/regidx.c
--rw-rw-rw-   0 root         (0) root         (0)     7744 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/region.c
--rw-rw-rw-   0 root         (0) root         (0)     2789 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/sam.5
--rw-rw-rw-   0 root         (0) root         (0)   210267 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/sam.c
--rw-rw-rw-   0 root         (0) root         (0)     3487 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/sam_internal.h
--rw-rw-rw-   0 root         (0) root         (0)    47473 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/synced_bcf_reader.c
--rw-rw-rw-   0 root         (0) root         (0)     6986 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/tabix.1
--rw-rw-rw-   0 root         (0) root         (0)    26296 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/tabix.c
--rw-rw-rw-   0 root         (0) root         (0)    15836 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/tbx.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.116595 modbampy-0.9.4/htslib/test/
--rw-rw-rw-   0 root         (0) root         (0)     2438 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/fieldarith.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.116595 modbampy-0.9.4/htslib/test/fuzz/
--rw-rw-rw-   0 root         (0) root         (0)     3964 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/fuzz/hts_open_fuzzer.c
--rw-rw-rw-   0 root         (0) root         (0)    12012 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/hfile.c
--rw-rw-rw-   0 root         (0) root         (0)    17620 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/hts_endian.c
--rw-rw-rw-   0 root         (0) root         (0)     7002 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/pileup.c
--rw-rw-rw-   0 root         (0) root         (0)     7081 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/pileup_mod.c
--rw-rw-rw-   0 root         (0) root         (0)     5072 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/plugins-dlhts.c
--rw-rw-rw-   0 root         (0) root         (0)    80762 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/sam.c
--rw-rw-rw-   0 root         (0) root         (0)     5167 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-bcf-sr.c
--rw-rw-rw-   0 root         (0) root         (0)     8964 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-bcf-translate.c
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-bcf_set_variant_type.c
--rw-rw-rw-   0 root         (0) root         (0)     7064 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-parse-reg.c
--rw-rw-rw-   0 root         (0) root         (0)    16871 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-regidx.c
--rw-rw-rw-   0 root         (0) root         (0)    23890 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-vcf-api.c
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test-vcf-sweep.c
--rw-rw-rw-   0 root         (0) root         (0)    31594 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_bgzf.c
--rw-rw-rw-   0 root         (0) root         (0)    12549 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_expr.c
--rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_index.c
--rw-rw-rw-   0 root         (0) root         (0)     3313 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_introspection.c
--rw-rw-rw-   0 root         (0) root         (0)     3639 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_kfunc.c
--rw-rw-rw-   0 root         (0) root         (0)    12102 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_kstring.c
--rw-rw-rw-   0 root         (0) root         (0)     7063 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_mod.c
--rw-rw-rw-   0 root         (0) root         (0)     5057 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_realn.c
--rw-rw-rw-   0 root         (0) root         (0)     8892 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_str2int.c
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_time_funcs.c
--rw-rw-rw-   0 root         (0) root         (0)    14820 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/test_view.c
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads1.c
--rw-rw-rw-   0 root         (0) root         (0)     1621 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads2.c
--rw-rw-rw-   0 root         (0) root         (0)     1729 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads3.c
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads4.c
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads5.c
--rw-rw-rw-   0 root         (0) root         (0)     3412 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads6.c
--rw-rw-rw-   0 root         (0) root         (0)     3661 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/test/thrash_threads7.c
--rw-rw-rw-   0 root         (0) root         (0)    11957 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/textutils.c
--rw-rw-rw-   0 root         (0) root         (0)    14883 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/textutils_internal.h
--rw-rw-rw-   0 root         (0) root         (0)    45743 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/thread_pool.c
--rw-rw-rw-   0 root         (0) root         (0)     5853 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/thread_pool_internal.h
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/vcf.5
--rw-rw-rw-   0 root         (0) root         (0)   172702 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/vcf.c
--rw-rw-rw-   0 root         (0) root         (0)     5570 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/vcf_sweep.c
--rw-rw-rw-   0 root         (0) root         (0)    34891 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/vcfutils.c
--rwxrwxrwx   0 root         (0) root         (0)     2223 2023-03-30 12:44:45.000000 modbampy-0.9.4/htslib/version.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.120596 modbampy-0.9.4/images/
--rw-rw-rw-   0 root         (0) root         (0)    35610 2023-03-30 12:44:37.000000 modbampy-0.9.4/images/ONT_logo_590x106.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.120596 modbampy-0.9.4/libdeflate/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/.cirrus.yml
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-03-30 12:44:45.000000 modbampy-0.9.4/libdeflate/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:42.972584 modbampy-0.9.4/libdeflate/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.124596 modbampy-0.9.4/libdeflate/.github/workflows/
--rw-rw-rw-   0 root         (0) root         (0)     4229 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/.github/workflows/android.yml
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/.github/workflows/ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    13278 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/Makefile.msc
--rw-rw-rw-   0 root         (0) root         (0)     9437 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/NEWS.md
--rw-rw-rw-   0 root         (0) root         (0)    12146 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.124596 modbampy-0.9.4/libdeflate/common/
--rw-rw-rw-   0 root         (0) root         (0)     9618 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/common/common_defs.h
--rw-rw-rw-   0 root         (0) root         (0)     7592 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/common/compiler_gcc.h
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/common/compiler_msc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.128596 modbampy-0.9.4/libdeflate/lib/
--rw-rw-rw-   0 root         (0) root         (0)     3638 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/adler32.c
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/adler32_vec_template.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.128596 modbampy-0.9.4/libdeflate/lib/arm/
--rw-rw-rw-   0 root         (0) root         (0)     4527 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/arm/adler32_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/arm/cpu_features.c
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/arm/cpu_features.h
--rw-rw-rw-   0 root         (0) root         (0)     7595 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/arm/crc32_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     2839 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/arm/matchfinder_impl.h
--rw-rw-rw-   0 root         (0) root         (0)    11537 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/bt_matchfinder.h
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/cpu_features_common.h
--rw-rw-rw-   0 root         (0) root         (0)    10495 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/crc32.c
--rw-rw-rw-   0 root         (0) root         (0)    25448 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/crc32_table.h
--rw-rw-rw-   0 root         (0) root         (0)     2114 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/crc32_vec_template.h
--rw-rw-rw-   0 root         (0) root         (0)    12769 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/decompress_template.h
--rw-rw-rw-   0 root         (0) root         (0)   124274 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/deflate_compress.c
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/deflate_compress.h
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/deflate_constants.h
--rw-rw-rw-   0 root         (0) root         (0)    38953 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/deflate_decompress.c
--rw-rw-rw-   0 root         (0) root         (0)     2744 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/gzip_compress.c
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/gzip_constants.h
--rw-rw-rw-   0 root         (0) root         (0)     4054 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/gzip_decompress.c
--rw-rw-rw-   0 root         (0) root         (0)    14042 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/hc_matchfinder.h
--rw-rw-rw-   0 root         (0) root         (0)     7207 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/ht_matchfinder.h
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/lib_common.h
--rw-rw-rw-   0 root         (0) root         (0)     5124 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/matchfinder_common.h
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/unaligned.h
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/utils.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.156599 modbampy-0.9.4/libdeflate/lib/x86/
--rw-rw-rw-   0 root         (0) root         (0)    12149 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/adler32_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/cpu_features.c
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/cpu_features.h
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/crc32_impl.h
--rw-rw-rw-   0 root         (0) root         (0)    10451 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/decompress_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     3742 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/x86/matchfinder_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/zlib_compress.c
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/zlib_constants.h
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/lib/zlib_decompress.c
--rw-rw-rw-   0 root         (0) root         (0)    15154 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/libdeflate.h
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/libdeflate.pc.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.164599 modbampy-0.9.4/libdeflate/programs/
--rw-rw-rw-   0 root         (0) root         (0)    17356 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/benchmark.c
--rw-rw-rw-   0 root         (0) root         (0)     4605 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/checksum.c
--rw-rw-rw-   0 root         (0) root         (0)    17311 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/gzip.c
--rw-rw-rw-   0 root         (0) root         (0)    11277 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/prog_util.c
--rw-rw-rw-   0 root         (0) root         (0)     4767 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/prog_util.h
--rw-rw-rw-   0 root         (0) root         (0)     5012 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_checksums.c
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_custom_malloc.c
--rw-rw-rw-   0 root         (0) root         (0)    11890 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_incomplete_codes.c
--rw-rw-rw-   0 root         (0) root         (0)     2207 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_litrunlen_overflow.c
--rw-rw-rw-   0 root         (0) root         (0)     2686 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_overread.c
--rw-rw-rw-   0 root         (0) root         (0)    22742 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_slow_decompression.c
--rw-rw-rw-   0 root         (0) root         (0)     5221 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_trailing_bytes.c
--rw-rw-rw-   0 root         (0) root         (0)     5695 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_util.c
--rw-rw-rw-   0 root         (0) root         (0)     2127 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/test_util.h
--rw-rw-rw-   0 root         (0) root         (0)     3530 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.168600 modbampy-0.9.4/libdeflate/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.192602 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.192602 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_compress/
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.204603 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/0
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.216604 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_decompress/
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.216604 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/0
--rwxrwxrwx   0 root         (0) root         (0)     2551 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/fuzz.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.228605 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/gzip_decompress/
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.248606 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/0
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.248606 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/zlib_decompress/
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.256607 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/0
--rwxrwxrwx   0 root         (0) root         (0)     1894 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/android_build.sh
--rwxrwxrwx   0 root         (0) root         (0)     1948 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/android_tests.sh
--rwxrwxrwx   0 root         (0) root         (0)     3374 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/checksum_benchmarks.sh
--rwxrwxrwx   0 root         (0) root         (0)     2361 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/deflate_benchmarks.sh
--rwxrwxrwx   0 root         (0) root         (0)     1512 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/detect.sh
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/exec_tests.sh
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/gen_crc32_multipliers.c
--rw-rw-rw-   0 root         (0) root         (0)     3156 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/gen_crc32_table.c
--rwxrwxrwx   0 root         (0) root         (0)     1273 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/gen_default_litlen_costs.py
--rwxrwxrwx   0 root         (0) root         (0)     1459 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/gen_offset_slot_map.py
--rwxrwxrwx   0 root         (0) root         (0)    11640 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/gzip_tests.sh
--rwxrwxrwx   0 root         (0) root         (0)      563 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/make-windows-releases.sh
--rwxrwxrwx   0 root         (0) root         (0)       75 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/msc_test.bat
--rwxrwxrwx   0 root         (0) root         (0)      617 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/pgo_build.sh
--rwxrwxrwx   0 root         (0) root         (0)     8427 2023-03-30 12:44:49.000000 modbampy-0.9.4/libdeflate/scripts/run_tests.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.260607 modbampy-0.9.4/modbampy/
--rw-rw-rw-   0 root         (0) root         (0)    14462 2023-03-30 12:44:37.000000 modbampy-0.9.4/modbampy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.260607 modbampy-0.9.4/modbampy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17924 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10523 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-30 12:45:42.000000 modbampy-0.9.4/modbampy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-03-30 12:44:37.000000 modbampy-0.9.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 12:45:43.272608 modbampy-0.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-03-30 12:44:37.000000 modbampy-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.268608 modbampy-0.9.4/src/
--rw-rw-rw-   0 root         (0) root         (0)    10424 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/args.c
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/args.h
--rw-rw-rw-   0 root         (0) root         (0)     6201 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/bamiter.c
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/bamiter.h
--rw-rw-rw-   0 root         (0) root         (0)     1498 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/common.c
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/common.h
--rw-rw-rw-   0 root         (0) root         (0)    27414 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/counts.c
--rw-rw-rw-   0 root         (0) root         (0)     5264 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/counts.h
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/modbam2bed.c
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-30 12:44:37.000000 modbampy-0.9.4/src/version.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:45:43.268608 modbampy-0.9.4/test/
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-03-30 12:44:37.000000 modbampy-0.9.4/test/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-03-30 12:44:37.000000 modbampy-0.9.4/test/test_motifs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.690623 modbampy-0.9.5/
+-rw-rw-rw-   0 root         (0) root         (0)    14378 2023-04-17 11:21:42.000000 modbampy-0.9.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-17 11:21:42.000000 modbampy-0.9.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3865 2023-04-17 11:21:42.000000 modbampy-0.9.5/Makefile
+-rw-r--r--   0 root         (0) root         (0)    18306 2023-04-17 11:25:14.690623 modbampy-0.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2023-04-17 11:21:42.000000 modbampy-0.9.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2023-04-17 11:21:42.000000 modbampy-0.9.5/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.506607 modbampy-0.9.5/htslib/
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/.appveyor.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4756 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/.cirrus.yml
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 11:21:44.000000 modbampy-0.9.5/htslib/.git
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/.gitmodules
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/INSTALL
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    43947 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    79495 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/NEWS
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/README
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/README.large_positions.md
+-rw-rw-rw-   0 root         (0) root         (0)     4131 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    22986 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/bcf_sr_sort.c
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/bcf_sr_sort.h
+-rw-rw-rw-   0 root         (0) root         (0)    81695 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/bgzf.c
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/bgzip.1
+-rw-rw-rw-   0 root         (0) root         (0)    15717 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/bgzip.c
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/builddir_vars.mk.in
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/config.mk.in
+-rw-rw-rw-   0 root         (0) root         (0)    21655 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/configure.ac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.514608 modbampy-0.9.5/htslib/cram/
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram.h
+-rw-rw-rw-   0 root         (0) root         (0)   121688 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_codecs.c
+-rw-rw-rw-   0 root         (0) root         (0)     8507 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_codecs.h
+-rw-rw-rw-   0 root         (0) root         (0)   126131 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_decode.c
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_decode.h
+-rw-rw-rw-   0 root         (0) root         (0)   137752 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_encode.c
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_encode.h
+-rw-rw-rw-   0 root         (0) root         (0)    13923 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_external.c
+-rw-rw-rw-   0 root         (0) root         (0)    22787 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_index.c
+-rw-rw-rw-   0 root         (0) root         (0)     3866 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_index.h
+-rw-rw-rw-   0 root         (0) root         (0)   173012 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_io.c
+-rw-rw-rw-   0 root         (0) root         (0)    18202 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_io.h
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_samtools.h
+-rw-rw-rw-   0 root         (0) root         (0)     7036 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_stats.c
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_stats.h
+-rw-rw-rw-   0 root         (0) root         (0)    29085 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/cram_structs.h
+-rw-rw-rw-   0 root         (0) root         (0)    17233 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/mFILE.c
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/mFILE.h
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/misc.h
+-rw-rw-rw-   0 root         (0) root         (0)    13991 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/open_trace_file.c
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/open_trace_file.h
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/os.h
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/pooled_alloc.c
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/pooled_alloc.h
+-rw-rw-rw-   0 root         (0) root         (0)     4422 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/string_alloc.c
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/cram/string_alloc.h
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/errmod.c
+-rw-rw-rw-   0 root         (0) root         (0)     6262 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/faidx.5
+-rw-rw-rw-   0 root         (0) root         (0)    27173 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/faidx.c
+-rw-rw-rw-   0 root         (0) root         (0)    80191 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/header.c
+-rw-rw-rw-   0 root         (0) root         (0)    10466 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/header.h
+-rw-rw-rw-   0 root         (0) root         (0)    39701 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile.c
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile_gcs.c
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)    48933 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile_libcurl.c
+-rw-rw-rw-   0 root         (0) root         (0)    39724 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile_s3.c
+-rw-rw-rw-   0 root         (0) root         (0)    24154 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hfile_s3_write.c
+-rw-rw-rw-   0 root         (0) root         (0)   155740 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts.c
+-rw-rw-rw-   0 root         (0) root         (0)    28360 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts_expr.c
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts_os.c
+-rwxrwxrwx   0 root         (0) root         (0)     3119 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts_probe_cc.sh
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/hts_time_funcs.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.514608 modbampy-0.9.5/htslib/htscodecs/
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/.appveyor.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4089 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/.cirrus.yml
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/.git
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/BENCHMARKS.md
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/MAINTAINERS.md
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/Makefile.am
+-rw-rw-rw-   0 root         (0) root         (0)     7339 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/NEWS.md
+-rw-rw-rw-   0 root         (0) root         (0)     9728 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7327 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/configure.ac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.522608 modbampy-0.9.5/htslib/htscodecs/htscodecs/
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/Makefile.am
+-rw-rw-rw-   0 root         (0) root         (0)    35772 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/arith_dynamic.c
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/arith_dynamic.h
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/c_range_coder.h
+-rw-rw-rw-   0 root         (0) root         (0)     5742 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/c_simple_model.h
+-rw-rw-rw-   0 root         (0) root         (0)    46411 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/fqzcomp_qual.c
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/fqzcomp_qual.h
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs.c
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs.h
+-rw-rw-rw-   0 root         (0) root         (0)     3557 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs_endian.h
+-rw-rw-rw-   0 root         (0) root         (0)    10630 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/pack.c
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/pack.h
+-rw-rw-rw-   0 root         (0) root         (0)    14270 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/permute.h
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/pooled_alloc.h
+-rw-rw-rw-   0 root         (0) root         (0)    18584 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_byte.h
+-rw-rw-rw-   0 root         (0) root         (0)    24824 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static.c
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static.h
+-rw-rw-rw-   0 root         (0) root         (0)    19473 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static16_int.h
+-rw-rw-rw-   0 root         (0) root         (0)    24916 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr.c
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr.h
+-rw-rw-rw-   0 root         (0) root         (0)    64565 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx2.c
+-rw-rw-rw-   0 root         (0) root         (0)    38963 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx512.c
+-rw-rw-rw-   0 root         (0) root         (0)    75051 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_neon.c
+-rw-rw-rw-   0 root         (0) root         (0)    70432 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_sse4.c
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static4x16.h
+-rw-rw-rw-   0 root         (0) root         (0)    52031 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static4x16pr.c
+-rw-rw-rw-   0 root         (0) root         (0)    16469 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_word.h
+-rw-rw-rw-   0 root         (0) root         (0)     6760 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rle.c
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/rle.h
+-rw-rw-rw-   0 root         (0) root         (0)    58271 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/tokenise_name3.c
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/tokenise_name3.h
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/utils.c
+-rw-rw-rw-   0 root         (0) root         (0)    11661 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/utils.h
+-rw-rw-rw-   0 root         (0) root         (0)    12439 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/varint.h
+-rw-rw-rw-   0 root         (0) root         (0)     9715 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/htscodecs/varint2.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.526609 modbampy-0.9.5/htslib/htscodecs/javascript/
+-rw-rw-rw-   0 root         (0) root         (0)     5655 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    16014 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/arith_gen.js
+-rw-rw-rw-   0 root         (0) root         (0)     5054 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/arith_sh.js
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/byte_model.js
+-rw-rw-rw-   0 root         (0) root         (0)    22412 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/fqzcomp.js
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/index.js
+-rw-rw-rw-   0 root         (0) root         (0)     6533 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/iostream.js
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/main_arith_gen.js
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/main_fqzcomp.js
+-rw-rw-rw-   0 root         (0) root         (0)     3026 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/main_rans.js
+-rw-rw-rw-   0 root         (0) root         (0)     3055 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/main_rans4x16.js
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/main_tok3.js
+-rw-rw-rw-   0 root         (0) root         (0)    14143 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/rans.js
+-rw-rw-rw-   0 root         (0) root         (0)    25671 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/rans4x16.js
+-rw-rw-rw-   0 root         (0) root         (0)    10220 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/javascript/tok3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.526609 modbampy-0.9.5/htslib/htscodecs/m4/
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/m4/ax_check_compile_flag.m4
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/m4/ax_with_libdeflate.m4
+-rw-rw-rw-   0 root         (0) root         (0)     5068 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/m4/vl_prog_warnings.m4
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/m4/zlib.m4
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.526609 modbampy-0.9.5/htslib/htscodecs/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/arith_dynamic_fuzz.c
+-rw-rw-rw-   0 root         (0) root         (0)     8886 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/arith_dynamic_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     8400 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/entropy.c
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c
+-rw-rw-rw-   0 root         (0) root         (0)    14190 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/fqzcomp_qual_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c
+-rw-rw-rw-   0 root         (0) root         (0)    10395 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/rANS_static4x16pr_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/rANS_static_fuzz.c
+-rw-rw-rw-   0 root         (0) root         (0)     8681 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/rANS_static_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/tokenise_name3_fuzz.c
+-rw-rw-rw-   0 root         (0) root         (0)     6384 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/tokenise_name3_test.c
+-rw-rw-rw-   0 root         (0) root         (0)    10245 2023-04-17 11:21:46.000000 modbampy-0.9.5/htslib/htscodecs/tests/varint_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     3775 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htscodecs_bundled.mk
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htscodecs_external.mk
+-rw-rw-rw-   0 root         (0) root         (0)     3857 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htsfile.1
+-rw-rw-rw-   0 root         (0) root         (0)     9617 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htsfile.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.566612 modbampy-0.9.5/htslib/htslib/
+-rw-rw-rw-   0 root         (0) root         (0)    16453 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/bgzf.h
+-rw-rw-rw-   0 root         (0) root         (0)    17961 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/cram.h
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/faidx.h
+-rw-rw-rw-   0 root         (0) root         (0)    13351 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hfile.h
+-rw-rw-rw-   0 root         (0) root         (0)    57362 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts.h
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts_defs.h
+-rw-rw-rw-   0 root         (0) root         (0)    11708 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts_endian.h
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts_expr.h
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts_log.h
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/hts_os.h
+-rw-rw-rw-   0 root         (0) root         (0)     5605 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/kbitset.h
+-rw-rw-rw-   0 root         (0) root         (0)     2828 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/kfunc.h
+-rw-rw-rw-   0 root         (0) root         (0)    22899 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/khash.h
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/khash_str2int.h
+-rw-rw-rw-   0 root         (0) root         (0)     5135 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/klist.h
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/knetfile.h
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/kroundup.h
+-rw-rw-rw-   0 root         (0) root         (0)     8916 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/kseq.h
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/ksort.h
+-rw-rw-rw-   0 root         (0) root         (0)    11462 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/kstring.h
+-rw-rw-rw-   0 root         (0) root         (0)     8881 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/regidx.h
+-rw-rw-rw-   0 root         (0) root         (0)    87719 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/sam.h
+-rw-rw-rw-   0 root         (0) root         (0)    16293 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/synced_bcf_reader.h
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/tbx.h
+-rw-rw-rw-   0 root         (0) root         (0)    12747 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/thread_pool.h
+-rw-rw-rw-   0 root         (0) root         (0)    66805 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/vcf.h
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/vcf_sweep.h
+-rw-rw-rw-   0 root         (0) root         (0)     4919 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib/vcfutils.h
+-rw-rw-rw-   0 root         (0) root         (0)     7338 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib-s3-plugin.7
+-rw-rw-rw-   0 root         (0) root         (0)     6849 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib.mk
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib.pc.in
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/htslib_vars.mk
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/kfunc.c
+-rw-rw-rw-   0 root         (0) root         (0)    10570 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/kstring.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.566612 modbampy-0.9.5/htslib/m4/
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/m4/ax_check_compile_flag.m4
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/m4/hts_hide_dynamic_syms.m4
+-rw-rw-rw-   0 root         (0) root         (0)     8273 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/m4/hts_prog_cc_warnings.m4
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/m4/pkg.m4
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/md5.c
+-rw-rw-rw-   0 root         (0) root         (0)     8488 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/multipart.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.570613 modbampy-0.9.5/htslib/os/
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/os/lzma_stub.h
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/os/rand.c
+-rw-rw-rw-   0 root         (0) root         (0)     6501 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/plugin.c
+-rw-rw-rw-   0 root         (0) root         (0)    16107 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/probaln.c
+-rw-rw-rw-   0 root         (0) root         (0)    12493 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/realn.c
+-rw-rw-rw-   0 root         (0) root         (0)    19883 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/regidx.c
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/region.c
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/sam.5
+-rw-rw-rw-   0 root         (0) root         (0)   210267 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/sam.c
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/sam_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)    47473 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/synced_bcf_reader.c
+-rw-rw-rw-   0 root         (0) root         (0)     6986 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/tabix.1
+-rw-rw-rw-   0 root         (0) root         (0)    26296 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/tabix.c
+-rw-rw-rw-   0 root         (0) root         (0)    15836 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/tbx.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.610616 modbampy-0.9.5/htslib/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/fieldarith.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.610616 modbampy-0.9.5/htslib/test/fuzz/
+-rw-rw-rw-   0 root         (0) root         (0)     3964 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/fuzz/hts_open_fuzzer.c
+-rw-rw-rw-   0 root         (0) root         (0)    12012 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/hfile.c
+-rw-rw-rw-   0 root         (0) root         (0)    17620 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/hts_endian.c
+-rw-rw-rw-   0 root         (0) root         (0)     7002 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/pileup.c
+-rw-rw-rw-   0 root         (0) root         (0)     7081 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/pileup_mod.c
+-rw-rw-rw-   0 root         (0) root         (0)     5072 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/plugins-dlhts.c
+-rw-rw-rw-   0 root         (0) root         (0)    80762 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/sam.c
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-bcf-sr.c
+-rw-rw-rw-   0 root         (0) root         (0)     8964 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-bcf-translate.c
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-bcf_set_variant_type.c
+-rw-rw-rw-   0 root         (0) root         (0)     7064 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-parse-reg.c
+-rw-rw-rw-   0 root         (0) root         (0)    16871 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-regidx.c
+-rw-rw-rw-   0 root         (0) root         (0)    23890 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-vcf-api.c
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test-vcf-sweep.c
+-rw-rw-rw-   0 root         (0) root         (0)    31594 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_bgzf.c
+-rw-rw-rw-   0 root         (0) root         (0)    12549 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_expr.c
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_index.c
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_introspection.c
+-rw-rw-rw-   0 root         (0) root         (0)     3639 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_kfunc.c
+-rw-rw-rw-   0 root         (0) root         (0)    12102 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_kstring.c
+-rw-rw-rw-   0 root         (0) root         (0)     7063 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_mod.c
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_realn.c
+-rw-rw-rw-   0 root         (0) root         (0)     8892 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_str2int.c
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_time_funcs.c
+-rw-rw-rw-   0 root         (0) root         (0)    14820 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/test_view.c
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads1.c
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads2.c
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads3.c
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads4.c
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads5.c
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads6.c
+-rw-rw-rw-   0 root         (0) root         (0)     3661 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/test/thrash_threads7.c
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/textutils.c
+-rw-rw-rw-   0 root         (0) root         (0)    14883 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/textutils_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)    45743 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/thread_pool.c
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/thread_pool_internal.h
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/vcf.5
+-rw-rw-rw-   0 root         (0) root         (0)   172702 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/vcf.c
+-rw-rw-rw-   0 root         (0) root         (0)     5570 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/vcf_sweep.c
+-rw-rw-rw-   0 root         (0) root         (0)    34891 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/vcfutils.c
+-rwxrwxrwx   0 root         (0) root         (0)     2223 2023-04-17 11:21:45.000000 modbampy-0.9.5/htslib/version.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.610616 modbampy-0.9.5/images/
+-rw-rw-rw-   0 root         (0) root         (0)    24104 2023-04-17 11:21:42.000000 modbampy-0.9.5/images/ONT_logo_590x106.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.630618 modbampy-0.9.5/libdeflate/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/.cirrus.yml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-17 11:21:45.000000 modbampy-0.9.5/libdeflate/.git
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.334592 modbampy-0.9.5/libdeflate/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.634618 modbampy-0.9.5/libdeflate/.github/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/.github/workflows/android.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/.github/workflows/ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    13278 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/Makefile.msc
+-rw-rw-rw-   0 root         (0) root         (0)     9437 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/NEWS.md
+-rw-rw-rw-   0 root         (0) root         (0)    12146 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.634618 modbampy-0.9.5/libdeflate/common/
+-rw-rw-rw-   0 root         (0) root         (0)     9618 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/common/common_defs.h
+-rw-rw-rw-   0 root         (0) root         (0)     7592 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/common/compiler_gcc.h
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/common/compiler_msc.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.642619 modbampy-0.9.5/libdeflate/lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/adler32.c
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/adler32_vec_template.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.646619 modbampy-0.9.5/libdeflate/lib/arm/
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/arm/adler32_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/arm/cpu_features.c
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/arm/cpu_features.h
+-rw-rw-rw-   0 root         (0) root         (0)     7595 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/arm/crc32_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/arm/matchfinder_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)    11537 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/bt_matchfinder.h
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/cpu_features_common.h
+-rw-rw-rw-   0 root         (0) root         (0)    10495 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/crc32.c
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/crc32_table.h
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/crc32_vec_template.h
+-rw-rw-rw-   0 root         (0) root         (0)    12769 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/decompress_template.h
+-rw-rw-rw-   0 root         (0) root         (0)   124274 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/deflate_compress.c
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/deflate_compress.h
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/deflate_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)    38953 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/deflate_decompress.c
+-rw-rw-rw-   0 root         (0) root         (0)     2744 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/gzip_compress.c
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/gzip_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)     4054 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/gzip_decompress.c
+-rw-rw-rw-   0 root         (0) root         (0)    14042 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/hc_matchfinder.h
+-rw-rw-rw-   0 root         (0) root         (0)     7207 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/ht_matchfinder.h
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/lib_common.h
+-rw-rw-rw-   0 root         (0) root         (0)     5124 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/matchfinder_common.h
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/unaligned.h
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/utils.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.646619 modbampy-0.9.5/libdeflate/lib/x86/
+-rw-rw-rw-   0 root         (0) root         (0)    12149 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/adler32_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/cpu_features.c
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/cpu_features.h
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/crc32_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)    10451 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/decompress_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)     3742 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/x86/matchfinder_impl.h
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/zlib_compress.c
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/zlib_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/lib/zlib_decompress.c
+-rw-rw-rw-   0 root         (0) root         (0)    15154 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/libdeflate.h
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/libdeflate.pc.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.670621 modbampy-0.9.5/libdeflate/programs/
+-rw-rw-rw-   0 root         (0) root         (0)    17356 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/benchmark.c
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/checksum.c
+-rw-rw-rw-   0 root         (0) root         (0)    17311 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/gzip.c
+-rw-rw-rw-   0 root         (0) root         (0)    11277 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/prog_util.c
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/prog_util.h
+-rw-rw-rw-   0 root         (0) root         (0)     5012 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_checksums.c
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_custom_malloc.c
+-rw-rw-rw-   0 root         (0) root         (0)    11890 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_incomplete_codes.c
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_litrunlen_overflow.c
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_overread.c
+-rw-rw-rw-   0 root         (0) root         (0)    22742 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_slow_decompression.c
+-rw-rw-rw-   0 root         (0) root         (0)     5221 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_trailing_bytes.c
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_util.c
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/test_util.h
+-rw-rw-rw-   0 root         (0) root         (0)     3530 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/programs/tgetopt.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_compress/
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/0
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_decompress/
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/0
+-rwxrwxrwx   0 root         (0) root         (0)     2551 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/fuzz.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/gzip_decompress/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/0
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.678622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/zlib_decompress/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.682622 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/0
+-rwxrwxrwx   0 root         (0) root         (0)     1894 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/android_build.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/android_tests.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3374 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/checksum_benchmarks.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2361 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/deflate_benchmarks.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/detect.sh
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/exec_tests.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/gen_crc32_multipliers.c
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/gen_crc32_table.c
+-rwxrwxrwx   0 root         (0) root         (0)     1273 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/gen_default_litlen_costs.py
+-rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/gen_offset_slot_map.py
+-rwxrwxrwx   0 root         (0) root         (0)    11640 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/gzip_tests.sh
+-rwxrwxrwx   0 root         (0) root         (0)      563 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/make-windows-releases.sh
+-rwxrwxrwx   0 root         (0) root         (0)       75 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/msc_test.bat
+-rwxrwxrwx   0 root         (0) root         (0)      617 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/pgo_build.sh
+-rwxrwxrwx   0 root         (0) root         (0)     8427 2023-04-17 11:21:48.000000 modbampy-0.9.5/libdeflate/scripts/run_tests.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.682622 modbampy-0.9.5/modbampy/
+-rw-rw-rw-   0 root         (0) root         (0)    14462 2023-04-17 11:21:42.000000 modbampy-0.9.5/modbampy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.682622 modbampy-0.9.5/modbampy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18306 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 11:25:14.000000 modbampy-0.9.5/modbampy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-17 11:21:42.000000 modbampy-0.9.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 11:25:14.690623 modbampy-0.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-17 11:21:42.000000 modbampy-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.690623 modbampy-0.9.5/src/
+-rw-rw-rw-   0 root         (0) root         (0)    10424 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/args.c
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/args.h
+-rw-rw-rw-   0 root         (0) root         (0)     6201 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/bamiter.c
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/bamiter.h
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/common.c
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/common.h
+-rw-rw-rw-   0 root         (0) root         (0)    27414 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/counts.c
+-rw-rw-rw-   0 root         (0) root         (0)     5264 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/counts.h
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/modbam2bed.c
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-17 11:21:42.000000 modbampy-0.9.5/src/version.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:25:14.690623 modbampy-0.9.5/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-04-17 11:21:42.000000 modbampy-0.9.5/test/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-17 11:21:42.000000 modbampy-0.9.5/test/test_motifs.py
```

### Comparing `modbampy-0.9.4/LICENSE` & `modbampy-0.9.5/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,70 @@
-Mozilla Public License Version 2.0
-==================================
+Oxford Nanopore Technologies PLC. Public License Version 1.0
+=============================================================
 
 1. Definitions
 --------------
 
 1.1. "Contributor"
     means each individual or legal entity that creates, contributes to
     the creation of, or owns Covered Software.
 
 1.2. "Contributor Version"
     means the combination of the Contributions of others (if any) used
-    by a Contributor and that particular Contributor's Contribution.
+    by a Contributor and that particular Contributor’s Contribution.
 
 1.3. "Contribution"
     means Covered Software of a particular Contributor.
 
 1.4. "Covered Software"
     means Source Code Form to which the initial Contributor has attached
     the notice in Exhibit A, the Executable Form of such Source Code
     Form, and Modifications of such Source Code Form, in each case
     including portions thereof.
 
-1.5. "Incompatible With Secondary Licenses"
-    means
-
-    (a) that the initial Contributor has attached the notice described
-        in Exhibit B to the Covered Software; or
-
-    (b) that the Covered Software was made available under the terms of
-        version 1.1 or earlier of the License, but not also under the
-        terms of a Secondary License.
-
-1.6. "Executable Form"
+1.5. "Executable Form"
     means any form of the work other than Source Code Form.
 
-1.7. "Larger Work"
+1.6. "Larger Work"
     means a work that combines Covered Software with other material, in
     a separate file or files, that is not Covered Software.
 
-1.8. "License"
+1.7. "License"
     means this document.
 
-1.9. "Licensable"
+1.8. "Licensable"
     means having the right to grant, to the maximum extent possible,
     whether at the time of the initial grant or subsequently, any and
     all of the rights conveyed by this License.
 
-1.10. "Modifications"
+1.9. "Modifications"
     means any of the following:
 
-    (a) any file in Source Code Form that results from an addition to,
-        deletion from, or modification of the contents of Covered
-        Software; or
-
-    (b) any new file in Source Code Form that contains any Covered
-        Software.
-
-1.11. "Patent Claims" of a Contributor
-    means any patent claim(s), including without limitation, method,
-    process, and apparatus claims, in any patent Licensable by such
-    Contributor that would be infringed, but for the grant of the
-    License, by the making, using, selling, offering for sale, having
-    made, import, or transfer of either its Contributions or its
-    Contributor Version.
+    (a)	  any file in Source Code Form that results from an addition to,
+          deletion from, or modification of the contents of Covered
+          Software; or
+    (b)   any new file in Source Code Form that contains any Covered
+          Software.
+
+1.10. "Research Purposes"
+    means use for internal research and not intended for or directed
+    towards commercial advantages or monetary compensation; provided,
+    however, that monetary compensation does not include sponsored
+    research of research funded by grants.
 
-1.12. "Secondary License"
+1.11  "Secondary License"
     means either the GNU General Public License, Version 2.0, the GNU
     Lesser General Public License, Version 2.1, the GNU Affero General
     Public License, Version 3.0, or any later versions of those
     licenses.
 
-1.13. "Source Code Form"
+1.12. "Source Code Form"
     means the form of the work preferred for making modifications.
 
-1.14. "You" (or "Your")
+1.13. "You" (or "Your")
     means an individual or a legal entity exercising rights under this
     License. For legal entities, "You" includes any entity that
     controls, is controlled by, or is under common control with You. For
     purposes of this definition, "control" means (a) the power, direct
     or indirect, to cause the direction or management of such entity,
     whether by contract or otherwise, or (b) ownership of more than
     fifty percent (50%) of the outstanding shares or beneficial
@@ -85,61 +72,55 @@
 
 2. License Grants and Conditions
 --------------------------------
 
 2.1. Grants
 
 Each Contributor hereby grants You a world-wide, royalty-free,
-non-exclusive license:
-
-(a) under intellectual property rights (other than patent or trademark)
-    Licensable by such Contributor to use, reproduce, make available,
-    modify, display, perform, distribute, and otherwise exploit its
-    Contributions, either on an unmodified basis, with Modifications, or
-    as part of a Larger Work; and
-
-(b) under Patent Claims of such Contributor to make, use, sell, offer
-    for sale, have made, import, and otherwise transfer either its
-    Contributions or its Contributor Version.
+non-exclusive license under Contributor copyrights Licensable by such
+Contributor to use, reproduce, make available, modify, display,
+perform, distribute, and otherwise exploit solely for Research Purposes
+its Contributions, either on an unmodified basis, with Modifications,
+or as part of a Larger Work.
 
 2.2. Effective Date
 
 The licenses granted in Section 2.1 with respect to any Contribution
-become effective for each Contribution on the date the Contributor first
-distributes such Contribution.
+become effective for each Contribution on the date the Contributor
+first distributes such Contribution.
 
 2.3. Limitations on Grant Scope
 
 The licenses granted in this Section 2 are the only rights granted under
 this License. No additional rights or licenses will be implied from the
-distribution or licensing of Covered Software under this License.
-Notwithstanding Section 2.1(b) above, no patent license is granted by a
-Contributor:
+distribution or licensing of Covered Software under this License. The
+License is incompatible with Secondary Licenses.  Notwithstanding
+Section 2.1 above, no copyright license is granted:
 
 (a) for any code that a Contributor has removed from Covered Software;
     or
 
-(b) for infringements caused by: (i) Your and any other third party's
-    modifications of Covered Software, or (ii) the combination of its
-    Contributions with other software (except as part of its Contributor
-    Version); or
-
-(c) under Patent Claims infringed by Covered Software in the absence of
-    its Contributions.
-
-This License does not grant any rights in the trademarks, service marks,
-or logos of any Contributor (except as may be necessary to comply with
-the notice requirements in Section 3.4).
+(b) use of the Contributions or its Contributor Version other than for
+Research Purposes only; or
+
+(c) for infringements caused by: (i) Your and any other third party’s
+modifications of Covered Software, or (ii) the combination of its
+Contributions with other software (except as part of its Contributor
+Version).
+
+This License does not grant any rights in the patents, trademarks,
+service marks, or logos of any Contributor (except as may be necessary
+to comply with the notice requirements in Section 3.4).
 
 2.4. Subsequent Licenses
 
 No Contributor makes additional grants as a result of Your choice to
 distribute the Covered Software under a subsequent version of this
-License (see Section 10.2) or under the terms of a Secondary License (if
-permitted under the terms of Section 3.3).
+License (see Section 10.2) or under the terms of a Secondary License
+(if permitted under the terms of Section 3.3).
 
 2.5. Representation
 
 Each Contributor represents that the Contributor believes its
 Contributions are its original creation(s) or it has sufficient rights
 to grant the rights to its Contributions conveyed by this License.
 
@@ -160,65 +141,55 @@
 3.1. Distribution of Source Form
 
 All distribution of Covered Software in Source Code Form, including any
 Modifications that You create or to which You contribute, must be under
 the terms of this License. You must inform recipients that the Source
 Code Form of the Covered Software is governed by the terms of this
 License, and how they can obtain a copy of this License. You may not
-attempt to alter or restrict the recipients' rights in the Source Code
-Form.
+attempt to alter or restrict the recipients’ rights in the Source Code Form.
 
 3.2. Distribution of Executable Form
 
 If You distribute Covered Software in Executable Form then:
 
 (a) such Covered Software must also be made available in Source Code
     Form, as described in Section 3.1, and You must inform recipients of
     the Executable Form how they can obtain a copy of such Source Code
     Form by reasonable means in a timely manner, at a charge no more
     than the cost of distribution to the recipient; and
 
 (b) You may distribute such Executable Form under the terms of this
-    License, or sublicense it under different terms, provided that the
-    license for the Executable Form does not attempt to limit or alter
-    the recipients' rights in the Source Code Form under this License.
+    License.
 
 3.3. Distribution of a Larger Work
 
 You may create and distribute a Larger Work under terms of Your choice,
 provided that You also comply with the requirements of this License for
-the Covered Software. If the Larger Work is a combination of Covered
-Software with a work governed by one or more Secondary Licenses, and the
-Covered Software is not Incompatible With Secondary Licenses, this
-License permits You to additionally distribute such Covered Software
-under the terms of such Secondary License(s), so that the recipient of
-the Larger Work may, at their option, further distribute the Covered
-Software under the terms of either this License or such Secondary
-License(s).
+the Covered Software. The Larger Work may not be a combination of Covered
+Software with a work governed by one or more Secondary Licenses.
 
 3.4. Notices
 
 You may not remove or alter the substance of any license notices
 (including copyright notices, patent notices, disclaimers of warranty,
 or limitations of liability) contained within the Source Code Form of
 the Covered Software, except that You may alter any license notices to
 the extent required to remedy known factual inaccuracies.
 
 3.5. Application of Additional Terms
 
-You may choose to offer, and to charge a fee for, warranty, support,
-indemnity or liability obligations to one or more recipients of Covered
-Software. However, You may do so only on Your own behalf, and not on
-behalf of any Contributor. You must make it absolutely clear that any
-such warranty, support, indemnity, or liability obligation is offered by
-You alone, and You hereby agree to indemnify every Contributor for any
-liability incurred by such Contributor as a result of warranty, support,
-indemnity or liability terms You offer. You may include additional
-disclaimers of warranty and limitations of liability specific to any
-jurisdiction.
+You may not choose to offer, or charge a fee for use of the Covered
+Software or a fee for, warranty, support, indemnity or liability
+obligations to one or more recipients of Covered Software.  You must
+make it absolutely clear that any such warranty, support, indemnity, or
+liability obligation is offered by You alone, and You hereby agree to
+indemnify every Contributor for any liability incurred by such
+Contributor as a result of warranty, support, indemnity or liability
+terms You offer. You may include additional disclaimers of warranty and
+limitations of liability specific to any jurisdiction.
 
 4. Inability to Comply Due to Statute or Regulation
 ---------------------------------------------------
 
 If it is impossible for You to comply with any of the terms of this
 License with respect to some or all of the Covered Software due to
 statute, judicial order, or regulation then You must: (a) comply with
@@ -229,31 +200,20 @@
 or regulation, such description must be sufficiently detailed for a
 recipient of ordinary skill to be able to understand it.
 
 5. Termination
 --------------
 
 5.1. The rights granted under this License will terminate automatically
-if You fail to comply with any of its terms. However, if You become
-compliant, then the rights granted under this License from a particular
-Contributor are reinstated (a) provisionally, unless and until such
-Contributor explicitly and finally terminates Your grants, and (b) on an
-ongoing basis, if such Contributor fails to notify You of the
-non-compliance by some reasonable means prior to 60 days after You have
-come back into compliance. Moreover, Your grants from a particular
-Contributor are reinstated on an ongoing basis if such Contributor
-notifies You of the non-compliance by some reasonable means, this is the
-first time You have received notice of non-compliance with this License
-from such Contributor, and You become compliant prior to 30 days after
-Your receipt of the notice.
+if You fail to comply with any of its terms.
 
-5.2. If You initiate litigation against any entity by asserting a patent
+5.2. If You initiate litigation against any entity by asserting an
 infringement claim (excluding declaratory judgment actions,
 counter-claims, and cross-claims) alleging that a Contributor Version
-directly or indirectly infringes any patent, then the rights granted to
+directly or indirectly infringes, then the rights granted to
 You by any and all Contributors for the Covered Software under Section
 2.1 of this License shall terminate.
 
 5.3. In the event of termination under Sections 5.1 or 5.2 above, all
 end user license agreements (excluding distributors and resellers) which
 have been validly granted by You or Your distributors under this License
 prior to termination shall survive termination.
@@ -288,30 +248,32 @@
 *  permitted above, be liable to You for any direct, indirect,         *
 *  special, incidental, or consequential damages of any character      *
 *  including, without limitation, damages for lost profits, loss of    *
 *  goodwill, work stoppage, computer failure or malfunction, or any    *
 *  and all other commercial damages or losses, even if such party      *
 *  shall have been informed of the possibility of such damages. This   *
 *  limitation of liability shall not apply to liability for death or   *
-*  personal injury resulting from such party's negligence to the       *
-*  extent applicable law prohibits such limitation. Some               *
+*  personal injury resulting from such party’s negligence to the       *
+*  extent applicable law prohibits such limitation, but in such event, *
+*  and to the greatest extent permissible, damages will be limited to  *
+*  direct damages not to exceed one hundred dollars. Some              *
 *  jurisdictions do not allow the exclusion or limitation of           *
 *  incidental or consequential damages, so this exclusion and          *
 *  limitation may not apply to You.                                    *
 *                                                                      *
 ************************************************************************
 
 8. Litigation
 -------------
 
 Any litigation relating to this License may be brought only in the
 courts of a jurisdiction where the defendant maintains its principal
 place of business and such litigation shall be governed by laws of that
 jurisdiction, without reference to its conflict-of-law provisions.
-Nothing in this Section shall prevent a party's ability to bring
+Nothing in this Section shall prevent a party’s ability to bring
 cross-claims or counter-claims.
 
 9. Miscellaneous
 ----------------
 
 This License represents the complete agreement concerning the subject
 matter hereof. If any provision of this License is held to be
@@ -321,18 +283,18 @@
 shall not be used to construe this License against a Contributor.
 
 10. Versions of the License
 ---------------------------
 
 10.1. New Versions
 
-Mozilla Foundation is the license steward. Except as provided in Section
-10.3, no one other than the license steward has the right to modify or
-publish new versions of this License. Each version will be given a
-distinguishing version number.
+Oxford Nanopore Technologies PLC. is the license steward. Except as
+provided in Section 10.3, no one other than the license steward has the
+right to modify or publish new versions of this License. Each version
+will be given a distinguishing version number.
 
 10.2. Effect of New Versions
 
 You may distribute the Covered Software under the terms of the version
 of the License under which You originally received the Covered Software,
 or under the terms of any subsequent version published by the license
 steward.
@@ -341,33 +303,20 @@
 
 If you create software not governed by this License, and you want to
 create a new license for such software, you may create and use a
 modified version of this License if you rename the license and remove
 any references to the name of the license steward (except to note that
 such modified license differs from this License).
 
-10.4. Distributing Source Code Form that is Incompatible With Secondary
-Licenses
-
-If You choose to distribute Source Code Form that is Incompatible With
-Secondary Licenses under the terms of this version of the License, the
-notice described in Exhibit B of this License must be attached.
-
 Exhibit A - Source Code Form License Notice
 -------------------------------------------
 
-  This Source Code Form is subject to the terms of the Mozilla Public
-  License, v. 2.0. If a copy of the MPL was not distributed with this
-  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+  This Source Code Form is subject to the terms of the Oxford Nanopore
+  Technologies PLC. Public License, v. 1.0. Full licence can be found
+  obtained from support@nanoporetech.com
 
 If it is not possible or desirable to put the notice in a particular
 file, then You may include the notice in a location (such as a LICENSE
 file in a relevant directory) where a recipient would be likely to look
 for such a notice.
 
 You may add additional accurate notices of copyright ownership.
-
-Exhibit B - "Incompatible With Secondary Licenses" Notice
----------------------------------------------------------
-
-  This Source Code Form is "Incompatible With Secondary Licenses", as
-  defined by the Mozilla Public License, v. 2.0.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modbampy-0.9.4/Makefile` & `modbampy-0.9.5/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 		-Isrc -Ihtslib $(EXTRA_CFLAGS) $(EXTRA_LDFLAGS)\
 		$^ $(ARGP) \
 		-lm -lz -llzma -lbz2 -lpthread -lcurl -lcrypto $(EXTRA_LIBS) \
 		-o $(@)
 
 .PHONY: clean
 clean: clean_obj clean_htslib
-	rm -rf modbam2bed
+	rm -rf modbam2bed modbampy.egg-info pymod.a  venv obj
 
 .PHONY: mem_check
 mem_check: modbam2bed
 	$(VALGRIND) --error-exitcode=1 --tool=memcheck --leak-check=full --show-leak-kinds=all -s \
 		./modbam2bed --threshold 0.66 -t 2 -r ecoli1 test_data/ecoli.fasta.gz test_data/400ecoli.bam test_data/400ecoli.bam > /dev/null
 
 
@@ -102,15 +102,15 @@
 PYTHON ?= python3
 VENV ?= venv
 venv: ${VENV}/bin/activate
 IN_VENV=. ./${VENV}/bin/activate
 
 $(VENV)/bin/activate:
 	test -d $(VENV) || $(PYTHON) -m venv $(VENV) --prompt "modbam"
-	${IN_VENV} && pip install pip --upgrade
+	${IN_VENV} && pip install pip==23.0.1 --upgrade
 	${IN_VENV} && pip install setuptools
 
 .PHONY: python
 python: htslib/libhts.a pymod.a $(VENV)/bin/activate
 	${IN_VENV} && pip install -r requirements.txt
 	${IN_VENV} && WITHDEFLATE=$(WITHDEFLATE) LDFLAGS=$(EXTRA_LDFLAGS) pip install -e .
```

### Comparing `modbampy-0.9.4/PKG-INFO` & `modbampy-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: modbampy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Accessing modified-base data from BAM files.
 Home-page: https://github.com/epi2me-labs/modbam2bed
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Oxford Nanopore Technologies logo](https://github.com/epi2me-labs/modbam2bed/raw/master/images/ONT_logo_590x106.png)
 
+
+We have a new bioinformatic resource that replaces the functionality of this project! See our new repository here: 
+[modkit](https://github.com/nanoporetech/modkit/).
+
+This repository is now unsupported and we do not recommend its use. Please contact Oxford Nanopore: support@nanoporetech.com for help with your application if it is not possible to upgrade.
+
+
+******************
+
+
 Modified-base BAM to bedMethyl
 ------------------------------
 
 A program to aggregate modified base counts stored in a
 [modified-base BAM](https://samtools.github.io/hts-specs/SAMtags.pdf) (Section 2.1) file to 
 a [bedMethyl](https://www.encodeproject.org/data-standards/wgbs/) file.
```

### Comparing `modbampy-0.9.4/README.md` & `modbampy-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 ![Oxford Nanopore Technologies logo](https://github.com/epi2me-labs/modbam2bed/raw/master/images/ONT_logo_590x106.png)
 
+
+We have a new bioinformatic resource that replaces the functionality of this project! See our new repository here: 
+[modkit](https://github.com/nanoporetech/modkit/).
+
+This repository is now unsupported and we do not recommend its use. Please contact Oxford Nanopore: support@nanoporetech.com for help with your application if it is not possible to upgrade.
+
+
+******************
+
+
 Modified-base BAM to bedMethyl
 ------------------------------
 
 A program to aggregate modified base counts stored in a
 [modified-base BAM](https://samtools.github.io/hts-specs/SAMtags.pdf) (Section 2.1) file to 
 a [bedMethyl](https://www.encodeproject.org/data-standards/wgbs/) file.
```

### Comparing `modbampy-0.9.4/build.py` & `modbampy-0.9.5/build.py`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/.appveyor.yml` & `modbampy-0.9.5/htslib/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/.cirrus.yml` & `modbampy-0.9.5/htslib/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/.gitattributes` & `modbampy-0.9.5/htslib/.gitattributes`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/.gitignore` & `modbampy-0.9.5/htslib/.gitignore`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/INSTALL` & `modbampy-0.9.5/htslib/INSTALL`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/LICENSE` & `modbampy-0.9.5/htslib/LICENSE`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/Makefile` & `modbampy-0.9.5/htslib/Makefile`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/NEWS` & `modbampy-0.9.5/htslib/NEWS`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/README` & `modbampy-0.9.5/htslib/README`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/README.large_positions.md` & `modbampy-0.9.5/htslib/README.large_positions.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/README.md` & `modbampy-0.9.5/htslib/README.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/bcf_sr_sort.c` & `modbampy-0.9.5/htslib/bcf_sr_sort.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/bcf_sr_sort.h` & `modbampy-0.9.5/htslib/bcf_sr_sort.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/bgzf.c` & `modbampy-0.9.5/htslib/bgzf.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/bgzip.1` & `modbampy-0.9.5/htslib/bgzip.1`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/bgzip.c` & `modbampy-0.9.5/htslib/bgzip.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/builddir_vars.mk.in` & `modbampy-0.9.5/htslib/builddir_vars.mk.in`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/config.mk.in` & `modbampy-0.9.5/htslib/config.mk.in`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/configure.ac` & `modbampy-0.9.5/htslib/configure.ac`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram.h` & `modbampy-0.9.5/htslib/cram/cram.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_codecs.c` & `modbampy-0.9.5/htslib/cram/cram_codecs.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_codecs.h` & `modbampy-0.9.5/htslib/cram/cram_codecs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_decode.c` & `modbampy-0.9.5/htslib/cram/cram_decode.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_decode.h` & `modbampy-0.9.5/htslib/cram/cram_decode.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_encode.c` & `modbampy-0.9.5/htslib/cram/cram_encode.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_encode.h` & `modbampy-0.9.5/htslib/cram/cram_encode.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_external.c` & `modbampy-0.9.5/htslib/cram/cram_external.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_index.c` & `modbampy-0.9.5/htslib/cram/cram_index.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_index.h` & `modbampy-0.9.5/htslib/cram/cram_index.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_io.c` & `modbampy-0.9.5/htslib/cram/cram_io.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_io.h` & `modbampy-0.9.5/htslib/cram/cram_io.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_samtools.h` & `modbampy-0.9.5/htslib/cram/cram_samtools.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_stats.c` & `modbampy-0.9.5/htslib/cram/cram_stats.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_stats.h` & `modbampy-0.9.5/htslib/cram/cram_stats.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/cram_structs.h` & `modbampy-0.9.5/htslib/cram/cram_structs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/mFILE.c` & `modbampy-0.9.5/htslib/cram/mFILE.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/mFILE.h` & `modbampy-0.9.5/htslib/cram/mFILE.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/misc.h` & `modbampy-0.9.5/htslib/cram/misc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/open_trace_file.c` & `modbampy-0.9.5/htslib/cram/open_trace_file.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/open_trace_file.h` & `modbampy-0.9.5/htslib/cram/open_trace_file.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/os.h` & `modbampy-0.9.5/htslib/cram/os.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/pooled_alloc.c` & `modbampy-0.9.5/htslib/cram/pooled_alloc.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/pooled_alloc.h` & `modbampy-0.9.5/htslib/cram/pooled_alloc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/string_alloc.c` & `modbampy-0.9.5/htslib/cram/string_alloc.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/cram/string_alloc.h` & `modbampy-0.9.5/htslib/cram/string_alloc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/errmod.c` & `modbampy-0.9.5/htslib/errmod.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/faidx.5` & `modbampy-0.9.5/htslib/faidx.5`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/faidx.c` & `modbampy-0.9.5/htslib/faidx.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/header.c` & `modbampy-0.9.5/htslib/header.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/header.h` & `modbampy-0.9.5/htslib/header.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile.c` & `modbampy-0.9.5/htslib/hfile.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile_gcs.c` & `modbampy-0.9.5/htslib/hfile_gcs.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile_internal.h` & `modbampy-0.9.5/htslib/hfile_internal.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile_libcurl.c` & `modbampy-0.9.5/htslib/hfile_libcurl.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile_s3.c` & `modbampy-0.9.5/htslib/hfile_s3.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hfile_s3_write.c` & `modbampy-0.9.5/htslib/hfile_s3_write.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts.c` & `modbampy-0.9.5/htslib/hts.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts_expr.c` & `modbampy-0.9.5/htslib/hts_expr.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts_internal.h` & `modbampy-0.9.5/htslib/hts_internal.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts_os.c` & `modbampy-0.9.5/htslib/hts_os.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts_probe_cc.sh` & `modbampy-0.9.5/htslib/hts_probe_cc.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/hts_time_funcs.h` & `modbampy-0.9.5/htslib/hts_time_funcs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/.appveyor.yml` & `modbampy-0.9.5/htslib/htscodecs/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/.cirrus.yml` & `modbampy-0.9.5/htslib/htscodecs/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/BENCHMARKS.md` & `modbampy-0.9.5/htslib/htscodecs/BENCHMARKS.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/LICENSE.md` & `modbampy-0.9.5/htslib/htscodecs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/MAINTAINERS.md` & `modbampy-0.9.5/htslib/htscodecs/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/Makefile.am` & `modbampy-0.9.5/htslib/htscodecs/Makefile.am`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/NEWS.md` & `modbampy-0.9.5/htslib/htscodecs/NEWS.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/README.md` & `modbampy-0.9.5/htslib/htscodecs/README.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/configure.ac` & `modbampy-0.9.5/htslib/htscodecs/configure.ac`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/Makefile.am` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/Makefile.am`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/arith_dynamic.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/arith_dynamic.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/arith_dynamic.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/arith_dynamic.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/c_range_coder.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/c_range_coder.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/c_simple_model.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/c_simple_model.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/fqzcomp_qual.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/fqzcomp_qual.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/fqzcomp_qual.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/fqzcomp_qual.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/htscodecs_endian.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/htscodecs_endian.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/pack.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/pack.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/pack.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/pack.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/permute.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/permute.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/pooled_alloc.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/pooled_alloc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_byte.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_byte.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static16_int.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static16_int.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx2.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx2.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx512.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_avx512.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_neon.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_neon.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static32x16pr_sse4.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static32x16pr_sse4.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static4x16.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static4x16.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_static4x16pr.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_static4x16pr.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rANS_word.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rANS_word.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rle.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rle.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/rle.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/rle.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/tokenise_name3.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/tokenise_name3.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/tokenise_name3.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/tokenise_name3.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/utils.c` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/utils.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/utils.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/utils.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/varint.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/varint.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/htscodecs/varint2.h` & `modbampy-0.9.5/htslib/htscodecs/htscodecs/varint2.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/Makefile` & `modbampy-0.9.5/htslib/htscodecs/javascript/Makefile`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/README.md` & `modbampy-0.9.5/htslib/htscodecs/javascript/README.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/arith_gen.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/arith_gen.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/arith_sh.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/arith_sh.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/byte_model.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/byte_model.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/fqzcomp.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/fqzcomp.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/index.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/index.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/iostream.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/iostream.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/main_arith_gen.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/main_arith_gen.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/main_fqzcomp.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/main_fqzcomp.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/main_rans.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/main_rans.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/main_rans4x16.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/main_rans4x16.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/main_tok3.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/main_tok3.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/rans.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/rans.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/rans4x16.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/rans4x16.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/javascript/tok3.js` & `modbampy-0.9.5/htslib/htscodecs/javascript/tok3.js`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/m4/ax_check_compile_flag.m4` & `modbampy-0.9.5/htslib/htscodecs/m4/ax_check_compile_flag.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/m4/ax_with_libdeflate.m4` & `modbampy-0.9.5/htslib/htscodecs/m4/ax_with_libdeflate.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/m4/vl_prog_warnings.m4` & `modbampy-0.9.5/htslib/htscodecs/m4/vl_prog_warnings.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/m4/zlib.m4` & `modbampy-0.9.5/htslib/htscodecs/m4/zlib.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/arith_dynamic_fuzz.c` & `modbampy-0.9.5/htslib/htscodecs/tests/arith_dynamic_fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/arith_dynamic_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/arith_dynamic_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/entropy.c` & `modbampy-0.9.5/htslib/htscodecs/tests/entropy.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c` & `modbampy-0.9.5/htslib/htscodecs/tests/fqzcomp_qual_fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/fqzcomp_qual_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/fqzcomp_qual_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c` & `modbampy-0.9.5/htslib/htscodecs/tests/rANS_static4x16pr_fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/rANS_static4x16pr_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/rANS_static4x16pr_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/rANS_static_fuzz.c` & `modbampy-0.9.5/htslib/htscodecs/tests/rANS_static_fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/rANS_static_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/rANS_static_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/tokenise_name3_fuzz.c` & `modbampy-0.9.5/htslib/htscodecs/tests/tokenise_name3_fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/tokenise_name3_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/tokenise_name3_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs/tests/varint_test.c` & `modbampy-0.9.5/htslib/htscodecs/tests/varint_test.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs_bundled.mk` & `modbampy-0.9.5/htslib/htscodecs_bundled.mk`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htscodecs_external.mk` & `modbampy-0.9.5/htslib/htscodecs_external.mk`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htsfile.1` & `modbampy-0.9.5/htslib/htsfile.1`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htsfile.c` & `modbampy-0.9.5/htslib/htsfile.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/bgzf.h` & `modbampy-0.9.5/htslib/htslib/bgzf.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/cram.h` & `modbampy-0.9.5/htslib/htslib/cram.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/faidx.h` & `modbampy-0.9.5/htslib/htslib/faidx.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hfile.h` & `modbampy-0.9.5/htslib/htslib/hfile.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts.h` & `modbampy-0.9.5/htslib/htslib/hts.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts_defs.h` & `modbampy-0.9.5/htslib/htslib/hts_defs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts_endian.h` & `modbampy-0.9.5/htslib/htslib/hts_endian.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts_expr.h` & `modbampy-0.9.5/htslib/htslib/hts_expr.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts_log.h` & `modbampy-0.9.5/htslib/htslib/hts_log.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/hts_os.h` & `modbampy-0.9.5/htslib/htslib/hts_os.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/kbitset.h` & `modbampy-0.9.5/htslib/htslib/kbitset.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/kfunc.h` & `modbampy-0.9.5/htslib/htslib/kfunc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/khash.h` & `modbampy-0.9.5/htslib/htslib/khash.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/khash_str2int.h` & `modbampy-0.9.5/htslib/htslib/khash_str2int.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/klist.h` & `modbampy-0.9.5/htslib/htslib/klist.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/knetfile.h` & `modbampy-0.9.5/htslib/htslib/knetfile.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/kroundup.h` & `modbampy-0.9.5/htslib/htslib/kroundup.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/kseq.h` & `modbampy-0.9.5/htslib/htslib/kseq.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/ksort.h` & `modbampy-0.9.5/htslib/htslib/ksort.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/kstring.h` & `modbampy-0.9.5/htslib/htslib/kstring.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/regidx.h` & `modbampy-0.9.5/htslib/htslib/regidx.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/sam.h` & `modbampy-0.9.5/htslib/htslib/sam.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/synced_bcf_reader.h` & `modbampy-0.9.5/htslib/htslib/synced_bcf_reader.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/tbx.h` & `modbampy-0.9.5/htslib/htslib/tbx.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/thread_pool.h` & `modbampy-0.9.5/htslib/htslib/thread_pool.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/vcf.h` & `modbampy-0.9.5/htslib/htslib/vcf.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/vcf_sweep.h` & `modbampy-0.9.5/htslib/htslib/vcf_sweep.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib/vcfutils.h` & `modbampy-0.9.5/htslib/htslib/vcfutils.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib-s3-plugin.7` & `modbampy-0.9.5/htslib/htslib-s3-plugin.7`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib.mk` & `modbampy-0.9.5/htslib/htslib.mk`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/htslib_vars.mk` & `modbampy-0.9.5/htslib/htslib_vars.mk`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/kfunc.c` & `modbampy-0.9.5/htslib/kfunc.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/kstring.c` & `modbampy-0.9.5/htslib/kstring.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/m4/ax_check_compile_flag.m4` & `modbampy-0.9.5/htslib/m4/ax_check_compile_flag.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/m4/hts_hide_dynamic_syms.m4` & `modbampy-0.9.5/htslib/m4/hts_hide_dynamic_syms.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/m4/hts_prog_cc_warnings.m4` & `modbampy-0.9.5/htslib/m4/hts_prog_cc_warnings.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/m4/pkg.m4` & `modbampy-0.9.5/htslib/m4/pkg.m4`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/md5.c` & `modbampy-0.9.5/htslib/md5.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/multipart.c` & `modbampy-0.9.5/htslib/multipart.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/os/lzma_stub.h` & `modbampy-0.9.5/htslib/os/lzma_stub.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/os/rand.c` & `modbampy-0.9.5/htslib/os/rand.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/plugin.c` & `modbampy-0.9.5/htslib/plugin.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/probaln.c` & `modbampy-0.9.5/htslib/probaln.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/realn.c` & `modbampy-0.9.5/htslib/realn.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/regidx.c` & `modbampy-0.9.5/htslib/regidx.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/region.c` & `modbampy-0.9.5/htslib/region.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/sam.5` & `modbampy-0.9.5/htslib/sam.5`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/sam.c` & `modbampy-0.9.5/htslib/sam.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/sam_internal.h` & `modbampy-0.9.5/htslib/sam_internal.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/synced_bcf_reader.c` & `modbampy-0.9.5/htslib/synced_bcf_reader.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/tabix.1` & `modbampy-0.9.5/htslib/tabix.1`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/tabix.c` & `modbampy-0.9.5/htslib/tabix.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/tbx.c` & `modbampy-0.9.5/htslib/tbx.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/fieldarith.c` & `modbampy-0.9.5/htslib/test/fieldarith.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/fuzz/hts_open_fuzzer.c` & `modbampy-0.9.5/htslib/test/fuzz/hts_open_fuzzer.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/hfile.c` & `modbampy-0.9.5/htslib/test/hfile.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/hts_endian.c` & `modbampy-0.9.5/htslib/test/hts_endian.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/pileup.c` & `modbampy-0.9.5/htslib/test/pileup.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/pileup_mod.c` & `modbampy-0.9.5/htslib/test/pileup_mod.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/plugins-dlhts.c` & `modbampy-0.9.5/htslib/test/plugins-dlhts.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/sam.c` & `modbampy-0.9.5/htslib/test/sam.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-bcf-sr.c` & `modbampy-0.9.5/htslib/test/test-bcf-sr.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-bcf-translate.c` & `modbampy-0.9.5/htslib/test/test-bcf-translate.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-bcf_set_variant_type.c` & `modbampy-0.9.5/htslib/test/test-bcf_set_variant_type.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-parse-reg.c` & `modbampy-0.9.5/htslib/test/test-parse-reg.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-regidx.c` & `modbampy-0.9.5/htslib/test/test-regidx.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-vcf-api.c` & `modbampy-0.9.5/htslib/test/test-vcf-api.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test-vcf-sweep.c` & `modbampy-0.9.5/htslib/test/test-vcf-sweep.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_bgzf.c` & `modbampy-0.9.5/htslib/test/test_bgzf.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_expr.c` & `modbampy-0.9.5/htslib/test/test_expr.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_index.c` & `modbampy-0.9.5/htslib/test/test_index.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_introspection.c` & `modbampy-0.9.5/htslib/test/test_introspection.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_kfunc.c` & `modbampy-0.9.5/htslib/test/test_kfunc.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_kstring.c` & `modbampy-0.9.5/htslib/test/test_kstring.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_mod.c` & `modbampy-0.9.5/htslib/test/test_mod.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_realn.c` & `modbampy-0.9.5/htslib/test/test_realn.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_str2int.c` & `modbampy-0.9.5/htslib/test/test_str2int.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_time_funcs.c` & `modbampy-0.9.5/htslib/test/test_time_funcs.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/test_view.c` & `modbampy-0.9.5/htslib/test/test_view.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads1.c` & `modbampy-0.9.5/htslib/test/thrash_threads1.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads2.c` & `modbampy-0.9.5/htslib/test/thrash_threads2.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads3.c` & `modbampy-0.9.5/htslib/test/thrash_threads3.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads4.c` & `modbampy-0.9.5/htslib/test/thrash_threads4.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads5.c` & `modbampy-0.9.5/htslib/test/thrash_threads5.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads6.c` & `modbampy-0.9.5/htslib/test/thrash_threads6.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/test/thrash_threads7.c` & `modbampy-0.9.5/htslib/test/thrash_threads7.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/textutils.c` & `modbampy-0.9.5/htslib/textutils.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/textutils_internal.h` & `modbampy-0.9.5/htslib/textutils_internal.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/thread_pool.c` & `modbampy-0.9.5/htslib/thread_pool.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/thread_pool_internal.h` & `modbampy-0.9.5/htslib/thread_pool_internal.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/vcf.5` & `modbampy-0.9.5/htslib/vcf.5`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/vcf.c` & `modbampy-0.9.5/htslib/vcf.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/vcf_sweep.c` & `modbampy-0.9.5/htslib/vcf_sweep.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/vcfutils.c` & `modbampy-0.9.5/htslib/vcfutils.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/htslib/version.sh` & `modbampy-0.9.5/htslib/version.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/.github/workflows/android.yml` & `modbampy-0.9.5/libdeflate/.github/workflows/android.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/.github/workflows/ci.yml` & `modbampy-0.9.5/libdeflate/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/COPYING` & `modbampy-0.9.5/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/Makefile` & `modbampy-0.9.5/libdeflate/Makefile`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/Makefile.msc` & `modbampy-0.9.5/libdeflate/Makefile.msc`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/NEWS.md` & `modbampy-0.9.5/libdeflate/NEWS.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/README.md` & `modbampy-0.9.5/libdeflate/README.md`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/common/common_defs.h` & `modbampy-0.9.5/libdeflate/common/common_defs.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/common/compiler_gcc.h` & `modbampy-0.9.5/libdeflate/common/compiler_gcc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/common/compiler_msc.h` & `modbampy-0.9.5/libdeflate/common/compiler_msc.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/adler32.c` & `modbampy-0.9.5/libdeflate/lib/adler32.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/adler32_vec_template.h` & `modbampy-0.9.5/libdeflate/lib/adler32_vec_template.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/arm/adler32_impl.h` & `modbampy-0.9.5/libdeflate/lib/arm/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/arm/cpu_features.c` & `modbampy-0.9.5/libdeflate/lib/arm/cpu_features.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/arm/cpu_features.h` & `modbampy-0.9.5/libdeflate/lib/arm/cpu_features.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/arm/crc32_impl.h` & `modbampy-0.9.5/libdeflate/lib/arm/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/arm/matchfinder_impl.h` & `modbampy-0.9.5/libdeflate/lib/arm/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/bt_matchfinder.h` & `modbampy-0.9.5/libdeflate/lib/bt_matchfinder.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/cpu_features_common.h` & `modbampy-0.9.5/libdeflate/lib/cpu_features_common.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/crc32.c` & `modbampy-0.9.5/libdeflate/lib/crc32.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/crc32_table.h` & `modbampy-0.9.5/libdeflate/lib/crc32_table.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/crc32_vec_template.h` & `modbampy-0.9.5/libdeflate/lib/crc32_vec_template.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/decompress_template.h` & `modbampy-0.9.5/libdeflate/lib/decompress_template.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/deflate_compress.c` & `modbampy-0.9.5/libdeflate/lib/deflate_compress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/deflate_constants.h` & `modbampy-0.9.5/libdeflate/lib/deflate_constants.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/deflate_decompress.c` & `modbampy-0.9.5/libdeflate/lib/deflate_decompress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/gzip_compress.c` & `modbampy-0.9.5/libdeflate/lib/gzip_compress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/gzip_constants.h` & `modbampy-0.9.5/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/gzip_decompress.c` & `modbampy-0.9.5/libdeflate/lib/gzip_decompress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/hc_matchfinder.h` & `modbampy-0.9.5/libdeflate/lib/hc_matchfinder.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/ht_matchfinder.h` & `modbampy-0.9.5/libdeflate/lib/ht_matchfinder.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/lib_common.h` & `modbampy-0.9.5/libdeflate/lib/lib_common.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/matchfinder_common.h` & `modbampy-0.9.5/libdeflate/lib/matchfinder_common.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/unaligned.h` & `modbampy-0.9.5/libdeflate/lib/unaligned.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/utils.c` & `modbampy-0.9.5/libdeflate/lib/utils.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/adler32_impl.h` & `modbampy-0.9.5/libdeflate/lib/x86/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/cpu_features.c` & `modbampy-0.9.5/libdeflate/lib/x86/cpu_features.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/cpu_features.h` & `modbampy-0.9.5/libdeflate/lib/x86/cpu_features.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/crc32_impl.h` & `modbampy-0.9.5/libdeflate/lib/x86/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/crc32_pclmul_template.h` & `modbampy-0.9.5/libdeflate/lib/x86/crc32_pclmul_template.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/decompress_impl.h` & `modbampy-0.9.5/libdeflate/lib/x86/decompress_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/x86/matchfinder_impl.h` & `modbampy-0.9.5/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/zlib_compress.c` & `modbampy-0.9.5/libdeflate/lib/zlib_compress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/lib/zlib_decompress.c` & `modbampy-0.9.5/libdeflate/lib/zlib_decompress.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/libdeflate.h` & `modbampy-0.9.5/libdeflate/libdeflate.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/benchmark.c` & `modbampy-0.9.5/libdeflate/programs/benchmark.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/checksum.c` & `modbampy-0.9.5/libdeflate/programs/checksum.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/gzip.c` & `modbampy-0.9.5/libdeflate/programs/gzip.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/prog_util.c` & `modbampy-0.9.5/libdeflate/programs/prog_util.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/prog_util.h` & `modbampy-0.9.5/libdeflate/programs/prog_util.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_checksums.c` & `modbampy-0.9.5/libdeflate/programs/test_checksums.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_custom_malloc.c` & `modbampy-0.9.5/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_incomplete_codes.c` & `modbampy-0.9.5/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_litrunlen_overflow.c` & `modbampy-0.9.5/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_overread.c` & `modbampy-0.9.5/libdeflate/programs/test_overread.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_slow_decompression.c` & `modbampy-0.9.5/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_trailing_bytes.c` & `modbampy-0.9.5/libdeflate/programs/test_trailing_bytes.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_util.c` & `modbampy-0.9.5/libdeflate/programs/test_util.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/test_util.h` & `modbampy-0.9.5/libdeflate/programs/test_util.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/programs/tgetopt.c` & `modbampy-0.9.5/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c` & `modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c` & `modbampy-0.9.5/libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/afl-fuzz/fuzz.sh` & `modbampy-0.9.5/libdeflate/scripts/afl-fuzz/fuzz.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c` & `modbampy-0.9.5/libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c` & `modbampy-0.9.5/libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/android_build.sh` & `modbampy-0.9.5/libdeflate/scripts/android_build.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/android_tests.sh` & `modbampy-0.9.5/libdeflate/scripts/android_tests.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/checksum_benchmarks.sh` & `modbampy-0.9.5/libdeflate/scripts/checksum_benchmarks.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/deflate_benchmarks.sh` & `modbampy-0.9.5/libdeflate/scripts/deflate_benchmarks.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/detect.sh` & `modbampy-0.9.5/libdeflate/scripts/detect.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/exec_tests.sh` & `modbampy-0.9.5/libdeflate/scripts/exec_tests.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/gen_crc32_multipliers.c` & `modbampy-0.9.5/libdeflate/scripts/gen_crc32_multipliers.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/gen_crc32_table.c` & `modbampy-0.9.5/libdeflate/scripts/gen_crc32_table.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/gen_default_litlen_costs.py` & `modbampy-0.9.5/libdeflate/scripts/gen_default_litlen_costs.py`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/gen_offset_slot_map.py` & `modbampy-0.9.5/libdeflate/scripts/gen_offset_slot_map.py`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/gzip_tests.sh` & `modbampy-0.9.5/libdeflate/scripts/gzip_tests.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/make-windows-releases.sh` & `modbampy-0.9.5/libdeflate/scripts/make-windows-releases.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/pgo_build.sh` & `modbampy-0.9.5/libdeflate/scripts/pgo_build.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/libdeflate/scripts/run_tests.sh` & `modbampy-0.9.5/libdeflate/scripts/run_tests.sh`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/modbampy/__init__.py` & `modbampy-0.9.5/modbampy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import collections
 
 import numpy as np
 
 import libmodbampy
 
 # remember to bump version in src/version.h too
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 ffi = libmodbampy.ffi
 libbam = libmodbampy.lib
 
 MAX_MODS = 256  # from htslib
 
 ModInfo = collections.namedtuple(
     'ModInfo', (
```

### Comparing `modbampy-0.9.4/modbampy.egg-info/PKG-INFO` & `modbampy-0.9.5/modbampy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: modbampy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Accessing modified-base data from BAM files.
 Home-page: https://github.com/epi2me-labs/modbam2bed
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Oxford Nanopore Technologies logo](https://github.com/epi2me-labs/modbam2bed/raw/master/images/ONT_logo_590x106.png)
 
+
+We have a new bioinformatic resource that replaces the functionality of this project! See our new repository here: 
+[modkit](https://github.com/nanoporetech/modkit/).
+
+This repository is now unsupported and we do not recommend its use. Please contact Oxford Nanopore: support@nanoporetech.com for help with your application if it is not possible to upgrade.
+
+
+******************
+
+
 Modified-base BAM to bedMethyl
 ------------------------------
 
 A program to aggregate modified base counts stored in a
 [modified-base BAM](https://samtools.github.io/hts-specs/SAMtags.pdf) (Section 2.1) file to 
 a [bedMethyl](https://www.encodeproject.org/data-standards/wgbs/) file.
```

### Comparing `modbampy-0.9.4/modbampy.egg-info/SOURCES.txt` & `modbampy-0.9.5/modbampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/setup.py` & `modbampy-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/args.c` & `modbampy-0.9.5/src/args.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/args.h` & `modbampy-0.9.5/src/args.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/bamiter.c` & `modbampy-0.9.5/src/bamiter.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/bamiter.h` & `modbampy-0.9.5/src/bamiter.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/common.c` & `modbampy-0.9.5/src/common.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/common.h` & `modbampy-0.9.5/src/common.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/counts.c` & `modbampy-0.9.5/src/counts.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/counts.h` & `modbampy-0.9.5/src/counts.h`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/src/modbam2bed.c` & `modbampy-0.9.5/src/modbam2bed.c`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/test/test_api.py` & `modbampy-0.9.5/test/test_api.py`

 * *Files identical despite different names*

### Comparing `modbampy-0.9.4/test/test_motifs.py` & `modbampy-0.9.5/test/test_motifs.py`

 * *Files identical despite different names*

