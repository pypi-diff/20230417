# Comparing `tmp/pyriksprot-2023.4.1.tar.gz` & `tmp/pyriksprot-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2023.4.1.tar", max compression
+gzip compressed data, was "pyriksprot-2023.4.2.tar", max compression
```

## Comparing `pyriksprot-2023.4.1.tar` & `pyriksprot-2023.4.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.1/LICENSE
--rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.1/README.md
--rw-r--r--   0        0        0     3406 2023-04-13 12:57:03.282516 pyriksprot-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0     1163 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/__init__.py
--rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     3526 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/utility.py
--rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     7718 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dehyphenation/utility.py
--rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.1/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    21549 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/gitchen.py
--rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/interface.py
--rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/config.py
--rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/repository.py
--rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/subset.py
--rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/verify.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/csv2pgsql.py
--rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/fix_speaker_notes.py
--rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2695 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     3475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech_text.py
--rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tfs.py
--rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/speaker_note2csv
--rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     1196 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/subset_corpus.py
--rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/utils.py
--rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/xml2csv
--rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/00_rename.sql
--rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/01_data_updates.sql
--rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/02_code_tables.sql
--rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/03_persons_of_interest.sql
--rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/04_terms_of_office.sql
--rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/05_person_party.sql
--rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/06_unknown.sql
--rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/09_cleanup.sql
--rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/__init__.py
--rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    12385 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/utility.py
--rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/_extract_speech_ids.py
--rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_speech_text.py
--rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/workflows/speech_index.py
--rw-r--r--   0        0        0     2230 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/subset_corpus.py
--rw-r--r--   0        0        0     5313 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4137 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.2/LICENSE
+-rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.2/README.md
+-rw-r--r--   0        0        0     3406 2023-04-17 14:56:36.929977 pyriksprot-2023.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1250 2023-04-17 14:55:11.204894 pyriksprot-2023.4.2/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     3528 2023-04-14 06:54:51.788513 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/corpus/utility.py
+-rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     8562 2023-04-17 14:55:11.248895 pyriksprot-2023.4.2/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dehyphenation/utility.py
+-rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.2/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    21549 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/gitchen.py
+-rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/interface.py
+-rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/config.py
+-rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/repository.py
+-rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/subset.py
+-rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/metadata/verify.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.2/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/csv2pgsql.py
+-rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2695 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     3475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech_text.py
+-rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tfs.py
+-rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/speaker_note2csv
+-rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     1196 2023-04-13 13:53:50.922546 pyriksprot-2023.4.2/pyriksprot/scripts/subset_corpus.py
+-rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/utils.py
+-rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.2/pyriksprot/scripts/xml2csv
+-rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/00_rename.sql
+-rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/01_data_updates.sql
+-rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/02_code_tables.sql
+-rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/03_persons_of_interest.sql
+-rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/04_terms_of_office.sql
+-rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/05_person_party.sql
+-rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/06_unknown.sql
+-rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/09_cleanup.sql
+-rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/sql/__init__.py
+-rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    12974 2023-04-17 05:36:18.788607 pyriksprot-2023.4.2/pyriksprot/utility.py
+-rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/_extract_speech_ids.py
+-rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_speech_text.py
+-rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.2/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.2/pyriksprot/workflows/subset_corpus.py
+-rw-r--r--   0        0        0     6120 2023-04-17 14:55:10.780889 pyriksprot-2023.4.2/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4137 2023-04-13 10:55:09.503216 pyriksprot-2023.4.2/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.2/PKG-INFO
```

### Comparing `pyriksprot-2023.4.1/LICENSE` & `pyriksprot-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/README.md` & `pyriksprot-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyproject.toml` & `pyriksprot-2023.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2023.4.1"
+version = "2023.4.2"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/__init__.py` & `pyriksprot-2023.4.2/pyriksprot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .dispatch import DispatchItem, SegmentMerger, create_grouping_hashcoder
 from .interface import ParlaClarinError, Protocol, SegmentLevel, Speech, Utterance
 from .to_speech import MergerFactory, MergeStrategyType, to_speeches
 from .utility import (
     compose,
     dedent,
     deprecated,
+    dget,
+    dotget,
     ensure_path,
     flatten,
     hasattr_path,
     is_empty,
     lookup,
     norm_join,
     parse_range_list,
@@ -33,8 +35,16 @@
     sync_delta_names,
     temporary_file,
     touch,
     ts_data_path,
     unlink,
 )
 from .workflows import compute_term_frequencies, extract_corpus_tags, extract_corpus_text
