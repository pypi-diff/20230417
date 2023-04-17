# Comparing `tmp/swh.indexer-2.9.1.tar.gz` & `tmp/swh.indexer-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.indexer-2.9.1.tar", last modified: Wed Nov 30 10:52:14 2022, max compression
+gzip compressed data, was "dist/swh.indexer-2.9.3.tar", last modified: Mon Feb 13 10:03:47 2023, max compression
```

## Comparing `swh.indexer-2.9.1.tar` & `swh.indexer-2.9.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      173 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      909 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       71 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      233 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)     1149 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/codemeta.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1086 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       64 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      155 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      151 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4896 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/dev-info.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)       28 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      194 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2842 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/images/tasks-metadata-indexers.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      421 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    10881 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/docs/metadata-workflow.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      593 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       99 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      138 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      145 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      238 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2320 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/sql/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/sql/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1741 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) docker     (999)      393 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/bin/dot_add_content
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/sql/doc/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/sql/doc/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/doc/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/doc/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      269 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/doc/json/indexer_configuration.tool_configuration.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1283 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/doc/json/revision_metadata.translated_metadata.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/sql/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      269 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/json/indexer_configuration.tool_configuration.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1283 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/sql/json/revision_metadata.translated_metadata.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/
--rw-r--r--   0 jenkins    (115) docker     (999)      424 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12476 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7466 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/codemeta.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     1030 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/Gitea.csv
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/data/codemeta/
--rw-r--r--   0 jenkins    (115) docker     (999)      490 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/codemeta/CITATION
--rw-r--r--   0 jenkins    (115) docker     (999)    10253 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/codemeta/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)     4362 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/codemeta/codemeta.jsonld
--rw-r--r--   0 jenkins    (115) docker     (999)    14995 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/codemeta/crosswalk.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     1023 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/composer.csv
--rw-r--r--   0 jenkins    (115) docker     (999)      990 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/nuget.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     1019 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/data/pubspec.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     5921 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/fossology_license.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24988 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/indexer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1644 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20357 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)      954 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_detector.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/
--rw-r--r--   0 jenkins    (115) docker     (999)     2005 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14971 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2461 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/cff.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7872 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1897 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/composer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2178 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/dart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4534 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5037 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6056 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/maven.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10946 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/npm.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3311 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/nuget.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2793 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/python.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4568 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/ruby.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3788 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/metadata_dictionary/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4863 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/mimetype.py
--rw-r--r--   0 jenkins    (115) docker     (999)      544 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/namespaces.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5933 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/origin_head.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     6927 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/rehash.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      121 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5728 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/50-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    12719 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/50-func.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4468 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     1301 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3665 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      530 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      432 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2930 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2284 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      475 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      347 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3743 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      387 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1568 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1677 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2734 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      311 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3718 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1506 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7560 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1618 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5324 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6879 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4417 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6094 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      607 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/sql/upgrades/137.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/storage/
--rw-r--r--   0 jenkins    (115) docker     (999)    22698 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/storage/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      806 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3328 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1486 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14976 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)      598 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15621 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13021 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2197 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3870 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2525 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/storage/writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1438 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      349 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4019 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5712 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_cff.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18435 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2125 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_composer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3965 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_dart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4209 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5419 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_github.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13207 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_maven.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13676 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_npm.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5961 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_nuget.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3600 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_python.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4433 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_ruby.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/
--rw-r--r--   0 jenkins    (115) docker     (999)      351 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2736 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5198 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/generate_data_test.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1831 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2229 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)      522 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3262 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1728 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)      962 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3966 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    62604 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/storage/test_storage.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1325 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26663 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7747 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4714 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_fossology_license.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7625 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_indexer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4045 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16076 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4288 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_mimetype.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8300 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_origin_head.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12457 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/test_origin_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23669 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh/indexer/tests/zz_celery/
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/zz_celery/README
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/zz_celery/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3185 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/swh/indexer/tests/zz_celery/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     5398 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      379 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-11-30 10:52:14.000000 swh.indexer-2.9.1/swh.indexer.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1641 2022-11-30 10:52:12.000000 swh.indexer-2.9.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      173 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       71 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      233 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)     1149 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/codemeta.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1086 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       64 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      155 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      151 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4896 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/dev-info.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)       28 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2842 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/tasks-metadata-indexers.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      539 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    10881 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/metadata-workflow.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      593 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       99 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      145 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      238 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2320 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1741 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      393 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/bin/dot_add_content
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/doc/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/doc/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/indexer_configuration.tool_configuration.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/revision_metadata.translated_metadata.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/indexer_configuration.tool_configuration.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/revision_metadata.translated_metadata.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/
+-rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12476 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7466 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/codemeta.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1030 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/Gitea.csv
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/
+-rw-r--r--   0 jenkins    (115) docker     (999)      490 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/CITATION
+-rw-r--r--   0 jenkins    (115) docker     (999)    10253 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)     4362 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/codemeta.jsonld
+-rw-r--r--   0 jenkins    (115) docker     (999)    14995 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/crosswalk.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     1023 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/composer.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)      990 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/nuget.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     1019 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/pubspec.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     5921 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/fossology_license.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24988 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/indexer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1644 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20357 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      954 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_detector.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2005 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14971 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2461 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/cff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7872 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1897 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/composer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2178 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/dart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4534 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5037 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6056 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/maven.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10946 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/npm.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3311 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/nuget.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2793 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/python.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4568 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/ruby.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3788 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4863 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/mimetype.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      544 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/namespaces.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5933 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/origin_head.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/rehash.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      121 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5728 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/50-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    12719 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/50-func.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1301 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3665 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      530 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      432 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2930 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2284 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3743 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      387 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1568 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1677 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2734 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      311 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3718 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1506 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7560 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5324 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6879 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4417 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6094 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      607 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/137.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/storage/
+-rw-r--r--   0 jenkins    (115) docker     (999)    24539 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/storage/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      806 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3365 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1486 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14976 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      598 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16262 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13021 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2197 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2398 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1438 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      349 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5712 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_cff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18435 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2125 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_composer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3965 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_dart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4209 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5419 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13207 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_maven.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13676 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_npm.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5961 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_nuget.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3600 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_python.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4433 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_ruby.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/
+-rw-r--r--   0 jenkins    (115) docker     (999)      351 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2736 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5198 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/generate_data_test.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2229 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      522 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3262 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1728 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1702 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3966 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    63148 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_storage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1325 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26663 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7747 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4714 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_fossology_license.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7625 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_indexer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4045 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16076 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4288 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_mimetype.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8300 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_origin_head.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12457 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_origin_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    23669 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/README
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3185 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh.indexer.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     5398 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh.indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      379 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1641 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/tox.ini
```

### Comparing `swh.indexer-2.9.1/.pre-commit-config.yaml` & `swh.indexer-2.9.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         entry: mypy
         args: [swh]
         pass_filenames: false
         language: system
         types: [python]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
 
   - repo: https://github.com/python/black
     rev: 22.10.0
     hooks:
       - id: black
