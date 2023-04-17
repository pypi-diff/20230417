# Comparing `tmp/lmql-0.0.4.2.tar.gz` & `tmp/lmql-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.4.2.tar", last modified: Thu Apr 13 08:25:21 2023, max compression
+gzip compressed data, was "lmql-0.0.5.tar", last modified: Mon Apr 17 14:49:12 2023, max compression
```

## Comparing `lmql-0.0.4.2.tar` & `lmql-0.0.5.tar`

### file list

```diff
@@ -1,239 +1,230 @@
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.234514 lmql-0.0.4.2/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.079098 lmql-0.0.4.2/.github/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.094689 lmql-0.0.4.2/.github/workflows/
--rw-r--r--   0 luca       (501) staff       (20)     1659 2023-04-09 19:01:32.000000 lmql-0.0.4.2/.github/workflows/lmql-web.yml
--rw-r--r--   0 luca       (501) staff       (20)     2701 2023-04-13 08:24:53.000000 lmql-0.0.4.2/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)    12820 2023-04-09 19:01:32.000000 lmql-0.0.4.2/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)      140 2023-04-09 19:01:32.000000 lmql-0.0.4.2/MANIFEST.in
--rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-13 08:25:21.234813 lmql-0.0.4.2/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     4214 2023-04-09 19:01:32.000000 lmql-0.0.4.2/README.md
--rw-r--r--   0 luca       (501) staff       (20)       75 2023-04-09 19:01:32.000000 lmql-0.0.4.2/TODO.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.097084 lmql-0.0.4.2/docs/
--rw-r--r--   0 luca       (501) staff       (20)      638 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/Makefile
--rw-r--r--   0 luca       (501) staff       (20)      444 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/RELEASE.md
--rw-r--r--   0 luca       (501) staff       (20)      799 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/make.bat
--rw-r--r--   0 luca       (501) staff       (20)       81 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/requirements.txt
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.101126 lmql-0.0.4.2/docs/source/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.101675 lmql-0.0.4.2/docs/source/_ext/
--rw-r--r--   0 luca       (501) staff       (20)     5526 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_ext/lmql_snippets.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.080299 lmql-0.0.4.2/docs/source/_static/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.102258 lmql-0.0.4.2/docs/source/_static/css/
--rw-r--r--   0 luca       (501) staff       (20)     5777 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_static/css/lmql-docs.css
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.102849 lmql-0.0.4.2/docs/source/_static/images/
--rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/_static/images/lmql.svg
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.103384 lmql-0.0.4.2/docs/source/_static/js/
--rw-r--r--   0 luca       (501) staff       (20)     2191 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/_static/js/lmql-playground.js
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.103920 lmql-0.0.4.2/docs/source/_templates/
--rw-r--r--   0 luca       (501) staff       (20)      292 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/_templates/layout.html
--rw-r--r--   0 luca       (501) staff       (20)     1167 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/conf.py
--rw-r--r--   0 luca       (501) staff       (20)     1293 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/dev-setup.md
--rw-r--r--   0 luca       (501) staff       (20)     2709 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/index.rst
--rw-r--r--   0 luca       (501) staff       (20)     2484 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/installation.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.107305 lmql-0.0.4.2/docs/source/language/
--rw-r--r--   0 luca       (501) staff       (20)     7435 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/constraints.md
--rw-r--r--   0 luca       (501) staff       (20)     4067 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/decoders.md
--rw-r--r--   0 luca       (501) staff       (20)     7850 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/functions.md
--rw-r--r--   0 luca       (501) staff       (20)     6566 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/models.md
--rw-r--r--   0 luca       (501) staff       (20)     8511 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/overview.md
--rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/language/scripted_prompts.md
--rw-r--r--   0 luca       (501) staff       (20)     3675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/lmql.svg
--rw-r--r--   0 luca       (501) staff       (20)    28444 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/logo.png
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.109818 lmql-0.0.4.2/docs/source/python/
--rw-r--r--   0 luca       (501) staff       (20)       11 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)    10629 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/langchain.ipynb
--rw-r--r--   0 luca       (501) staff       (20)    75148 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/python/lmql.txt
--rw-r--r--   0 luca       (501) staff       (20)     8583 2023-04-13 08:24:53.000000 lmql-0.0.4.2/docs/source/python/python.ipynb
--rw-r--r--   0 luca       (501) staff       (20)     3135 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/source/quickstart.md
--rw-r--r--   0 luca       (501) staff       (20)      257 2023-04-09 19:01:32.000000 lmql-0.0.4.2/docs/todo.md
--rw-r--r--   0 luca       (501) staff       (20)      137 2023-04-09 19:01:32.000000 lmql-0.0.4.2/pyproject.toml
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-09 19:01:32.000000 lmql-0.0.4.2/requirements.txt
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.111757 lmql-0.0.4.2/scripts/
--rw-r--r--   0 luca       (501) staff       (20)      295 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/activate-dev.sh
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.113294 lmql-0.0.4.2/scripts/conda/
--rw-r--r--   0 luca       (501) staff       (20)      209 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/conda/requirements-no-gpu.yml
--rw-r--r--   0 luca       (501) staff       (20)      343 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/conda/requirements.yml
--rw-r--r--   0 luca       (501) staff       (20)      486 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/pypi-release.sh
--rw-r--r--   0 luca       (501) staff       (20)      817 2023-04-09 19:01:32.000000 lmql-0.0.4.2/scripts/wheel.sh
--rw-r--r--   0 luca       (501) staff       (20)      828 2023-04-13 08:25:21.235930 lmql-0.0.4.2/setup.cfg
--rw-r--r--   0 luca       (501) staff       (20)       37 2023-04-09 19:01:32.000000 lmql-0.0.4.2/setup.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.081673 lmql-0.0.4.2/src/
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.116199 lmql-0.0.4.2/src/lmql/
--rw-r--r--   0 luca       (501) staff       (20)     4985 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/__init__.py
--rwxr-xr-x   0 luca       (501) staff       (20)     7337 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/cli.py
--rw-r--r--   0 luca       (501) staff       (20)     1577 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/demo.py
--rw-r--r--   0 luca       (501) staff       (20)     1229 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/http.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.126283 lmql-0.0.4.2/src/lmql/language/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    18943 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/language/compiler.py
--rw-r--r--   0 luca       (501) staff       (20)    10194 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/fragment_parser.py
--rw-r--r--   0 luca       (501) staff       (20)      979 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/qstrings.py
--rw-r--r--   0 luca       (501) staff       (20)     1804 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/language/validator.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.129484 lmql-0.0.4.2/src/lmql/lib/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)      775 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/errors.py
--rw-r--r--   0 luca       (501) staff       (20)      810 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/expr_jitter.py
--rw-r--r--   0 luca       (501) staff       (20)     1998 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/scope.py
--rw-r--r--   0 luca       (501) staff       (20)      495 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/lib/state.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.134975 lmql-0.0.4.2/src/lmql/model/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    24608 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/async_generation_utils.py
--rw-r--r--   0 luca       (501) staff       (20)    12601 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/client.py
--rw-r--r--   0 luca       (501) staff       (20)    17716 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/hf_beam_search.py
--rw-r--r--   0 luca       (501) staff       (20)     1299 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/local_client.py
--rw-r--r--   0 luca       (501) staff       (20)    17134 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/model/serve.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.137285 lmql-0.0.4.2/src/lmql/ops/
--rw-r--r--   0 luca       (501) staff       (20)       93 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     7565 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/follow_map.py
--rw-r--r--   0 luca       (501) staff       (20)    32961 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ops/ops.py
--rw-r--r--   0 luca       (501) staff       (20)    15564 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ops/token_set.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.148146 lmql-0.0.4.2/src/lmql/runtime/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     2554 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/backtracker.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.150270 lmql-0.0.4.2/src/lmql/runtime/bopenai/
--rw-r--r--   0 luca       (501) staff       (20)     1863 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    25702 2023-04-13 08:25:04.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/batched_openai.py
--rw-r--r--   0 luca       (501) staff       (20)    17000 2023-04-09 20:15:19.000000 lmql-0.0.4.2/src/lmql/runtime/bopenai/openai_api.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.154659 lmql-0.0.4.2/src/lmql/runtime/dclib/
--rw-r--r--   0 luca       (501) staff       (20)      467 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)    18632 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_array.py
--rw-r--r--   0 luca       (501) staff       (20)      538 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_global.py
--rw-r--r--   0 luca       (501) staff       (20)    23530 2023-04-10 21:23:08.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_model.py
--rw-r--r--   0 luca       (501) staff       (20)    28796 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_seq.py
--rw-r--r--   0 luca       (501) staff       (20)    20610 2023-04-10 21:23:36.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/decoders.py
--rw-r--r--   0 luca       (501) staff       (20)    10602 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/lmql_adapter.py
--rw-r--r--   0 luca       (501) staff       (20)     4138 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/dclib/trie_cache.py
--rw-r--r--   0 luca       (501) staff       (20)     3037 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/decoder_head.py
--rw-r--r--   0 luca       (501) staff       (20)     5056 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/hf_integration.py
--rw-r--r--   0 luca       (501) staff       (20)      250 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/interrupt.py
--rw-r--r--   0 luca       (501) staff       (20)     1084 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/langchain.py
--rw-r--r--   0 luca       (501) staff       (20)     5806 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/lmql_runtime.py
--rw-r--r--   0 luca       (501) staff       (20)     1186 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/maiohttp.py
--rw-r--r--   0 luca       (501) staff       (20)      732 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/model_registry.py
--rw-r--r--   0 luca       (501) staff       (20)     8564 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/multi_head_interpretation.py
--rw-r--r--   0 luca       (501) staff       (20)    44472 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/openai_integration.py
--rw-r--r--   0 luca       (501) staff       (20)     1979 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/openai_secret.py
--rw-r--r--   0 luca       (501) staff       (20)     2086 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/output_writer.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.156890 lmql-0.0.4.2/src/lmql/runtime/postprocessing/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     6163 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-r--r--   0 luca       (501) staff       (20)      203 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/postprocessing/group_by.py
--rw-r--r--   0 luca       (501) staff       (20)     1543 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/program_state.py
--rw-r--r--   0 luca       (501) staff       (20)    36840 2023-04-13 08:04:33.000000 lmql-0.0.4.2/src/lmql/runtime/prompt_interpreter.py
--rw-r--r--   0 luca       (501) staff       (20)     8367 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/rewriter.py
--rw-r--r--   0 luca       (501) staff       (20)       86 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/runtime.py
--rw-r--r--   0 luca       (501) staff       (20)     1123 2023-04-10 20:34:48.000000 lmql-0.0.4.2/src/lmql/runtime/stats.py
--rw-r--r--   0 luca       (501) staff       (20)     2150 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/runtime/tok.ipynb
--rw-r--r--   0 luca       (501) staff       (20)     8312 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/runtime/tokenizer.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.164302 lmql-0.0.4.2/src/lmql/tests/
--rw-r--r--   0 luca       (501) staff       (20)     5015 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/expr_test_utils.py
--rw-r--r--   0 luca       (501) staff       (20)     1611 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/mask_product_test.py
--rw-r--r--   0 luca       (501) staff       (20)     2789 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/monotonicity.py
--rw-r--r--   0 luca       (501) staff       (20)      546 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/one_of_tests.py
--rw-r--r--   0 luca       (501) staff       (20)      758 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/sentences_op.py
--rw-r--r--   0 luca       (501) staff       (20)      984 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/starts_with_op_test.py
--rw-r--r--   0 luca       (501) staff       (20)     1236 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/stops_at.py
--rw-r--r--   0 luca       (501) staff       (20)      537 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/str_in_str_tests.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.165080 lmql-0.0.4.2/src/lmql/tests/system/
--rw-r--r--   0 luca       (501) staff       (20)     3402 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/system/basic_use_cases.py
--rw-r--r--   0 luca       (501) staff       (20)     4738 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/test_multi_head.py
--rw-r--r--   0 luca       (501) staff       (20)     3036 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/tests/token_set_test.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.167874 lmql-0.0.4.2/src/lmql/ui/
--rw-r--r--   0 luca       (501) staff       (20)     6148 2023-04-10 11:59:45.000000 lmql-0.0.4.2/src/lmql/ui/.DS_Store
--rw-r--r--   0 luca       (501) staff       (20)       27 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/__init__.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.171671 lmql-0.0.4.2/src/lmql/ui/live/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     6747 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/live.js
--rw-r--r--   0 luca       (501) staff       (20)     3299 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/live.py
--rw-r--r--   0 luca       (501) staff       (20)     3885 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/livelib.py
--rw-r--r--   0 luca       (501) staff       (20)      349 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/package.json
--rw-r--r--   0 luca       (501) staff       (20)    33701 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/live/yarn.lock
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.177348 lmql-0.0.4.2/src/lmql/ui/playground/
--rw-r--r--   0 luca       (501) staff       (20)       31 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.dockerignore
--rw-r--r--   0 luca       (501) staff       (20)       34 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.env
--rw-r--r--   0 luca       (501) staff       (20)      310 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/.gitignore
--rw-r--r--   0 luca       (501) staff       (20)      354 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/Dockerfile
--rw-r--r--   0 luca       (501) staff       (20)     3359 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/README.md
--rw-r--r--   0 luca       (501) staff       (20)     1327 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/package.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.182529 lmql-0.0.4.2/src/lmql/ui/playground/public/
--rw-r--r--   0 luca       (501) staff       (20)       90 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/_headers
--rw-r--r--   0 luca       (501) staff       (20)     3870 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/favicon.ico
--rw-r--r--   0 luca       (501) staff       (20)     1678 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/index.html
--rw-r--r--   0 luca       (501) staff       (20)     2817 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/lmql.svg
--rw-r--r--   0 luca       (501) staff       (20)      306 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/manifest.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.203625 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/
--rw-r--r--   0 luca       (501) staff       (20)  1227728 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/calc.json
--rw-r--r--   0 luca       (501) staff       (20)   295285 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/chat.json
--rw-r--r--   0 luca       (501) staff       (20)   160153 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/cot.json
--rw-r--r--   0 luca       (501) staff       (20)    81768 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-r--r--   0 luca       (501) staff       (20)     5221 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/hello.json
--rw-r--r--   0 luca       (501) staff       (20)    89531 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/joke.json
--rw-r--r--   0 luca       (501) staff       (20)  1710847 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/kv.json
--rw-r--r--   0 luca       (501) staff       (20)    52748 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/list.json
--rw-r--r--   0 luca       (501) staff       (20)   628184 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/meta.json
--rw-r--r--   0 luca       (501) staff       (20)   264768 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/translation.json
--rw-r--r--   0 luca       (501) staff       (20)   215050 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-r--r--   0 luca       (501) staff       (20)       67 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/robots.txt
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.205833 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/
--rw-r--r--   0 luca       (501) staff       (20)   381736 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-r--r--   0 luca       (501) staff       (20)   252806 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-r--r--   0 luca       (501) staff       (20)       62 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/ref.py
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/run-in-docker.sh
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.222161 lmql-0.0.4.2/src/lmql/ui/playground/src/
--rw-r--r--   0 luca       (501) staff       (20)    67646 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/App.jsx
--rw-r--r--   0 luca       (501) staff       (20)      246 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/App.test.js
--rw-r--r--   0 luca       (501) staff       (20)    29983 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-r--r--   0 luca       (501) staff       (20)      807 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Configuration.js
--rw-r--r--   0 luca       (501) staff       (20)     1174 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DataListView.js
--rw-r--r--   0 luca       (501) staff       (20)    20848 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DecoderGraph.js
--rw-r--r--   0 luca       (501) staff       (20)      329 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/DecodingTree.js
--rw-r--r--   0 luca       (501) staff       (20)       89 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Embed.jsx
--rw-r--r--   0 luca       (501) staff       (20)     9601 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/Explore.jsx
--rw-r--r--   0 luca       (501) staff       (20)      675 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/SharedState.js
--rw-r--r--   0 luca       (501) staff       (20)     3868 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/State.js
--rw-r--r--   0 luca       (501) staff       (20)     5738 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-r--r--   0 luca       (501) staff       (20)     9360 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/browser_process.js
--rw-r--r--   0 luca       (501) staff       (20)     1163 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/build_info.js
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.223378 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/
--rw-r--r--   0 luca       (501) staff       (20)     8673 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-r--r--   0 luca       (501) staff       (20)     4758 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/editor/theme.json
--rw-r--r--   0 luca       (501) staff       (20)      889 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/explore.svg
--rw-r--r--   0 luca       (501) staff       (20)     1345 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/graph-layout.css
--rw-r--r--   0 luca       (501) staff       (20)     1698 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/index.css
--rw-r--r--   0 luca       (501) staff       (20)      489 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/index.js
--rw-r--r--   0 luca       (501) staff       (20)     2632 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/logo.svg
--rw-r--r--   0 luca       (501) staff       (20)     8077 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/queries.js
--rw-r--r--   0 luca       (501) staff       (20)     5990 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/remote_process.js
--rw-r--r--   0 luca       (501) staff       (20)      362 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/reportWebVitals.js
--rw-r--r--   0 luca       (501) staff       (20)     9520 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/screenshot.css
--rw-r--r--   0 luca       (501) staff       (20)      241 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/setupTests.js
--rw-r--r--   0 luca       (501) staff       (20)     3466 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/spinner.svg
--rw-r--r--   0 luca       (501) staff       (20)     2949 2023-04-10 14:55:16.000000 lmql-0.0.4.2/src/lmql/ui/playground/src/tagged-model-result.js
--rw-r--r--   0 luca       (501) staff       (20)   449905 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/playground/yarn.lock
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.229927 lmql-0.0.4.2/src/lmql/ui/vscode/
--rw-r--r--   0 luca       (501) staff       (20)       76 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.gitattributes
--rw-r--r--   0 luca       (501) staff       (20)       19 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.gitignore
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.230695 lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/
--rw-r--r--   0 luca       (501) staff       (20)      540 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/launch.json
--rw-r--r--   0 luca       (501) staff       (20)       66 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/.vscodeignore
--rw-r--r--   0 luca       (501) staff       (20)    12820 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)      357 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/README.md
--rw-r--r--   0 luca       (501) staff       (20)      959 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/language-configuration.json
--rw-r--r--   0 luca       (501) staff       (20)    11532 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/lmql-vscode.png
--rw-r--r--   0 luca       (501) staff       (20)     1214 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/package.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.232551 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/
--rw-r--r--   0 luca       (501) staff       (20)      518 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-r--r--   0 luca       (501) staff       (20)      642 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-r--r--   0 luca       (501) staff       (20)      853 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.234023 lmql-0.0.4.2/src/lmql/utils/
--rw-r--r--   0 luca       (501) staff       (20)        0 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/utils/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     5384 2023-04-13 08:24:53.000000 lmql-0.0.4.2/src/lmql/utils/graph.py
--rw-r--r--   0 luca       (501) staff       (20)     1474 2023-04-09 19:01:32.000000 lmql-0.0.4.2/src/lmql/utils/nputil.py
--rw-r--r--   0 luca       (501) staff       (20)      115 2023-04-13 08:25:13.000000 lmql-0.0.4.2/src/lmql/version.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-04-13 08:25:21.122163 lmql-0.0.4.2/src/lmql.egg-info/
--rw-r--r--   0 luca       (501) staff       (20)     4646 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     6621 2023-04-13 08:25:21.000000 lmql-0.0.4.2/src/lmql.egg-info/SOURCES.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/dependency_links.txt
--rw-r--r--   0 luca       (501) staff       (20)       39 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/entry_points.txt
--rw-r--r--   0 luca       (501) staff       (20)       80 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/requires.txt
--rw-r--r--   0 luca       (501) staff       (20)        5 2023-04-13 08:25:20.000000 lmql-0.0.4.2/src/lmql.egg-info/top_level.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1618 2023-04-17 14:48:56.000000 lmql-0.0.5/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2710 2023-04-17 14:48:56.000000 lmql-0.0.5/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.5/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4644 2023-04-17 14:49:12.881538 lmql-0.0.5/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4214 2023-04-17 14:44:31.000000 lmql-0.0.5/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.5/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.5/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.861538 lmql-0.0.5/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5777 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/_templates/layout.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2709 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6566 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8511 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    13222 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9213 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.5/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.5/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.5/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.5/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.5/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-17 14:48:56.000000 lmql-0.0.5/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-17 14:48:56.000000 lmql-0.0.5/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.5/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.5/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      826 2023-04-17 14:49:12.885538 lmql-0.0.5/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.5/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6700 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     7529 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20390 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17924 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8387 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7565 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    39511 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18023 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1863 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    25946 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17000 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/bopenai/openai_api.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      467 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18632 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27495 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29933 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20646 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27888 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6049 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    43100 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.869538 lmql-0.0.5/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8456 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5011 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/expr_test_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/str_in_str_tests.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2149 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/tests/test_sample_queries.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/tests/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3256 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.873538 lmql-0.0.5/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.877538 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.877538 lmql-0.0.5/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    68636 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20848 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.5/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.881538 lmql-0.0.5/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1882 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      113 2023-04-17 14:49:07.000000 lmql-0.0.5/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-17 14:49:12.865538 lmql-0.0.5/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4644 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6371 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-04-17 14:49:12.000000 lmql-0.0.5/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.5/src/lmql.svg
```

### Comparing `lmql-0.0.4.2/.github/workflows/lmql-web.yml` & `lmql-0.0.5/.github/workflows/lmql-web.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-nodejs
 
 name: Browser Build & Web Deploy
 
 on:
   push:
     branches: [ "main", "updated-web"]
