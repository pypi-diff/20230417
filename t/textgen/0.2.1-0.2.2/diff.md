# Comparing `tmp/textgen-0.2.1.tar.gz` & `tmp/textgen-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.2.1.tar", last modified: Fri Apr 14 03:39:06 2023, max compression
+gzip compressed data, was "textgen-0.2.2.tar", last modified: Mon Apr 17 14:32:15 2023, max compression
```

## Comparing `textgen-0.2.1.tar` & `textgen-0.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.101297 textgen-0.2.1/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.1/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    31932 2023-04-14 03:39:06.101662 textgen-0.2.1/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    26931 2023-04-14 03:27:18.000000 textgen-0.2.1/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-14 03:39:06.102206 textgen-0.2.1/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1419 2023-04-14 03:39:03.000000 textgen-0.2.1/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.051495 textgen-0.2.1/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-14 03:39:03.000000 textgen-0.2.1/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.061156 textgen-0.2.1/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.1/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.1/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.1/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.1/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.1/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.1/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.065210 textgen-0.2.1/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.1/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    31490 2023-04-13 13:14:14.000000 textgen-0.2.1/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.1/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.068221 textgen-0.2.1/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.1/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    14437 2023-04-13 13:05:38.000000 textgen-0.2.1/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.069715 textgen-0.2.1/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.1/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.073006 textgen-0.2.1/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.1/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.1/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.076325 textgen-0.2.1/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.1/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.1/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.1/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.082343 textgen-0.2.1/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.1/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.1/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.1/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.1/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.1/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.086202 textgen-0.2.1/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.1/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    23037 2023-04-13 13:50:42.000000 textgen-0.2.1/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5753 2023-04-13 14:13:30.000000 textgen-0.2.1/textgen/llama/llama_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.093854 textgen-0.2.1/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.1/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73142 2023-04-12 10:22:29.000000 textgen-0.2.1/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.1/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.1/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.1/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.1/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.1/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.098379 textgen-0.2.1/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.1/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.1/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.1/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50541 2023-02-16 08:10:32.000000 textgen-0.2.1/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.1/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.100461 textgen-0.2.1/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.1/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.1/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.1/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-14 03:39:06.053838 textgen-0.2.1/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    31932 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      158 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-14 03:39:05.000000 textgen-0.2.1/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.105381 textgen-0.2.2/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.2/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-17 14:32:15.105904 textgen-0.2.2/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.2/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-17 14:32:15.106668 textgen-0.2.2/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-17 14:02:51.000000 textgen-0.2.2/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.047149 textgen-0.2.2/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-17 13:39:14.000000 textgen-0.2.2/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.055964 textgen-0.2.2/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.2/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.2/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.2/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.2/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.2/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.2/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.058842 textgen-0.2.2/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.2/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    31478 2023-04-17 14:30:17.000000 textgen-0.2.2/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.2/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.062480 textgen-0.2.2/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.2/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14497 2023-04-14 05:57:19.000000 textgen-0.2.2/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.064526 textgen-0.2.2/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.2/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.068106 textgen-0.2.2/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.2/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.2/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.071986 textgen-0.2.2/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.2/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.2/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.2/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.079396 textgen-0.2.2/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.2/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.2/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.2/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.2/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.2/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.084416 textgen-0.2.2/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.2/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23156 2023-04-17 04:08:29.000000 textgen-0.2.2/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5753 2023-04-13 14:13:30.000000 textgen-0.2.2/textgen/llama/llama_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.093358 textgen-0.2.2/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.2/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.2/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.2/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.2/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.2/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.2/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.2/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.101326 textgen-0.2.2/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.2/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.2/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.2/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.2/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.2/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.103988 textgen-0.2.2/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.2/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.2/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.2/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 14:32:15.050098 textgen-0.2.2/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-17 14:32:14.000000 textgen-0.2.2/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.2.1/LICENSE` & `textgen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/PKG-INFO` & `textgen-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,102 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/textgen.svg)](https://github.com/shibing624/textgen/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
-        🌈 Implementation of Text Generation models.
+        🌈Implementation of Text Generation models.
         
         **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
-        - [Reference](#reference)
+        - [License](#License)
         
-        # Feature
+        ## 😊Feature
         
-        ## 文本生成
+        ### 文本生成
         
         1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
         2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
         3. t5: T5、CopyT5
         
-        ## 文本扩增
+        ### 文本扩增
         
-        ### 词粒度扩增
+        #### 词粒度扩增
         
         1. UDA，非核心词替换
         2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
         
-        ### 句粒度扩增
+        #### 句粒度扩增
         
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
-        ## 功能列表
+        ### 功能列表
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
-          算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-        - [TGLS](textgen/unsup_generation)
-          ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
+        - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
-        ## Release Models
+        ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
-        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
-        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
         
-        # Demo
+        |Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
+        |:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        
+        ## 🚀Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
-        model trained
-        by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+        model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
         
-        # Install
+        ## 💾Install
         
         ```shell
         pip install git+https://github.com/huggingface/transformers
         pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
@@ -119,42 +105,57 @@
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
         python setup.py install
         ```
         
-        # Usage
+        ## 😎Usage
         
-        ## ChatGLM-6B LoRA 模型
+        ### ChatGLM-6B LoRA 模型
         
-        ### 使用ChatGLM-6B LoRA微调后的模型
+        安装最新开发版的peft库，支持LoRA模型
+        
+        ```shell
+        pip install git+https://github.com/huggingface/peft
+        ```
+        
+        #### 使用ChatGLM-6B LoRA微调后的模型
         
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import ChatGlmModel
         
         model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
-        ### 训练ChatGLM-6B LoRA模型
+        PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
+        
+        #### 训练ChatGLM-6B LoRA模型
         
         支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
-        ## LLAMA LoRA 模型
+        ### LLAMA LoRA 模型
         
-        ### 使用LLAMA LoRA微调后的模型
+        安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
+        
+        ```shell
+        pip install transformers>=4.28.1
+        pip install git+https://github.com/huggingface/peft
+        ```
+        
+        #### 使用LLAMA LoRA微调后的模型
         
         example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
@@ -167,19 +168,19 @@
         
         model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
-        ### 训练LLAMA LoRA模型
+        #### 训练LLAMA LoRA模型
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
-        ## ConvSeq2Seq 模型
+        ### ConvSeq2Seq 模型
         
         训练并预测ConvSeq2Seq模型：
         
         example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
         ```python
         import argparse
@@ -224,30 +225,30 @@
         output:
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
-        ## BART 模型
+        ### BART 模型
         
         训练并预测BART模型：
         
         example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
-        ## T5 模型
+        ### T5 模型
         
-        example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
+        example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
         import pandas as pd
         import sys
         
@@ -338,48 +339,48 @@
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
-        ## GPT2 模型
+        ### GPT2 模型
         
-        ### 中文GPT2 - 文章生成
+        #### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
-        example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
+        example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
         
-        ### 中文GPT2 - 对联生成
+        #### 中文GPT2 - 对联生成
         
         使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
         
-        example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
+        example: [examples/gpt2/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_couplet_gpt2_demo.py)
         
-        #### GPT2 vs T5：
+        GPT2 vs T5：
         
         1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
         2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
         3. GPT2的模型优势是自由创作，如写一篇短文
         4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
         
         - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         
-        ## SongNet 模型
+        ### SongNet 模型
         
         格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
         适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
         
-        example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
+        example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
         
-        ## Keyword Text Augmentation(EDA/UDA)
+        ### Keyword Text Augmentation(EDA/UDA)
         
-        example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
+        example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
         from textgen.augment import TextAugment
         
@@ -416,19 +417,19 @@
         random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
         insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
         delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
         tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
         mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
         ```
         
-        ## TGLS 模型（无监督相似文本生成模型）
+        ### TGLS 模型（无监督相似文本生成模型）
         
         无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
         
-        example: [examples/unsup_generation_demo.py](examples/unsup_generation_demo.py)
+        example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
         
         ```python
         import os
         import sys
         
         sys.path.append('..')
         from textgen.unsup_generation import TglsModel, load_list
@@ -483,71 +484,72 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
-        # Dataset
+        ## 📚Dataset 
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3.
-        5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
-           ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
-        # Contact
+        ## ☎️Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        # Citation
+        ## 😇Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
           author={Xu Ming},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
-        # License
+        ## 🤗License
         
         授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
         
-        # Contribute
+        ## 😍Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        ## Reference
+        ## 💕Acknowledgements 
         
         - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
         - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
         - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
-        - [Tiiiger/bert_score]()
+        - [Tiiiger/bert_score](https://github.com/Tiiiger/bert_score)
+        - [ThilinaRajapakse/simpletransformers](https://github.com/ThilinaRajapakse/simpletransformers)
         - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
         - [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
+        
+        Thanks for their great work!
 Keywords: textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `textgen-0.2.1/README.md` & `textgen-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,94 @@
 [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
 [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/textgen.svg)](https://github.com/shibing624/textgen/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
 # TextGen
 
-🌈 Implementation of Text Generation models.
+🌈Implementation of Text Generation models.
 
 **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
 
 **Guide**
 
 - [Feature](#Feature)
 - [Install](#install)
 - [Usage](#usage)
 - [Contact](#Contact)
-- [Reference](#reference)
+- [License](#License)
 
-# Feature
+## 😊Feature
 
-## 文本生成
+### 文本生成
 
 1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
 2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
 3. t5: T5、CopyT5
 
-## 文本扩增
+### 文本扩增
 
-### 词粒度扩增
+#### 词粒度扩增
 
 1. UDA，非核心词替换
 2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
 
-### 句粒度扩增
+#### 句粒度扩增
 
 1. 回译（BT, Back Translate）：中文-英文-中文
 2. GPT2模型续写：短文本->长文本
 3. BART摘要模型：长文本->短文本
 4. TGLS：无监督相似文本生成模型
 
-## 功能列表
+### 功能列表
 
 - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
 - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-- [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
-  算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+- [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
 - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
 - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
 - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
 - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
 - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-- [TGLS](textgen/unsup_generation)
-  ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
+- [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
 
-## Release Models
+### Release Models
 
 release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
 
-|Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
-|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
-|[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
-script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
-script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
-script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
-script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
-|[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
-script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
-script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
 
-# Demo
+|Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
+|:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+|[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
+|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+|[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+
+## 🚀Demo
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
 
 ![](docs/hf.png)
 
 run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
 
 ```shell
 python examples/gradio_demo.py
 ```
 
-model trained
-by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
 
-# Install
+## 💾Install
 
 ```shell
 pip install git+https://github.com/huggingface/transformers
 pip install git+https://github.com/huggingface/peft
 pip install -U textgen
 ```
 
@@ -111,42 +97,57 @@
 ```shell
 pip install torch # conda install pytorch
 git clone https://github.com/shibing624/textgen.git
 cd textgen
 python setup.py install
 ```
 
-# Usage
+## 😎Usage
 
-## ChatGLM-6B LoRA 模型
+### ChatGLM-6B LoRA 模型
 
-### 使用ChatGLM-6B LoRA微调后的模型
+安装最新开发版的peft库，支持LoRA模型
+
+```shell
+pip install git+https://github.com/huggingface/peft
+```
+
+#### 使用ChatGLM-6B LoRA微调后的模型
 
 example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
 
 ```python
 import sys
 
 sys.path.append('../..')
 from textgen import ChatGlmModel
 
 model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
 r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
 print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
 ```
 
-### 训练ChatGLM-6B LoRA模型
+PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
+
+#### 训练ChatGLM-6B LoRA模型
 
 支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
 
 example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
 
-## LLAMA LoRA 模型
+### LLAMA LoRA 模型
 
-### 使用LLAMA LoRA微调后的模型
+安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
+
+```shell
+pip install transformers>=4.28.1
+pip install git+https://github.com/huggingface/peft
+```
+
+#### 使用LLAMA LoRA微调后的模型
 
 example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
 
 ```python
 import sys
 
 sys.path.append('../..')
@@ -159,19 +160,19 @@
 
 model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
 predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
 r = model.predict([predict_sentence])
 print(r)  # ['地球是唯一一颗拥有生命的行星。']
 ```
 
-### 训练LLAMA LoRA模型
+#### 训练LLAMA LoRA模型
 
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
 
-## ConvSeq2Seq 模型
+### ConvSeq2Seq 模型
 
 训练并预测ConvSeq2Seq模型：
 
 example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
 
 ```python
 import argparse
@@ -216,30 +217,30 @@
 output:
 
 ```bash
 inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
 outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
 ```
 
-## BART 模型
+### BART 模型
 
 训练并预测BART模型：
 
 example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
 
 output:
 
 ```shell
 inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
 outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
 ```
 
-## T5 模型
+### T5 模型
 
-example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
+example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
 
 ```python
 import argparse
 from loguru import logger
 import pandas as pd
 import sys
 
@@ -330,48 +331,48 @@
 output:
 
 ```shell
 inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
 outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
 ```
 
-## GPT2 模型
+### GPT2 模型
 
-### 中文GPT2 - 文章生成
+#### 中文GPT2 - 文章生成
 
 使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
 
-example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
+example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
 
-### 中文GPT2 - 对联生成
+#### 中文GPT2 - 对联生成
 
 使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
 
-example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
+example: [examples/gpt2/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_couplet_gpt2_demo.py)
 
-#### GPT2 vs T5：
+GPT2 vs T5：
 
 1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
 2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
 3. GPT2的模型优势是自由创作，如写一篇短文
 4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
 
 - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
 - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
 
-## SongNet 模型
+### SongNet 模型
 
 格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
 适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
 
-example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
+example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
 
-## Keyword Text Augmentation(EDA/UDA)
+### Keyword Text Augmentation(EDA/UDA)
 
-example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
+example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
 from textgen.augment import TextAugment
 
@@ -408,19 +409,19 @@
 random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
 insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
 delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
 tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
 mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
 ```
 
-## TGLS 模型（无监督相似文本生成模型）
+### TGLS 模型（无监督相似文本生成模型）
 
 无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
 
-example: [examples/unsup_generation_demo.py](examples/unsup_generation_demo.py)
+example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
 
 ```python
 import os
 import sys
 
 sys.path.append('..')
 from textgen.unsup_generation import TglsModel, load_list
@@ -475,64 +476,65 @@
 希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
 就是精华液太少了，保湿效果不错。
 面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
 ```
 
 前10句是真实用户评论，后10句是生成的。
 
-# Dataset
+## 📚Dataset 
 
 1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-3.
-5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
 4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
-   ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
 
-# Contact
+## ☎️Contact
 
 - Issue(建议)
   ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
-# Citation
+## 😇Citation
 
 如果你在研究中使用了textgen，请按如下格式引用：
 
 ```latex
 @misc{textgen,
   title={textgen: Text Generation Tool},
   author={Xu Ming},
   year={2021},
   howpublished={\url{https://github.com/shibing624/textgen}},
 }
 ```
 
-# License
+## 🤗License
 
 授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
 
-# Contribute
+## 😍Contribute
 
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
 - 在`tests`添加相应的单元测试
 - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
 
 之后即可提交PR。
 
-## Reference
+## 💕Acknowledgements 
 
 - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
 - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
 - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 - [asyml/texar](https://github.com/asyml/texar)
 - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
 - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
 - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
-- [Tiiiger/bert_score]()
+- [Tiiiger/bert_score](https://github.com/Tiiiger/bert_score)
+- [ThilinaRajapakse/simpletransformers](https://github.com/ThilinaRajapakse/simpletransformers)
 - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
-- [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
+- [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
+
+Thanks for their great work!
```

### Comparing `textgen-0.2.1/setup.py` & `textgen-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.2.1',
+    version='0.2.2',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
@@ -24,15 +24,15 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     python_requires=">=3.6",
     keywords='textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation',
     install_requires=[
         'loguru',
         'jieba>=0.39',
-        'transformers',
+        'transformers>=4.28.1',
         'datasets',
         'gensim>=4.0.0',
         'text2vec',
         'tensorboard',
         'tensorboardX',
         'tqdm>=4.47.0',
         'pandas',
```

### Comparing `textgen-0.2.1/textgen/__init__.py` & `textgen-0.2.2/textgen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
```

### Comparing `textgen-0.2.1/textgen/augment/sentence_level_augment.py` & `textgen-0.2.2/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/augment/text_augment.py` & `textgen-0.2.2/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/augment/tokenizer.py` & `textgen-0.2.2/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/augment/translate_api.py` & `textgen-0.2.2/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/augment/word_level_augment.py` & `textgen-0.2.2/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/augment/word_vocab.py` & `textgen-0.2.2/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/chatglm/chatglm_model.py` & `textgen-0.2.2/textgen/chatglm/chatglm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         Args:
             model_type: The type of model (chatglm)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
             lora_name (optional): Lora name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
-            cuda_device (optional): Specific GPU that should be used. Will use the first available GPU by default.
+            cuda_device (int, optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
 
         if isinstance(args, dict):
             self.args.update_from_dict(args)
@@ -101,22 +101,25 @@
             self.args.int8 = False
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
         config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, **kwargs)
+
         self.model = model_class.from_pretrained(
             model_name,
             config=config,
             trust_remote_code=True,
             load_in_8bit=self.args.int8,
-            torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
-            device_map="auto",
         )
+        if self.args.fp16:
+            self.model.half()
+        self.model.to(self.device)
+
         if self.args.quantization_bit:
             logger.debug(f"Quantized to {self.args.quantization_bit} bit")
             self.model = self.model.quantize(self.args.quantization_bit)
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
             self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name, trust_remote_code=True)
         else:
@@ -256,15 +259,14 @@
             eval_dataset = self.load_and_cache_examples(eval_data, evaluate=True)
             if verbose:
                 logger.debug(f"eval_dataset len: {len(eval_dataset)}, eval_dataset[0]: {eval_dataset[0]}")
 
         # start train
         training_args = TrainingArguments(
             output_dir=self.args.output_dir,
-            auto_find_batch_size=True,
             learning_rate=self.args.learning_rate,
             num_train_epochs=self.args.num_train_epochs,
             logging_dir=f"{self.args.output_dir}/logs",
             logging_steps=self.args.logging_steps,
             max_steps=self.args.max_steps,
             per_device_train_batch_size=self.args.per_device_train_batch_size,
             per_device_eval_batch_size=self.args.per_device_train_batch_size,
@@ -274,14 +276,15 @@
             optim=self.args.optimizer,
             save_strategy=self.args.save_strategy,
             evaluation_strategy=self.args.evaluation_strategy,
             eval_steps=self.args.eval_steps,
             save_total_limit=self.args.save_total_limit,
             fp16=self.args.fp16,
             remove_unused_columns=self.args.remove_unused_columns,
+            report_to=self.args.report_to,
             overwrite_output_dir=self.args.overwrite_output_dir,
             no_cuda=True if self.device == "cpu" else False,
             **kwargs
         )
         # Log on each process the small summary:
         logger.warning(
             f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
@@ -345,16 +348,14 @@
                 lora_path = os.path.join(self.args.output_dir, self.args.lora_name)
                 if lora_path and os.path.exists(lora_path):
                     self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
                     logger.info(f"Loaded lora model from {lora_path}")
                     self.lora_loaded = True
             if torch.__version__ >= "2" and sys.platform != "win32":
                 self.model = torch.compile(self.model)
-            if self.args.fp16:
-                self.model.half()
 
     def process_response(self, response):
         response = response.strip().replace("[[训练时间]]", "2023年")
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
@@ -378,14 +379,16 @@
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if not self.lora_loaded:
             self.load_lora()
+        if self.args.fp16:
+            self.model.half()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
```

### Comparing `textgen-0.2.1/textgen/chatglm/chatglm_utils.py` & `textgen-0.2.2/textgen/chatglm/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/config/global_args.py` & `textgen-0.2.2/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/config/model_args.py` & `textgen-0.2.2/textgen/config/model_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,15 @@
     quantization_bit: int = None  # if use quantization bit, set 4, else None
     debug: bool = False
     max_seq_length: int = 256  # max length of input sequence
     max_length = 384  # max length of the sequence to be generated
     do_sample: bool = True
     early_stopping: bool = True
     evaluate_generated_text: bool = True
+    report_to = "tensorboard"
     optimizer: str = "adamw_torch"
     save_strategy: str = "steps"
     evaluation_strategy: str = "no"
     eval_steps: int = None
     save_steps: int = 400
     max_eval_samples: int = 20
     length_penalty: float = 2.0
@@ -400,14 +401,15 @@
     max_seq_length: int = 256  # max length of input sequence
     max_length = 384  # max length of the sequence to be generated
     do_sample: bool = True
     early_stopping: bool = True
     evaluate_generated_text: bool = True
     is_chat_task: bool = True
     warmup_steps: int = 50
+    report_to = "tensorboard"
     optimizer: str = "adamw_torch"
     save_strategy: str = "steps"
     eval_steps: int = 200
     save_steps: int = 400
     pad_to_multiple_of: int = 8
     max_eval_samples: int = 20
     length_penalty: float = 2.0
```

### Comparing `textgen-0.2.1/textgen/custom_models/models.py` & `textgen-0.2.2/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/data/HowNetPOSWord.txt` & `textgen-0.2.2/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/data/stopwords.txt` & `textgen-0.2.2/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_generation/language_generation_model.py` & `textgen-0.2.2/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_generation/language_generation_utils.py` & `textgen-0.2.2/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_modeling/language_modeling_model.py` & `textgen-0.2.2/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.2.2/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_modeling/songnet_model.py` & `textgen-0.2.2/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/language_modeling/songnet_utils.py` & `textgen-0.2.2/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/llama/llama_model.py` & `textgen-0.2.2/textgen/llama/llama_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         Args:
             model_type: The type of model (llama)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
             lora_name (optional): Lora name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
-            cuda_device (optional): Specific GPU that should be used. Will use the first available GPU by default.
+            cuda_device (int, optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
 
         if isinstance(args, dict):
             self.args.update_from_dict(args)
@@ -86,14 +86,15 @@
             if self.args.n_gpu > 0:
                 torch.cuda.manual_seed_all(self.args.manual_seed)
 
         if use_cuda:
             if torch.cuda.is_available():
                 if cuda_device == -1:
                     self.device = torch.device("cuda")
+                    cuda_device = 0
                 else:
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
@@ -105,20 +106,20 @@
             self.args.int8 = False
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
         config = AutoConfig.from_pretrained(model_name, **kwargs)
+
         device_map = "auto"
         world_size = int(os.environ.get("WORLD_SIZE", 1))
         self.ddp = world_size != 1
-        if self.ddp:
-            device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
-
+        if self.ddp or torch.cuda.device_count() > 1:
+            device_map = {"": int(os.environ.get("LOCAL_RANK") or cuda_device)}
         self.model = model_class.from_pretrained(
             model_name,
             config=config,
             load_in_8bit=self.args.int8,
             torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
             device_map=device_map,
         )
@@ -272,14 +273,15 @@
             evaluation_strategy='steps' if eval_data is not None else 'no',
             eval_steps=self.args.eval_steps if eval_data is not None else None,
             load_best_model_at_end=True if eval_data is not None else False,
             ddp_find_unused_parameters=False if self.ddp else None,
             save_total_limit=self.args.save_total_limit,
             fp16=self.args.fp16,
             remove_unused_columns=self.args.remove_unused_columns,
+            report_to=self.args.report_to,
             overwrite_output_dir=self.args.overwrite_output_dir,
             no_cuda=True if self.device == "cpu" else False,
             **kwargs
         )
         # Log on each process the small summary:
         logger.warning(
             f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
@@ -380,16 +382,14 @@
             # unwind broken decapoda-research config
             self.tokenizer.padding_side = "left"
             self.model.config.pad_token_id = self.tokenizer.pad_token_id = 0  # unk
             self.model.config.bos_token_id = 1
             self.model.config.eos_token_id = 2
             if torch.__version__ >= "2" and sys.platform != "win32":
                 self.model = torch.compile(self.model)
-            if self.args.fp16:
-                self.model.half()
 
     @torch.no_grad()
     def predict(self, sentences, keep_prompt=False, max_length=None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
@@ -399,14 +399,16 @@
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if not self.lora_loaded:
             self.load_lora()
+        if self.args.fp16:
+            self.model.half()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
```

### Comparing `textgen-0.2.1/textgen/llama/llama_utils.py` & `textgen-0.2.2/textgen/llama/llama_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.2.2/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
 
         if args.wandb_project:
             wandb.init(
                 project=args.wandb_project,
                 config={**asdict(args)},
                 **args.wandb_kwargs,
             )
-            wandb.run._label(repo="simpletransformers")
+            wandb.run._label(repo="textgen")
             wandb.watch(self.model)
             self.wandb_run_id = wandb.run.id
 
         if args.fp16:
             from torch.cuda import amp
 
             scaler = amp.GradScaler()
```

### Comparing `textgen-0.2.1/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.2.2/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.2.2/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/seq2seq/data_reader.py` & `textgen-0.2.2/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/seq2seq/seq2seq_model.py` & `textgen-0.2.2/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.2.2/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/t5/copyt5_model.py` & `textgen-0.2.2/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/t5/copyt5_utils.py` & `textgen-0.2.2/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/t5/t5_model.py` & `textgen-0.2.2/textgen/t5/t5_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,15 +476,15 @@
 
         if args.wandb_project:
             wandb.init(
                 project=args.wandb_project,
                 config={**asdict(args)},
                 **args.wandb_kwargs,
             )
-            wandb.run._label(repo="simpletransformers")
+            wandb.run._label(repo="textgen")
             wandb.watch(self.model)
             self.wandb_run_id = wandb.run.id
 
         if args.fp16:
             from torch.cuda import amp
 
             scaler = amp.GradScaler()
```

### Comparing `textgen-0.2.1/textgen/t5/t5_utils.py` & `textgen-0.2.2/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/unsup_generation/tgls_model.py` & `textgen-0.2.2/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen/unsup_generation/tgls_util.py` & `textgen-0.2.2/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.1/textgen.egg-info/PKG-INFO` & `textgen-0.2.2/textgen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,102 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/textgen.svg)](https://github.com/shibing624/textgen/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
-        🌈 Implementation of Text Generation models.
+        🌈Implementation of Text Generation models.
         
         **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
-        - [Reference](#reference)
+        - [License](#License)
         
-        # Feature
+        ## 😊Feature
         
-        ## 文本生成
+        ### 文本生成
         
         1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
         2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
         3. t5: T5、CopyT5
         
-        ## 文本扩增
+        ### 文本扩增
         
-        ### 词粒度扩增
+        #### 词粒度扩增
         
         1. UDA，非核心词替换
         2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
         
-        ### 句粒度扩增
+        #### 句粒度扩增
         
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
-        ## 功能列表
+        ### 功能列表
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)
-          算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
+        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
-        - [TGLS](textgen/unsup_generation)
-          ：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
+        - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
-        ## Release Models
+        ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Introduce|Training|Inference| |:-- |:--- |:--- |:--- |:--- |
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
-        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
-        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重|[training
-        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|[predict
-        script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)|
         
-        # Demo
+        |Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
+        |:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        
+        ## 🚀Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
-        model trained
-        by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
+        model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
         
-        # Install
+        ## 💾Install
         
         ```shell
         pip install git+https://github.com/huggingface/transformers
         pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
@@ -119,42 +105,57 @@
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
         python setup.py install
         ```
         
-        # Usage
+        ## 😎Usage
         
-        ## ChatGLM-6B LoRA 模型
+        ### ChatGLM-6B LoRA 模型
         
-        ### 使用ChatGLM-6B LoRA微调后的模型
+        安装最新开发版的peft库，支持LoRA模型
+        
+        ```shell
+        pip install git+https://github.com/huggingface/peft
+        ```
+        
+        #### 使用ChatGLM-6B LoRA微调后的模型
         
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import ChatGlmModel
         
         model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
-        ### 训练ChatGLM-6B LoRA模型
+        PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
+        
+        #### 训练ChatGLM-6B LoRA模型
         
         支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
-        ## LLAMA LoRA 模型
+        ### LLAMA LoRA 模型
         
-        ### 使用LLAMA LoRA微调后的模型
+        安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
+        
+        ```shell
+        pip install transformers>=4.28.1
+        pip install git+https://github.com/huggingface/peft
+        ```
+        
+        #### 使用LLAMA LoRA微调后的模型
         
         example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
         
         ```python
         import sys
         
         sys.path.append('../..')
@@ -167,19 +168,19 @@
         
         model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
-        ### 训练LLAMA LoRA模型
+        #### 训练LLAMA LoRA模型
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
-        ## ConvSeq2Seq 模型
+        ### ConvSeq2Seq 模型
         
         训练并预测ConvSeq2Seq模型：
         
         example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
         ```python
         import argparse
@@ -224,30 +225,30 @@
         output:
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
-        ## BART 模型
+        ### BART 模型
         
         训练并预测BART模型：
         
         example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
-        ## T5 模型
+        ### T5 模型
         
-        example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
+        example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
         import pandas as pd
         import sys
         
@@ -338,48 +339,48 @@
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
-        ## GPT2 模型
+        ### GPT2 模型
         
-        ### 中文GPT2 - 文章生成
+        #### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
-        example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
+        example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
         
-        ### 中文GPT2 - 对联生成
+        #### 中文GPT2 - 对联生成
         
         使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
         
-        example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
+        example: [examples/gpt2/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_couplet_gpt2_demo.py)
         
-        #### GPT2 vs T5：
+        GPT2 vs T5：
         
         1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
         2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
         3. GPT2的模型优势是自由创作，如写一篇短文
         4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
         
         - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         
-        ## SongNet 模型
+        ### SongNet 模型
         
         格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
         适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
         
-        example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
+        example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
         
-        ## Keyword Text Augmentation(EDA/UDA)
+        ### Keyword Text Augmentation(EDA/UDA)
         
-        example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
+        example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
         from textgen.augment import TextAugment
         
@@ -416,19 +417,19 @@
         random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
         insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
         delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
         tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
         mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
         ```
         
-        ## TGLS 模型（无监督相似文本生成模型）
+        ### TGLS 模型（无监督相似文本生成模型）
         
         无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
         
-        example: [examples/unsup_generation_demo.py](examples/unsup_generation_demo.py)
+        example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
         
         ```python
         import os
         import sys
         
         sys.path.append('..')
         from textgen.unsup_generation import TglsModel, load_list
@@ -483,71 +484,72 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
-        # Dataset
+        ## 📚Dataset 
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3.
-        5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)
-           ：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
-        # Contact
+        ## ☎️Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        # Citation
+        ## 😇Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
           author={Xu Ming},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
-        # License
+        ## 🤗License
         
         授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
         
-        # Contribute
+        ## 😍Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        ## Reference
+        ## 💕Acknowledgements 
         
         - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
         - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
         - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
-        - [Tiiiger/bert_score]()
+        - [Tiiiger/bert_score](https://github.com/Tiiiger/bert_score)
+        - [ThilinaRajapakse/simpletransformers](https://github.com/ThilinaRajapakse/simpletransformers)
         - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
         - [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
+        
+        Thanks for their great work!
 Keywords: textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `textgen-0.2.1/textgen.egg-info/SOURCES.txt` & `textgen-0.2.2/textgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