```

### Comparing `swh.indexer-2.9.1/CODE_OF_CONDUCT.md` & `swh.indexer-2.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/LICENSE` & `swh.indexer-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/PKG-INFO` & `swh.indexer-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.indexer
-Version: 2.9.1
+Version: 2.9.3
 Summary: Software Heritage Content Indexer
 Home-page: https://forge.softwareheritage.org/diffusion/78/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-indexer
```

### Comparing `swh.indexer-2.9.1/README.md` & `swh.indexer-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/codemeta.json` & `swh.indexer-2.9.3/codemeta.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/conftest.py` & `swh.indexer-2.9.3/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/docs/README.md` & `swh.indexer-2.9.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/docs/dev-info.rst` & `swh.indexer-2.9.3/docs/dev-info.rst`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/docs/images/tasks-metadata-indexers.uml` & `swh.indexer-2.9.3/docs/images/tasks-metadata-indexers.uml`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/docs/metadata-workflow.rst` & `swh.indexer-2.9.3/docs/metadata-workflow.rst`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/mypy.ini` & `swh.indexer-2.9.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/setup.py` & `swh.indexer-2.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/sql/bin/db-upgrade` & `swh.indexer-2.9.3/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/sql/doc/json/revision_metadata.translated_metadata.json` & `swh.indexer-2.9.3/sql/doc/json/revision_metadata.translated_metadata.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/sql/json/revision_metadata.translated_metadata.json` & `swh.indexer-2.9.3/sql/json/revision_metadata.translated_metadata.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/cli.py` & `swh.indexer-2.9.3/swh/indexer/cli.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/codemeta.py` & `swh.indexer-2.9.3/swh/indexer/codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/Gitea.csv` & `swh.indexer-2.9.3/swh/indexer/data/Gitea.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/codemeta/LICENSE` & `swh.indexer-2.9.3/swh/indexer/data/codemeta/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/codemeta/codemeta.jsonld` & `swh.indexer-2.9.3/swh/indexer/data/codemeta/codemeta.jsonld`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/codemeta/crosswalk.csv` & `swh.indexer-2.9.3/swh/indexer/data/codemeta/crosswalk.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/composer.csv` & `swh.indexer-2.9.3/swh/indexer/data/composer.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/nuget.csv` & `swh.indexer-2.9.3/swh/indexer/data/nuget.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/data/pubspec.csv` & `swh.indexer-2.9.3/swh/indexer/data/pubspec.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/fossology_license.py` & `swh.indexer-2.9.3/swh/indexer/fossology_license.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/indexer.py` & `swh.indexer-2.9.3/swh/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/journal_client.py` & `swh.indexer-2.9.3/swh/indexer/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata.py` & `swh.indexer-2.9.3/swh/indexer/metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_detector.py` & `swh.indexer-2.9.3/swh/indexer/metadata_detector.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/__init__.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/base.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/base.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/cff.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/cff.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/codemeta.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/composer.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/composer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/dart.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/dart.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/gitea.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/gitea.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/github.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/github.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/maven.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/maven.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/npm.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/npm.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/nuget.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/nuget.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/python.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/python.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/ruby.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/ruby.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/metadata_dictionary/utils.py` & `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/utils.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/mimetype.py` & `swh.indexer-2.9.3/swh/indexer/mimetype.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/namespaces.py` & `swh.indexer-2.9.3/swh/indexer/namespaces.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/origin_head.py` & `swh.indexer-2.9.3/swh/indexer/origin_head.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/rehash.py` & `swh.indexer-2.9.3/swh/indexer/rehash.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/30-schema.sql` & `swh.indexer-2.9.3/swh/indexer/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/50-func.sql` & `swh.indexer-2.9.3/swh/indexer/sql/50-func.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/60-indexes.sql` & `swh.indexer-2.9.3/swh/indexer/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/115.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/116.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/116.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/117.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/119.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/120.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/123.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/125.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/126.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/126.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/127.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/129.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/130.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/131.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/131.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/132.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/132.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/133.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/133.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/134.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/135.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/135.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/136.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/sql/upgrades/137.sql` & `swh.indexer-2.9.3/swh/indexer/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/__init__.py` & `swh.indexer-2.9.3/swh/indexer/storage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from collections import Counter
 from importlib import import_module
 import json
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 import warnings
 