-  pull_request:
-    branches: [ "main" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `lmql-0.0.4.2/.gitignore` & `lmql-0.0.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -165,8 +165,9 @@
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks
 
-wip-snippets
+wip-snippets
+.vscode
```

### Comparing `lmql-0.0.4.2/LICENSE` & `lmql-0.0.5/LICENSE`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,214 @@
-MIT License
+Copyright 2022- The LMQL Language Team. All rights reserved.
 
-Copyright (c) 2023 lmql-lang
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+   1. Definitions.
 
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
 ================================================================================
 
-The project also includes two files adapted from the huggingface/tranformers project:
+The project also includes one file adapted from the huggingface/tranformers project:
 
-- hf_beam_search.py
 - async_generation_utils.py
 
 These files are adapted from their original project and redistributed according to the following license agreement:
 
 Copyright 2018- The Hugging Face team. All rights reserved.
 
                                  Apache License
```

### Comparing `lmql-0.0.4.2/PKG-INFO` & `lmql-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.4.2
+Version: 0.0.5
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.4.2 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.5 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.4.2/README.md` & `lmql-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/Makefile` & `lmql-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/make.bat` & `lmql-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.5/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.5/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/_static/images/lmql.svg` & `lmql-0.0.5/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.5/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/conf.py` & `lmql-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/dev-setup.md` & `lmql-0.0.5/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/index.rst` & `lmql-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/installation.md` & `lmql-0.0.5/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/constraints.md` & `lmql-0.0.5/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/decoders.md` & `lmql-0.0.5/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/functions.md` & `lmql-0.0.5/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/models.md` & `lmql-0.0.5/docs/source/language/models.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/overview.md` & `lmql-0.0.5/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/language/scripted_prompts.md` & `lmql-0.0.5/docs/source/language/scripted_prompts.md`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
 # print output: \['A good pair of blue/gel saskaers', 'A good sun tanner', 'A good air freshener', 'A good spot forwashing your hands', 'A good spot for washing your feet'\]
 ```
 
 Because we decode our list `THING` by `THING`, we can easily access the individual items, without having to think about parsing or validation. We just add them to a `backpack` list of things, which we then can process further.
 
 ## Python Compatibility
 
-Going beyond simple control flow, LMQL supports most valid Python constructs in the prompt clause of a query, where top-level strings like `"-[THING]"` are automatically interpreted as model input and template variables are assigned accordingly. For more advanced usage, also see the [External Functions](functions.md) chaptor.
+Going beyond simple control flow, LMQL supports most valid Python constructs in the prompt clause of a query, where top-level strings like `"-[THING]"` are automatically interpreted as model input and template variables are assigned accordingly. For more advanced usage, also see the [External Functions](functions.md) chapter.
```

### Comparing `lmql-0.0.4.2/docs/source/lmql.svg` & `lmql-0.0.5/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/logo.png` & `lmql-0.0.5/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/python/langchain.ipynb` & `lmql-0.0.5/docs/source/python/langchain.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936320515422078%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}, 8: {delete: ['attachments']}, 9: {'execution_count': "*

 * *            "4, 'outputs': {0: {'text': {insert: [(0, '\\\\nQuestion: What is LMQL?\\n'), (2, "*

 * *            "'LMQL stands for Language Model Query Language. It is a high-level query language for "*

 * *            'Language Models (LMs) that allows for scripted prompting and has declarative SQL-like '*

 * *            'elements with an imperative syntax. LMQL is known for its great expressiveness, which '*

 * *            'a […]*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# LangChain Integration \ud83e\udd9c\ud83d\udd17 "
             ]
         },
         {
@@ -87,48 +86,59 @@
                 "\n",
                 "embeddings = OpenAIEmbeddings()\n",
                 "docsearch = Chroma.from_texts(texts, embeddings, \n",
                 "    metadatas=[{\"text\": t} for t in texts], persist_directory=\"lmql-index\")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We then construct a chatbot function, using a simple LMQL query, that first prompts the user for a question via `await input(...)`, retrieves relevant text paragraphs using LangChain and then produces an answer using `openai/gpt-3.5-turbo` (ChatGPT)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\n",
-                        "Question: What is LMQL?\n",
+                        "\\nQuestion: What is LMQL?\n",
                         "\u001b[32mReading relevant pages...\u001b[0m\n",
-                        "LMQL stands for Language Model Query Language. It is a high-level language with declarative SQL-like elements and an imperative syntax for querying language models. LMQL allows for great expressiveness and supports scripted prompting and just a set of high-level constraints. It has been evaluated comprehensively and shown to be able to express a wide range of techniques."
+                        "LMQL stands for Language Model Query Language. It is a high-level query language for Language Models (LMs) that allows for scripted prompting and has declarative SQL-like elements with an imperative syntax. LMQL is known for its great expressiveness, which allows for several approaches from current state-of-the-art methods to be directly expressed.\\nQuestion: Who are you?\n",
+                        "\u001b[32mReading relevant pages...\u001b[0m\n",
+                        "I am a chatbot designed to help users answer questions. The person who addressed the question of who I am is not provided in the relevant information.\\nQuestion: exit\n"
                     ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "[LMQLResult(prompt='You are a chatbot that helps users answer questions.\\nYou are first provided with the question and relevant information.Question: What is LMQL?\\n   \\n   Relevant Information: ...just a set of high-level constraints (Section 5).\\n\u2022 A comprehensive evaluation of LMQL that shows how to express a wide ...\\\\n\\\\n...techniques (Section 2).\\n\u2022 LMQL, an efficient, high-level query language for LMs with support for scripted prompting and ...\\\\n\\\\n...hat: i) LMQL allows great expressiveness, i.e. several approaches from current state-of-the-art methods can be directly ...\\\\n\\\\n...Model Query Language (LMQL). LMQL is a high-level language with declarative SQL-like elements and an imperative syntax f...\\n   Your response based on relevant information: LMQL stands for Language Model Query Language. It is a high-level query language for Language Models (LMs) that allows for scripted prompting and has declarative SQL-like elements with an imperative syntax. LMQL is known for its great expressiveness, which allows for several approaches from current state-of-the-art methods to be directly expressed.Question: Who are you?\\n   \\n   Relevant Information: ...erson to answer this question is                    .\\nIndeed,                     addressed this question:\\nPrompt 1 LM c...\\\\n\\\\n...y.\\n\u2022 a physicist, like Thomas Kugler at UC Irvine or one of the other physicists working with NASA \u2026\\n\u2022 a man named David...\\\\n\\\\n...rer-kellner@inf.ethz.ch\\nMarc Fischer\\nETH ZurichSwitzerland\\nmarc.fischer@inf.ethz.ch\\nMartin Vechev\\nETH ZurichSwitzerland\\n...\\\\n\\\\n...son\\n\u2022 William O\u2019Malley, who has a PhD in Geodesy and is a professor at Colorado State University.\\n\u2022 the person having th...\\n   Your response based on relevant information: I am a chatbot designed to help users answer questions. The person who addressed the question of who I am is not provided in the relevant information.', variables={'RESPONSE': ' I am a chatbot designed to help users answer questions. The person who addressed the question of who I am is not provided in the relevant information.'}, distribution_variable=None, distribution_values=None)]"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import termcolor\n",
                 "\n",
                 "@lmql.query\n",
                 "async def chatbot():\n",
                 "        '''\n",
                 "sample(temperature=0.2, max_len=2048, openai_chunksize=2048)\n",
                 "    \"\"\"You are a chatbot that helps users answer questions.\n",
                 "    You are first provided with the question and relevant information.\"\"\"\n",
                 "    while True:\n",
                 "        q = await input(\"\\\\nQuestion: \")\n",
+                "        if q == \"exit\": break\n",
                 "        \"Question: {q}\\\\n\"\n",
                 "        print(termcolor.colored(\"Reading relevant pages...\", \"green\"))\n",
                 "        results = set([d.page_content for d in docsearch.similarity_search(q, 4)])\n",
                 "        information = \"\\\\n\\\\n\".join([\"...\" + r + \"...\" for r in list(results)])\n",
                 "        \"\\\\nRelevant Information: {information}\\\\n\"\n",
                 "        \"Your response based on relevant information:[RESPONSE]\"\n",
                 "from\n",
@@ -161,15 +171,15 @@
                 "For this consider, the sequential prompting example from the `langchain` documentation, where we first prompt the language model to propose a company name for a given product, and then ask it for a catchphrase.\n",
                 "\n",
                 "To get started, we first import the relevant langchain components, as well as LMQL."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain import LLMChain, PromptTemplate\n",
                 "from langchain.chat_models import ChatOpenAI\n",
                 "from langchain.prompts.chat import (ChatPromptTemplate,HumanMessagePromptTemplate)\n",
                 "from langchain.llms import OpenAI\n",
@@ -184,15 +194,15 @@
                 "Our chain has two stages: (1) Asking the model for a company name, and (2) asking the model for a catchphrase. For the sake of this example, we will implement (1) in with a langchain prompt and (2) with an LMQL query. \n",
                 "\n",
                 "First, we define the langchain prompt for the company name and instantiate the resulting `LLMChain`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# setup the LM to be used by langchain\n",
                 "llm = OpenAI(temperature=0.9)\n",
                 "\n",
                 "human_message_prompt = HumanMessagePromptTemplate(\n",
@@ -211,24 +221,24 @@
             "metadata": {},
             "source": [
                 "This can already be executed to produce a company name:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'Rainbow Sock Co.'"
+                            "'Rainbow Socks Co.'"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "chain.run(\"colorful socks\")"
             ]
@@ -238,62 +248,62 @@
             "metadata": {},
             "source": [
                 "Next, we define prompt (2) in LMQL, i.e. the LMQL query generating the catchphrase:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@lmql.query\n",
                 "async def write_catch_phrase(company_name: str):\n",
                 "    '''\n",
-                "    argmax \"Write a catchphrase for the following company: {company_name}. [CATCHPHRASE]\" from \"chatgpt\"\n",
+                "    argmax \"Write a catchphrase for the following company: {company_name}. [catchphrase]\" from \"chatgpt\"\n",
                 "    '''"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Again, we can run this part in isolation, like so:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "' \"Step up your style with Socks Inc.\"'"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "(await write_catch_phrase(\"Socks Inc\"))[0].variables[\"CATCHPHRASE\"]"
+                "(await write_catch_phrase(\"Socks Inc\"))[0].variables[\"catchphrase\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To chain the two prompts together, we can use a `SimpleSequentialChain` from `langchain`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain.chains import SimpleSequentialChain\n",
                 "overall_chain = SimpleSequentialChain(chains=[chain, write_catch_phrase], verbose=True)"
             ]
         },