-from .workflows.tag import ITagger, TaggedDocument, tag_protocol, tag_protocol_xml, tag_protocols
+from .workflows.tag import (
+    ITagger,
+    ITaggerFactory,
+    TaggedDocument,
+    TaggerRegistry,
+    tag_protocol,
+    tag_protocol_xml,
+    tag_protocols,
+)
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/corpus_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/iterate.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/convert.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,24 +75,24 @@
 
 
 def convert_protocol(
     input_filename: str = None,
     output_filename: str = None,
     template_name: str = None,
     merge_strategy: to_speech.MergeStrategyType = to_speech.MergeStrategyType.who_speaker_note_id_sequence,
-    dehyphen_folder: str = None,
+    dehyphen_datadir: str = None,
 ):
     """Convert protocol in `input_filename' using template `template_name`. Store result in `output_filename`.
 
     Args:
         input_filename (str, optional): Source file. Defaults to None.
         output_filename (str, optional): Target file. Defaults to None.
         template_name (str, optional): Template name (found in resource-folder). Defaults to None.
     """
-    set_dehyphenator(data_folder=dehyphen_folder)
+    set_dehyphenator(data_folder=dehyphen_datadir)
     protocol: interface.Protocol = parse.ProtocolMapper.parse(input_filename)
     content: str = ""
 
     if protocol.has_text:
         converter: ProtocolConverter = ProtocolConverter(template_name)
         speeches: List[interface.Speech] = to_speech.to_speeches(protocol=protocol, merge_strategy=merge_strategy)
         content: str = converter.convert(protocol, speeches, strip_paths(input_filename))
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/parse.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/parse.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/tagged/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/tagged/persist.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/corpus/utility.py` & `pyriksprot-2023.4.2/pyriksprot/corpus/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2023.4.2/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2023.4.2/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 Published in PARLACLARIN 2020. https://www.semanticscholar.org/paper/Anf%C3%B6randen%3A-Annotated-and-Augmented-Parliamentary-Eide/46baeb3f444a085540a1b57278de7ed4ea385b04
 
 This source code is heavily influenced by the source code found at https://gitlab.com/Julipan/swedish-de-hyphenator/, released under GNU GPLv3.
 
 License: https://gitlab.com/Julipan/swedish-de-hyphenator/-/blob/master/LICENSE
 
 """
-import os
 import re
 from dataclasses import dataclass, field
 from enum import IntEnum
+from os.path import isfile, join
 from typing import Callable
 
 from .utility import load_dict, load_token_set, store_dict, store_token_set
 
 PARAGRAPH_MARKER = '##PARAGRAPH##'
 
 # pylint: disable=too-many-arguments
-jj = os.path.join
+jj = join
 
 
 class WhitelistReason(IntEnum):
     Undefined = 0
     HyphenatedCompound = 1
     Frequency = 2
     UnknownParts = 3
@@ -65,39 +65,60 @@
 
 class ParagraphMergeStrategy(IntEnum):
     DoNotMerge = (0,)
     MergeIfWordsOnlySeparatedByTwoNewlines = (1,)
     MergeAll = 2
 
 
+WORD_FREQUENCIES_NAME: str = 'word-frequencies.pkl'
+
+
 @dataclass
 class SwedishDehyphenator:
     """Dehyphens Swedish text"""
 
     data_folder: str
-    word_frequencies: dict[str, int]
+    word_frequencies: dict[str, int] | str
 
     # Internal data
     whitelist: set[str] = field(default_factory=set)
     whitelist_log: dict[str, int] = field(default_factory=dict)
     unresolved: set[str] = field(default_factory=set)
 
     paragraph_merge_strategy: ParagraphMergeStrategy = 0
 
-    def __post_init__(self) -> "SwedishDehyphenator":
-        if self.word_frequencies is None:
-            self.word_frequencies = os.path.join(self.data_folder, 'riksdagen-corpus-term-frequencies.pkl')
+    word_frequencies_filename: str = field(default=WORD_FREQUENCIES_NAME)
 
-        if isinstance(self.word_frequencies, str):
-            if not os.path.isfile(self.word_frequencies):
-                raise FileNotFoundError(self.word_frequencies)
-            self.word_frequencies = load_dict(self.word_frequencies)
+    def __post_init__(self) -> "SwedishDehyphenator":
+        if not isinstance(self.word_frequencies, (dict, type(None))):
+            self.word_frequencies_filename: str = self.resolve_word_frequencies_filename()
+            self.word_frequencies = load_dict(self.word_frequencies_filename)
 
         self.load()
 
+    def resolve_word_frequencies_filename(self) -> str:
+        if not isinstance(self.word_frequencies, str):
+            if not isfile(self.word_frequencies_filename):
+                return jj(self.data_folder, self.word_frequencies_filename)
+            return self.word_frequencies_filename
+
+        if isfile(self.word_frequencies):
+            return self.word_frequencies
+
+        if isfile(jj(self.data_folder, self.word_frequencies)):
+            return jj(self.data_folder, self.word_frequencies)
+
+        if isfile(jj(self.data_folder, self.word_frequencies_filename)):
+            return jj(self.data_folder, self.word_frequencies_filename)
+
+        if isfile(self.word_frequencies_filename):
+            return self.word_frequencies_filename
+
+        raise FileNotFoundError(f"expected TF file {self.word_frequencies} not found")
+
     @property
     def whitelist_filename(self) -> str:
         return jj(self.data_folder, 'dehyphen_whitelist.txt.gz')
 
     @property
     def whitelist_log_filename(self) -> str:
         return jj(self.data_folder, 'dehyphen_whitelist_log.pkl')
@@ -208,15 +229,15 @@
     def load(self) -> None:
         self.whitelist = load_token_set(self.whitelist_filename)
         self.whitelist_log = load_dict(self.whitelist_log_filename)
         self.unresolved = load_token_set(self.unresolved_filename)
 
     @staticmethod
     def create_dehypen(data_folder: str, word_frequencies: str | dict = None) -> Callable[[str], str]:
-        """Create a dehypen service. Return wrapped dehypen function."""
+        """Create a dehyphen service. Return wrapped dehyphen function."""
         dehyphenator: SwedishDehyphenator = SwedishDehyphenator(
             data_folder=data_folder, word_frequencies=word_frequencies
         )
 
         def dehyphen(text: str) -> str:
             """Remove hyphens from `text`."""
             dehyphenated_text = dehyphenator.dehyphen_text(text)
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/dehyphenation/utility.py` & `pyriksprot-2023.4.2/pyriksprot/dehyphenation/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2023.4.2/pyriksprot/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dispatch/item.py` & `pyriksprot-2023.4.2/pyriksprot/dispatch/item.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dispatch/merge.py` & `pyriksprot-2023.4.2/pyriksprot/dispatch/merge.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/dispatch/utility.py` & `pyriksprot-2023.4.2/pyriksprot/dispatch/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv` & `pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2023.4.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/pos_tags.py` & `pyriksprot-2023.4.2/pyriksprot/foss/pos_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/sparv_tokenize.py` & `pyriksprot-2023.4.2/pyriksprot/foss/sparv_tokenize.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/stopwords.py` & `pyriksprot-2023.4.2/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/foss/untangle.py` & `pyriksprot-2023.4.2/pyriksprot/foss/untangle.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/gitchen.py` & `pyriksprot-2023.4.2/pyriksprot/gitchen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/interface.py` & `pyriksprot-2023.4.2/pyriksprot/interface.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/__init__.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/codecs.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/codecs.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/config.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/generate.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/generate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/person.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/person.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/repository.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/repository.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/subset.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/subset.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/utility.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/utterance.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/utterance.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/metadata/verify.py` & `pyriksprot-2023.4.2/pyriksprot/metadata/verify.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/csv2pgsql.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/csv2pgsql.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/fix_speaker_notes.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/fix_speaker_notes.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/metadata2db.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech_text.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2tagged.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2text.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/riksprot2text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/speaker_note2csv` & `pyriksprot-2023.4.2/pyriksprot/scripts/speaker_note2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/speech_index.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/subset_corpus.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/utils.py` & `pyriksprot-2023.4.2/pyriksprot/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/scripts/xml2csv` & `pyriksprot-2023.4.2/pyriksprot/scripts/xml2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/00_rename.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/00_rename.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/01_data_updates.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/01_data_updates.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/02_code_tables.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/02_code_tables.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/03_persons_of_interest.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/03_persons_of_interest.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/04_terms_of_office.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/04_terms_of_office.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/05_person_party.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/05_person_party.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/06_unknown.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/06_unknown.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/sql/09_cleanup.sql` & `pyriksprot-2023.4.2/pyriksprot/sql/09_cleanup.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/to_speech.py` & `pyriksprot-2023.4.2/pyriksprot/to_speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/utility.py` & `pyriksprot-2023.4.2/pyriksprot/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,40 @@
         value = self.get(*args)
         return dotdict(value) if isinstance(value, dict) else value
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
+def dotget(data: dict, path: str | list[str], default: Any = None) -> Any:
+    if path is None or not data:
+        return default
+
+    ps: list[str] = path if isinstance(path, (list, tuple)) else [path]
+
+    d = None
+
+    for p in ps:
+        d = data
+        for attr in p.split('.'):
+            d: dict = d.get(attr) if isinstance(d, dict) else None
+
+            if d is None:
+                break
+
+        if d is not None:
+            return d
+
+    return d or default
+
+
+def dget(data: dict, *paths: list[str], default: Any = None) -> Any:
+    return dotget(data, paths, default)
+
+
 def sync_delta_names(
     source_folder: str, source_extension: str, target_folder: str, target_extension: str, delete: bool = False
 ) -> Set(str):
     """Returns basenames in targat_folder that doesn't exist in source folder (with respectively extensions)"""
 
     source_names = strip_paths(glob.glob(jj(source_folder, "*", f"*.{source_extension}")))
     target_names = strip_paths(glob.glob(jj(target_folder, "*", f"*.{target_extension}")))
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/_extract_speech_ids.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/_extract_speech_ids.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/extract_speech_text.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/extract_speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/extract_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/extract_text.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/extract_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/speech_index.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/subset_corpus.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/tag.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import abc
 import itertools
 from functools import reduce
 from glob import glob