+import attr
 import psycopg2
 import psycopg2.pool
 
 from swh.core.db.common import db_transaction
 from swh.indexer.storage.interface import IndexerStorageInterface
 from swh.model.hashutil import hash_to_bytes, hash_to_hex
 from swh.model.model import SHA1_SIZE
@@ -111,25 +112,27 @@
     a `ValueError`.
 
     Values associated to the key must be hashable.
 
     Args:
         data (List[dict]): List of dictionaries to be inserted
 
+    >>> tool1 = {"name": "foo", "version": "1.2.3", "configuration": {}}
+    >>> tool2 = {"name": "foo", "version": "1.2.4", "configuration": {}}
     >>> check_id_duplicates([
-    ...     ContentLicenseRow(id=b'foo', indexer_configuration_id=42, license="GPL"),
-    ...     ContentLicenseRow(id=b'foo', indexer_configuration_id=32, license="GPL"),
+    ...     ContentLicenseRow(id=b'foo', tool=tool1, license="GPL"),
+    ...     ContentLicenseRow(id=b'foo', tool=tool2, license="GPL"),
     ... ])
     >>> check_id_duplicates([
-    ...     ContentLicenseRow(id=b'foo', indexer_configuration_id=42, license="AGPL"),
-    ...     ContentLicenseRow(id=b'foo', indexer_configuration_id=42, license="AGPL"),
+    ...     ContentLicenseRow(id=b'foo', tool=tool1, license="AGPL"),
+    ...     ContentLicenseRow(id=b'foo', tool=tool1, license="AGPL"),
     ... ])
     Traceback (most recent call last):
     ...