```

### Comparing `lmql-0.0.4.2/docs/source/python/lmql.txt` & `lmql-0.0.5/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/docs/source/python/python.ipynb` & `lmql-0.0.5/docs/source/python/python.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989671910430839%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(8, '%autoreload 2\\n'), (9, '\\n'), (10, '# disable logit "*

 * *            "bias logging\\n'), (11, 'import lmql.runtime.bopenai.batched_openai as "*

 * *            "batched_openai\\n'), (12, 'batched_openai.set_logit_bias_logging(False)')], delete: "*

 * *            "[8]}}, 4: {'source': {insert: [(3, 'async def hello(): \\n'), (4, '    "*

 * *            '"""\\n\'), (5, \'    argmax \\n\'), (6, \'        "Hello[WHO]" \\n\'), (7, \'    from '*

 * *            '\\n\'), (8, \'        "opena […]*

```diff
@@ -20,15 +20,19 @@
                 "import sys \n",
                 "sys.path.append(\"../../../src/\")\n",
                 "# load and set OPENAI_API_KEY\n",
                 "import os \n",
                 "os.environ[\"OPENAI_API_KEY\"] = open(\"../../../api.env\").read().split(\"\\n\")[1].split(\": \")[1].strip()\n",
                 "\n",
                 "%load_ext autoreload\n",
-                "%autoreload 2"
+                "%autoreload 2\n",
+                "\n",
+                "# disable logit bias logging\n",
+                "import lmql.runtime.bopenai.batched_openai as batched_openai\n",
+                "batched_openai.set_logit_bias_logging(False)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -61,42 +65,47 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import lmql\n",
                 "\n",
                 "@lmql.query\n",
-                "async def hello():\n",
-                "    '''\n",
-                "    argmax \"Hello[WHO]\" from \"openai/text-ada-001\" where len(WHO) < 10\n",
-                "    '''\n",
+                "async def hello(): \n",
+                "    \"\"\"\n",
+                "    argmax \n",
+                "        \"Hello[WHO]\" \n",
+                "    from \n",
+                "        \"openai/text-ada-001\" \n",
+                "    where \n",
+                "        len(WHO) < 10\n",
+                "    \"\"\"\n",
                 "\n",
                 "(await hello())[0].prompt"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Asynchronous API** LMQL implements a fully asynchronous API. This means that all LMQL queries are executed asynchronously, and return a `Future` object. To execute a query, you therefore have to use the `await` keyword as shown above. By relying on the `asyncio` library, LMQL also supports the execution of arbitrary many queries in parallel, using `asyncio.gather`, where on the backend the runtime will automatically optimize and schedule the queries to maximize throughput (e.g. auto batching across multiple queries).\n",
                 "\n",
-                "**Result Type** An LMQL query that is executed in a Python context, always returns a list of `LMQLResult` objects, where the length is determined by the underlying decoding algorithm (e.g. `n` with `beam(n=n)`). The `LMQLResult` object is a simple dataclass with the following fields:\n",
+                "**Result Type** An LMQL query that is executed in a Python context, always returns a list of `LMQLResult` objects, where the number of elements is determined by the underlying decoding algorithm (e.g. `n` with `beam(n=n)`). The `LMQLResult` object is a simple dataclass with the following fields:\n",
                 "\n",
                 "```python\n",
                 "class LMQLResult:\n",
                 "    # full prompt with all variables substituted\n",
                 "    prompt: str \n",
                 "    # a dictionary of all assigned template variable values\n",
                 "    variables: Dict[str, str] \n",
                 "```\n",
                 "\n",
-                "From such a result object, you can easily extract the prompt and the assigned variable values, no need for any further processing. For `distribution` variables (cf. [Distribution Clause](../language/overview.md#extracting-more-information-with-distributions)), the `variables` dictionary will additionally contain `log P(VAR)` and `P(VAR)` entries, allowing users to easily extract the probability of the assigned value.\n",
+                "From such a result object, you can easily extract the prompt and the assigned variable values, no need for further processing. For `distribution` variables (cf. [Distribution Clause](../language/overview.md#extracting-more-information-with-distributions)), the `variables` dictionary will additionally contain `log P(VAR)` and `P(VAR)` entries, allowing users to easily extract the probability of the assigned value.\n",
                 "\n",
-                "`@lmql.query` functions like `hello()`, also conform to the interface required by the `langchain` library, as detailed in the [LangChain Integration](./langchain.ipynb#Using-LMQL-from-LangChain) chapter."
+                "`@lmql.query` functions like `hello()` also conform to the interface required by the `langchain` library, as detailed in the [LangChain Integration](./langchain.ipynb#Using-LMQL-from-LangChain) chapter."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -194,14 +203,22 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "> **Escaping**: When embedding LMQL code in Python, make sure to always use double-escaped special characters like `\\\\n`. Single escaped characters (e.g. just `\\n`) will always be interpreted literally the query code and therefore lead to parser errors. "
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "This capability of calling arbitrary program logic during query execution, enables powerful use cases like the integration of retrieval, as discussed in the [LangChain Integration](./langchain.ipynb) chapter."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `lmql-0.0.4.2/docs/source/quickstart.md` & `lmql-0.0.5/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/scripts/wheel.sh` & `lmql-0.0.5/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/setup.cfg` & `lmql-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.4.2
+version = 0.0.5
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.4.2/src/lmql/__init__.py` & `lmql-0.0.5/src/lmql/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import lmql.version as version_info
-from lmql.runtime.lmql_runtime import LMQLInputVariableScope
 
 """
 lmql.
 
 A query language for language models.
 """
 
 __version__ = version_info.version
 __author__ = 'Luca Beurer-Kellner, Marc Fischer and Mark Mueller'
 __email__ = "luca.beurer-kellner@inf.ethz.ch"
 __license__ = "MIT"
 
-from lmql.language.compiler import LMQLCompiler
-import lmql.runtime.lmql_runtime as lmql_runtime
+import os
 import tempfile
-from lmql.runtime.output_writer import silent, stream, printing
-from lmql.runtime.model_registry import LMQLModelRegistry
-from lmql.runtime.lmql_runtime import LMQLQueryFunction, FunctionContext
 
+import lmql.runtime.lmql_runtime as lmql_runtime
 import lmql.runtime.lmql_runtime as runtime_support
-
+from lmql.language.compiler import LMQLCompiler
 # re-export lmql runtime functions
-from lmql.runtime.lmql_runtime import compiled_query, tag
-
-import os
+from lmql.runtime.lmql_runtime import (FunctionContext, LMQLInputVariableScope,
+                                       LMQLQueryFunction, compiled_query, tag)
+from lmql.runtime.model_registry import LMQLModelRegistry
+from lmql.runtime.output_writer import headless, printing, silent, stream
 
 model_registry = LMQLModelRegistry
 
 def connect(server="http://localhost:8080", model_name="EleutherAI/gpt-j-6B"):
     from lmql.runtime.hf_integration import transformers_model
 
     Model = transformers_model(server, model_name)
@@ -36,15 +33,15 @@
     lmql_runtime.register_model("*", Model)
 
 def _autoconnect_model(model_name):
     if model_name.startswith("openai/"):
         from lmql.runtime.openai_integration import openai_model
 
         # hard-code openai/ namespace to be openai-API-based
-        Model = openai_model(model_name)
+        Model = openai_model(model_name[7:])
         lmql_runtime.register_model(model_name, Model)
         lmql_runtime.register_model("*", Model)
     else:
         if "LMQL_BROWSER" in os.environ:
             assert False, "Cannot use HuggingFace Transformers models in browser. Please use openai/ models or install lmql on your local machine."
 
         from lmql.runtime.hf_integration import transformers_model
@@ -109,24 +106,73 @@
 def _query_from_string(s):
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(s)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     return module.query
         
+def _get_decorated_function_code(fct):
+    import ast
+    import inspect
+
+    source = ""
+
+    try:
+        source = inspect.getsource(fct)
+        tree = ast.parse(source)
+        docstring_element = tree.body[0].body[0].value
+        docstring = docstring_element.s
+        # get range of source that corresonds to the docstring
+        start = docstring_element.lineno
+        end = docstring_element.end_lineno
+        startcol = docstring_element.col_offset
+        endcol = docstring_element.end_col_offset
+        
+        # get source code of the function
+        source = source.splitlines()
+
+        # remove common indent
+        common_indent = None
+        lines = []
+        for line in source[start-1:end]:
+            if line.strip() == "":
+                lines.append(line)
+                continue
+            if common_indent is None:
+                common_indent = len(line) - len(line.lstrip())
+            else:
+                common_indent = min(common_indent, len(line) - len(line.lstrip()))
+            lines.append(line[common_indent:])
+        
+        lines[0] = lines[0][startcol - common_indent:]
+        lines[-1] = lines[-1][:endcol]
+
+        source = "\n".join(lines)
+
+        quote_types = "'''" if source.endswith("'''") else '"""'
+        if source.startswith(quote_types):
+            source = source[len(quote_types):]
+        assert source.endswith(quote_types), f"Docstring of @lmql.query function {fct.__name__} must be on the first line of the function, but is:\n {source}"
+        source = source[:-len(quote_types)].strip("\n")
+    except:
+        raise RuntimeError("Failed to parse docstring of query function as LMQL code:\n\n" + str(source))
+
+    return source
+
+
 def query(fct):
     import inspect
-    
+
     # support for lmql.query(<query string>)
     if type(fct) is str: return _query_from_string(fct)
     
     calling_frame = inspect.stack()[1]
     scope = LMQLInputVariableScope(fct, calling_frame)
-    code = fct.__doc__
-    
+    code = _get_decorated_function_code(fct)
+        
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(code)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     
     assert inspect.iscoroutinefunction(fct), f"@lmql.query {fct.__name__} must be declared async."
```

### Comparing `lmql-0.0.4.2/src/lmql/cli.py` & `lmql-0.0.5/src/lmql/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import subprocess
 import os
 import argparse
 import lmql
+from lmql.runtime.interpreter import LMQLResult
 
 import lmql.version as version_info
 
 project_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 def cmd_serve_model():
     """emoji:🏄 Serve a 🤗 Transformers model via the LMQL inference API"""
@@ -39,27 +40,28 @@
 
     results = asyncio.run(lmql.run_file(absolute_path, output_writer=writer))
     
     if type(results) is not list:
         results = [results]
     
     for r in results:
-        for v in [v for v in r.variables if v.startswith("P(")]:
-            distribution = r.variables[v]
-            max_prob = max([p for _,p in distribution])
-            labels = []
-            for value, prob in distribution:
-                label = value if prob != max_prob else f"{value} (*)"
-                labels.append(label)
-            max_length = max([len(str(l)) for l in labels])
-
-            print(v)
-            for (value, prob), label in zip(distribution, labels):
-                label = label.ljust(max_length)
-                print(" - {} {}".format(label, prob))
+        if isinstance(r, LMQLResult):
+            for v in [v for v in r.variables if v.startswith("P(")]:
+                distribution = r.variables[v]
+                max_prob = max([p for _,p in distribution])
+                labels = []
+                for value, prob in distribution:
+                    label = value if prob != max_prob else f"{value} (*)"
+                    labels.append(label)
+                max_length = max([len(str(l)) for l in labels])
+
+                print(v)
+                for (value, prob), label in zip(distribution, labels):
+                    label = label.ljust(max_length)
+                    print(" - {} {}".format(label, prob))
 
     if args.time:
         print("Query took:", time.time() - start)
 
 def ensure_node_install():
     try:
         v = subprocess.check_output("node --version", shell=True, stderr=subprocess.DEVNULL).decode("utf-8").strip()
@@ -157,21 +159,21 @@
 
 def hello():
     import asyncio
     code_local = """
 argmax "Hello[WHO]" from "local:gpt2-medium" where len(WHO) < 10    
 """
     print("[Greeting 🤗 Transformers]")
-    asyncio.run(lmql.run(code_local))
+    asyncio.run(lmql.run(code_local, output_writer=lmql.printing))
     
     print("[Greeting OpenAI]")
     code_openai = """
 argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
 """
-    asyncio.run(lmql.run(code_openai))
+    asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
 
 hidden_commands = {
     "hello": hello
 }
 
 def main():
     if len(sys.argv) < 2:
```

### Comparing `lmql-0.0.4.2/src/lmql/demo.py` & `lmql-0.0.5/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/http.py` & `lmql-0.0.5/src/lmql/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""
+Dispatching implementation for a simple HTTP fetch() function.
+
+Dispatches to the LMQL Browser Runtime if the LMQL_BROWSER environment variable is set, 
+otherwise uses aiohttp.
+
+For browser use this is required, as the native Python networking stack
+is not available when running via Pyodide.
+"""
+
 import os
 import json
     
 if "LMQL_BROWSER" in os.environ:
     import js
     from pyodide.ffi import to_js
```

### Comparing `lmql-0.0.4.2/src/lmql/language/compiler.py` & `lmql-0.0.5/src/lmql/language/compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,24 +35,33 @@
         # capture set of defined vars
         declared_template_vars = [v.name for v in qstring_to_stmts(qstring) if type(v) is TemplateVariable]
         for v in declared_template_vars: 
             self.defined_vars.add(v)
             self.written_vars.add(v)
             if v in self.free_vars: self.free_vars.remove(v)
 
-        # capture set of format vars
-        used_fstring_expr = [v[1:-1] for v in re.findall("\{[^\}]+\}", qstring)]
+        # capture set of format vars (exclude {{ and }})
+        # replace {{ and }} with escape sequence \u007b and \u007d 
+        qstring = qstring.replace("{{", "__curly_open__").replace("}}", "__curly_close__")
+        used_fstring_expr = [v[1:-1] for v in re.findall("\{[^\}\{]+\}", qstring)]
         for v in used_fstring_expr:
             if v.startswith(":"):
                 continue
-            parsed = ast.parse(v).body[0].value
-            self.visit(parsed)
+            try:
+                parsed = ast.parse(v).body[0].value
+                self.visit(parsed)
+            except:
+                raise RuntimeError("Failed to parse fstring expression: ", v)
+
             
             # if v not in self.defined_vars and v not in self.free_vars and v not in self.written_vars:
             #     self.free_vars.add(v)
+
+        # put double curly braces back in
+        qstring = qstring.replace("__curly_open__", "{{").replace("__curly_close__", "}}")
                 
         template_tags = [v[1:-1] for v in re.findall("\{:[A-z0-9]+\}", qstring)]
         for tt in template_tags:
             qstring = qstring.replace(f"{{{tt}}}", f"{{lmql.tag('{tt[1:]}')}}")
         
         node.value = qstring
 
@@ -85,14 +94,24 @@
 
     def visit_Expr(self, expr):
         if type(expr.value) is ast.Constant:
             expr.value = self.transform_Constant(expr.value)
         else:
             self.generic_visit(expr)
         return expr
+    
+    # translate id access to context
+    def visit_Name(self, node: ast.Name):
+        name = str(node.id)
+        
+        if type(node.ctx) is ast.Load:
+            if name == "context":
+                return ast.parse("(" + yield_call("get_context", ()) + ")").body[0].value
+        return node
+
 
     def transform_Constant(self, constant):
         if type(constant.value) is not str: return constant
         qstring = constant.value
         # TODO: handle escaping more completely and gracefully
         qstring = qstring.replace("\n", "\\\\n")
         compiled_qstring = ""
@@ -108,18 +127,20 @@
                 else:
                     declared_template_vars.add(stmt.name)
                     compiled_qstring += "[" + stmt.name + "]"
 
         if len(compiled_qstring) == 0:
             return constant
 
-        result_code = f'yield context.query(f"""{compiled_qstring}""")'
+        # result_code = f'yield context.query(f"""{compiled_qstring}""")'
+        result_code = interrupt_call('query', f'f"""{compiled_qstring}"""')
 
         for v in declared_template_vars:
-            result_code += f"\n{v} = context.get_var('{v}')"
+            get_var_call = yield_call('get_var', f'"{v}"')
+            result_code += f"\n{v} = " + get_var_call
         return ast.parse(result_code)
 
     # def transform_prompt_stmt(self, stmt):
     #     if type(stmt) is ast.Expr:
     #         if type(stmt.value) is ast.Constant and type(stmt.value.value) is str:
     #             # print(stmt.value.value)
     #             stmt.value = self.transform_query_string(stmt.value.value)
@@ -453,14 +474,20 @@
             lmql_code = lmql_code[1:]
     
     # remove common indent
     lines = lmql_code.split("\n")
     common_indent = min([len(l) - len(l.lstrip()) for l in lines if len(l.strip()) > 0])
     return "\n".join([l[common_indent:] for l in lines])
 
+def yield_call(func, *args):
+    return f"""yield lmql.runtime_support.context_call("{func}", {", ".join([str(a) for a in args])})"""
+
+def interrupt_call(func, *args):
+    return f"""yield lmql.runtime_support.interrupt_call("{func}", {", ".join([str(a) for a in args])})"""
+
 class LMQLCompiler:
     def __init__(self):
         pass
 
     def compile(self, filepath):
         try:
             # parse file
@@ -492,27 +519,31 @@
                 model_name = "'" + model_name_aliases[model_name[1:-1]] + "'"
 
             # resulting code
             code = None
             output_variables = "output_variables=[" + ", ".join([f'"{v}"' for v in scope.defined_vars]) + "]"
 
             # generate function that runs query
-            with PythonFunctionWriter("query", output_file, list(scope.free_vars) + ["context"], 
+            parameters = list(sorted(list(scope.free_vars.union(set(["context"])))))
+
+            with PythonFunctionWriter("query", output_file, parameters, 
                 q.prologue, decorators=["lmql.compiled_query"], decorators_args=[output_variables]) as writer:
                 
-                writer.add(f"context.set_model({model_name})")
-                writer.add(f"context.set_decoder({astunparse.unparse(q.decode.method).strip()}, {unparse_list(q.decode.decoding_args)})")
+                writer.add(yield_call("set_model", model_name))
+                # writer.add(f"context.set_decoder({})")
+                writer.add(yield_call("set_decoder", astunparse.unparse(q.decode.method).strip(), unparse_list(q.decode.decoding_args)))
                 writer.add("# where")
                 writer.add(q.where)
-                writer.add(f"context.set_where_clause({q.where_expr})")
+                writer.add(yield_call("set_where_clause", q.where_expr))
                 writer.add("# prompt")
                 writer.add(astunparse.unparse(q.prompt))
                 if q.distribution:
                     writer.add("# distribution")
-                    writer.add("context.set_distribution('{}', {})".format(q.distribution.variable_name, astunparse.unparse(q.distribution.values).strip()))
+                    # writer.add("context.set_distribution('{}', {})".format(q.distribution.variable_name, astunparse.unparse(q.distribution.values).strip()))
+                    writer.add(yield_call("set_distribution", "\"" + q.distribution.variable_name + "\"", astunparse.unparse(q.distribution.values).strip()))
                 
-                writer.add(f"yield ('result', context.get_return_value())")
+                writer.add(f"yield ('result', (" + yield_call("get_return_value", ()) + "))")
 
             return LMQLModule(output_file, lmql_code=lmql_code, output_variables=[v for v in scope.defined_vars])
         except FragmentParserError as e:
             sys.stderr.write("error: " + str(e) + "\n")
```

### Comparing `lmql-0.0.4.2/src/lmql/language/fragment_parser.py` & `lmql-0.0.5/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/language/qstrings.py` & `lmql-0.0.5/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/language/validator.py` & `lmql-0.0.5/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/model/async_generation_utils.py` & `lmql-0.0.5/src/lmql/model/async_generation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,14 @@
     MaxNewTokensCriteria,
     MaxTimeCriteria,
     StoppingCriteriaList,
     validate_stopping_criteria,
 )
 from transformers.utils import logging
 
-from lmql.model.hf_beam_search import BeamSearchScorer, BeamScorer
-from lmql.runtime.rewriter import RewrittenInputIds, ActivePromptTokens
-
 logger = logging.get_logger(__name__)
 
 def ensure_tensor(v):
     if torch.is_tensor(v): 
         return v
     else:
         return torch.tensor(v)
```

### Comparing `lmql-0.0.4.2/src/lmql/model/client.py` & `lmql-0.0.5/src/lmql/model/served_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self.consumed_tokens = 0
         self.num_queries = 0
         self.num_generate_calls = 0
         self.billable_tokens = 0
 
     def report_stats(self, printer, decoder_step=None):
         if printer is None:
-            print("no printer")
             return
         if hasattr(printer, "report_model_stats"):
             data = {
                 "tokens": self.billable_tokens,
                 "model": self.model_identifier
             }
             if decoder_step is not None:
@@ -119,87 +118,14 @@
             if remaining_sleep_time > 0: await asyncio.sleep(remaining_sleep_time)
 
     def _timeout(self, sample_id):
         if sample_id in self.pending:
             self.pending[sample_id].set_exception(TimeoutError("Timed out waiting for result of sample {}".format(sample_id)))
             del self.pending[sample_id]
 
-    async def detokenize(self, input_ids):
-        self.create_result_processor_task_if_required()
-        loop = asyncio.get_event_loop()
-
-        # handle torch tensors
-        if type(input_ids) is torch.Tensor:
-            input_ids = input_ids.tolist()
-
-        sample_id = self.sample_id
-        self.sample_id += 1
-        
-        payload = {
-            "action": "detokenize",
-            "client_id": self.client_id,
-            "input_ids": input_ids,
-            "sample_id": sample_id
-        }
-
-        try:
-            assert sample_id not in self.pending, "sample_id {} already in self.pending".format(sample_id)
-            # setup future and timeout
-            self.pending[sample_id] = loop.create_future()
-            r = requests.post(f"{self.host}/queue", json=payload)
-
-            if r.status_code != 200:
-                raise Exception(f"Error posting to {self.host}/queue: {r.status_code}")
-            
-            loop.call_later(self.timeout, self._timeout, sample_id)
-            
-            return (await self.pending[sample_id])["text"]
-        except requests.exceptions.ConnectionError as e:
-            # check for connection refused
-            if "Connection refused" in str(e):
-                raise Exception(f"Error connecting to {self.host}/queue. Please make sure an instance of the LMQL inference API for this model is running. To start it, run `python -m serve <MODEL>`.")
-            else:
-                raise e
-
-    async def tokenize(self, text):
-        self.create_result_processor_task_if_required()
-        loop = asyncio.get_event_loop()
-
-        assert type(text) == str, "The provided text for tokenize() must be str."
-
-        sample_id = self.sample_id
-        self.sample_id += 1
-
-        payload = {
-            "action": "tokenize",
-            "text": text,
-            "client_id": self.client_id,
-            "sample_id": sample_id
-        }
-
-        try:
-            assert sample_id not in self.pending, "sample_id {} already in self.pending".format(sample_id)
-            # setup future and timeout
-            self.pending[sample_id] = loop.create_future()
-            
-            r = requests.post(f"{self.host}/queue", json=payload)
-            
-            if r.status_code != 200:
-                raise Exception(f"Error posting to {self.host}/queue: {r.status_code}")
-            
-            loop.call_later(self.timeout, self._timeout, sample_id)
-            
-            return (await self.pending[sample_id])["input_ids"]
-        except requests.exceptions.ConnectionError as e:
-            # check for connection refused
-            if "Connection refused" in str(e):
-                raise Exception(f"Error connecting to {self.host}/queue. Please make sure an instance of the LMQL inference API for this model is running. To start it, run `python -m serve <MODEL>`.")
-            else:
-                raise e
-
     def reset_stats(self):
         self.consumed_tokens = 0
         self.num_queries = 0
 
     def forward(self, input_ids, attention_mask=None):
         assert input_ids.numel() > 0, "input_ids must not be empty"
         # keep stats
@@ -249,51 +175,14 @@
         except requests.exceptions.ConnectionError as e:
             # check for connection refused
             if "Connection refused" in str(e):
                 raise Exception(f"Error connecting to {self.host}/queue. Please make sure an instance of the LMQL inference API for this model is running. To start it, run `python -m serve <MODEL>`.")
             else:
                 raise e
 
-
-class Sample:
-    def __init__(self, model, seq=None, input_ids=None):
-        assert not (self.seq is None and self.input_ids), "Either seq or input_ids must be provided for a Sample()"
-        
-        self.model = model
-        self._seq = seq
-        self._input_ids = input_ids
-    
-    async def seq(self):
-        if self._seq is None:
-            assert self._input_ids is not None
-            self._seq = await self.model.detokenize(self._input_ids)
-        return self._seq
-    
-    async def input_ids(self):
-        if self._input_ids is None:
-            assert self.seq is not None
-            self._input_ids = await self.model.tokenize(self._seq)
-        return self._input_ids
-
-    async def successor(self, token_id) -> 'Sample':
-        return Sample(self.model, input_ids=(await self.input_ids()) + [token_id])
-
-    async def distribution(self):
-        res = await self.model.forward(await self.input_ids())
-        return res["next_token_logits"]
-    
-    def __repr__(self) -> str:
-        return "<Sample seq={} input_ids={}>".format(self._seq, self._input_ids)
-
-    async def concat(self, text):
-        seq = (await self.seq()) + text
-        input_ids = await self.model.tokenize(seq)
-        
-        return Sample(self.model, seq=seq, input_ids=input_ids)
-
 @dataclass
 class ServedPretrainedModelOutput:
     logits: torch.Tensor
 
     # enable 'in' operator
     def __contains__(self, item):
         return item in self.__dict__.keys()
```

### Comparing `lmql-0.0.4.2/src/lmql/model/local_client.py` & `lmql-0.0.5/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/model/serve.py` & `lmql-0.0.5/src/lmql/model/serve.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,19 @@
     
     sample_count: int = 0
     client_results_queues: Dict[str,Queue] = field(default_factory=dict)
     
     exit: bool = False
 
 class TokenizerProcessor:
-    def __init__(self, state: InferenceServerState):
+    def __init__(self, state: InferenceServerState, ready_event: multiprocessing.Event = None):
         self.model_identifier = state.tokenizer_descriptor
         self.queue = state.tokenize_queue
         self.state = state
+        self.ready_event = ready_event
 
     def shutdown(self):
         self.state.exit = True
 
     def tokenize(self, tokenizer, sample_id, client_id, item):
         text = item["text"]
 
@@ -75,14 +76,17 @@
         })
 
     def run(self, index):
         # load tokenizer
         tokenizer = AutoTokenizer.from_pretrained(self.model_identifier)
         print("Tokenizer #{} {} ready!".format(index, self.model_identifier))
 
+        if self.ready_event:
+            self.ready_event.set()
+
         while not self.state.exit:
             item = self.queue.get()
             if item is None:
                 time.sleep(0.1)
                 continue
 
             sample_id = item["sample_id"]
@@ -107,19 +111,20 @@
             p = multiprocessing.Process(target=self.run, args=(i,))
             p.start()
             workers.append(p)
         
         return workers
 
 class ModelProcessor:
-    def __init__(self, state: InferenceServerState, cuda: bool = False, cache: str = None):
+    def __init__(self, state: InferenceServerState, cuda: bool = False, cache: str = None, ready_event: multiprocessing.Event = None):
         self.model_identifier = state.model_identifier
         self.queue = state.queue
         self.state = state
         self.cuda = cuda
+        self.ready_event = ready_event
         
         self.cache = None
         if cache is not None:
             from rocksdict import Rdict
             self.cache = Rdict(cache)
             
         self.request_count = 0
@@ -180,14 +185,17 @@
         else:
             print("Loading {} (Multi-GPU)".format(self.model_identifier))
             self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True, device_map="auto")
         self.model.eval()
         
         print("Ready!".format(self.model_identifier))
 
+        if self.ready_event:
+            self.ready_event.set()
+
         while not self.state.exit:
             self.print_stats()
             # wait for self.queue to have an item
             try:
                 item = self.queue.get(timeout=1.0)
             except Empty:
                 continue
@@ -440,14 +448,15 @@
     parser.add_argument("model", type=str)
     parser.add_argument("--tokenizer", type=str, default=None)
     parser.add_argument("--port", type=int, default=8080)
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--cuda", action="store_true", default=False)
     parser.add_argument("--cache", type=str, default=None)
     parser.add_argument("--dtype", type=str, default="none")
+    parser.add_argument("--wait_until_ready", action="store_true", default=False, help="Whether the server should start only after the model and tokenizer have been loaded.")
     parser.add_argument("--num-tokenizer-processes", type=int, default=2, dest="num_tokenizer_processes")
     
     args = parser.parse_args()
     
     manager = multiprocessing.Manager()
     
     # prepare configuration
@@ -459,21 +468,26 @@
                                  tokenizer_descriptor, 
                                  args.dtype, 
                                  queue=manager.Queue(), 
                                  tokenize_queue=manager.Queue(),
                                  all_results_queue=manager.Queue())
 
     # run model in separate process
-    processor = ModelProcessor(state, cuda=args.cuda, cache=args.cache)
+    processor = ModelProcessor(state, cuda=args.cuda, cache=args.cache, ready_event=(multiprocessing.Event() if args.wait_until_ready else None))
     processor.run_in_parallel()
 
     # run tokenizers in separate process
-    tokenizer_processor = TokenizerProcessor(state)
+    tokenizer_processor = TokenizerProcessor(state, ready_event=(multiprocessing.Event() if args.wait_until_ready else None))
     tokenizer_processor.run_in_parallel(n=args.num_tokenizer_processes)
 
+    # don't serve until the model and tokenizer are ready
+    if args.wait_until_ready:
+        processor.ready_event.wait()
+        tokenizer_processor.ready_event.wait()
+
     # run inference API server in this process
     server_address = (args.host, args.port)
     httpd = HTTPServer(server_address, LMQLInferenceAPIHandler)
     httpd.state = state
     
     try:
         print("Serving LMQL inference API on {}:{}".format(args.host, args.port))
```

### Comparing `lmql-0.0.4.2/src/lmql/ops/follow_map.py` & `lmql-0.0.5/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ops/ops.py` & `lmql-0.0.5/src/lmql/ops/ops.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     return class_transformer
 
 class Node:
     def __init__(self, predecessors):
         assert type(predecessors) is list, "Predecessors must be a list, not {}".format(type(predecessors))
         self.predecessors = predecessors
         self.depends_on_context = False
-        
-        self.follow_map = None
     
     def execute_predecessors(self, trace, context):
         return [execute_op(p, trace=trace, context=context) for p in self.predecessors]
 
     def forward(self, *args, **kwargs):
         raise NotImplementedError(type(self) + " does not implement forward()")
 
@@ -38,14 +36,37 @@
     def final(self, args, **kwargs):
         if all([a == "fin" for a in args]):
             return "fin"
         return "var"
 
     def __nodelabel__(self):
         return str(type(self))
+    
+    def postprocess_var(self, var_name):
+        """
+        Returns true if this operations provides postprocessing semantics for complete values for the given variable name.
+        """
+        return False
+
+    def postprocess(self, operands, value):
+        """
+        Returns the postprocessed variant of `value`. Only called if `postprocess_var` returns true for variable name of value.
+        
+        You can return a tuple of postprocessed_rewrite (prompt) and postprocessed_value (variable value), to additionally 
+        provide different postprocessing semantics for the variable value and the rewrite of the prompt.
+        """
+        pass
+
+    def postprocess_order(self, other, **kwargs):
+        """
+        Orders application of postprocessing operations. Returns "before", "after" or 0 if order is not defined.
+        
+        Only invoked for `other` operations, that return true for the same `postprocess_var`.
+        """
+        return 0 # by default, no order is defined (only one postprocessing operation per variable can be applied)
 
 def DynamicTypeDispatch(name, type_map):
     def get_handler(args):
         for signature, op in type_map:
             # fallback implementation
             if signature == "*": return op
             
@@ -86,21 +107,31 @@
     return t == NextToken
 
 def strip_next_token(x):
     if type(x) is list:
         return [i for i in x if not is_next_token(i)]
     elif type(x) is tuple:
         return tuple(i for i in x if not is_next_token(i))
+    if type(x) is not str:
+        return x
     if x.endswith(NextToken):
         x = x[:-len(NextToken)]
     return x
 
+class postprocessed_value:
+    def __init__(self, value):
+        self.value = value
+class postprocessed_rewrite:
+    def __init__(self, rewrite):
+        self.rewrite = rewrite
+
+
 @LMQLOp("SENTENCES")
 class Sentences(Node):
-    def forward(self, v):
+    def forward(self, v, **kwargs):
         sentences = tuple(self.split(v, separator=["."]))
         return self.strip(sentences)
     
     def strip(self, sentences):
         if len(sentences) == 0:
             return sentences
         elif sentences[-1] == ():
@@ -151,17 +182,18 @@
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
     
 
 @LMQLOp("INT")
 class IntOp(Node):
-    def forward(self, x):
+    def forward(self, x, final=None, **kwargs):
         if x is None: return None
         if x == "": return None
+        if final is not None and all(f == "fin" for f in final): return True
 
         # check int contains digits only
         if x.startswith(" "):
             x = x[1:]
         if not all([c in "0123456789" for c in x]):
             return False
         else:
@@ -171,19 +203,19 @@
         if v is None: return None
         
         has_next_token = v != strip_next_token(v)
         v = strip_next_token(v)
 
         context = kwargs.get("context", None)
         if context.runtime.prefers_compact_mask:
-            number_tokens = tset("1","2","3","4","5","6","7","8","9","Ġ2","Ġ3","Ġ4","Ġ5","Ġ0","Ġ6","Ġ7","Ġ8","Ġ9","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","37","48","66","55","47","49","65","68","31","67","59","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True)
-            number_continuation_tokens = tset("0","1","2","3","4","5","6","7","8","9","00","01","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","05","37","48","66","55","47","08","49","09","65","07","02","04","03","68","31","67","59","06","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True)
+            number_tokens = tset("1","2","3","4","5","6","7","8","9","Ġ2","Ġ3","Ġ4","Ġ5","Ġ0","Ġ6","Ġ7","Ġ8","Ġ9","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","37","48","66","55","47","49","65","68","31","67","59","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True, name="number_tokens")
+            number_continuation_tokens = tset("0","1","2","3","4","5","6","7","8","9","00","01","10","12","50","19","11","20","30","15","14","16","13","25","18","17","24","80","40","22","60","23","29","27","26","28","99","33","70","45","35","64","75","21","38","44","36","32","39","34","05","37","48","66","55","47","08","49","09","65","07","02","04","03","68","31","67","59","06","77","58","69","88","46","57","43","42","78","79","90","95","41","56","54","98","76","52","53","51","86","74","89","72","73","96","71","63","62","85","61","97","84","87","94","92","83","93","91","82","81", exact=True, name="number_continuation_tokens")
         else:
-            number_tokens = tset("[ 1-9][0-9]*$", regex=True)
-            number_continuation_tokens = tset("[0-9]+$", regex=True)
+            number_tokens = tset("[ 1-9][0-9]*$", regex=True, name="full_number_tokens")
+            number_continuation_tokens = tset("[0-9]+$", regex=True, name="full_number_continuation_tokens")
 
         if not has_next_token:
             return fmap(
                 ("eos", len(v.strip()) != 0),
                 ("*", self.forward(v))
             )
 
@@ -203,31 +235,48 @@
 
             return fmap(
                 (number_continuation_tokens, True),
                 ("eos", True),
                 ("*", False)
             )
         
+    def postprocess_var(self, var_name):
+        return var_name == self.predecessors[0].name
+
+    def postprocess(self, operands, raw):
+        value = int(raw)
+        if raw.startswith(" "):
+            value = " " + str(value)
+        return postprocessed_rewrite(str(value)), postprocessed_value(value)
+
+    def postprocess_order(self, other, **kwargs):
+        if isinstance(other, StopAtOp):
+            return "after" # apply Int after StopAt
+        else:
+            return 0 # cannot be compared
+
     def final(self, x, operands=None, result=None, **kwargs):
         if result == False and x[0] == "inc":
             return "fin"
         return super().final(x, operands=operands, result=result, **kwargs)
 
 @LMQLOp("TOKENS")
 class TokensOp(Node):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         
         self.depends_on_context = True
 
-    def forward(self, x, context):
+    def forward(self, x, context, **kwargs):
         import asyncio
         if x is None: return None
         if x == "": return []
-        
+
+        assert False, "TOKENS() operation is currently not supported"
+
         tokens = context.runtime.model.sync_tokenize(x)
         return tokens
 
     def follow(self, v, context=None, **kwargs):
         if v is None: return None
         contains_next_token = v != strip_next_token(v)
         words = self.forward(strip_next_token(v), context)
@@ -243,15 +292,15 @@
         )
 
     def final(self, x, context, operands=None, result=None, **kwargs):
         return x[0]
 
 @LMQLOp("WORDS")
 class WordsOp(Node):
-    def forward(self, x):
+    def forward(self, x, **kwargs):
         if x is None: return None
         if x == "": return []
         # split on " " or "\n"
         x = x.replace(" ", " ")
         x = x.replace("\n", " ")
         x = x.replace("\u0120", " ")
         words = x.split(" ")
@@ -279,23 +328,26 @@
         )
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
 @LMQLOp("len")
 class LenOp(Node):
-    def forward(self, x):
+    def forward(self, x, **kwargs):
         if x is None: return None
+        if type(x) is not str: 
+            x = str(x)
         return len(x)
     
     def follow(self, v, **kwargs):
         if v is None: return None
         if type(v) is list or type(v) is tuple:
             return len(v)
         else:
+            v = str(v)
             assert type(v) is str, "len() can only be applied to strings, lists, or tuples"
             if NextToken not in v:
                 return len(v)
             v = strip_next_token(v)
             
             len_masks = []
             all = "∅"
@@ -312,22 +364,22 @@
             
             return fmap(*len_masks)
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
 class NotOp(Node):
-    def forward(self, op):
+    def forward(self, op, **kwargs):
         return not op
 
     def follow(self, v, **kwargs):
         return not v
 
 class Lt(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         return args[0] < args[1]
     
     def follow(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         return args[0] < args[1]
 
@@ -354,15 +406,15 @@
 
 def Gt(preds): return Lt(list(reversed(preds)))
 
 class EqOp(Node):
     def __init__(self, predecessors):
         super().__init__(predecessors)
 
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         return all([a == args[0] for a in args])
 
     def follow(self, *args, **kwargs):
         op1 = args[0]
         op2 = args[1]
         
         if op1 is None or op2 is None:
@@ -436,15 +488,15 @@
                 if not fixed_value.startswith(o): return "fin"
             else: # of == "var":
                 continue
         
         return super().final(operand_final, operands=operands, result=result, **kwargs)
 
 class SelectOp(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if len(args[0]) <= args[1]:
             return None
         return args[0][args[1]]
 
     def follow(self, *args, **kwargs):
         l = args[0]
         idx = args[1]
@@ -481,15 +533,15 @@
         
         # indicates whether the downstream node requires text diff information
         self.diff_aware_read = False
 
     async def json(self):
         return self.name
 
-    def forward(self, context):
+    def forward(self, context, **kwargs):
         if self.diff_aware_read:
             return (context.get(self.name, None), context.get_diff(self.name, None))
         return context.get(self.name, None)
     
     def follow(self, context, **kwargs):
         value = context.get(self.name, None)
         if value is None: return None
@@ -518,15 +570,15 @@
     def __init__(self, args):
         super().__init__([])
         
         value, final = args
         self.value = value
         self.final_value = final
 
-    def forward(self):
+    def forward(self, **kwargs):
         return self.value
 
     def follow(self, **kwargs):
         return fmap(
             ("*", self.value)
         )
 
@@ -542,15 +594,15 @@
         if len(phrase) > len(x):
             yield phrase[len(x):]
         else:
             if allow_full_matches: 
                 yield ""
 
 class InOpStrInStr(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
 
         return args[0] in args[1]
 
     def follow(self, *args, **kwargs):
         op1 = strip_next_token(args[0])
         op1_generating = args[0] != op1
@@ -585,15 +637,15 @@
         if not result:
             return super().final(op_final, result=result, **kwargs)
         if op_final[1] == "inc" and op_final[0] == "fin":
             return "fin"
         return super().final(op_final, result=result, **kwargs)
 
 class InOpStrInSet(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         
         x = args[0]
         allowed_phrases = args[1]
         
         if x is None: 
             return None
@@ -644,15 +696,15 @@
 
 InOp = DynamicTypeDispatch("InOp", (
     ((str, str), InOpStrInStr),
     ("*", InOpStrInSet),
 ))
 
 class OrOp(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a == True for a in args]):
             return True
         elif all([a == False for a in args]):
             return False
         else:
             return None
 
@@ -668,15 +720,15 @@
             return "var"
         else: # not result
             if any(a == "var" for a in args):
                 return "var"
             return "fin"
 
 class AndOp(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if type(args[0]) is tuple and len(args) == 1:
             args = args[0]
 
         if any([a == False for a in args]):
             return False
         elif any([a is None for a in args]):
             return None
@@ -709,15 +761,15 @@
             overlap = i
 
     if overlap == 0: return None
     else: return phrase[i:]
 
 @LMQLOp("STARTS_WITH")
 class StartsWithOp(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         
         x = args[0]
         allowed_phrases = args[1]
 
         for phrase in allowed_phrases:
             if x.startswith(phrase):
@@ -807,17 +859,20 @@
         if tokenizer in self._tokenized_stopping_phrase_cache:
             return self._tokenized_stopping_phrase_cache[tokenizer]
         else:
             result = (await tokenizer(self.stopping_phrase))
             self._tokenized_stopping_phrase_cache[tokenizer] = result
             return result
 
-    def forward(self, *args):
+    def forward(self, *args, final, **kwargs):
         if any([a is None for a in args]): return None
 
+        if all([a == "fin" for a in final]):
+            return True
+
         op1, op1_diff = args[0]
         op2 = args[1]
 
         if op1 is None: return
         if op1_diff is None: op1_diff = ""
 
         matched_phrase_index = op1.rfind(op2)
@@ -826,21 +881,20 @@
         return not op2_in_op1 or op1.endswith(op2)
 
     def follow(self, *args, previous_result=None, **kwargs):
         if any([a is None for a in args]): 
             return None
 
         op1, op1_diff = args[0]
-        if op1 is None:return None
+        if op1 is None: return None
         if op1_diff is None: op1_diff = ""
 
         op1 = strip_next_token(op1)
         op2 = args[1]
 
-
         matched_phrase_index = op1.rfind(op2)
         op2_in_op1 = matched_phrase_index != -1 and matched_phrase_index + len(op2) > len(op1) - len(op1_diff)
 
         if not op2_in_op1: return fmap(("*", True))
 
         ends_with_stopping_phrase = op1.endswith(op2)
 
@@ -862,16 +916,47 @@
                 r = "var"
             elif ops_final[0] == "dec": 
                 r = "var"
             else: 
                 r = "fin"
             return r
 
+    def postprocess_var(self, var_name):
+        return var_name == self.predecessors[0].name
+
+    def postprocess(self, operands, value):
+        op2 = operands[1]
+        matched_phrase_index = value.rfind(op2)
+        if matched_phrase_index != -1:
+            value = value[:matched_phrase_index + len(op2)]
+
+        return postprocessed_rewrite(value), postprocessed_value(value)
+    
+    def postprocess_order(self, other, operands, other_inputs, **kwargs):
+        if type(other) is IntOp:
+            return "before"
+        if type(other) is StopAtOp:
+            value, value_diff = operands[0]
+            op2 = operands[1]
+            assert value == other_inputs[0][0], "internal error: comparing postprocess_order with two StopAtOps with different values (do they refer to different variables) {}".format((value, other_inputs[0]))
+            matched_phrase_index = value.rfind(op2)
+            other_matched_phrase_index = other_inputs[0][0].rfind(other_inputs[1])
+            if matched_phrase_index == -1:
+                return "before" # this operator does not match, so order does not matter
+            if other_matched_phrase_index == -1:
+                return "after" # other operator does not match, so order does not matter
+            if matched_phrase_index < other_matched_phrase_index:
+                return "before"
+            else:
+                return "after"
+        
+        return 0 # other constraints cannot be compared
+
 class OpaqueLambdaOp(Node):
-    def forward(self, *args):
+    def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         fct, *args = args
         return fct(*args)
     
     def follow(self, *v, **kwargs):
         if any([a is None for a in v]): return None
 
@@ -921,22 +1006,24 @@
             return "*"
 
     return allowed_tokens
 
 def is_node(op):
     return issubclass(type(op), Node)
 
-def derive_final(op, trace, context, result):
+def derive_predecessor_final(op, trace):
     def get_final(v):
         # for nodes, get final value from trace
         if is_node(v): return trace[v][1]
         # for constants, final value is always "fin"
         return "fin"
+    return [get_final(p) for p in op.predecessors]
 
-    predecessor_final = [get_final(p) for p in op.predecessors]
+def derive_final(op, trace, context, result):
+    predecessor_final = derive_predecessor_final(op, trace)
 
     def get_predecessor_result(v):
         if is_node(v): return trace[v][0]
         return v
     
     predecessor_values = [get_predecessor_result(p) for p in op.predecessors]
 
@@ -963,64 +1050,129 @@
             execute_op_stops_at_only(p, result=result)
     else:
         # other ops are no-ops from a STOPS_AT perspective (cannot contain additional STOPS_AT ops)
         # TODO: what about not
         return []
     return result
 
+def execute_postprocess(op: Node, var_name: str, value: str, trace=None, context=None):
+    """
+    Applies any postprocess() operations of the provided constraints
+    to the specified variable and value.
+
+    Returns a tuple of (postprocessed_value, rewritten_prompt)
+    """
+    if op is None: return value, value
+
+    nodes = [op]
+
+    trace = {}
+    postprocessors = []
+
+    # collect and sort set of postprocessing operations
+    while len(nodes) > 0:
+        op = nodes.pop()
+        nodes += [p for p in op.predecessors if isinstance(p, Node)]
+
+        if op.postprocess_var(var_name):
+            # compute operation inputs
+            inputs = op.execute_predecessors(trace, context)
+            # determine insertion index in postprocessors
+            i = 0
+            while i < len(postprocessors):
+                current_op, current_op_inputs = postprocessors[i]
+                relative_order = op.postprocess_order(current_op, operands=inputs, other_inputs=current_op_inputs)
+                if relative_order == "before":
+                    break
+                elif relative_order == "after":
+                    i += 1
+                else:
+                    assert len(postprocessors) == 0, "The specified set of constraints contains multiple incompatible postprocessing operations for the same variable. The conflicting operations are: {} and {}. Please make sure the used constraints implement postprocess_order for each other, to use them together.".format(current_op, op)
+            postprocessors.insert(i, (op, inputs))
+    
+    rewritten_value = None
+    rewritten_prompt = value
+
+    # apply postprocessing operations
+    for pop in postprocessors:
+        pop, inputs = pop # unpack to get op and inputs
+        result = pop.postprocess(inputs, rewritten_prompt)
+
+        if result is not None:
+            
+            if type(result) is tuple:
+                for v in result:
+                    if type(v) is postprocessed_value:
+                        rewritten_value = v.value
+                    elif type(v) is postprocessed_rewrite:
+                        rewritten_prompt = v.rewrite
+                    else:
+                        assert False, "Invalid postprocess() return value: {} for {}".format(v, op)
+            else:
+                rewritten_value = result
+    
+    if rewritten_prompt is None:
+        rewritten_prompt = str(value)
+    if rewritten_value is None:
+        rewritten_value = value
+    
+    return rewritten_value, rewritten_prompt
+
 def execute_op(op: Node, trace=None, context=None, return_final=False):
     # for constant dependencies, just return their value
     if not is_node(op): 
         return op
     
     # only evaluate each operation once
     if op in trace.keys(): 
         return trace[op][0]
     
     # compute predecessor values
     inputs = op.execute_predecessors(trace, context)
     
     if op.depends_on_context: 
         inputs += (context,)
-    
-    result = op.forward(*inputs)
+
+    inputs_final = derive_predecessor_final(op, trace)
+    result = op.forward(*inputs, final=inputs_final)
     is_final = derive_final(op, trace, context, result)
     
     if trace is not None: 
         trace[op] = (result, is_final)
 
     if return_final:
         return result, is_final
 
     return result
 
 def digest(expr, context, follow_context, no_follow=False):
-    if expr is None: return True, "fin", {}
+    if expr is None: return True, "fin", {}, {}
 
     trace = {}
+    follow_trace = {}
     expr_value, is_final = execute_op(expr, trace=trace, context=context, return_final=True)
 
     if no_follow:
-        return expr_value, is_final, trace
+        return expr_value, is_final, trace, follow_trace
 
     for op, value in trace.items():
         # determine follow map of predecessors
         if len(op.predecessors) == 0: 
             # empty argtuple translates to no follow input
             intm = all_fmap((ArgTuple(), ["fin"])) 
         else:
             # use * -> value, for constant value predecessor nodes
             def follow_map(p):
-                if is_node(p): return p.follow_map
+                if is_node(p): return follow_trace[p]
                 else: return fmap(("*", (p, ("fin",))))
             intm = fmap_product(*[follow_map(p) for p in op.predecessors])
         
         # apply follow map
         op_follow_map = follow_apply(intm, op, value, context=follow_context)
 
         # name = op.__class__.__name__
         # print(name, value)
         # print("follow({}) = {}".format(name, op_follow_map))
 
-        setattr(op, "follow_map", op_follow_map)
+        follow_trace[op] = op_follow_map
     
-    return expr_value, is_final, trace
+    return expr_value, is_final, trace, follow_trace
```

### Comparing `lmql-0.0.4.2/src/lmql/ops/token_set.py` & `lmql-0.0.5/src/lmql/ops/token_set.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,111 @@
 import re
+import atexit
 
 from tokenize import Token
 from typing import Iterable, Tuple
 from itertools import product
 
 from lmql.utils import nputil
 import numpy as np
+from lmql.runtime.stats import Stats
 
 def get_vocab(tokenizer):
     if hasattr(tokenizer, "vocab"):
         return tokenizer.vocab
     elif hasattr(tokenizer, "get_vocab"):
         return tokenizer.get_vocab()
     else:
         assert False, "Could not obtain full vocabulary from unknown tokenizer type: {}".format(type(tokenizer))
 
 class VocabularyMatcher:
     """
     Generates sub-token level logit masks from provided tokens.
     """
-    def __init__(self, tokenizer):
+    def __init__(self, tokenizer, model_identifier):
         self.tokenizer = tokenizer
+        self.model_identifier = model_identifier
         self.vocab = {v: k for k, v in get_vocab(self.tokenizer).items()}
 
         # TODO: this should be more complete
         self.space_repr = self.tokenizer.tokenize(" ")[0]
         self.nl_repr = self.tokenizer.tokenize("\n")[0]
         
         self.token_lengths = None
 
+        self.stats = Stats("VocabularyMatcher")
+        self.disk_cached = 0
+
     @property
     def eos_token_id(self):
         return self.tokenizer.eos_token_id
 
     @staticmethod
     def init(tokenizer):
-        vm = VocabularyMatcher(tokenizer)
-        VocabularyMatcher._instance = vm
+        if VocabularyMatcher._instance is not None:
+            return
+
+        # first try to load pickled matcher from cache (faster)
+        import pickle
+        import pathlib
+
+        cache_dir = pathlib.Path.home() / ".cache" / "lmql"
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        cache_identifier = tokenizer.model_identifier.replace("/", "-")
+        cache_path = cache_dir / f"token-mask-cache-{cache_identifier}.pkl"
+        matcher_path = cache_dir / f"matcher-{cache_identifier}.pkl"
+
+        try:
+            with open(matcher_path, "rb") as f:
+                VocabularyMatcher._instance = pickle.load(f)
+                VocabularyMatcher._instance.stats = Stats("VocabularyMatcher")
+        except:
+            VocabularyMatcher._instance = VocabularyMatcher(tokenizer, tokenizer.model_identifier)
+
+        if cache_path.exists():
+            with open(cache_path, "rb") as f:
+                try:
+                    import time
+                    s = time.time()
+                    VocabularyMatcher.cache = pickle.load(f)
+                    VocabularyMatcher._instance.disk_cached = len(VocabularyMatcher.cache)
+                    # print("Matcher cache loaded in {}s".format(time.time() - s))
+                except:
+                    print("Failed to load token mask cache from {}. If the cache is corrupted, please delete it.".format(cache_path))
+
+        atexit.register(lambda: VocabularyMatcher._instance.save())
+
+    def save(self):
+        # save cache to disk
+        import pickle
+        import pathlib
+
+        # assert False
+
+        cache_dir = pathlib.Path.home() / ".cache" / "lmql"
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        cache_identifier = self.model_identifier.replace("/", "-")
+        cache_path = cache_dir / f"token-mask-cache-{cache_identifier}.pkl"
+        matcher_path = cache_dir / f"matcher-{cache_identifier}.pkl"
+
+        with open(matcher_path, "wb") as f:
+            stats = self.stats
+            self.stats = None
+            pickle.dump(self, f)
+            self.stats = stats
+
+        def is_cached(k):
+            if k.startswith("named:"):
+                return True
+            if k.startswith("charlen:"):
+                return True
+            return False
+
+        with open(cache_path, "wb") as f:
+            pickle.dump({k: v for k, v in VocabularyMatcher.cache.items() if is_cached(k)}, f)
 
     @staticmethod
     def instance():
         if VocabularyMatcher._instance is None:
             raise Exception("VocabularyMatcher not initialized.")
         return VocabularyMatcher._instance
 
@@ -48,27 +113,56 @@
     def ensure_ready():
         VocabularyMatcher.instance()
 
     @property
     def vocab_size(self):
         return len(self.vocab)
 
-    def make_mask(self, tokens=None, regex=None, minus=None, prefix=False, exact=False, charlen=None):
-        if tokens is not None:
-            mask = self._make_mask_from_tokens(tokens, prefix, exact=exact)
+    @staticmethod
+    def with_cache(keys, provider):
+        keys = [k for k in keys if k is not None]
+        for k in keys:
+            if k in VocabularyMatcher.cache.keys():
+                return VocabularyMatcher.cache[k]
+        else:
+            result = provider()
+            for k in keys:
+                VocabularyMatcher.cache[k] = result
+            return result
+
+    def mask_cache_name(self, tokens=None, regex=None, minus=None, prefix=None, exact=None, charlen=None, name=None):
+        keys = ["named:" + name] if name is not None else []
+        if regex is not None:
+            return keys + ["regex:"]
         elif charlen is not None:
-            mask = self._make_mask_from_char_length(charlen)
+            return keys + ["charlen:" + str(charlen)]
         else:
-            assert regex is not None, "TokenSetConcrete: either tokens or regex must be set."
-            assert not prefix, "TokenSetConcrete: prefix is not supported for regex."
-            mask = self._make_mask_from_regex(regex)
+            assert tokens is not None
+            t = ("prefix " if prefix else "") + ("* \ " if minus else "") + "|".join(sorted(list(tokens)))
+            return keys + [t]
 
-        if minus: mask = np.logical_not(mask)
+    def make_mask(self, tokens=None, regex=None, minus=None, prefix=False, exact=False, charlen=None, name=None):
+        with self.stats.timer("make_mask"):
+            cache_keys = self.mask_cache_name(tokens, regex, minus, prefix, exact, charlen, name)
+            
+            def do_make_mask():
+                if tokens is not None:
+                    mask = self._make_mask_from_tokens(tokens, prefix, exact=exact)
+                elif charlen is not None:
+                    mask = self._make_mask_from_char_length(charlen)
+                else:
+                    assert regex is not None, "TokenSetConcrete: either tokens or regex must be set."
+                    assert not prefix, "TokenSetConcrete: prefix is not supported for regex."
+                    mask = self._make_mask_from_regex(regex)
 
-        return mask
+                if minus: mask = np.logical_not(mask)
+
+                return mask
+            
+            return VocabularyMatcher.with_cache(cache_keys, do_make_mask)
 
     def _make_mask_from_regex(self, regex):
         regex = regex.replace(" ", self.space_repr)
         regex = regex.replace("\n", self.nl_repr)
 
         regex = regex.replace(" ", self.tokenizer.tokenize(" ")[0])
 
@@ -129,14 +223,17 @@
         return mask
 
     def str(self, mask, full=False):
         prefix = ""
         tokens = []
         mask = mask
 
+        def tstr(t):
+            return str([t])[1:-1]
+
         if mask.sum() == mask.shape[0]:
             return "*"
 
         if mask.sum() > np.logical_not(mask).sum() and np.logical_not(mask).sum() > 0:
             prefix = "* \ "
             mask = np.logical_not(mask)
 
@@ -150,64 +247,31 @@
             if i == self.eos_token_id:
                 tokens.append("eos")
             else:
                 s = self.vocab[i]
                 # replace nl and space
                 s = self.tokenizer.convert_tokens_to_string([s])
                 s = s.encode("unicode_escape").decode("utf-8")
-                tokens.append(s)
+                tokens.append(tstr(s))
 
         return prefix + "{{{}}}".format(
             ", ".join([t for t in sorted(list(tokens))]) + ("..." if truncated else "")
         )
 
 VocabularyMatcher._instance = None
+VocabularyMatcher.cache = {}
 
 class TokenSetConcrete:
-    def __new__(cls, *args, **kwargs):
-        if "mask" in kwargs.keys():
-            mask = kwargs["mask"]
-            return super(TokenSetConcrete, cls).__new__(cls)
-        elif "regex" in kwargs.keys():
-            regex = kwargs["regex"]
-            key = "regex:" + regex
-            if key in TokenSetConcrete.cache.keys():
-                return TokenSetConcrete.cache[key]
-            else:
-                TokenSetConcrete.cache[key] = super(TokenSetConcrete, cls).__new__(cls)
-                return TokenSetConcrete.cache[key]
-        elif "charlen" in kwargs.keys():
-            key = "charlen:" + str(kwargs["charlen"])
-            if key in TokenSetConcrete.cache.keys():
-                return TokenSetConcrete.cache[key]
-            else:
-                TokenSetConcrete.cache[key] = super(TokenSetConcrete, cls).__new__(cls)
-                return TokenSetConcrete.cache[key]
-        else:
-            tokens = kwargs.get("tokens", args[0])
-            assert tokens is not None
-        
-            minus = kwargs.get("minus", False)
-            prefix = kwargs.get("prefix", False)
-            
-            t = ("prefix " if prefix else "") + ("* \ " if minus else "") + "|".join(sorted(list(tokens)))
-            
-            if t in TokenSetConcrete.cache.keys():
-                return TokenSetConcrete.cache[t]
-            else:
-                TokenSetConcrete.cache[t] = super(TokenSetConcrete, cls).__new__(cls)
-                return TokenSetConcrete.cache[t]
-
-    def __init__(self, tokens=None, minus=False, mask=None, regex=None, prefix=False, exact=False, charlen=None):
+    def __init__(self, tokens=None, minus=False, mask=None, regex=None, prefix=False, exact=False, charlen=None, name=None):
         VocabularyMatcher.ensure_ready()
 
         if mask is not None:
             self.mask = mask.copy()
         else: 
-            self.mask = VocabularyMatcher.instance().make_mask(tokens=tokens, regex=regex, minus=minus, prefix=prefix, exact=exact, charlen=charlen)
+            self.mask = VocabularyMatcher.instance().make_mask(tokens=tokens, regex=regex, minus=minus, prefix=prefix, exact=exact, charlen=charlen, name=name)
 
         self._token_str = None
         # for TokenSetSymbolic compatibility
         self.minusset = False
 
     def union(self, other):
         if other == "∅": 
@@ -403,23 +467,23 @@
     if p1 == "*": return p1
     if p2 == "*": return p2
     if p1 == "∅": return p2
     if p2 == "∅": return p1
 
     return p1.union(p2)
 
-def tset(*tokens, regex=False, prefix=False, exact=False, charlen=None):
+def tset(*tokens, regex=False, prefix=False, exact=False, charlen=None, name=None):
     if charlen is not None:
-        return TokenSet(charlen=charlen)
+        return TokenSet(charlen=charlen, name=name)
     if regex:
         assert len(tokens) == 1, "cannot create a TokenSet from multiple regexes."
-        return TokenSet(regex=tokens[0])
+        return TokenSet(regex=tokens[0], name=name)
     if len(tokens) == 1 and type(tokens[0]) is set:
-        return TokenSet(set(list(tokens[0])), minus=False)
-    return TokenSet(set(tokens), minus=False, prefix=prefix, exact=exact)
+        return TokenSet(set(list(tokens[0])), minus=False, name=name)
+    return TokenSet(set(tokens), minus=False, prefix=prefix, exact=exact, name=name)
 
 def ntset(*tokens):
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=True)
     return TokenSet(set(tokens), minus=True)
 
 class ArgTuple(tuple):
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.5/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.5/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 import pickle
 import os
 import time
 from functools import total_ordering
 
 from .openai_api import complete, OpenAIRateLimitError, Capacity
 
+global logit_bias_logging
+logit_bias_logging = True
+
+def set_logit_bias_logging(value):
+    global logit_bias_logging
+    logit_bias_logging = value
+
 class EmptyStreamError(Exception): pass
 
 class ChaosException(openai.APIError): pass
 class MaximumRetriesExceeded(Exception): 
     def __init__(self, error: Exception, retries: int):
         self.error = error
         self.retries = retries
@@ -649,15 +656,17 @@
         if "logit_bias" in kwargs and len(kwargs["logit_bias"]) > 300:
             biases = list(kwargs["logit_bias"].items())
             # make sure to always include eos if set and truncating
             if 50256 in kwargs["logit_bias"]:
                 biases = biases[:299] + [(50256, kwargs["logit_bias"][50256])]
             else:
                 biases = biases[:300]
-            print("warning: the required logit_bias is too large to be handled by the OpenAI API and will be limited to the first 300 tokens. This can lead to the violation of the provided constraints or undesired model output. To avoid this use less broad or no constraints.")
+            global logit_bias_logging
+            if logit_bias_logging:
+                print("warning: the required logit_bias is too large to be handled by the OpenAI API and will be limited to the first 300 tokens. This can lead to the violation of the provided constraints or undesired model output. To avoid this use less broad or no constraints.", file=sys.stderr)
             kwargs["logit_bias"] = {t:b for t,b in biases}
 
 
         assert kwargs.get("echo", False), f"bopenai requires echo=True for to enable proper error recovery. Please handle proper prompt removal in client code."
 
         r = RequestQueueItem(kwargs, request_id)
         await self.complete_api_call_queue.put(r)
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.5/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.5/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.5/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.5/src/lmql/runtime/dclib/dclib_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
 from collections import namedtuple
 from typing import List, Union
 
 from .dclib_array import DataArray
 from .dclib_global import stats
-from .dclib_seq import DecoderSequence, detseq, deepcopy, deepmerge, DecoderSequence, DeterministicDecoderSequence
+from .dclib_seq import DecoderSequence, detseq, deepcopy, deepmerge, DecoderSequence, DeterministicDecoderSequence, Continuation
 import numpy as np
 from lmql.utils import nputil
 from dataclasses import dataclass
 import sys
 
+from lmql.runtime.stats import Stats
+
 @dataclass
 class DcModelLogitsTask:
     model: any
     input_ids: np.ndarray
     logits_mask: np.ndarray
     kwargs: dict
     result_fut: asyncio.Future
@@ -92,31 +94,34 @@
             vocab_size = existing[0].shape[1] if existing[0].ndim == 2 else existing[0].shape[0]
             lm = np.stack([m if m is not None else np.zeros((vocab_size), dtype=np.bool) for m in logit_masks])
             return lm
 
 ModelQueue._instances = {}
 
 class DcModel:
-    def __init__(self, model, bos_token_id, eos_token_id, truncation_threshold=-3e38, init_workers=True, **kwargs):
+    def __init__(self, model, tokenizer, truncation_threshold=-3e38, init_workers=True, **kwargs):
         """
         Parameters:
         
         model: The model to use for inference.
         bos_token_id: The token id to use for the beginning of a sequence.
         eos_token_id: The token id to use for the end of a sequence.
         truncation_threshold: The threshold to use for logit truncation (cf. DecoderSequence.truncation_threshold). Logits below this threshold are considered to be -inf and will never be considered as next token.
         """
         self.model = model
+        self.tokenizer = tokenizer
         self.model_identifier = model.model_identifier
         self.model_args = kwargs
 
-        self.bos_token_id = bos_token_id
-        self.eos_token_id = eos_token_id
+        self.bos_token_id = tokenizer.bos_token_id
+        self.eos_token_id = tokenizer.eos_token_id
         self.truncation_threshold = truncation_threshold
 
+        self.stats = Stats("dcmodel")
+
         if init_workers: self.logits_queue = ModelQueue.get(self.model_identifier)
         else: self.logits_queue = None
 
     def log_billable_tokens(self, n: int):
         if hasattr(self.model, "billable_tokens"):
             self.model.billable_tokens += n
         
@@ -182,52 +187,58 @@
             else:
                 result_logits.append(processed_logits[ptr])
                 result_raw.append(processed_logits_raw[ptr])
                 ptr += 1
         
         return np.stack(result_logits, axis=0), np.stack(result_raw, axis=0)
 
-    async def compute_logits_mask(self, input_ids, user_data, is_constrained, **kwargs):
+    async def compute_logits_mask(self, input_ids, user_data, is_constrained, seqs, **kwargs):
+        if "modern_logits_processor" in kwargs:
+            processor = kwargs["modern_logits_processor"]
+            mask = await processor(seqs, additional_logits_processor_mask=is_constrained)
+            return mask
+
         if "dclib_additional_logits_processor" not in kwargs:
             return namedtuple("LogitsMaskResult", ["logits_mask", "user_data"])([None], user_data)
         
         processor = kwargs["dclib_additional_logits_processor"]
         mask = await processor(input_ids, user_data=user_data, additional_logits_processor_mask=is_constrained)
 
         return mask
 
     async def logits(self, seqs, max_batch_size=16, **kwargs):
-        input_ids = [s.input_ids for s in seqs]
-        user_data = [s.data() for s in seqs]
-        cache = [(s.logits, s.raw_logits) if s.logits is not None else None for s in seqs]
-
-        # determine set of sequences that are constrained
-        constrained_seqs = np.array([s.is_query_constrained for s in seqs], dtype=np.bool_)
-
-        # compute logits mask
-        logits_mask_result = await self.compute_logits_mask(input_ids, user_data, constrained_seqs, **kwargs)
-        logits_mask = logits_mask_result.logits_mask
-        if len(logits_mask) == 1 and logits_mask[0] is None: logits_mask = None
-        
-        # update user data with new information obtained when computing logits masks
-        for s, updated_user_data in zip(seqs, logits_mask_result.user_data):
-            if updated_user_data is None: continue
-            # TODO: update instead of reassign
-            s.user_data = updated_user_data
-            s.user_data["set_by"] = "where"
-
-        # compute logits with automatic batching
-        result_logits, result_raw = await self.autobatch_logits_with_cache(self.model, input_ids, max_batch_size=max_batch_size, cache=cache, logits_mask=logits_mask, **kwargs)
-
-        # cache logits in nodes (if self.input_ids is used)
-        for s,logits,raw in zip(seqs, result_logits, result_raw):
-            s.logits = logits
-            s.raw_logits = raw
-        
-        return result_logits, result_raw
+        with self.stats.timer("logits"):
+            input_ids = [s.input_ids for s in seqs]
+            user_data = [s.data() for s in seqs]
+            cache = [(s.logits, s.raw_logits) if s.logits is not None else None for s in seqs]
+
+            # determine set of sequences that are constrained
+            constrained_seqs = np.array([s.is_query_constrained for s in seqs], dtype=np.bool_)
+
+            # compute logits mask
+            logits_mask_result = await self.compute_logits_mask(input_ids, user_data, constrained_seqs, seqs, **kwargs)
+            logits_mask = logits_mask_result.logits_mask
+            if len(logits_mask) == 1 and logits_mask[0] is None: logits_mask = None
+            
+            # update user data with new information obtained when computing logits masks
+            for s, updated_user_data in zip(seqs, logits_mask_result.user_data):
+                if updated_user_data is None: continue
+                # TODO: update instead of reassign
+                s.user_data = updated_user_data
+                s.user_data["set_by"] = "where"
+
+            # compute logits with automatic batching
+            result_logits, result_raw = await self.autobatch_logits_with_cache(self.model, input_ids, max_batch_size=max_batch_size, cache=cache, logits_mask=logits_mask, **kwargs)
+
+            # cache logits in nodes (if self.input_ids is used)
+            for s,logits,raw in zip(seqs, result_logits, result_raw):
+                s.logits = logits
+                s.raw_logits = raw
+            
+            return result_logits, result_raw
 
     async def argmax(self, sequences, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
         kwargs = {**self.model_args, **kwargs}
 
@@ -246,50 +257,63 @@
             next_token_ids = logits.argmax(axis=-1)
             next_token_scores = np.take_along_axis(logits, next_token_ids.reshape(-1,1), axis=-1)
             return [s.make_successors(next_token_ids[i].reshape(1), next_token_scores[i], logits=raw_logits[i]) for i,s in enumerate(seqs)]
         
         return await sequences.aelement_wise(op_argmax)
 
 
-    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, deterministic=False, stop_phrase=False, needs_rewrite=True):
-        assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
-        
-        if max_batch_size is None:
-            max_batch_size = DcModel.batch_size
-        
-        completion = [np.array(cont) for cont in tokens]
-
-        def make_detseq(s, token_score, completion, user_data):
-            return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
-                    next_ids=completion[1:],
-                    logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
-                    next_logprobs=token_score[1:],
-                    deterministic=np.concatenate([s.deterministic, np.array([deterministic])]),
-                    next_deterministic=np.array([deterministic] * len(completion[1:])),
-                    predecessor=s,
-                    user_data=None,
-                    stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
-                    needs_rewrite=needs_rewrite,
-                    sticky_user_data_keys=s.sticky_user_data_keys)
-        results = []
-
-        for i in range(0, len(sqs), max_batch_size):
-            batch_sqs = sqs[i:i+max_batch_size]
-            batch_input_ids = np.stack([s.input_ids for s in batch_sqs], axis=0)
-            batch_completion = np.stack(self.model.right_pad(completion[i:i+max_batch_size], pad_token_id=self.eos_token_id)["input_ids"], axis=0)
+    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False):
+        with self.stats.timer("score"):
+            assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
+            
+            if max_batch_size is None:
+                max_batch_size = DcModel.batch_size
+            
+            completion = [np.array(cont) for cont in tokens]
 
-            token_scores, _ = await self.model.score(
-                batch_input_ids,
-                batch_completion,
-                eos_token_id=self.eos_token_id
-            )
-            for s,c,ts in zip(batch_sqs,completion[i:i+max_batch_size], token_scores):
-                results.append(make_detseq(s, ts[:len(c)], c, s.user_data))
+            def make_detseq(s, token_score, completion):
+                # compose deterministic flags
+                if type(deterministic) is bool:
+                    deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
+                    next_deterministic = np.array([deterministic] * len(completion[1:]))
+                else:
+                    assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored"
+                    deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
+                    next_deterministic = np.array(deterministic[1:])
+
+                return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
+                        next_ids=completion[1:],
+                        logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
+                        next_logprobs=token_score[1:],
+                        deterministic=deterministic_flags,
+                        next_deterministic=next_deterministic,
+                        predecessor=s,
+                        user_data=user_data,
+                        stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
+                        needs_rewrite=needs_rewrite,
+                        sticky_user_data_keys=s.sticky_user_data_keys)
+            results = []
+
+            for i in range(0, len(sqs), max_batch_size):
+                batch_sqs = sqs[i:i+max_batch_size]
+                batch_input_ids = np.stack([s.input_ids for s in batch_sqs], axis=0)
+                batch_completion = np.stack(self.model.right_pad(completion[i:i+max_batch_size], pad_token_id=self.eos_token_id)["input_ids"], axis=0)
+
+                if noscore:
+                    token_scores = np.zeros_like(batch_completion)
+                else:
+                    token_scores, _ = await self.model.score(
+                        batch_input_ids,
+                        batch_completion,
+                        eos_token_id=self.eos_token_id
+                    )
+                for s,c,ts in zip(batch_sqs,completion[i:i+max_batch_size], token_scores):
+                    results.append(make_detseq(s, ts[:len(c)], c))
 
-        return results
+            return results
 
     async def score_old(self, seqs: Union[DataArray, DecoderSequence], tokens: Union[List[int], List[List[int]]], max_batch_size=4, deterministic=False, stop_phrase=False):
         if type(tokens[0]) is int:
             tokens = [tokens]
         
         unwrap = False
         if type(seqs) is DecoderSequence:
@@ -385,105 +409,145 @@
 
         result_items = await asyncio.gather(*[op_topk(path, seqs, k) for path, seqs in sequences.sequences.items()])
         return DataArray(dict(result_items))
     
     def report_stats(self, printer, decoder_step=None):
         self.model.report_stats(printer, decoder_step)
         
-    async def _rewrite_seq(self, seqs_or_seq):
-        # check self.model_args for an input_id_rewriter (e.g. LMQL interpreter)
-        if "input_id_rewriter" not in self.model_args:
+    async def _rewrite_seq(self, seqs_or_seq, noscore=False):
+        # check self.model_args for a "modern_rewriter" key
+        if "modern_rewriter" not in self.model_args:
             return seqs_or_seq
-        rewriter = self.model_args.get("input_id_rewriter", None)
         
         # accept both a single sequence or a list of sequences
         unwrap = lambda v: v
         seqs = seqs_or_seq 
         if type(seqs_or_seq) is not list:
             seqs = [seqs_or_seq]
             unwrap = lambda v: v[0] if type(v) is list and len(v) == 1 else v
 
         # do not rewrite deterministic sequences (rewrite mask set to False)
         mask_seq_to_rewrite = np.array([s.needs_rewrite for s in seqs], dtype=np.bool_)
 
-        rewritten_ids = await rewriter.input_ids_rewriter_fn(
-                input_ids=[s.input_ids for s in seqs], 
-                next_token_scores=[None for _ in range(len(seqs))], 
-                next_token_logprob=[s.logprobs[-1] for s in seqs],
-                mask_seq_to_rewrite=mask_seq_to_rewrite,
-                user_data=[s.data() for s in seqs]
-        )
-        
+        rewriter = self.model_args["modern_rewriter"]
+        rewritten_ids = await rewriter(seqs, mask_seq_to_rewrite)
+    
         # update user data, if rewriter provides it
         for s, user_data in zip(seqs, rewritten_ids.user_data):
             s.user_data = deepmerge(deepcopy(s.user_data), user_data) if user_data is not None else s.user_data
             s.user_data["set_by"] = "rewrite"
 
-        to_append = rewritten_ids.appended_input_ids
-        if to_append is None:
-            to_append = [None for _ in range(len(seqs))]
+        all_updated_ids = rewritten_ids.appended_input_ids
+        if all_updated_ids is None:
+            all_updated_ids = [None for _ in range(len(seqs))]
+
+        # extract the offset of value tokens in appended_ids, before the sequence is deterministic
+        value_offset = rewritten_ids.value_offset
+        if value_offset is None:
+            value_offset = [0 for _ in range(len(seqs))]
 
         # concat existing input_ids (minus eos if strip_eos) with appended input_ids
         rewriting_tasks = []
-        for seqidx, (s, deterministic_ids) in enumerate(zip(seqs, to_append)):
+        for seqidx, (s, updated_ids, offset) in enumerate(zip(seqs, all_updated_ids, value_offset)):
             # run actually rewrites asynchronously
-            rewriting_tasks.append(self._rewrite_seq_task(s, seqidx, seqs, rewritten_ids, deterministic_ids))
+            rewriting_tasks.append(self._rewrite_seq_task(s, seqidx, seqs, rewritten_ids, updated_ids, offset, noscore=noscore))
         rewritten_seqs = [s for s in await asyncio.gather(*rewriting_tasks) if s is not None]
         return unwrap(rewritten_seqs)
 
-    async def _rewrite_seq_task(self, s, seqidx, seqs, rewritten_ids, deterministic_ids):
-        if (deterministic_ids is None or len(deterministic_ids) == 0) and not get_strip_eos(seqidx, rewritten_ids.strip_eos):
+    async def _rewrite_seq_task(self, s, seqidx, seqs, rewritten_ids, updated_ids, value_offset, noscore=False):
+        if (updated_ids is None or len(updated_ids) == 0) and not get_strip_eos(seqidx, rewritten_ids.strip_eos):
             return s
         else:
             ids = _stripped_ids(seqs, seqidx, rewritten_ids.strip_eos)
 
             # if the rewritten sequence is identical to the original sequence, we can just keep the original sequence (with updated user data)
-            if (deterministic_ids is not None) and (len(ids) == len(s.input_ids) - 1 and len(deterministic_ids) == 1 and deterministic_ids[0] == s.input_ids[-1]):
+            if (updated_ids is not None) and (len(ids) == len(s.input_ids) - 1 and len(updated_ids) == 1 and updated_ids[0] == s.input_ids[-1]):
                 return s
-
-            # find the sequence that is continued by the rewritten sequence
-            continued_seq: DecoderSequence = s
-            while continued_seq is not None and len(continued_seq.input_ids) > len(ids):
+            
+            # find the common prefix between the original sequence and the rewritten sequence
+            continued_seq = s
+            # keep track of current continuation seqs, to potentially traverse forward again (matching updated ids)
+            successors = [] 
+            # traverse backwards until continued_seq matches ids in length - 1
+            while len(continued_seq.input_ids) > len(ids) and continued_seq.predecessor is not None:
+                successors.insert(0, continued_seq)
                 continued_seq = continued_seq.predecessor
 
-            assert continued_seq is not None, "error: a rewritten sequence is not a continuation of any sequence already decoded."
+            # traverse forward again, until the sequence no longer matches with updated_ids
+            last_rewrite_offset = len(continued_seq.input_ids)
+            offset = last_rewrite_offset
+            while offset < len(successors) + last_rewrite_offset and \
+                updated_ids is not None and \
+                offset < len(updated_ids) and \
+                successors[offset - last_rewrite_offset].input_ids[-1] == updated_ids[offset]:
+                
+                offset += 1
+                continued_seq = successors[offset - last_rewrite_offset - 1]
+
+            assert continued_seq is not None, "error: a rewritten sequence is not a continuation of any sequence already decoded. Going from {} to {} with common text {}".format(
+                await s.text(),
+                await self.detokenize(updated_ids),
+                # common ids
+                await self.detokenize(ids),
+            )
 
             # align user data
             user_data = continued_seq.extend_user_data(user_data=s.user_data)
-            if "inserted_stopping_phrase" in user_data.keys():
-                del user_data["inserted_stopping_phrase"]
 
-            if deterministic_ids is None:
+            if updated_ids is None:
                 s = DecoderSequence(continued_seq.input_ids, continued_seq.logprobs, continued_seq.deterministic, stop_phrase=continued_seq.stop_phrase, 
                                     predecessor=continued_seq, user_data=user_data, sticky_user_data_keys=continued_seq.sticky_user_data_keys, epsilon_node=True)
+                s.needs_rewrite = False
                 return s
 
-            continuation = (await self.score([continued_seq], [deterministic_ids.reshape(-1)], deterministic=True, stop_phrase=False, needs_rewrite=False))[0]
-            continuation.stop_phrase = s.stop_phrase
-            continuation.user_data = user_data
+            # offset updated_ids to the number of tokens that are already present as continued_seq
+            appended_ids = updated_ids[offset:]
+
+            if len(appended_ids) == 0:
+                return DecoderSequence(continued_seq.input_ids, continued_seq.logprobs, continued_seq.deterministic, stop_phrase=continued_seq.stop_phrase,
+                                    predecessor=continued_seq, user_data=user_data, sticky_user_data_keys=continued_seq.sticky_user_data_keys, epsilon_node=True)
+
+            # check if rewriting action provides user data specifically for the rewritten sequence
+            # user_data = rewritten_ids.rewritten_seq_user_data[seqidx] or user_data
+
+            # value tokens
+            num_value_tokens = value_offset - offset
+            deterministic = [True if i + 1 > num_value_tokens else False for i in range(len(appended_ids))]
+            continuation = (await self.score([continued_seq], [appended_ids], deterministic=deterministic, stop_phrase=False, needs_rewrite=False, user_data=user_data, noscore=noscore))[0]
+            
+            continuation.stop_phrase = s.stop_phrase[:len(continuation.input_ids)]
             continuation.needs_rewrite = False
+            
+            steps = 0
+            while type(continuation) is DeterministicDecoderSequence and len(continuation.next_ids) > 0 and steps < num_value_tokens:
+                continuation.user_data = deepcopy(s.predecessor.user_data)
+                # print("continuation.user_data", continuation.user_data, flush=True)
+                continuation = continuation.extend(Continuation(continuation.next_ids[0], continuation.next_logprobs[0], continuation.user_data))
+                steps += 1
+            
+            continuation.user_data = rewritten_ids.rewritten_seq_user_data[seqidx] or user_data
 
             return continuation
 
-    async def rewrite(self, ar: Union[DataArray, List[DecoderSequence], DecoderSequence]):
+    async def rewrite(self, ar: Union[DataArray, List[DecoderSequence], DecoderSequence], noscore=False):
         """
         Applies the active rewriting strategy (e.g. the LMQL interpreter) to the provided (array of) sequences.
         
         This may add, remove or change tokens in the sequence, including the EOS token.
         """
         if type(ar) is not DataArray:
             return await self._rewrite_seq(ar)
 
         async def op_rewrite(path, seqs):
             """
             Rewrites the sequences in the pool using the rewriting strategy provided in kwargs.
 
             If no rewriting strategy is provided, no rewriting is performed.
             """
-            return path, await self._rewrite_seq(seqs)
+            return path, await self._rewrite_seq(seqs, noscore=noscore)
         
         with stats.timer("rewrite"):
             result_items = await asyncio.gather(*[op_rewrite(path, seqs) for path, seqs in ar.sequences.items()])
         return DataArray(dict(result_items))
 
 DcModel.batch_size = 1
 
@@ -509,15 +573,15 @@
     return AsyncTokenizer(eos_token_id=eos_token_id, bos_token_id=bos_token_id)
 
 def _stripped_ids(seqs, seqidx, strip_eos):
     if strip_eos == True:
         return seqs[seqidx].input_ids[:-1]
     elif type(strip_eos) is list:
         sequence_strip = strip_eos[seqidx]
-        if sequence_strip == True:  
+        if sequence_strip == True:
             return seqs[seqidx].input_ids[:-1]
         elif type(sequence_strip) is int:
             return seqs[seqidx].input_ids[:sequence_strip] 
         else:
             return seqs[seqidx].input_ids
     else:
         return seqs[seqidx].input_ids
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.5/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, Union, Optional
+from typing import List, Any, Union, Optional, NamedTuple
 
 import asyncio
 import numpy as np
 from lmql.utils import nputil
 
 from dataclasses import dataclass
 
@@ -50,15 +50,15 @@
             self.json_snapshot.step_not_updated_count = {}
         
         for k, v in self.nodes.items():
             hash = None
             if diff and k in self.json_snapshot.node_hashes:
                 # this will ignore changes to nodes that have not been updated for 3 steps (may miss changes to nodes that 
                 # are not updated for a long time, careful for now)
-                if k in self.json_snapshot.step_not_updated_count and self.json_snapshot.step_not_updated_count[k] > 2:
+                if k in self.json_snapshot.step_not_updated_count and self.json_snapshot.step_not_updated_count[k] > 4:
                     continue
                 hash = await v.json_hash()
                 if self.json_snapshot.node_hashes[k] == str(hash):
                     self.json_snapshot.step_not_updated_count[k] = self.json_snapshot.step_not_updated_count.get(k, 0) + 1
                     continue
                     
                 # else:
@@ -113,26 +113,26 @@
         if deterministic is None: self.deterministic = np.array([True for _ in range(len(input_ids))])
         else: self.deterministic = deterministic
         assert len(self.deterministic) == len(self.input_ids), "Length of determinism status does not match length of inputs"
 
         # if no stop_phrase is provided assume no tokens to be stop_phrase
         if stop_phrase is None: self.stop_phrase = np.array([False for _ in range(len(input_ids))])
         else: self.stop_phrase = stop_phrase
-        assert len(self.stop_phrase) == len(self.input_ids), "Length of determinism status does not match length of inputs"
+        assert len(self.stop_phrase) == len(self.input_ids), "Length of stop_phrase status does not match length of inputs for {} and {}".format(self.stop_phrase, self.input_ids)
 
         # cache for logits when model is called with this sequence
         self.logits = None
         self.raw_logits = None
 
         if DecoderSequence.graph is not None:
             self.pool = None
 
         self.user_data = user_data
         self.sticky_user_data_keys = sticky_user_data_keys if sticky_user_data_keys is not None else set()
-        self.sticky_user_data_keys.add("head.variable")
+        # self.sticky_user_data_keys.add("head.variable")
 
         # alternative operation that may called to obtain a score in self.score_next_token if self.raw_logits are not available
         self.score_next_tokens_op = None
 
         # indicates to dc.rewrite whether this sequence can be rewritten
         self.needs_rewrite = True
 
@@ -268,14 +268,17 @@
                         return [await self.default(v) for v in o]
                     elif type(o) is tuple:
                         return tuple(await self.default(list(o)))
                     return super().default(o)
                 except:
                     if hasattr(o, "json") and callable(o.json):
                         return await self.default(await o.json())
+                    # check for NamedTuple
+                    elif hasattr(o, "_asdict") and callable(o._asdict):
+                        return await self.default(o._asdict())
                     elif type(o) is int:
                         return o
                     elif type(o) is float:
                         return o
                     elif type(o) is bool:
                         return o
                     else:
@@ -312,15 +315,15 @@
             user_data=self.extend_user_data(continuation),
             sticky_user_data_keys=self.sticky_user_data_keys
         )
 
     def detect_stop_phrase(self, continuation):
         old_stop_phrase = self.stop_phrase
         new_stop_phrase = np.concatenate([old_stop_phrase, np.array([False])])
-        stop_phrases = self.data("head.stopping_phrases.tokenized")
+        stop_phrases = self.data("head").stopping_phrases["tokenized"]
 
         if stop_phrases is None:
             return new_stop_phrase
 
         ids = np.concatenate([self.input_ids, continuation.token.reshape(1)]),
         for stop in stop_phrases:
             len_stop = len(stop)
@@ -333,16 +336,22 @@
     def __len__(self):
         return len(self.input_ids)
 
     def __repr__(self) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
-    async def text(self) -> str:
-        return str([await get_tokenizer().decode(self.input_ids)])
+    async def text(self, offset:int=None, limit:int=None, pretty=True) -> str:
+        offset = offset or 0
+        limit = limit or len(self.input_ids)
+        raw_text = await get_tokenizer().decode(self.input_ids[offset:limit])
+        if not pretty: 
+            return raw_text
+        else:
+            return str([raw_text])[2:-2]
 
     async def str(self, full=False) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         if detokenize_seqs:
             s = await get_tokenizer().decode(self.input_ids)
             if not full:
                 s = "..." + s[-40:]
@@ -371,14 +380,16 @@
 DecoderSequence.truncation_threshold = -3e38
 
 def resolve_path(d, path):
     if d is None:
         return None
     segments = path.split(".")
     for segment in segments:
+        if hasattr(d, "_asdict") and callable(d._asdict):
+            d = d._asdict()
         if segment not in d:
             return None
         d = d[segment]
     return d
 
 def set_path(d, path, value, create_missing=False, replace=True):
     if d is None:
@@ -424,35 +435,42 @@
         self.needs_rewrite = needs_rewrite
 
         if next_logprobs is not None: assert len(next_logprobs) == len(next_ids), "Length of deterministic continuation did not match length of provided logprobs"
         if next_deterministic is not None: assert len(next_deterministic) == len(next_ids), "Length of determinism status did not match length of provided logrprobs"
 
         self.align_user_data()
 
+    # async def text(self, offset: int = None, limit: int = None, pretty=True) -> str:
+    #     return "<detseq> " + await super().text(offset, limit, pretty)
+
     def align_user_data(self):
+        if self.user_data is None: return
+
         # lmql-specific user data should be different for deterministic sequences
         head_variable = resolve_path(self.user_data, "head.variable")
+
         if head_variable is not None:
-            if "before(" in head_variable:
-                head_variable = head_variable.split(":before(", 1)[0]
-            if head_variable == "__done__":
-                set_path(self.user_data, "head.variable", "__done__")
-            else:
-                if len(self.next_ids) > 0:
-                    set_path(self.user_data, "head.variable", head_variable + ":before(" + str(len(self.next_ids)) + ")")
-                else:
-                    set_path(self.user_data, "head.variable", head_variable)
+            # if "before(" in head_variable:
+            #     head_variable = head_variable.split(":before(", 1)[0]
+            # if head_variable == "__done__":
+            #     set_path(self.user_data, "head", self.user_data["head"].updated(variable="__done__"))
+            # else:
+            #     if len(self.next_ids) > 0:
+            #         set_path(self.user_data, "head", self.user_data["head"].updated(variable=head_variable + ":before(" + str(len(self.next_ids)) + ")"))
+            #     else:
+            #         set_path(self.user_data, "head", self.user_data["head"].updated(variable=head_variable))
             # deterministic sequences don't have stopping phrases
-            set_path(self.user_data, "head.stopping_phrases", {"tokenized": [], "text": []})
+            set_path(self.user_data, "head", self.user_data["head"].updated(stopping_phrases={"tokenized": [], "text": []}))
         else:
-            set_path(self.user_data, "head.variable", "<prompt>")
+            set_path(self.user_data, "head", self.user_data["head"].updated(variable="<prompt>"))
+        
         if len(self.next_ids) > 0:
-            set_path(self.user_data, "head.mask", "{token_id=" + str(self.next_ids[0]) + "}")
+            set_path(self.user_data, "head", self.user_data["head"].updated(mask="{token_id=" + str(self.next_ids[0]) + "}"))
         else:
-            set_path(self.user_data, "head.mask", "<not available yet>")
+            set_path(self.user_data, "head", self.user_data["head"].updated(mask="<not available yet>"))
     
     @property
     def is_query_constrained(self):
         """Deterministic sequences are not query constrained, as long as they are fixed to their predetermined content."""
         return True if len(self.next_ids) == 0 else False
 
     async def json(self):
@@ -469,32 +487,33 @@
             # "input_ids": self.input_ids.tolist(),
             "text": [text],
             "seqtext": seqtext,
             "root": root,
             "logprob": self.logprobs[-1],
             "seqlogprob": self.logprobs.sum(),
             "pool": self.pool,
-            "deterministic": True,
+            **({"deterministic": True} if self.deterministic[-1] else {}),
             "next_ids": self.next_ids.tolist(),
             "next_logprobs": self.next_logprobs.tolist() if self.next_logprobs is not None else None,
             "user_data": await self.user_data_json(),
             "token_id": self.input_ids[-1],
             "deterministic_5": self.deterministic[-5:].tolist(),
             "stop_phrase_5": self.stop_phrase[-5:].tolist(),
             "score_det": alpha_length_normalized.score(self.logprobs[self.prompt_len:][self.deterministic[self.prompt_len:]]),
             "score_nor": alpha_length_normalized.score(self.logprobs[self.prompt_len:][~self.deterministic[self.prompt_len:]]),
             "score_tot": alpha_length_normalized_det.score(self.logprobs, self),
             **({"done": True} if self.data("head.variable") == "__done__" else {}),
             "sticky_user_data_keys": list(self.sticky_user_data_keys)
         }
 
-    def expand(self):
+    def expand(self, limit=None):
         """ Returns the sequence that corresponds to the full expansion of this pre-determined deterministic sequence. """
         s = self
-        while type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0:
+        steps = 0
+        while type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0 and (limit is None or steps < limit):
             s = s.extend(Continuation(s.next_ids[0], s.next_logprobs[0], s.user_data))
         return s
 
     def extend_user_data(self, continuation=None, user_data=None):
         # additionally add self.user_data for deterministic sequence extensions
         return deepmerge(deepcopy(self.user_data), super().extend_user_data(continuation=continuation, user_data=user_data))
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.5/src/lmql/runtime/dclib/decoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,46 +9,47 @@
 from lmql.runtime.stats import Stats
 
 @dc.decoder
 async def argmax(prompt_ids: np.ndarray, n=1, max_len=2048, **kwargs):
     model = dc.model(**kwargs)
     h = dc.seqs([dc.seq(prompt_ids)] * n)
     done = dc.seqs()
-    
     step = 0
     
     # provide early first result to user
     yield h
 
     while len(h) > 0:
         h = h.extend(await model.argmax(h))
-        h = await model.rewrite(h)
+        h = await model.rewrite(h, noscore=True)
         h, done = (h + done).separate_by(dc.logical_not(dc.eos), dc.lt(max_len))
         
         step += 1
-        
+
         yield (h, done)
 
     dc.finish(done)
 
 @dc.decoder
 async def sample(prompt_ids: np.ndarray, temperature=1, n=1, max_len=2048, **kwargs):
     model = dc.model(**kwargs)
     h = dc.seqs([dc.seq(prompt_ids)] * n)
     done = dc.seqs()
 
     while len(h) > 0:
         h = h.extend(await model.sample(h, temperature=temperature))
-        h = await model.rewrite(h)
+        h = await model.rewrite(h, noscore=True)
         h, done = (h + done).separate_by(dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len)))
 
         yield (h, done)
     
     yield (h, done)
 
+    dc.finish(done)
+
 
 @dc.decoder
 async def best_k(prompt_ids: np.ndarray, k=4, budget=30, kappa=1, beta=0.5, gamma=0.05, max_heap_size=500, top_k_continuations=5, max_len=None, **kwargs):
 
     class BestKScorer(dc.topk_scorer):
         def __init__(self, base_scorer, t=0, kappa=1, beta=0.5, *args, **kwargs):
             self.t = t
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.5/src/lmql/runtime/dclib/trie_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict, Union
 import numpy as np
 import asyncio
-from lmql.model.client import ServedPretrainedModel
+from lmql.model.served_model import ServedPretrainedModel
 from lmql.runtime.hf_integration import transformers_model
 
 from .dclib_model import model
 
 from dataclasses import dataclass
 
 class TrieNode:
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/langchain.py` & `lmql-0.0.5/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.5/src/lmql/runtime/lmql_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+"""
+Runtime support used by compiled LMQL query code.
+"""
+
 import inspect
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from lmql.ops.ops import *
-from lmql.runtime.output_writer import silent
-from lmql.runtime.prompt_interpreter import PromptInterpreter, LMQLResult
+from lmql.runtime.langchain import LMQLChainMixIn
 from lmql.runtime.model_registry import LMQLModelRegistry
-from lmql.runtime.postprocessing.conditional_prob import ConditionalDistributionPostprocessor
+from lmql.runtime.output_writer import silent
+from lmql.runtime.interpreter import PromptInterpreter
+from lmql.runtime.postprocessing.conditional_prob import \
+    ConditionalDistributionPostprocessor
 from lmql.runtime.postprocessing.group_by import GroupByPostprocessor
-from lmql.runtime.langchain import LMQLChainMixIn
+
 
 def register_model(identifier, ModelClass):
     LMQLModelRegistry.registry[identifier] = ModelClass
 
 class LMQLInputVariableScope:
     def __init__(self, f, calling_frame):
         self.fct = f
@@ -141,14 +147,20 @@
             for postprocessor in self.postprocessors:
                 results = await postprocessor.process(results, self.output_writer)
         
         interpreter.print_stats()
 
         return results
 
+def context_call(fct_name, *args, **kwargs):
+    return ("call:" + fct_name, args, kwargs)
+
+def interrupt_call(fct_name, *args, **kwargs):
+    return ("interrupt:" + fct_name, args, kwargs)
+
 def tag(t):
     return f"<lmql:{t}/>"
 
 def compiled_query(output_variables=None, group_by=None):
     if output_variables is None:
         output_variables = []
     
@@ -162,8 +174,9 @@
     # TODO validate that only one postprocessor is used
 
     def func_transformer(fct):
         return LMQLQueryFunction(fct, 
                                  output_variables=output_variables, 
                                  postprocessors=postprocessors, 
                                  scope=LMQLInputVariableScope(fct, calling_frame))
-    return func_transformer
+    return func_transformer
+
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/maiohttp.py` & `lmql-0.0.5/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/model_registry.py` & `lmql-0.0.5/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/runtime/openai_integration.py` & `lmql-0.0.5/src/lmql/runtime/openai_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import asyncio
-import os
 import inspect
-import lmql.runtime.bopenai as openai
-from lmql.runtime.stats import Stats
+import os
+from collections import namedtuple
 from dataclasses import dataclass
-from typing import Any, Callable, Optional, List, Union
+from typing import Any, Callable, List, Optional, Union
 
-from collections import namedtuple
 import numpy as np
-from lmql.utils import nputil
-
-from lmql.runtime.decoder_head import DecoderHead
-from lmql.runtime.rewriter import InputIdRewriter, ActivePromptingRewriter
 
-from lmql.runtime.tokenizer import load_tokenizer
-from lmql.runtime.dclib.lmql_adapter import QueryDcLibAdapter
-from lmql.runtime.dclib.dclib_model import DcModel
-from lmql.runtime.dclib.dclib_seq import deepcopy, deepmerge, is_deterministic, detseq, DecoderSequence
+import lmql.runtime.bopenai as openai
 import lmql.runtime.dclib as dc
+from lmql.runtime.dclib.dclib_model import DcModel
+from lmql.runtime.dclib.dclib_seq import (DecoderSequence, deepcopy, deepmerge,
+                                          detseq, is_deterministic)
+from lmql.runtime.stats import Stats
+from lmql.runtime.tokenizer import load_tokenizer
+from lmql.utils import nputil
+
 
 def is_allowed(m): 
     """
     Given a logits mask, sets tensor cell value to True iff the corresponding token is allowed according to the mask.
     """
     return np.isclose(m, 0, atol=1e-8)
 
@@ -107,21 +105,21 @@
         # if available, store reference to output writer for eager stats reporting
         self.output_writer = None
         if "output_writer" in kwargs:
             self.output_writer = kwargs["output_writer"]
         
         self.model_identifier = "openai/" + self.model.model_identifier
 
-        self.model.chunk_size = kwargs.get("openai_chunksize", 32)
+        self.model.chunk_size = kwargs.get("openai_chunksize", 64)
         self.num_billed_tokens = {}
         self.num_requests = 0
 
         self.stats = Stats("openai")
 
-        # openai.Completion.set_chaos(0.05)
+        # openai.Completion.set_chaos(0.05) # for unreliably testing
         openai.AsyncConfiguration.set_tokenizer(self.tokenize)
 
     def log_billable_tokens(self, n: int):
         pass # openai keeps track of billable tokens vai bopenai
     
     def log_queries(self, n: int):
         pass # openai keeps track of queries via bopenai
@@ -132,15 +130,15 @@
 
         Returns Values:
             - (mask_dict, "*"): Complete with the full vocabulary (no logit_bias necessary)
             - (mask_dict, "complete"): Complete with the provided mask mask_dict, to be passed like this to the OpenAI endpoint.
             - (token_id, "fixed"): Complete with the provided token_id with full probability 1.0 (no API use necessary)
 
         """
-        stopping_phrases = s.data("head.stopping_phrases.text")
+        stopping_phrases = s.data("head").stopping_phrases["text"]
 
         if mask is None:
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         invert = False
         num_allowed = is_allowed(mask).sum(axis=-1)
         assert num_allowed > 0, "DclibOpenAiModel: encountered logits mask with no allowed tokens"
@@ -181,37 +179,48 @@
     async def queue_api_score(self, kwargs):
         # put task in self.score_queue and await result
         loop = asyncio.get_running_loop()
         result_fut = loop.create_future()
         self.score_queue.put_nowait((kwargs,result_fut))
         return await result_fut
 
-    async def _score_next_tokens(self, s, next_tokens):
+    async def _score_next_tokens(self, s, next_tokens, noscore=False):
+        if noscore:
+            return np.zeros(len(next_tokens), dtype=np.float32)
         return (await self.api_score(np.concatenate([s.input_ids, next_tokens], axis=0), len(s.input_ids)))
     
-    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic=False, stop_phrase=False, needs_rewrite=True):
+    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False):
         assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
         
         completion = [np.array(cont) for cont in tokens]
 
         def make_detseq(s, token_score, completion):
