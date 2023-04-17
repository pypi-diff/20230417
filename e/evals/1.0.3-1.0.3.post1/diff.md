# Comparing `tmp/evals-1.0.3.tar.gz` & `tmp/evals-1.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-1.0.3.tar", last modified: Mon Apr 17 18:34:45 2023, max compression
+gzip compressed data, was "evals-1.0.3.post1.tar", last modified: Mon Apr 17 18:38:40 2023, max compression
```

## Comparing `evals-1.0.3.tar` & `evals-1.0.3.post1.tar`

### file list

```diff
@@ -1,137 +1,296 @@
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.876217 evals-1.0.3/
--rw-r--r--   0 kondrich   (502) staff       (20)     1063 2023-04-17 18:33:55.000000 evals-1.0.3/LICENSE
--rw-r--r--   0 kondrich   (502) staff       (20)       90 2023-04-17 18:34:23.000000 evals-1.0.3/MANIFEST.in
--rw-r--r--   0 kondrich   (502) staff       (20)       94 2023-04-17 18:34:45.875832 evals-1.0.3/PKG-INFO
--rw-r--r--   0 kondrich   (502) staff       (20)     5239 2023-04-17 18:33:55.000000 evals-1.0.3/README.md
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.680714 evals-1.0.3/evals/
--rw-r--r--   0 kondrich   (502) staff       (20)      316 2023-04-17 18:33:55.000000 evals-1.0.3/evals/__init__.py
--rw-r--r--   0 kondrich   (502) staff       (20)     2964 2023-04-17 18:33:55.000000 evals-1.0.3/evals/api.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1900 2023-04-17 18:33:55.000000 evals-1.0.3/evals/base.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.686904 evals-1.0.3/evals/cli/
--rw-r--r--   0 kondrich   (502) staff       (20)     5645 2023-04-17 18:33:55.000000 evals-1.0.3/evals/cli/oaieval.py
--rw-r--r--   0 kondrich   (502) staff       (20)     3294 2023-04-17 18:33:55.000000 evals-1.0.3/evals/cli/oaievalset.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.690979 evals-1.0.3/evals/completion_fns/
--rw-r--r--   0 kondrich   (502) staff       (20)        0 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/__init__.py
--rw-r--r--   0 kondrich   (502) staff       (20)     2678 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/cot.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1245 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1068 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/langchain_math.py
--rw-r--r--   0 kondrich   (502) staff       (20)     4941 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/openai.py
--rw-r--r--   0 kondrich   (502) staff       (20)     4422 2023-04-17 18:33:55.000000 evals-1.0.3/evals/completion_fns/retrieval.py
--rw-r--r--   0 kondrich   (502) staff       (20)     5699 2023-04-17 18:33:55.000000 evals-1.0.3/evals/data.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.692152 evals-1.0.3/evals/elsuite/
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.693975 evals-1.0.3/evals/elsuite/basic/
--rw-r--r--   0 kondrich   (502) staff       (20)     1655 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1241 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/basic/includes.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1185 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1831 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/basic/match.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.695168 evals-1.0.3/evals/elsuite/modelgraded/
--rw-r--r--   0 kondrich   (502) staff       (20)     6719 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 kondrich   (502) staff       (20)     9342 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 kondrich   (502) staff       (20)     3805 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 kondrich   (502) staff       (20)     2682 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/translate.py
--rw-r--r--   0 kondrich   (502) staff       (20)     5958 2023-04-17 18:33:55.000000 evals-1.0.3/evals/elsuite/utils.py
--rw-r--r--   0 kondrich   (502) staff       (20)     5534 2023-04-17 18:33:55.000000 evals-1.0.3/evals/eval.py
--rw-r--r--   0 kondrich   (502) staff       (20)     1137 2023-04-17 18:33:55.000000 evals-1.0.3/evals/formatting.py
--rw-r--r--   0 kondrich   (502) staff       (20)     2455 2023-04-17 18:33:55.000000 evals-1.0.3/evals/metrics.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.695572 evals-1.0.3/evals/prompt/
--rw-r--r--   0 kondrich   (502) staff       (20)     4093 2023-04-17 18:33:55.000000 evals-1.0.3/evals/prompt/base.py
--rw-r--r--   0 kondrich   (502) staff       (20)    17237 2023-04-17 18:33:55.000000 evals-1.0.3/evals/record.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.668024 evals-1.0.3/evals/registry/
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.700576 evals-1.0.3/evals/registry/completion_fns/
--rw-r--r--   0 kondrich   (502) staff       (20)      391 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      103 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      524 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.710290 evals-1.0.3/evals/registry/eval_sets/
--rw-r--r--   0 kondrich   (502) staff       (20)       99 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      119 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      560 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      412 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      113 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      312 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.860419 evals-1.0.3/evals/registry/evals/
--rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      297 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      229 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      310 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      159 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      246 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/born-first.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      288 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      305 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      309 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/chess.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      160 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      335 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1287 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      151 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/crepe.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      167 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/determinant.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      202 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      387 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      195 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      254 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/finance.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      183 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      276 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      928 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      265 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      222 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      327 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      198 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      242 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/logic.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      153 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      674 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      278 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1193 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      186 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      292 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      221 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      188 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      378 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      255 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/rot13.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      236 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/rucola.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      199 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      364 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     4472 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      272 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      150 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/taxes.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1218 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      400 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1273 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     3046 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      174 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      365 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/evals/which-is-heavier.yaml
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.873498 evals-1.0.3/evals/registry/modelgraded/
--rw-r--r--   0 kondrich   (502) staff       (20)      492 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      291 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1070 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     1157 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     2564 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 kondrich   (502) staff       (20)     9600 2023-04-17 18:33:55.000000 evals-1.0.3/evals/registry.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.875269 evals-1.0.3/evals/utils/
--rw-r--r--   0 kondrich   (502) staff       (20)     1504 2023-04-17 18:33:55.000000 evals-1.0.3/evals/utils/api_utils.py
--rw-r--r--   0 kondrich   (502) staff       (20)      713 2023-04-17 18:33:55.000000 evals-1.0.3/evals/utils/misc.py
--rw-r--r--   0 kondrich   (502) staff       (20)     3991 2023-04-17 18:33:55.000000 evals-1.0.3/evals/utils/snowflake.py
-drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:34:45.685274 evals-1.0.3/evals.egg-info/
--rw-r--r--   0 kondrich   (502) staff       (20)       94 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/PKG-INFO
--rw-r--r--   0 kondrich   (502) staff       (20)     4361 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/SOURCES.txt
--rw-r--r--   0 kondrich   (502) staff       (20)        1 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/dependency_links.txt
--rw-r--r--   0 kondrich   (502) staff       (20)       90 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/entry_points.txt
--rw-r--r--   0 kondrich   (502) staff       (20)      207 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/requires.txt
--rw-r--r--   0 kondrich   (502) staff       (20)        6 2023-04-17 18:34:45.000000 evals-1.0.3/evals.egg-info/top_level.txt
--rw-r--r--   0 kondrich   (502) staff       (20)      546 2023-04-17 18:34:23.000000 evals-1.0.3/pyproject.toml
--rw-r--r--   0 kondrich   (502) staff       (20)       38 2023-04-17 18:34:45.876316 evals-1.0.3/setup.cfg
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:40.047809 evals-1.0.3.post1/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1063 2023-04-17 18:37:21.000000 evals-1.0.3.post1/LICENSE
+-rw-r--r--   0 kondrich   (502) staff       (20)      136 2023-04-17 18:37:21.000000 evals-1.0.3.post1/MANIFEST.in
+-rw-r--r--   0 kondrich   (502) staff       (20)      100 2023-04-17 18:38:40.047539 evals-1.0.3.post1/PKG-INFO
+-rw-r--r--   0 kondrich   (502) staff       (20)     5239 2023-04-17 18:37:21.000000 evals-1.0.3.post1/README.md
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.829610 evals-1.0.3.post1/evals/
+-rw-r--r--   0 kondrich   (502) staff       (20)      316 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/__init__.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2964 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/api.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1900 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/base.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.834103 evals-1.0.3.post1/evals/cli/
+-rw-r--r--   0 kondrich   (502) staff       (20)     5645 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/cli/oaieval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3294 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/cli/oaievalset.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.837476 evals-1.0.3.post1/evals/completion_fns/
+-rw-r--r--   0 kondrich   (502) staff       (20)        0 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/__init__.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2678 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/cot.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1245 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1068 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     4941 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/openai.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     4422 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/completion_fns/retrieval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5699 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/data.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.838315 evals-1.0.3.post1/evals/elsuite/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.840237 evals-1.0.3.post1/evals/elsuite/basic/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1655 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1241 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/basic/includes.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1185 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1831 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/basic/match.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.842131 evals-1.0.3.post1/evals/elsuite/modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)     6719 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     9342 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3805 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2682 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/translate.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5958 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/elsuite/utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     5534 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/eval.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     1137 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/formatting.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     2455 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/metrics.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.842534 evals-1.0.3.post1/evals/prompt/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4093 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/prompt/base.py
+-rw-r--r--   0 kondrich   (502) staff       (20)    17237 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/record.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.814872 evals-1.0.3.post1/evals/registry/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.843837 evals-1.0.3.post1/evals/registry/completion_fns/
+-rw-r--r--   0 kondrich   (502) staff       (20)      391 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      103 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      524 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.813809 evals-1.0.3.post1/evals/registry/data/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.844330 evals-1.0.3.post1/evals/registry/data/aba_mrpc_true_false/
+-rw-r--r--   0 kondrich   (502) staff       (20)    40248 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/aba_mrpc_true_false/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.845006 evals-1.0.3.post1/evals/registry/data/actors-sequence/
+-rw-r--r--   0 kondrich   (502) staff       (20)    65813 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/actors-sequence/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.847192 evals-1.0.3.post1/evals/registry/data/anagrams/
+-rw-r--r--   0 kondrich   (502) staff       (20)      748 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/anagrams/fewshot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    60081 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/anagrams/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.847873 evals-1.0.3.post1/evals/registry/data/balance_chemical_equation/
+-rw-r--r--   0 kondrich   (502) staff       (20)    45027 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/balance_chemical_equation/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.848490 evals-1.0.3.post1/evals/registry/data/belarusian_lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)    62852 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/belarusian_lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.849010 evals-1.0.3.post1/evals/registry/data/bigrams/
+-rw-r--r--   0 kondrich   (502) staff       (20)    72408 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/bigrams/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.849485 evals-1.0.3.post1/evals/registry/data/born_first/
+-rw-r--r--   0 kondrich   (502) staff       (20)    22392 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/born_first/born_first.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.849927 evals-1.0.3.post1/evals/registry/data/brazilian-lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)  8355773 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/brazilian-lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.855727 evals-1.0.3.post1/evals/registry/data/bulgarian-lexicon/
+-rw-r--r--   0 kondrich   (502) staff       (20)   154565 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/bulgarian-lexicon/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.856335 evals-1.0.3.post1/evals/registry/data/chess/
+-rw-r--r--   0 kondrich   (502) staff       (20)    48775 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/chess/match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.856827 evals-1.0.3.post1/evals/registry/data/chess_piece_count/
+-rw-r--r--   0 kondrich   (502) staff       (20)   155059 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/chess_piece_count/fuzzy_match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.857330 evals-1.0.3.post1/evals/registry/data/complex_replace_characters/
+-rw-r--r--   0 kondrich   (502) staff       (20)    71392 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/complex_replace_characters/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.857900 evals-1.0.3.post1/evals/registry/data/connect4/
+-rw-r--r--   0 kondrich   (502) staff       (20)   271001 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/connect4/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.858749 evals-1.0.3.post1/evals/registry/data/convert-hex-hsl-lightness/
+-rw-r--r--   0 kondrich   (502) staff       (20)   219903 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/convert-hex-hsl-lightness/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.860513 evals-1.0.3.post1/evals/registry/data/coqa/
+-rw-r--r--   0 kondrich   (502) staff       (20)    16912 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/coqa/match.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    33337 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/coqa/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.863150 evals-1.0.3.post1/evals/registry/data/crepe/
+-rw-r--r--   0 kondrich   (502) staff       (20)   795920 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/crepe/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.864279 evals-1.0.3.post1/evals/registry/data/cube-pack/
+-rw-r--r--   0 kondrich   (502) staff       (20)    45998 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/cube-pack/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.864870 evals-1.0.3.post1/evals/registry/data/decrypt_caesar_cipher/
+-rw-r--r--   0 kondrich   (502) staff       (20)  9361003 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/decrypt_caesar_cipher/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.871337 evals-1.0.3.post1/evals/registry/data/determinant/
+-rw-r--r--   0 kondrich   (502) staff       (20)    95681 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/determinant/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.872363 evals-1.0.3.post1/evals/registry/data/diagrammatic_logic/
+-rw-r--r--   0 kondrich   (502) staff       (20)  1924826 2023-04-17 18:37:23.000000 evals-1.0.3.post1/evals/registry/data/diagrammatic_logic/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.874167 evals-1.0.3.post1/evals/registry/data/emotional-intelligence/
+-rw-r--r--   0 kondrich   (502) staff       (20)   117966 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/emotional-intelligence/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.874882 evals-1.0.3.post1/evals/registry/data/escher_sentences/
+-rw-r--r--   0 kondrich   (502) staff       (20)    33240 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/escher_sentences/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.875362 evals-1.0.3.post1/evals/registry/data/finance/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4507 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/finance/credit.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.875835 evals-1.0.3.post1/evals/registry/data/first-letters/
+-rw-r--r--   0 kondrich   (502) staff       (20)    34457 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/first-letters/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.876346 evals-1.0.3.post1/evals/registry/data/formal_logic/
+-rw-r--r--   0 kondrich   (502) staff       (20) 84600957 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/formal_logic/formal_logic_expressions.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.929335 evals-1.0.3.post1/evals/registry/data/forth_stack_sim/
+-rw-r--r--   0 kondrich   (502) staff       (20)   122005 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/forth_stack_sim/basic_samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   322293 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/forth_stack_sim/detailed_samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    25750 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/forth_stack_sim/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.930130 evals-1.0.3.post1/evals/registry/data/heart-disease/
+-rw-r--r--   0 kondrich   (502) staff       (20)   698130 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/heart-disease/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.931411 evals-1.0.3.post1/evals/registry/data/hebrew_rhyme/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14045 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/hebrew_rhyme/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.932011 evals-1.0.3.post1/evals/registry/data/illinois-law/
+-rw-r--r--   0 kondrich   (502) staff       (20)   310186 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/illinois-law/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.932832 evals-1.0.3.post1/evals/registry/data/imperial_date_to_string/
+-rw-r--r--   0 kondrich   (502) staff       (20)   337028 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/imperial_date_to_string/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.933741 evals-1.0.3.post1/evals/registry/data/infiniteloop-match/
+-rw-r--r--   0 kondrich   (502) staff       (20)    79881 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/infiniteloop-match/infiniteloop-match.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.934614 evals-1.0.3.post1/evals/registry/data/last_word_nth/
+-rw-r--r--   0 kondrich   (502) staff       (20)    30971 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/last_word_nth/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.935182 evals-1.0.3.post1/evals/registry/data/lat_long_identify/
+-rw-r--r--   0 kondrich   (502) staff       (20)   186974 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/lat_long_identify/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.936298 evals-1.0.3.post1/evals/registry/data/logic/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4833 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/logic/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.938499 evals-1.0.3.post1/evals/registry/data/logic-statements/
+-rw-r--r--   0 kondrich   (502) staff       (20)    55936 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/logic-statements/logic-statements.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.939292 evals-1.0.3.post1/evals/registry/data/logiqa/
+-rw-r--r--   0 kondrich   (502) staff       (20)  2192544 2023-04-17 18:37:23.000000 evals-1.0.3.post1/evals/registry/data/logiqa/logiqa.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.942915 evals-1.0.3.post1/evals/registry/data/manga-translation/
+-rw-r--r--   0 kondrich   (502) staff       (20)   636299 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/manga-translation/bubbles.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   227677 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/manga-translation/pages.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   622876 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/manga-translation/panels.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.943816 evals-1.0.3.post1/evals/registry/data/map-electronic-component-part-to-fact/
+-rw-r--r--   0 kondrich   (502) staff       (20)    32339 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/map-electronic-component-part-to-fact/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.944442 evals-1.0.3.post1/evals/registry/data/mendelian_inheritance/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14338 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/mendelian_inheritance/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.945195 evals-1.0.3.post1/evals/registry/data/moral_exceptQA/
+-rw-r--r--   0 kondrich   (502) staff       (20)    87418 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/moral_exceptQA/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.946446 evals-1.0.3.post1/evals/registry/data/naughty_strings/
+-rw-r--r--   0 kondrich   (502) staff       (20)   102512 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/naughty_strings/samples.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    61312 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/naughty_strings/security.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.947028 evals-1.0.3.post1/evals/registry/data/number_pattern/
+-rw-r--r--   0 kondrich   (502) staff       (20)    51330 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/number_pattern/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.947710 evals-1.0.3.post1/evals/registry/data/number_reading/
+-rw-r--r--   0 kondrich   (502) staff       (20)    22951 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/number_reading/number_reading.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.948287 evals-1.0.3.post1/evals/registry/data/partially_solved_crossword_clues/
+-rw-r--r--   0 kondrich   (502) staff       (20)    30125 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/partially_solved_crossword_clues/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.948899 evals-1.0.3.post1/evals/registry/data/pattern_identification/
+-rw-r--r--   0 kondrich   (502) staff       (20)   172000 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/pattern_identification/samples.v0.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.949826 evals-1.0.3.post1/evals/registry/data/poker_hand_ranks/
+-rw-r--r--   0 kondrich   (502) staff       (20)  2510549 2023-04-17 18:37:23.000000 evals-1.0.3.post1/evals/registry/data/poker_hand_ranks/full_samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.951842 evals-1.0.3.post1/evals/registry/data/reasoning/
+-rw-r--r--   0 kondrich   (502) staff       (20)    19951 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/reasoning/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.952372 evals-1.0.3.post1/evals/registry/data/regex-match/
+-rw-r--r--   0 kondrich   (502) staff       (20)    87293 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/regex-match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.952934 evals-1.0.3.post1/evals/registry/data/reverse_string/
+-rw-r--r--   0 kondrich   (502) staff       (20)     7178 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/reverse_string/reverse_string.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.953563 evals-1.0.3.post1/evals/registry/data/rot13/
+-rw-r--r--   0 kondrich   (502) staff       (20)    49168 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/rot13/rot13.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.954686 evals-1.0.3.post1/evals/registry/data/rucola/
+-rw-r--r--   0 kondrich   (502) staff       (20)     2746 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/rucola/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    75375 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/rucola/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.955425 evals-1.0.3.post1/evals/registry/data/russian-nlp-tasks/
+-rw-r--r--   0 kondrich   (502) staff       (20)    96677 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/russian-nlp-tasks/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.956456 evals-1.0.3.post1/evals/registry/data/sarcasm/
+-rw-r--r--   0 kondrich   (502) staff       (20)      963 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/sarcasm/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)  6906270 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/sarcasm/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.961169 evals-1.0.3.post1/evals/registry/data/simple-knowledge-mongolian/
+-rw-r--r--   0 kondrich   (502) staff       (20)    11069 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/simple-knowledge-mongolian/samples.v0.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.968222 evals-1.0.3.post1/evals/registry/data/stock_options/
+-rw-r--r--   0 kondrich   (502) staff       (20)     5742 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_bear_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     3824 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_bull_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11195 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_inverse_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11103 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_inverse_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    10995 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    11019 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_option_terms_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     9092 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_bear_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     6062 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_bull_call_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16822 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_inverse_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16745 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_inverse_iron_condor_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16688 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_iron_butterfly_spread.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)    16741 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/stock_options/stock_options_iron_condor_spread.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.968916 evals-1.0.3.post1/evals/registry/data/swedish-spelling/
+-rw-r--r--   0 kondrich   (502) staff       (20)    32883 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/swedish-spelling/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.969612 evals-1.0.3.post1/evals/registry/data/taxes/
+-rw-r--r--   0 kondrich   (502) staff       (20)    80167 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/taxes/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.970158 evals-1.0.3.post1/evals/registry/data/test_comp_sci/
+-rw-r--r--   0 kondrich   (502) staff       (20)    14311 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_comp_sci/questions.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.970608 evals-1.0.3.post1/evals/registry/data/test_fuzzy_match/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1503 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_fuzzy_match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.971063 evals-1.0.3.post1/evals/registry/data/test_match/
+-rw-r--r--   0 kondrich   (502) staff       (20)      499 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_match/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.971695 evals-1.0.3.post1/evals/registry/data/test_metaeval/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1712 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_metaeval/joke_fruits_labeled.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.972774 evals-1.0.3.post1/evals/registry/data/test_modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)    19232 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_modelgraded/humor_people_jp.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)      522 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_modelgraded/joke_fruits.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.813047 evals-1.0.3.post1/evals/registry/data/test_multiio/
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.975001 evals-1.0.3.post1/evals/registry/data/test_multiio/battles/
+-rw-r--r--   0 kondrich   (502) staff       (20)      858 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_multiio/battles/joke_animals_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     4863 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_multiio/battles/rap_animals_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5043 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_multiio/battles/rap_people_vs_fruits.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)     5187 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/test_multiio/battles/rap_people_vs_people.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.975458 evals-1.0.3.post1/evals/registry/data/ukraine_eit/
+-rw-r--r--   0 kondrich   (502) staff       (20) 13814472 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/ukraine_eit/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.984582 evals-1.0.3.post1/evals/registry/data/us_tort_law/
+-rw-r--r--   0 kondrich   (502) staff       (20)     4406 2023-04-17 18:37:26.000000 evals-1.0.3.post1/evals/registry/data/us_tort_law/few_shot.jsonl
+-rw-r--r--   0 kondrich   (502) staff       (20)   474865 2023-04-17 18:37:24.000000 evals-1.0.3.post1/evals/registry/data/us_tort_law/samples.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.985369 evals-1.0.3.post1/evals/registry/data/which_is_heavier/
+-rw-r--r--   0 kondrich   (502) staff       (20)    37434 2023-04-17 18:37:25.000000 evals-1.0.3.post1/evals/registry/data/which_is_heavier/which_is_heavier.jsonl
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.988775 evals-1.0.3.post1/evals/registry/eval_sets/
+-rw-r--r--   0 kondrich   (502) staff       (20)       99 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      119 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      560 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      412 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      113 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      312 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:40.037667 evals-1.0.3.post1/evals/registry/evals/
+-rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      297 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      229 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      310 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      159 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      246 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      288 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      305 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      309 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/chess.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      160 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      335 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1287 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      151 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      167 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      202 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      387 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      195 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      254 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/finance.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      183 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      276 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      928 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      250 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      265 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      222 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      327 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      198 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      214 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      242 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/logic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      153 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      674 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      278 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      215 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1193 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      186 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      292 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      258 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      221 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      188 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      175 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      378 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      255 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      236 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      199 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      364 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     4472 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      272 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      150 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1218 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      400 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1273 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      347 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     3046 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      174 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      329 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      365 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/evals/which-is-heavier.yaml
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:40.040992 evals-1.0.3.post1/evals/registry/modelgraded/
+-rw-r--r--   0 kondrich   (502) staff       (20)      492 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      291 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1070 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      274 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     1157 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     2564 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)      230 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 kondrich   (502) staff       (20)     9600 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/registry.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:40.047118 evals-1.0.3.post1/evals/utils/
+-rw-r--r--   0 kondrich   (502) staff       (20)     1504 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/utils/api_utils.py
+-rw-r--r--   0 kondrich   (502) staff       (20)      713 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/utils/misc.py
+-rw-r--r--   0 kondrich   (502) staff       (20)     3991 2023-04-17 18:37:21.000000 evals-1.0.3.post1/evals/utils/snowflake.py
+drwxr-xr-x   0 kondrich   (502) staff       (20)        0 2023-04-17 18:38:39.832977 evals-1.0.3.post1/evals.egg-info/
+-rw-r--r--   0 kondrich   (502) staff       (20)      100 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/PKG-INFO
+-rw-r--r--   0 kondrich   (502) staff       (20)     9375 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/SOURCES.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)        1 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/dependency_links.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)       90 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/entry_points.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)      207 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/requires.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)        6 2023-04-17 18:38:39.000000 evals-1.0.3.post1/evals.egg-info/top_level.txt
+-rw-r--r--   0 kondrich   (502) staff       (20)      552 2023-04-17 18:38:03.000000 evals-1.0.3.post1/pyproject.toml
+-rw-r--r--   0 kondrich   (502) staff       (20)       38 2023-04-17 18:38:40.047881 evals-1.0.3.post1/setup.cfg
```

### Comparing `evals-1.0.3/LICENSE` & `evals-1.0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/README.md` & `evals-1.0.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/api.py` & `evals-1.0.3.post1/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/base.py` & `evals-1.0.3.post1/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/cli/oaieval.py` & `evals-1.0.3.post1/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/cli/oaievalset.py` & `evals-1.0.3.post1/evals/cli/oaievalset.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/completion_fns/cot.py` & `evals-1.0.3.post1/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/completion_fns/langchain_llm.py` & `evals-1.0.3.post1/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/completion_fns/langchain_math.py` & `evals-1.0.3.post1/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/completion_fns/openai.py` & `evals-1.0.3.post1/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/completion_fns/retrieval.py` & `evals-1.0.3.post1/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/data.py` & `evals-1.0.3.post1/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/basic/fuzzy_match.py` & `evals-1.0.3.post1/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/basic/includes.py` & `evals-1.0.3.post1/evals/elsuite/basic/includes.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/basic/json_validator.py` & `evals-1.0.3.post1/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/basic/match.py` & `evals-1.0.3.post1/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/modelgraded/base.py` & `evals-1.0.3.post1/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/modelgraded/classify.py` & `evals-1.0.3.post1/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/modelgraded/classify_utils.py` & `evals-1.0.3.post1/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/translate.py` & `evals-1.0.3.post1/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/elsuite/utils.py` & `evals-1.0.3.post1/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/eval.py` & `evals-1.0.3.post1/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/formatting.py` & `evals-1.0.3.post1/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/metrics.py` & `evals-1.0.3.post1/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/prompt/base.py` & `evals-1.0.3.post1/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/record.py` & `evals-1.0.3.post1/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/completion_fns/langchain_llms.yaml` & `evals-1.0.3.post1/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/eval_sets/stock-options.yaml` & `evals-1.0.3.post1/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/coqa-ex.yaml` & `evals-1.0.3.post1/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/forth-stack-sim.yaml` & `evals-1.0.3.post1/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/manga-translation.yaml` & `evals-1.0.3.post1/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/naughty_strings.yaml` & `evals-1.0.3.post1/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/stock-options.yaml` & `evals-1.0.3.post1/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/test-basic.yaml` & `evals-1.0.3.post1/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-1.0.3.post1/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/evals/test-modelgraded.yaml` & `evals-1.0.3.post1/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/modelgraded/closedqa.yaml` & `evals-1.0.3.post1/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/modelgraded/fact.yaml` & `evals-1.0.3.post1/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry/modelgraded/humor.yaml` & `evals-1.0.3.post1/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/registry.py` & `evals-1.0.3.post1/evals/registry.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/utils/api_utils.py` & `evals-1.0.3.post1/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/utils/misc.py` & `evals-1.0.3.post1/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/evals/utils/snowflake.py` & `evals-1.0.3.post1/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-1.0.3/pyproject.toml` & `evals-1.0.3.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "evals"
-version = "1.0.3"
+version = "1.0.3.post1"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
```