-    swh.indexer.storage.exc.DuplicateId: [{'id': b'foo', 'indexer_configuration_id': 42, 'license': 'AGPL'}]
+    swh.indexer.storage.exc.DuplicateId: [{'id': b'foo', 'license': 'AGPL', 'tool_configuration': '{}', 'tool_name': 'foo', 'tool_version': '1.2.3'}]
 
     """  # noqa
     counter = Counter(tuple(sorted(item.unique_key().items())) for item in data)
     duplicates = [id_ for (id_, count) in counter.items() if count >= 2]
     if duplicates:
         raise DuplicateId(list(map(dict, duplicates)))
 
@@ -143,15 +146,15 @@
         """
         Args:
             db: either a libpq connection string, or a psycopg2 connection
             journal_writer: configuration passed to
                             `swh.journal.writer.get_journal_writer`
 
         """
-        self.journal_writer = JournalWriter(self._tool_get_from_id, journal_writer)
+        self.journal_writer = JournalWriter(journal_writer)
         try:
             if isinstance(db, psycopg2.extensions.connection):
                 self._pool = None
                 self._db = Db(db)
             else:
                 self._pool = psycopg2.pool.ThreadedConnectionPool(
                     min_pool_conns, max_pool_conns, db
@@ -165,14 +168,40 @@
             return self._db
         return Db.from_pool(self._pool)
 
     def put_db(self, db):
         if db is not self._db:
             db.put_conn()
 
+    def _join_indexer_configuration(self, entries, db, cur):
+        """Replaces ``entry.indexer_configuration_id`` with a full tool dict
+        in ``entry.tool``."""
+        joined_entries = []
+
+        # usually, all the additions in a batch are from the same indexer,
+        # so this cache allows doing a single query for all the entries.
+        tool_cache = {}
+
+        for entry in entries:
+            # get the tool used to generate this addition
+            tool_id = entry.indexer_configuration_id
+            assert tool_id
+            if tool_id not in tool_cache:
+                tool_cache[tool_id] = dict(
+                    self._tool_get_from_id(tool_id, db=db, cur=cur)
+                )
+                del tool_cache[tool_id]["id"]
+            entry = attr.evolve(
+                entry, tool=tool_cache[tool_id], indexer_configuration_id=None
+            )
+
+            joined_entries.append(entry)
+
+        return joined_entries
+
     @timed
     @db_transaction()
     def check_config(self, *, check_write, db=None, cur=None):
         # Check permissions on one of the tables
         if check_write:
             check = "INSERT"
         else:
@@ -289,16 +318,19 @@
     @db_transaction()
     def content_mimetype_add(
         self,
         mimetypes: List[ContentMimetypeRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(mimetypes)
-        self.journal_writer.write_additions("content_mimetype", mimetypes)
+        mimetypes_with_tools = self._join_indexer_configuration(
+            mimetypes, db=db, cur=cur
+        )
+        check_id_duplicates(mimetypes_with_tools)
+        self.journal_writer.write_additions("content_mimetype", mimetypes_with_tools)
         db.mktemp_content_mimetype(cur)
         db.copy_to(
             [m.to_dict() for m in mimetypes],
             "tmp_content_mimetype",
             ["id", "mimetype", "encoding", "indexer_configuration_id"],
             cur,
         )
@@ -336,16 +368,19 @@
     @db_transaction()
     def content_fossology_license_add(
         self,
         licenses: List[ContentLicenseRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(licenses)
-        self.journal_writer.write_additions("content_fossology_license", licenses)
+        licenses_with_tools = self._join_indexer_configuration(licenses, db=db, cur=cur)
+        check_id_duplicates(licenses_with_tools)
+        self.journal_writer.write_additions(
+            "content_fossology_license", licenses_with_tools
+        )
         db.mktemp_content_fossology_license(cur)
         db.copy_to(
             [license.to_dict() for license in licenses],
             tblname="tmp_content_fossology_license",
             columns=["id", "license", "indexer_configuration_id"],
             cur=cur,
         )
@@ -400,16 +435,17 @@
     @db_transaction()
     def content_metadata_add(
         self,
         metadata: List[ContentMetadataRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(metadata)
-        self.journal_writer.write_additions("content_metadata", metadata)
+        metadata_with_tools = self._join_indexer_configuration(metadata, db=db, cur=cur)
+        check_id_duplicates(metadata_with_tools)
+        self.journal_writer.write_additions("content_metadata", metadata_with_tools)
 
         db.mktemp_content_metadata(cur)
 
         rows = [m.to_dict() for m in metadata]
         for row in rows:
             row["metadata"] = sanitize_json(row["metadata"])
 
@@ -453,16 +489,19 @@
     @db_transaction()
     def directory_intrinsic_metadata_add(
         self,
         metadata: List[DirectoryIntrinsicMetadataRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(metadata)
-        self.journal_writer.write_additions("directory_intrinsic_metadata", metadata)
+        metadata_with_tools = self._join_indexer_configuration(metadata, db=db, cur=cur)
+        check_id_duplicates(metadata_with_tools)
+        self.journal_writer.write_additions(
+            "directory_intrinsic_metadata", metadata_with_tools
+        )
 
         db.mktemp_directory_intrinsic_metadata(cur)
 
         rows = [m.to_dict() for m in metadata]
         for row in rows:
             row["metadata"] = sanitize_json(row["metadata"])
 
@@ -496,16 +535,19 @@
     @db_transaction()
     def origin_intrinsic_metadata_add(
         self,
         metadata: List[OriginIntrinsicMetadataRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(metadata)
-        self.journal_writer.write_additions("origin_intrinsic_metadata", metadata)
+        metadata_with_tools = self._join_indexer_configuration(metadata, db=db, cur=cur)
+        check_id_duplicates(metadata_with_tools)
+        self.journal_writer.write_additions(
+            "origin_intrinsic_metadata", metadata_with_tools
+        )
 
         db.mktemp_origin_intrinsic_metadata(cur)
 
         rows = [m.to_dict() for m in metadata]
         for row in rows:
             row["metadata"] = sanitize_json(row["metadata"])
 
@@ -637,16 +679,19 @@
     @db_transaction()
     def origin_extrinsic_metadata_add(
         self,
         metadata: List[OriginExtrinsicMetadataRow],
         db=None,
         cur=None,
     ) -> Dict[str, int]:
-        check_id_duplicates(metadata)
-        self.journal_writer.write_additions("origin_extrinsic_metadata", metadata)
+        metadata_with_tools = self._join_indexer_configuration(metadata, db=db, cur=cur)
+        check_id_duplicates(metadata_with_tools)
+        self.journal_writer.write_additions(
+            "origin_extrinsic_metadata", metadata_with_tools
+        )
 
         db.mktemp_origin_extrinsic_metadata(cur)
 
         rows = [m.to_dict() for m in metadata]
         for row in rows:
             row["metadata"] = sanitize_json(row["metadata"])
```

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/api/client.py` & `swh.indexer-2.9.3/swh/indexer/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/api/serializers.py` & `swh.indexer-2.9.3/swh/indexer/storage/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/api/server.py` & `swh.indexer-2.9.3/swh/indexer/storage/api/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
 
 @app.errorhandler(Exception)
 def my_error_handler(exception):
     return error_handler(exception, encode_data)
 
 
+app.setup_psycopg2_errorhandlers()
+
+
 @app.errorhandler(IndexerStorageArgumentException)
 def argument_error_handler(exception):
     return error_handler(exception, encode_data, status_code=400)
 
 
 @app.route("/")
 def index():
```

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/converters.py` & `swh.indexer-2.9.3/swh/indexer/storage/converters.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/db.py` & `swh.indexer-2.9.3/swh/indexer/storage/db.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/exc.py` & `swh.indexer-2.9.3/swh/indexer/storage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/in_memory.py` & `swh.indexer-2.9.3/swh/indexer/storage/in_memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
+import attr
+
 from swh.core.collections import SortedList
 from swh.model.hashutil import hash_to_bytes, hash_to_hex
 from swh.model.model import SHA1_SIZE
 from swh.storage.utils import get_partition_bounds_bytes
 
 from . import MAPPING_NAMES, check_id_duplicates
 from .exc import IndexerStorageArgumentException
@@ -79,14 +81,38 @@
         self.row_class = row_class
         self._tools = tools
         self._sorted_ids = SortedList[bytes, Sha1]()
         self._data = defaultdict(dict)
         self._journal_writer = journal_writer
         self._tools_per_id = defaultdict(set)
 
+    def _join_indexer_configuration(self, entries):
+        """Replaces ``entry.indexer_configuration_id`` with a full tool dict
+        in ``entry.tool``."""
+        joined_entries = []
+
+        for entry in entries:
+            # get the tool used to generate this addition
+            tool_id = entry.indexer_configuration_id
+            assert tool_id
+            tool = self._tools[tool_id]
+            entry = attr.evolve(
+                entry,
+                tool={
+                    "name": tool["tool_name"],
+                    "version": tool["tool_version"],
+                    "configuration": tool["tool_configuration"],
+                },
+                indexer_configuration_id=None,
+            )
+
+            joined_entries.append(entry)
+
+        return joined_entries
+
     def _key_from_dict(self, d) -> Tuple:
         """Like the global _key_from_dict, but filters out dict keys that don't
         belong in the unique key."""
         return _key_from_dict({k: d[k] for k in self.row_class.UNIQUE_KEY_FIELDS})
 
     def missing(self, keys: Iterable[Dict]) -> List[Sha1]:
         """List data missing from storage.