+            # compose deterministic flags
+            if type(deterministic) is bool:
+                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
+                next_deterministic = np.array([deterministic] * len(completion[1:]))
+            else:
+                assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored"
+                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
+                next_deterministic = np.array(deterministic[1:])
+
             return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
                     next_ids=completion[1:],
                     logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
                     next_logprobs=token_score[1:],
-                    deterministic=np.concatenate([s.deterministic, np.array([deterministic])]),
-                    next_deterministic=np.array([deterministic] * len(completion[1:])),
+                    deterministic=deterministic_flags,
+                    next_deterministic=next_deterministic,
                     predecessor=s,
-                    user_data=None,
+                    user_data=user_data,
                     stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
                     needs_rewrite=needs_rewrite,
                     sticky_user_data_keys=s.sticky_user_data_keys)
         results = []
 
-        for s,compl,result in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl) for s, compl in zip(sqs, completion)))):
+        for s,compl,result in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl, noscore=noscore) for s, compl in zip(sqs, completion)))):
             results.append(make_detseq(s, result, compl))
 
         return results
 
     async def async_complete(self, completion_call: Union[CompletionCall, List[CompletionCall]], **kwargs) -> openai.response_buffer:
         assert type(completion_call) is CompletionCall
 
@@ -340,15 +349,15 @@
     async def completion_buffer(self, seqs, temperature=1, **kwargs):
         kwargs.update({"temperature": temperature})
         
         async def get_buffer(i, s):
             with self.stats.timer("logit_masks"):
                 # print("completion_buffer", s)
                 constrained_seqs = np.array([s.is_query_constrained], dtype=np.bool_)