-from os.path import getmtime, isfile, join
-from typing import Any, Callable, List, Mapping, Union
+from os.path import dirname, getmtime, isfile, join, split
+from typing import Any, Callable, List, Mapping, Type, Union
 
 from loguru import logger
 from tqdm import tqdm
 
 from pyriksprot.corpus.parlaclarin import parse
 from pyriksprot.corpus.tagged import persist
 
@@ -17,14 +17,22 @@
 from ..utility import ensure_path, strip_path_and_extension, touch, unlink
 
 METADATA_FILENAME: str = 'metadata.json'
 
 TaggedDocument = Mapping[str, List[str]]
 
 
+class ITaggerFactory(abc.ABC):
+    identifier: str = "undefined"
+
+    @abc.abstractmethod
+    def create(self) -> "ITagger":
+        ...
+
+
 class ITagger(abc.ABC):
     def __init__(self, preprocessors: Callable[[str], str] = None):
         self.preprocessors: Callable[[str], str] = preprocessors or []
 
     def tag(self, text: Union[str, List[str]], preprocess: bool = True) -> List[TaggedDocument]:
         """Tag text. Return dict if lists."""
         if isinstance(text, str):
@@ -71,14 +79,30 @@
 
     def preprocess(self, text: str) -> str:
         """Transform `text` with preprocessors."""
         text: str = reduce(lambda res, f: f(res), self.preprocessors, text)
         return text
 
 