@@ -206,47 +232,39 @@
               - **id**: sha1
               - **indexer_configuration_id**: tool used to compute the
                 results
               - arbitrary data
 
         """
         data = list(data)
-        check_id_duplicates(data)
+        data_with_tools = self._join_indexer_configuration(data)
+        check_id_duplicates(data_with_tools)
         object_type = self.row_class.object_type  # type: ignore
-        self._journal_writer.write_additions(object_type, data)
+        self._journal_writer.write_additions(object_type, data_with_tools)
         count = 0
-        for obj in data:
+        for (obj, obj_with_tool) in zip(data, data_with_tools):
             item = obj.to_dict()
             id_ = item.pop("id")
             tool_id = item["indexer_configuration_id"]
-            key = _key_from_dict(obj.unique_key())
+            key = _key_from_dict(obj_with_tool.unique_key())
             self._data[id_][key] = item
             self._tools_per_id[id_].add(tool_id)
             count += 1
             if id_ not in self._sorted_ids:
                 self._sorted_ids.add(id_)
         return count
 
 
 class IndexerStorage:
     """In-memory SWH indexer storage."""
 
     def __init__(self, journal_writer=None):
         self._tools = {}
 
-        def tool_getter(id_):
-            tool = self._tools[id_]
-            return {
-                "id": tool["id"],
-                "name": tool["tool_name"],
-                "version": tool["tool_version"],
-                "configuration": tool["tool_configuration"],
-            }
-
-        self.journal_writer = JournalWriter(tool_getter, journal_writer)
+        self.journal_writer = JournalWriter(journal_writer)
         args = (self._tools, self.journal_writer)
         self._mimetypes = SubStorage(ContentMimetypeRow, *args)
         self._licenses = SubStorage(ContentLicenseRow, *args)
         self._content_metadata = SubStorage(ContentMetadataRow, *args)
         self._directory_intrinsic_metadata = SubStorage(
             DirectoryIntrinsicMetadataRow, *args
         )
```

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/interface.py` & `swh.indexer-2.9.3/swh/indexer/storage/interface.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/metrics.py` & `swh.indexer-2.9.3/swh/indexer/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/storage/model.py` & `swh.indexer-2.9.3/swh/indexer/storage/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 # See top-level LICENSE file for more information
 
 """Classes used internally by the in-memory idx-storage, and will be
 used for the interface of the idx-storage in the near future."""
 
 from __future__ import annotations
 
+import json
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 import attr
 from typing_extensions import Final
 
 from swh.model.model import Sha1Git, dictify
 
 TSelf = TypeVar("TSelf")
 
 
 @attr.s
 class BaseRow:
-    UNIQUE_KEY_FIELDS: Tuple = ("id", "indexer_configuration_id")
+    UNIQUE_KEY_FIELDS: Tuple = ("id",)
 
     id = attr.ib(type=Any)
     indexer_configuration_id = attr.ib(type=Optional[int], default=None, kw_only=True)
     tool = attr.ib(type=Optional[Dict], default=None, kw_only=True)
 
     def __attrs_post_init__(self):
         if self.indexer_configuration_id is None and self.tool is None:
@@ -51,38 +52,47 @@
         return d
 
     @classmethod
     def from_dict(cls: Type[TSelf], d) -> TSelf:
         return cls(**d)
 
     def unique_key(self) -> Dict:
-        obj = self
-
-        # tool["id"] and obj.indexer_configuration_id are the same value, but
-        # only one of them is set for any given object
-        if obj.indexer_configuration_id is None:
-            assert obj.tool  # constructors ensures tool XOR indexer_configuration_id
-            obj = attr.evolve(obj, indexer_configuration_id=obj.tool["id"], tool=None)
+        if not self.tool:
+            raise ValueError(
+                f"Cannot compute unique_key of {self.__class__.__name__} with no tool "
+                f"dictionary (indexer_configuration_id was given instead)"
+            )
 
-        return {key: getattr(obj, key) for key in self.UNIQUE_KEY_FIELDS}
+        tool_dict = {
+            "tool_name": self.tool["name"],
+            "tool_version": self.tool["version"],
+            "tool_configuration": json.dumps(
+                self.tool["configuration"], sort_keys=True
+            ),
+        }
+
+        return {
+            **{key: getattr(self, key) for key in self.UNIQUE_KEY_FIELDS},
+            **tool_dict,
+        }
 
 
 @attr.s
 class ContentMimetypeRow(BaseRow):
     object_type: Final = "content_mimetype"
 
     id = attr.ib(type=Sha1Git)
     mimetype = attr.ib(type=str)
     encoding = attr.ib(type=str)
 
 
 @attr.s
 class ContentLicenseRow(BaseRow):
     object_type: Final = "content_fossology_license"
-    UNIQUE_KEY_FIELDS = ("id", "indexer_configuration_id", "license")
+    UNIQUE_KEY_FIELDS = ("id", "license")
 
     id = attr.ib(type=Sha1Git)
     license = attr.ib(type=str)
 
 
 @attr.s
 class ContentMetadataRow(BaseRow):
```

### Comparing `swh.indexer-2.9.1/swh/indexer/tasks.py` & `swh.indexer-2.9.3/swh/indexer/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/conftest.py` & `swh.indexer-2.9.3/swh/indexer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_cff.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_cff.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_codemeta.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_composer.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_composer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_dart.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_dart.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_gitea.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_gitea.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_github.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_github.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_maven.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_maven.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_npm.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_nuget.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_nuget.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_python.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_python.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/metadata_dictionary/test_ruby.py` & `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_ruby.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/conftest.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/generate_data_test.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/generate_data_test.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_converters.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_in_memory.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_init.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_metrics.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_server.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/storage/test_storage.py` & `swh.indexer-2.9.3/swh/indexer/tests/storage/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,23 @@
     DirectoryIntrinsicMetadataRow,
     OriginExtrinsicMetadataRow,
     OriginIntrinsicMetadataRow,
 )
 from swh.model.hashutil import hash_to_bytes
 
 
+def _remove_tool_ids(rows):
+    results = []
+    for row in rows:
+        tool = dict(row.tool)
+        del tool["id"]
+        results.append(attr.evolve(row, tool=tool))
+    return results
+
+
 def prepare_mimetypes_from_licenses(
     fossology_licenses: List[ContentLicenseRow],
 ) -> List[ContentMimetypeRow]:
     """Fossology license needs some consistent data in db to run."""
     mimetypes = []
     for c in fossology_licenses:
         mimetypes.append(
@@ -354,19 +363,21 @@
             self.row_class.from_dict(
                 {"id": data.sha1_2, **self.example_data[0], "tool": tool}
             )
         ]
 
         assert actual_data == expected_data
 
+        expected_journal_data = _remove_tool_ids(expected_data)
+
         journal_objects = storage.journal_writer.journal.objects  # type: ignore
         actual_journal_data = [
             obj for (obj_type, obj) in journal_objects if obj_type == self.endpoint_type
         ]
-        assert list(sorted(actual_journal_data)) == list(sorted(expected_data))
+        assert list(sorted(actual_journal_data)) == list(sorted(expected_journal_data))
 
 
 class TestIndexerStorageContentMimetypes(StorageETypeTester):
     """Test Indexer Storage content_mimetype related methods"""
 
     endpoint_type = "content_mimetype"
     tool_name = "file"
@@ -570,19 +581,21 @@
                     "tool": tool,
                 }
             )
         ]
 
         assert actual_data in (expected_data_postgresql, expected_data_verbatim)
 
+        expected_journal_data = _remove_tool_ids(expected_data_verbatim)
+
         journal_objects = storage.journal_writer.journal.objects  # type: ignore
         actual_journal_data = [
             obj for (obj_type, obj) in journal_objects if obj_type == self.endpoint_type
         ]
-        assert list(sorted(actual_journal_data)) == list(sorted(expected_data_verbatim))
+        assert list(sorted(actual_journal_data)) == list(sorted(expected_journal_data))
 
 
 class TestIndexerStorageDirectoryIntrinsicMetadata(StorageETypeTester):
     """Test Indexer Storage directory_intrinsic_metadata related methods"""
 
     tool_name = "swh-metadata-detector"
     endpoint_type = "directory_intrinsic_metadata"
@@ -908,21 +921,25 @@
                 from_directory=data.directory_id_2,
                 mappings=["mapping1"],
             )
         ]
 
         assert actual_metadata == expected_metadata
 
+        expected_journal_metadata = _remove_tool_ids(expected_metadata)
+
         journal_objects = storage.journal_writer.journal.objects  # type: ignore
         actual_journal_metadata = [
             obj
             for (obj_type, obj) in journal_objects
             if obj_type == "origin_intrinsic_metadata"
         ]
-        assert list(sorted(actual_journal_metadata)) == list(sorted(expected_metadata))
+        assert list(sorted(actual_journal_metadata)) == list(
+            sorted(expected_journal_metadata)
+        )
 
     def test_origin_intrinsic_metadata_add_update_in_place_duplicate(
         self, swh_indexer_storage_with_data: Tuple[IndexerStorageInterface, Any]
     ) -> None:
         storage, data = swh_indexer_storage_with_data
         # given
         tool_id = data.tools["swh-metadata-detector"]["id"]
@@ -1523,21 +1540,25 @@
                 from_remd_id=b"\x02" * 20,
                 mappings=["mapping1"],
             )
         ]
 
         assert actual_metadata == expected_metadata
 
+        expected_journal_metadata = _remove_tool_ids(expected_metadata)
+
         journal_objects = storage.journal_writer.journal.objects  # type: ignore
         actual_journal_metadata = [
             obj
             for (obj_type, obj) in journal_objects
             if obj_type == "origin_extrinsic_metadata"
         ]
-        assert list(sorted(actual_journal_metadata)) == list(sorted(expected_metadata))
+        assert list(sorted(actual_journal_metadata)) == list(
+            sorted(expected_journal_metadata)
+        )
 
     def test_origin_extrinsic_metadata_add_update_in_place_duplicate(
         self, swh_indexer_storage_with_data: Tuple[IndexerStorageInterface, Any]
     ) -> None:
         storage, data = swh_indexer_storage_with_data
         # given
         tool_id = data.tools["swh-metadata-detector"]["id"]
```

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/tasks.py` & `swh.indexer-2.9.3/swh/indexer/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_cli.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_codemeta.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_fossology_license.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_fossology_license.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_indexer.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_journal_client.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_metadata.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_mimetype.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_mimetype.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_origin_head.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_origin_head.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/test_origin_metadata.py` & `swh.indexer-2.9.3/swh/indexer/tests/test_origin_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/utils.py` & `swh.indexer-2.9.3/swh/indexer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh/indexer/tests/zz_celery/test_tasks.py` & `swh.indexer-2.9.3/swh/indexer/tests/zz_celery/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/swh.indexer.egg-info/PKG-INFO` & `swh.indexer-2.9.3/swh.indexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.indexer
-Version: 2.9.1
+Version: 2.9.3
 Summary: Software Heritage Content Indexer
 Home-page: https://forge.softwareheritage.org/diffusion/78/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-indexer
```

### Comparing `swh.indexer-2.9.1/swh.indexer.egg-info/SOURCES.txt` & `swh.indexer-2.9.3/swh.indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.1/tox.ini` & `swh.indexer-2.9.3/tox.ini`

 * *Files identical despite different names*