-                logits_mask_result = await self.compute_logits_mask(s.input_ids.reshape(1, -1), [s.user_data], constrained_seqs, **kwargs)
+                logits_mask_result = await self.compute_logits_mask(s.input_ids.reshape(1, -1), [s.user_data], constrained_seqs, [s], **kwargs)
                 logits_mask = logits_mask_result.logits_mask[0]
 
             # update user data with new information obtained when computing logits masks
             if s.user_data is None:
                 s.user_data = {}
             s.user_data = deepmerge(deepcopy(s.user_data), logits_mask_result.user_data[0])
             s.user_data["set_by"] = "where"
@@ -382,15 +391,14 @@
         return await asyncio.gather(*[get_buffer(i, s) for i, s in enumerate(seqs)])
 
     async def argmax(self, sequences, **kwargs):
         return await self.sample(sequences, num_samples=1, temperature=0)
 
     def report_stats(self, printer, decoder_step=None):
         if printer is None:
-            print("no printer")
             return
         if hasattr(printer, "report_model_stats"):
             s = openai.Completion.get_stats()
             data = {
                 "tokens": s.tokens,
                 "model": self.model_identifier,
                 "req.": s.requests,
@@ -425,15 +433,15 @@
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
                     next_token = complete_data["logprobs"]["tokens"]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
                     next_token_ids.append(np.array([next_token], dtype=np.int64))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
                     
-                    full_logits = np.ones(self.model.tokenizer.vocab_size) * np.finfo(np.float32).min
+                    full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
                     if next_token < len(full_logits):
                         full_logits[next_token] = next_token_score
                     # else: 
                     #  next_token is a special token, which is not in the vocab
                     logits.append(full_logits)
                     continue
 
@@ -443,22 +451,22 @@
                 
                 probs = sorted(list(complete_data["logprobs"]["top_logprobs"].items()))
                 logprobs = [p[1] for p in probs]
                 tokens = [p[0] for p in probs]
                 prob_tokens = await self.tokenize_list(tokens)
                 token_ids = np.array(prob_tokens, dtype=np.int64).reshape(-1)
 
-                full_logits = np.ones(self.model.tokenizer.vocab_size) * np.finfo(np.float32).min
+                full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
                 full_logits[token_ids] = np.array(logprobs)
                 full_logits[next_token] = np.finfo(np.float32).min
                 assert kwargs.get("temperature", 1.0) != 0.0 or np.all(full_logits < next_token_score), "next token score is not the highest"
 
                 # retroactively apply logits mask to logits
                 mask = completion.logit_mask_or_fixed_id
-                if mask is None: 
+                if mask is None:
                     pass
                 elif type(mask) is int: 
                     full_logits[mask] = np.finfo(np.float32).min
                 else: 
                     full_logits[mask < 0] = np.finfo(np.float32).min
 
                 additional_sampled_token_ids, _ = nputil.multinomial(full_logits, num_samples=num_samples - 1)
@@ -473,15 +481,15 @@
                 logits.append(full_logits)
 
             logits = logits
             next_token_ids = next_token_ids
             next_token_scores = next_token_scores
 
             def successor_user_data(continuation_buffer: SequenceResult, num_successors):
-                default_user_data = {"head": {"variable": s.data("head.variable"), "head_index": s.data("head.head_index")}}
+                default_user_data = {}
                 if continuation_buffer.continuation_type is None:
                     return [default_user_data.copy()] * num_successors
                 continuation_as_user_data = {
                     "openai-continuations": {
                         continuation_buffer.continuation_type: continuation_buffer
                     },
                     **(default_user_data.copy())
@@ -523,51 +531,51 @@
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
                     next_token = complete_data["logprobs"]["tokens"]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
                     next_token_ids.append(np.array([next_token], dtype=np.int64))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
                     
-                    full_logits = np.ones(self.model.tokenizer.vocab_size) * np.finfo(np.float32).min
+                    full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
                     full_logits[next_token] = next_token_score
                     logits.append(full_logits)
                     continue
 
                 # get sampled token and score
                 next_token = complete_data["logprobs"]["tokens"][0]
                 next_token_score = complete_data["logprobs"]["token_logprobs"]
                 
                 probs = sorted(list(complete_data["logprobs"]["top_logprobs"].items()), key=lambda x: x[1], reverse=True)
                 logprobs = [p[1] for p in probs]
                 tokens = [p[0] for p in probs]
-                token_ids = np.array([self.model.tokenizer(t)["input_ids"][0] for t in tokens], dtype=np.int64)
+                token_ids = np.array([self.model.get_tokenizer()(t)["input_ids"][0] for t in tokens], dtype=np.int64)
 
                 assert token_ids[0] == next_token, f"top1 logprob token is not the same as the predicted token {token_ids[0]} (top1) != {next_token} (predicted)"
 
-                full_logits = np.ones(self.model.tokenizer.vocab_size) * np.finfo(np.float32).min
+                full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
                 full_logits[token_ids] = np.array(logprobs)
 
                 # retroactively apply logits mask to logits
                 mask = completion.logit_mask_or_fixed_id
                 if mask is None: pass
                 elif type(mask) is int: full_logits[mask] = np.finfo(np.float32).min
                 else: full_logits[mask < 0] = np.finfo(np.float32).min
                 
+                # make sure all token_ids are unique
+                token_ids = np.array(list(set(token_ids)))
+
                 # re-determine logprobs with logits mask applied
                 logprobs = np.take_along_axis(full_logits, token_ids, axis=-1)
 
-                # make sure all token_ids are different
-                assert len(token_ids) == len(set(token_ids)), "token_ids are not unique"
-
                 next_token_ids.append(token_ids)
                 next_token_scores.append(logprobs)
                 logits.append(full_logits)
 
             def successor_user_data(continuation_buffer: SequenceResult, num_successors):
-                default_user_data = {"head": {"variable": s.data("head.variable"), "head_index": s.data("head.head_index")}}
+                default_user_data = {}
                 if continuation_buffer.continuation_type is None:
                     return [default_user_data.copy()] * num_successors
                 continuation_as_user_data = {
                     "openai-continuations": {
                         continuation_buffer.continuation_type: continuation_buffer
                     },
                     **(default_user_data.copy())
@@ -808,15 +816,14 @@
 
         self.num_calls = 0
 
     async def tokenize(self, *args, **kwargs):
         def task():
             return self.tokenizer.encode(*args, **kwargs)
         return await asyncio.get_event_loop().run_in_executor(None, task)
-        return self.tokenizer.tokenize(*args, **kwargs)
     
     async def detokenize(self, *args, **kwargs):
         def task():
             return self.tokenizer.decode(*args, **kwargs)
         return await asyncio.get_event_loop().run_in_executor(None, task)
         # return self.tokenizer.decode(*args, **kwargs)
 
@@ -915,70 +922,35 @@
     def cost_estimate(self, model):
         return openai.AsyncConfiguration.get_stats().cost_estimate(model)
 
 def openai_model(model_identifier):
     # make sure openai org and secret are available
     import lmql.runtime.openai_secret
     
-    class ServedModelInterfaceCls:
+    class OpenAIModel:
         def __init__(self) -> None:
             self.model_identifier = model_identifier
-            self.decoder_args = None
-
-            self.use_dclib_decoders = False
-            self.active_prompting = False
-
             self.served_model = None
             self._tokenizer = None
 
-            self.bos_token_id = self.get_tokenizer().bos_token_id
-            self.eos_token_id = self.get_tokenizer().eos_token_id
-
-            self.adapter = QueryDcLibAdapter(self.get_tokenizer().vocab_size, self.tokenize, self.detokenize, self.bos_token_id, self.eos_token_id)
-            self.hf_stats = HFModelStatsAdapter()
+            self.chunk_size = 64
 
         def get_tokenizer(self):
             if self._tokenizer is None:
                 self._tokenizer = load_tokenizer("gpt2")
-            self.served_model = OptimisticChunkBasedOpenAIModel(model_identifier, self._tokenizer)
+            self.served_model = self
             return self._tokenizer
 
-        def set_decoder(self, method, **kwargs):
-            # defaults
-            DEFAULTS = {
-                "max_len": 512,
-                "decoder": method
-            }
-            self.decoder_args = DEFAULTS.copy()
-
-            # custom user arguments
-            protected_args = set(["input_ids", "additional_logits_processors", "bos_token_id", "eos_token_id"])
-            for key, value in kwargs.items():
-                if key in protected_args:
-                    print("warning: cannot override runtime determined decoder argument {}.".format(key))
-                    continue
-                self.decoder_args[key] = value
-        
         def get_dclib_model(self):
             bos_token_id = self.get_tokenizer().bos_token_id
             eos_token_id = self.get_tokenizer().eos_token_id
 
-            return DclibOpenAiModel(self.served_model, bos_token_id, eos_token_id, **self.decoder_args)
-
-        async def score_distribution_values(self, prompt, values):
-            return await self.adapter.score_distribution_values(prompt, values, self.get_dclib_model())
+            dc.set_dclib_tokenizer(dc.tokenizer("lmql-adapter-tokenizer", self.tokenize, self.detokenize, bos_token_id, eos_token_id))
 
-        async def query(self, prompt, mask_logits_processor, head_input_id_rewriter, active_prompt_rewriter):
-            assert self.decoder_args is not None, "Cannot query() a model without calling set_decoder first."
-
-            dclib_model = self.get_dclib_model()
-            return await self.adapter.query(prompt, mask_logits_processor, head_input_id_rewriter, active_prompt_rewriter, dclib_model, self.decoder_args)
+            return DclibOpenAiModel(self.served_model, self.get_tokenizer())
 
         async def tokenize(self, text):
             return self.get_tokenizer()(text)["input_ids"]
         
         async def detokenize(self, input_ids):
             return self.get_tokenizer().decode(input_ids)
-
-        def sync_tokenize(self, text):
-            return self.get_tokenizer()(text)["input_ids"]
-    return ServedModelInterfaceCls
+    return OpenAIModel
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/openai_secret.py` & `lmql-0.0.5/src/lmql/runtime/openai_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ]
         
         if not any(os.path.exists(p) for p in search_paths):
             m = """api.env not found in any of the following locations:\n\n{}\n\n To use OpenAI models you need to create an api.env file with the following contents:
         openai-secret: <your openai secret>
         openai-org: <your openai org>
         
-        Alternatively, you may just define the environment variable OPENAI_API_KEY=sk-...
+Alternatively, you may just define the environment variable OPENAI_API_KEY=sk-...
         """.format("\n".join(" - " + p for p in search_paths))
             raise FileNotFoundError(m)
 
         valid_paths = [p for p in search_paths if os.path.exists(p)]
 
         # get openai secret from file
         with open(valid_paths[0], "r") as f:
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/program_state.py` & `lmql-0.0.5/src/lmql/runtime/program_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 class ProgramState:
     def __init__(self, runtime=None):
         self.variable_values = {}
+        # postprocessed, converted variable values if not just str (e.g. objects, int)
+        self.variable_program_values = {}
         self.variable_diffs = {}
         self.variable_scores = {}
         self.variable_monotonicity = {}
 
         self.runtime = runtime
 
     async def json(self):
@@ -16,30 +18,35 @@
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __setitem__(self, key, value):
         self.set(key, value)
 
-    def set(self, name, value, scores=None, diff=None, montonicity="var"):
+    def set(self, name, value, program_value=None, scores=None, diff=None, montonicity="var"):
         self.variable_values[name] = value
+        self.variable_program_values[name] = program_value if program_value is not None else value
         self.variable_diffs[name] = diff
         self.variable_scores[name] = scores
         self.variable_monotonicity[name] = montonicity
 
     def get(self, name, default=None):
         return self.variable_values.get(name, default)
+
+    def get_program_value(self, name, default=None):
+        return self.variable_program_values.get(name, default)
     
     def get_diff(self, name, default=None):
         return self.variable_diffs.get(name, default)
 
     def final(self, name):
         return self.variable_monotonicity.get(name, "var")
 
     def copy(self):
         s = ProgramState()
         s.variable_values = self.variable_values.copy()
+        s.variable_program_values = self.variable_program_values.copy()
         s.variable_monotonicity = self.variable_monotonicity.copy()
         s.variable_diffs = self.variable_diffs.copy()
         s.variable_scores = self.variable_scores.copy()
         s.runtime = self.runtime
         return s
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/stats.py` & `lmql-0.0.5/src/lmql/runtime/stats.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+"""
+Simple environment timer to measure the runtime of different parts of the
+code. 
+
+Usage:
+
+stats = Stats("my_stats") # singleton instance
+
+with stats.timer("my_tag"):
+    # do something
+"""
+
 import time
 
 class StatsTimer:
     def __init__(self, stats, tag):
         self.stats = stats
         self.tag = tag
         self.start = time.time()
```

### Comparing `lmql-0.0.4.2/src/lmql/runtime/tokenizer.py` & `lmql-0.0.5/src/lmql/runtime/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import asyncio
+
 def get_js_tokenizer(model_identifier):
     import js
     from pyodide.ffi import to_js
 
     assert "gpt" in model_identifier, "JS tokenizer only supports GPT models."
 
     class JSBridgedTokenizer:
@@ -56,17 +58,17 @@
 
 global special_token_mappings
 special_token_mappings = {}
 global reverse_special_token_mappings
 reverse_special_token_mappings = {}
 
 class LMQLTokenizer:
-    def __init__(self, tokenizer_impl):
+    def __init__(self, tokenizer_impl, model_identifier):
         self.tokenizer_impl = tokenizer_impl
-
+        self.model_identifier = model_identifier
         self.detokenizer_cache = {}
 
     @property
     def vocab_size(self):
         return self.tokenizer_impl.vocab_size
 
     @property
@@ -129,15 +131,15 @@
 
     def __call__(self, s: str):
         input_ids = []
         unpack = False
         if type(s) is not list:
             s = [s]
             unpack = True
-
+        
         for seq in s:
             chunk_input_ids = []
             for chunk in self.chunk_out_by_tags(seq):
                 if type(chunk) is int:
                     chunk_input_ids.append(chunk)
                 else:
                     chunk_input_ids += self.tokenizer_impl(chunk)["input_ids"]
@@ -193,15 +195,15 @@
         return segments
 
 def load_tokenizer(model_identifier):
     import os
 
     # check environment of USE_JS_TOKENIZER
     if "LMQL_BROWSER" in os.environ:
-        return LMQLTokenizer(get_js_tokenizer(model_identifier))
+        return LMQLTokenizer(get_js_tokenizer(model_identifier), model_identifier)
 
     from transformers import AutoTokenizer
     import torch
 
     # first try to load pickled tokenizer from cache (faster)
     import pickle
     import pathlib
@@ -209,21 +211,21 @@
     cache_dir = pathlib.Path.home() / ".cache" / "lmql"
     cache_dir.mkdir(parents=True, exist_ok=True)
     cache_identifier = model_identifier.replace("/", "-")
     cache_path = cache_dir / f"tokenizer-{cache_identifier}.pkl"
 
     if cache_path.exists():
         with open(cache_path, "rb") as f:
-            return LMQLTokenizer(pickle.load(f))
+            return LMQLTokenizer(pickle.load(f), model_identifier)
     else:
         from transformers import AutoTokenizer
         t = AutoTokenizer.from_pretrained(model_identifier)
         with open(cache_path, "wb") as f:
             pickle.dump(t, f)
-        return LMQLTokenizer(t)
+        return LMQLTokenizer(t, model_identifier)
 
 if __name__ == "__main__":
     import sys
 
     model_identifier = sys.argv[1]
     t = load_tokenizer(model_identifier)
```

### Comparing `lmql-0.0.4.2/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.5/src/lmql/tests/expr_test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import sys
 import ast
 import types
 import astunparse
 import inspect
 from lmql.language.fragment_parser import LMQLQuery
 from lmql.language.compiler import PromptScope, SNFList, WhereClauseTransformation
-from lmql.ops.ops import NextToken
-from lmql.runtime.prompt_interpreter import ProgramState, digest
+from lmql.ops.ops import NextToken, digest
+from lmql.runtime.program_state import ProgramState
+
 
 global show_transformed
 show_transformed = False
 
 SEQ = "<SEQ placeholder>"
 
 class LMQLExpr:
```

### Comparing `lmql-0.0.4.2/src/lmql/tests/mask_product_test.py` & `lmql-0.0.5/src/lmql/tests/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/monotonicity.py` & `lmql-0.0.5/src/lmql/tests/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/one_of_tests.py` & `lmql-0.0.5/src/lmql/tests/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/sentences_op.py` & `lmql-0.0.5/src/lmql/tests/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/starts_with_op_test.py` & `lmql-0.0.5/src/lmql/tests/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/stops_at.py` & `lmql-0.0.5/src/lmql/tests/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/str_in_str_tests.py` & `lmql-0.0.5/src/lmql/tests/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.5/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/test_multi_head.py` & `lmql-0.0.5/src/lmql/tests/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/tests/token_set_test.py` & `lmql-0.0.5/src/lmql/tests/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/live/live.js` & `lmql-0.0.5/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/live/live.py` & `lmql-0.0.5/src/lmql/ui/live/live.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,16 @@
     def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         from lmql.utils.graph import CytoscapeGraphWriter
         
         def node_data(op):
             result = "-"
             if trace is not None and op in trace:
                 result = trace[op]
-
-            follow_map = "-"
-            if hasattr(op, "follow_map"):
-                follow_map = str(op.follow_map)
+                follow_map = "<follow_map output not supporte>"
+            
             return {
                 "result": result,
                 "follow_map": follow_map,
                 "repr": repr(op)
             }
 
         writer = CytoscapeGraphWriter(extra_data_provider=node_data)
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/live/livelib.py` & `lmql-0.0.5/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/live/yarn.lock` & `lmql-0.0.5/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/README.md` & `lmql-0.0.5/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/package.json` & `lmql-0.0.5/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.5/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/index.html` & `lmql-0.0.5/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.5/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.5/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.5/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.5/src/lmql/ui/playground/src/App.jsx`

 * *Files 1% similar despite different names*

```diff
@@ -38,31 +38,31 @@
   /* width: 900pt; */
   display: flex;
   flex-direction: column;
   justify-content: flex-start;
   
   color: white;
   flex: 1;
-  height: calc(100% - 40pt);
-  width: 100%;
   position: fixed;
   top: 0;
   left: 0;
-  width: 100%;
-  height: 100%;
+  width: calc(100% - 4pt);
+  height: calc(100% - 2pt);
+  margin: 2pt;
 `;
 
 const Panel = styled.div.attrs(props => ({ className: "panel" }))`
   /* min-height: 300pt; */
   background-color: ${bg};
   border-radius: 5pt;
   padding: 10px;
   display: flex;
   flex-direction: column;
-  margin-left: 2.5pt;
+  margin-left: 1.5pt;
+  margin-right: 1.5pt;
   width: 40%;
   position: relative;
 
   // animate width and opacity change
   transition: width 0.1s, opacity 0.1s, padding 0.1s;
   overflow: hidden;
 
@@ -793,19 +793,20 @@
   }
 
   div .variable {
     color: white;
     background-color: #333;
     opacity: 1.0;
     border-radius: 2pt;
-    margin-left: 1pt;
+    margin-left: 2pt;
   }
 
   div .variable:hover {
     position: relative;
+    transform: scale(1.1);
   }
 
   div .badge {
     padding: 2.5pt 4pt;
     border-radius: 2pt;
     font-size: 8pt;
     background-color: rgba(0, 0, 0, 0.5);
@@ -1846,14 +1847,32 @@
   justify-content: flex-start;
   align-items: center;
   margin-bottom: 0pt;
 
   .bottom {
     margin-top: 40pt;
   }
+
+  >a {
+    display: block;
+    margin: 4pt;
+    margin-left: 8pt;
+    font-size: 10pt;
+    color: black;
+
+    text-decoration: none;
+
+    @media screen and (max-width: 40em) {
+      display: none;
+    }
+
+    :hover {
+      text-decoration: underline;
+    }
+  }
 `
 
 const ButtonGroup = styled.div`
   display: flex;
   background-color: ${bg};
   padding: 4pt;
   padding-left: 2pt;
@@ -1901,15 +1920,15 @@
         background-color: #5db77a31;
         border-color: transparent;
         color: #ffffff44;
       }
     }
   }
 