+class TaggerRegistry:
+    """Simple tagger cache since somee taggers are expensive to setup"""
+
+    instances: Mapping[Type[ITagger], ITagger] = {}
+
+    @staticmethod
+    def get(factory: "ITaggerFactory") -> ITagger:
+        if isinstance(factory, ITagger):
+            return factory
+
+        if factory.identifier not in TaggerRegistry.instances:
+            TaggerRegistry.instances[factory.identifier] = factory.create()
+
+        return TaggerRegistry.instances[factory.identifier]
+
+
 def tag_protocol(tagger: ITagger, protocol: interface.Protocol, preprocess=False) -> interface.Protocol:
     texts = [u.text for u in protocol.utterances]
 
     documents: List[TaggedDocument] = tagger.tag(texts, preprocess=preprocess)
 
     for i, document in enumerate(documents):
         protocol.utterances[i].annotation = tagger.to_csv(document)
@@ -131,22 +155,29 @@
 
     except Exception:
         logger.error(f"FAILED: {input_filename}")
         unlink(output_filename)
         raise
 
 
-def tag_protocols(tagger: ITagger, source_folder: str, target_folder: str, force: bool):
+def tag_protocols(
+    tagger: ITagger,
+    source_folder: str,
+    target_folder: str,
+    force: bool,
+    recursive: bool = False,
+):
     """Tags protocols in `source_folder`. Stores result in `target_folder`.
     Note: not used by Snakemake workflow (used by tag CLI script)
     """
 
-    source_files: list[str] = glob(join(source_folder, "prot-*.xml"))
+    source_files: list[str] = glob(join(source_folder, "prot-*.xml"), recursive=recursive)
     for source_file in tqdm(source_files):
-        target_file = join(target_folder, f"{strip_path_and_extension(source_file)}.zip")
+        subfolder: str = split(dirname(source_file))[1] if recursive else ''
+        target_file = join(target_folder, subfolder, f"{strip_path_and_extension(source_file)}.zip")
         if force or expired(target_file, source_file):
             tag_protocol_xml(source_file, target_file, tagger, storage_format="json", force=force)
         else:
             touch(target_file)
 
 
 def expired(filename: str, expiry_instance: float | str) -> bool:
```

### Comparing `pyriksprot-2023.4.1/pyriksprot/workflows/tf.py` & `pyriksprot-2023.4.2/pyriksprot/workflows/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.1/PKG-INFO` & `pyriksprot-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Python API for Riksdagens Protokoll
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
```