-  @media (max-width: 40em) {
+  @media (max-width: 50em) {
     &.in-toolbar {
       position: absolute;
       bottom: 20pt;
       right: 20pt;
       z-index: 999;
 
       box-shadow: 0 0 40pt 0pt #100f1f44;
@@ -2427,19 +2446,36 @@
     LMQLProcess.addRenderer(this)
     LMQLProcess.addStatusListener(this.onStatus.bind(this))
 
     BUILD_INFO.addListener(this.setBuildInfo.bind(this))
 
     // when document browser scale is changed
     window.addEventListener("resize", ResizeObservers.notify)
+    
+    this.onKeyDown = this.onKeyDown.bind(this)
+    window.addEventListener("keydown", this.onKeyDown)
+  }
+
+  onKeyDown(event) {
+    /* On R*/
+    if (event.keyCode == 82 && event.ctrlKey) {
+      this.onRun();
+    }
+    /* On Escape */
+    if (event.keyCode == 27) {
+      LMQLProcess.kill();
+    }
   }
 
   componentWillUnmount() {
     LMQLProcess.remove("render", this)
     LMQLProcess.remove("status", this.onStatus.bind(this))
+    
+    window.removeEventListener("resize", ResizeObservers.notify)
+    window.removeEventListener("keydown", this.onKeyDown)
   }
 
   onExportState() {
     let graphData = persistedState.dump()
     let dataUrl = "data:text/json;charset=utf-8," + encodeURIComponent(graphData)
     // trigger download of data
     let a = document.createElement('a');
@@ -2509,24 +2545,26 @@
 
   render() {
     trackingState.setSelectedNode = n => {
       this.onSelectNode(n)
       this.state.selectedNodeTrigger.trigger(n)
     };
 
-    const simpleModeClassName = this.state.simpleMode ? "" : "simple-mode";
+    const simpleModeClassName = (this.state.simpleMode && displayState.mode != "embed") ? "" : "simple-mode";
 
     return (
       <ContentContainer className={this.state.graphLayout ? 'graph-layout' : ''}>
         {displayState.mode != "embed" && <Toolbar>
           <Title>
             <img src="/lmql.svg" alt="LMQL Logo"/>  
             LMQL Playground
           </Title>
           {configuration.DEMO_MODE && <FancyButton className="in-toolbar" onClick={() => ExploreState.setVisibility(true)}><ExploreIc/> Explore LMQL</FancyButton>}
+          {window.location.hostname.includes("lmql.ai") && <a href={"https://docs.lmql.ai/en/latest/quickstart.html"} target="_blank" rel="noreferrer" className="hidden-on-small">
+          Install LMQL Locally </a>}
           <Spacer />
           {/* show tooltip with build time */}
           {/* trigger button */}
           {/* <ToggleButton onClick={() => this.setGraphLayout(!this.state.graphLayout)} toggled={this.state.graphLayout}>
             <BsLayoutWtf size={14} />
           </ToggleButton> */}
           <ToggleButton onClick={() => this.setSimpleMode(!this.state.simpleMode)} toggled={this.state.simpleMode} className="hidden-on-small">
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.5/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.5/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.5/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.5/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.5/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.5/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/State.js` & `lmql-0.0.5/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.5/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         let cy = cyRef.current
 
         if (cy) {
               setActiveNode(null)
               cy.nodes().remove()
               cy.edges().remove()
 
-              if (!props.graph) return;
+              if (!props.graph || props.graph == "None") return;
 
               props.graph.nodes.forEach(n => {
                   let label = n.data.label;
                   n.data.original_label = label
 
                   // check and remove prefix <class 'lmql.ops.ops.Lt'>
                   if (label.startsWith("<class 'lmql.ops.ops.")) {
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.5/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.5/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -85,14 +85,15 @@
             "sample",
             "FROM",
             "from",
             "WHERE",
             "where",
             "DISTRIBUTION",
             "distribution",
+            "context",
 
             // This section is the result of running
             // `import keyword; for k in sorted(keyword.kwlist + keyword.softkwlist): print("  '" + k + "',")`
             // in a Python REPL,
             // though note that the output from Python 3 is not a strict superset of the
             // output from Python 2.
             'False', // promoted to keyword.kwlist in Python 3
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.5/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.5/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.5/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/index.css` & `lmql-0.0.5/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.5/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.5/src/lmql/ui/playground/src/queries.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -59,16 +59,15 @@
    "openai/text-davinci-003"
 where
    RESULT in ["A", "B", "C", "D", "E", "F"]`,
                 state: 'precomputed/cot.json'
             }, {
                 name: "👩‍🔬 Meta Prompting",
                 description: "Asking an expert to answer.",
-                code: `
-# metaprompting based on https://arxiv.org/pdf/2102.07350.pdf
+                code: `# metaprompting based on https://arxiv.org/pdf/2102.07350.pdf
 beam(n=2)
    "Q: What are Large Language Models?\\n\\n"
    "A good person to answer this question would be[EXPERT]\\n\\n"
    expert_name = EXPERT.rstrip(".\\n")
    "For instance,{expert_name} would answer[ANSWER]"
 from 
    "openai/text-davinci-001"
@@ -198,14 +197,15 @@
    "openai/text-davinci-003"
 distribution
    CLASSIFICATION in [" positive", " neutral", " negative"]`,
                 state: 'precomputed/distribution.json'
             }]
         }, {
             category: "Chatbots",
+            requires_input: true,
             queries: [{
                 name: "🗣️ Chatbot",
                 description: "Build a chatbot using interactive querying.",
                 code: `argmax 
    "{:system} You are a marketing chatbot for the language model query language (LMQL)."
    for i in range(10):
       "{:user} {await input()}"
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.5/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.5/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.5/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.5/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.5/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.5/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.5/src/lmql/ui/vscode/LICENSE`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,214 @@
-MIT License
+Copyright 2022- The LMQL Language Team. All rights reserved.
 
-Copyright (c) 2023 lmql-lang
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+   1. Definitions.
 
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
 ================================================================================
 
-The project also includes two files adapted from the huggingface/tranformers project:
+The project also includes one file adapted from the huggingface/tranformers project:
 
-- hf_beam_search.py
 - async_generation_utils.py
 
 These files are adapted from their original project and redistributed according to the following license agreement:
 
 Copyright 2018- The Hugging Face team. All rights reserved.
 
                                  Apache License
```

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.5/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.5/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/package.json` & `lmql-0.0.5/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.5/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/utils/graph.py` & `lmql-0.0.5/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.4.2/src/lmql/utils/nputil.py` & `lmql-0.0.5/src/lmql/utils/nputil.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,8 +42,24 @@
 
     return next_token_id, next_token_score
 
 def unsqueeze(a, axis):
     if is_array(a):
         return np.expand_dims(a, axis)
     else:
-        return a
+        return a
+    
+def replace_inf_nan_with_str(d):
+    import math
+
+    if type(d) is dict:
+        for k, v in d.items():
+            d[k] = replace_inf_nan_with_str(v)
+        return d
+    elif type(d) is list:
+        for i, v in enumerate(d):
+            d[i] = replace_inf_nan_with_str(v)
+        return d
+    elif type(d) is float:
+        if math.isinf(d) or math.isnan(d):
+            return str(d)
+    return d
```

### Comparing `lmql-0.0.4.2/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.5/src/lmql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.4.2
+Version: 0.0.5
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.4.2 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.5 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.4.2/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.5/src/lmql.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/python/.gitignore
 docs/source/python/langchain.ipynb
 docs/source/python/lmql.txt
 docs/source/python/python.ipynb
+docs/source/releases/release-0.0.5.md
 scripts/activate-dev.sh
 scripts/pypi-release.sh
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
 scripts/conda/requirements.yml
+src/lmql.svg
 src/lmql/__init__.py
 src/lmql/cli.py
 src/lmql/demo.py
 src/lmql/http.py
 src/lmql/version.py
 src/lmql.egg-info/PKG-INFO
 src/lmql.egg-info/SOURCES.txt
@@ -52,75 +54,64 @@
 src/lmql.egg-info/requires.txt
 src/lmql.egg-info/top_level.txt
 src/lmql/language/__init__.py
 src/lmql/language/compiler.py
 src/lmql/language/fragment_parser.py
 src/lmql/language/qstrings.py
 src/lmql/language/validator.py
-src/lmql/lib/__init__.py
-src/lmql/lib/errors.py
-src/lmql/lib/expr_jitter.py
-src/lmql/lib/scope.py
-src/lmql/lib/state.py
 src/lmql/model/__init__.py
 src/lmql/model/async_generation_utils.py
-src/lmql/model/client.py
-src/lmql/model/hf_beam_search.py
 src/lmql/model/local_client.py
 src/lmql/model/serve.py
+src/lmql/model/served_model.py
 src/lmql/ops/__init__.py
 src/lmql/ops/follow_map.py
 src/lmql/ops/ops.py
 src/lmql/ops/token_set.py
 src/lmql/runtime/__init__.py
-src/lmql/runtime/backtracker.py
-src/lmql/runtime/decoder_head.py
 src/lmql/runtime/hf_integration.py
+src/lmql/runtime/interpreter.py
 src/lmql/runtime/interrupt.py
 src/lmql/runtime/langchain.py
 src/lmql/runtime/lmql_runtime.py
 src/lmql/runtime/maiohttp.py
 src/lmql/runtime/model_registry.py
 src/lmql/runtime/multi_head_interpretation.py
 src/lmql/runtime/openai_integration.py
 src/lmql/runtime/openai_secret.py
 src/lmql/runtime/output_writer.py
 src/lmql/runtime/program_state.py
-src/lmql/runtime/prompt_interpreter.py
-src/lmql/runtime/rewriter.py
-src/lmql/runtime/runtime.py
 src/lmql/runtime/stats.py
-src/lmql/runtime/tok.ipynb
 src/lmql/runtime/tokenizer.py
 src/lmql/runtime/bopenai/__init__.py
 src/lmql/runtime/bopenai/batched_openai.py
 src/lmql/runtime/bopenai/openai_api.py
 src/lmql/runtime/dclib/__init__.py
 src/lmql/runtime/dclib/dclib_array.py
 src/lmql/runtime/dclib/dclib_global.py
 src/lmql/runtime/dclib/dclib_model.py
 src/lmql/runtime/dclib/dclib_seq.py
 src/lmql/runtime/dclib/decoders.py
-src/lmql/runtime/dclib/lmql_adapter.py
 src/lmql/runtime/dclib/trie_cache.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
+src/lmql/tests/README.md
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/mask_product_test.py
 src/lmql/tests/monotonicity.py
 src/lmql/tests/one_of_tests.py
 src/lmql/tests/sentences_op.py
 src/lmql/tests/starts_with_op_test.py
 src/lmql/tests/stops_at.py
 src/lmql/tests/str_in_str_tests.py
 src/lmql/tests/test_multi_head.py
+src/lmql/tests/test_sample_queries.py
 src/lmql/tests/token_set_test.py
 src/lmql/tests/system/basic_use_cases.py
-src/lmql/ui/.DS_Store
 src/lmql/ui/.gitignore
 src/lmql/ui/__init__.py
 src/lmql/ui/live/__init__.py
 src/lmql/ui/live/live.js
 src/lmql/ui/live/live.py
 src/lmql/ui/live/livelib.py
 src/lmql/ui/live/package.json
```

