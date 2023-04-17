# Comparing `tmp/similarities-1.0.4.tar.gz` & `tmp/similarities-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarities-1.0.4.tar", last modified: Sun Dec 11 05:15:28 2022, max compression
+gzip compressed data, was "similarities-1.0.5.tar", last modified: Mon Apr 17 07:03:40 2023, max compression
```

## Comparing `similarities-1.0.4.tar` & `similarities-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-11 05:15:28.936010 similarities-1.0.4/
--rw-r--r--   0 xuming     (501) staff       (20)    20099 2022-12-11 05:15:28.935616 similarities-1.0.4/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    15402 2022-11-28 06:41:39.000000 similarities-1.0.4/README.md
--rw-r--r--   0 xuming     (501) staff       (20)       38 2022-12-11 05:15:28.936193 similarities-1.0.4/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1760 2022-05-24 03:30:40.000000 similarities-1.0.4/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-11 05:15:28.920303 similarities-1.0.4/similarities/
--rw-r--r--   0 xuming     (501) staff       (20)      836 2022-12-11 03:55:29.000000 similarities-1.0.4/similarities/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6773 2022-03-11 13:33:50.000000 similarities-1.0.4/similarities/clip_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4874 2022-03-10 11:02:09.000000 similarities-1.0.4/similarities/data_loader.py
--rw-r--r--   0 xuming     (501) staff       (20)     6761 2022-03-11 09:18:28.000000 similarities-1.0.4/similarities/evaluation.py
--rw-r--r--   0 xuming     (501) staff       (20)     8423 2022-03-10 15:50:38.000000 similarities-1.0.4/similarities/fastsim.py
--rw-r--r--   0 xuming     (501) staff       (20)    17849 2022-03-11 13:36:56.000000 similarities-1.0.4/similarities/imagesim.py
--rw-r--r--   0 xuming     (501) staff       (20)    36781 2022-12-11 05:07:52.000000 similarities-1.0.4/similarities/literalsim.py
--rw-r--r--   0 xuming     (501) staff       (20)     7802 2022-03-12 07:28:53.000000 similarities-1.0.4/similarities/similarity.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-11 05:15:28.933762 similarities-1.0.4/similarities/utils/
--rw-r--r--   0 xuming     (501) staff       (20)      271 2022-03-08 14:06:06.000000 similarities-1.0.4/similarities/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6563 2022-12-11 04:55:59.000000 similarities-1.0.4/similarities/utils/distance.py
--rw-r--r--   0 xuming     (501) staff       (20)     3010 2022-03-11 08:27:51.000000 similarities-1.0.4/similarities/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)    24585 2022-03-07 06:50:41.000000 similarities-1.0.4/similarities/utils/imagehash.py
--rw-r--r--   0 xuming     (501) staff       (20)     6215 2022-03-21 14:07:37.000000 similarities-1.0.4/similarities/utils/ngram_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 similarities-1.0.4/similarities/utils/rank_bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)     2413 2022-09-26 07:54:49.000000 similarities-1.0.4/similarities/utils/tfidf.py
--rw-r--r--   0 xuming     (501) staff       (20)      953 2022-03-03 07:22:03.000000 similarities-1.0.4/similarities/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)    11926 2022-03-09 03:33:22.000000 similarities-1.0.4/similarities/utils/util.py
--rw-r--r--   0 xuming     (501) staff       (20)      102 2022-12-11 05:14:05.000000 similarities-1.0.4/similarities/version.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-11 05:15:28.924532 similarities-1.0.4/similarities.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    20099 2022-12-11 05:15:28.000000 similarities-1.0.4/similarities.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      743 2022-12-11 05:15:28.000000 similarities-1.0.4/similarities.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-12-11 05:15:28.000000 similarities-1.0.4/similarities.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-03-06 17:17:16.000000 similarities-1.0.4/similarities.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       55 2022-12-11 05:15:28.000000 similarities-1.0.4/similarities.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       13 2022-12-11 05:15:28.000000 similarities-1.0.4/similarities.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.578270 similarities-1.0.5/
+-rw-r--r--   0 xuming     (501) staff       (20)    19179 2023-04-17 07:03:40.577900 similarities-1.0.5/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    14874 2023-04-16 03:33:18.000000 similarities-1.0.5/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-04-17 07:03:40.578392 similarities-1.0.5/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1562 2023-04-16 05:28:26.000000 similarities-1.0.5/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.566375 similarities-1.0.5/similarities/
+-rw-r--r--   0 xuming     (501) staff       (20)      836 2022-12-11 03:55:29.000000 similarities-1.0.5/similarities/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6773 2022-03-11 13:33:50.000000 similarities-1.0.5/similarities/clip_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4874 2022-03-10 11:02:09.000000 similarities-1.0.5/similarities/data_loader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6761 2022-03-11 09:18:28.000000 similarities-1.0.5/similarities/evaluation.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9577 2023-04-16 07:54:24.000000 similarities-1.0.5/similarities/fastsim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17682 2023-04-16 06:28:41.000000 similarities-1.0.5/similarities/imagesim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    35902 2023-04-16 06:28:41.000000 similarities-1.0.5/similarities/literalsim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10201 2023-04-16 06:54:36.000000 similarities-1.0.5/similarities/similarity.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.576458 similarities-1.0.5/similarities/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-16 05:45:19.000000 similarities-1.0.5/similarities/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6929 2023-02-01 07:40:21.000000 similarities-1.0.5/similarities/utils/distance.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3010 2022-03-11 08:27:51.000000 similarities-1.0.5/similarities/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)    24585 2022-03-07 06:50:41.000000 similarities-1.0.5/similarities/utils/imagehash.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 similarities-1.0.5/similarities/utils/rank_bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2413 2022-09-26 07:54:49.000000 similarities-1.0.5/similarities/utils/tfidf.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11926 2023-04-16 05:28:26.000000 similarities-1.0.5/similarities/utils/util.py
+-rw-r--r--   0 xuming     (501) staff       (20)      102 2023-04-16 05:28:26.000000 similarities-1.0.5/similarities/version.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.569503 similarities-1.0.5/similarities.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    19179 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      678 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-03-06 17:17:16.000000 similarities-1.0.5/similarities.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       55 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       13 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/top_level.txt
```

### Comparing `similarities-1.0.4/PKG-INFO` & `similarities-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: similarities
-Version: 1.0.4
+Version: 1.0.5
 Summary: Similarities is a toolkit for compute similarity scores between two sets of strings.
 Home-page: https://github.com/shibing624/similarities
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [![PyPI version](https://badge.fury.io/py/similarities.svg)](https://badge.fury.io/py/similarities)
         [![Downloads](https://pepy.tech/badge/similarities)](https://pepy.tech/project/similarities)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/similarities.svg)](https://github.com/shibing624/similarities/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/similarities.svg)](https://github.com/shibing624/similarities/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # Similarities
         
@@ -36,35 +35,35 @@
         
         ### 文本相似度计算（文本匹配）
         - 余弦相似（Cosine Similarity）：两向量求余弦
         - 点积（Dot Product）：两向量归一化后求内积
         - 汉明距离（Hamming Distance），编辑距离（Levenshtein Distance），欧氏距离（Euclidean Distance），曼哈顿距离（Manhattan Distance）等
         
         #### 语义模型
-        - [CoSENT文本匹配模型](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L79)[推荐]
+        - [CoSENT文本匹配模型](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L79)【推荐】
         - BERT模型（文本向量表征）
         - SentenceBERT文本匹配模型
         
         
         #### 字面模型
-        - [Word2Vec文本浅层语义表征](https://github.com/shibing624/similarities/blob/main/similarities/literalsim.py#L374)[推荐]
+        - [Word2Vec文本浅层语义表征](https://github.com/shibing624/similarities/blob/main/similarities/literalsim.py#L374)【推荐】
         - 同义词词林
         - 知网Hownet义原匹配
         - BM25、RankBM25
         - TFIDF
         - SimHash
         
         ### 图像相似度计算（图像匹配）
         #### 语义模型
         - [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
         - VGG(doing)
         - ResNet(doing)
         
         #### 特征提取
-        - [pHash](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L164)[推荐], dHash, wHash, aHash
+        - [pHash](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L164)【推荐】, dHash, wHash, aHash
         - SIFT, Scale Invariant Feature Transform(SIFT)
         - SURF, Speeded Up Robust Features(SURF)(doing)
         
         ### 图文相似度计算
         - [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
         
         ### 匹配搜索
@@ -88,42 +87,20 @@
         | :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
         | Word2Vec | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 10283 |
         | SBERT-multi | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 2371 |
         | Text2vec | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 2572 |
         
         > 结果值使用spearman系数
         
-        Model(doing):
+        Model:
         - Cilin
         - Hownet
         - SimHash
         - TFIDF
         
-        #### 文本检索评测结果
-        
-        | Model | MS MARCO | QPS |
-        | :---- | :-: | :-: |
-        | Word2Vec | - | - |
-        | SBERT-multi | - | - |
-        | Text2vec | - | - |
-        | BM25 | - | - |
-        | ColBERT | - | - |
-        
-        > 结果值使用MRR@10、nDCG@10
-        ### 图像匹配和图像检索
-        #### 图像匹配模型评测结果
-        
-        缺标准评估数据集
-        
-        > 结果值使用F1
-        #### 图像检索评测结果
-        
-        缺标准评估数据集
-        
-        > 结果值使用MRR@10、nDCG@10
         
         
         # Install
         
         ```
         pip3 install torch # conda install pytorch
         pip3 install -U similarities
@@ -154,20 +131,19 @@
         Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
                    model_name_or_path="shibing624/text2vec-base-chinese",
                    max_seq_length=128)
         ```
         
         > 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
         
-        > corpus表示搜索的doc集，仅搜索时需要，输入doc格式兼容：句子列表和{corpus_id: sentence}的dict格式
+        > corpus表示：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
         
-        > model_name_or_path表示模型，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言
-        表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
+        > model_name_or_path表示：模型名称或者模型路径，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
         
-        > max_seq_length表示输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
+        > max_seq_length表示：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
         
         ### 2. 文本语义匹配搜索
         
         一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
         
         example: [examples/base_demo.py](./examples/base_demo.py)
         
@@ -464,14 +440,10 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `similarities-1.0.4/README.md` & `similarities-1.0.5/similarities.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,453 +1,449 @@
-[![PyPI version](https://badge.fury.io/py/similarities.svg)](https://badge.fury.io/py/similarities)
-[![Downloads](https://pepy.tech/badge/similarities)](https://pepy.tech/project/similarities)
-[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/similarities.svg)](https://github.com/shibing624/similarities/graphs/contributors)
-[![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
-[![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
-[![GitHub issues](https://img.shields.io/github/issues/shibing624/similarities.svg)](https://github.com/shibing624/similarities/issues)
-[![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
-
-# Similarities
-
-Similarities is a toolkit for similarity calculation and semantic search, supports text and image.
-
-similarities：相似度计算、语义匹配搜索工具包。
-
-**similarities** 实现了多种相似度计算、匹配搜索算法，支持文本、图像，python3开发，pip安装，开箱即用。
-
-**Guide**
-
-- [Feature](#Feature)
-- [Evaluation](#Evaluation)
-- [Install](#install)
-- [Usage](#usage)
-- [Contact](#Contact)
-- [Reference](#reference)
-
-# Feature
-
-### 文本相似度计算（文本匹配）
-- 余弦相似（Cosine Similarity）：两向量求余弦
-- 点积（Dot Product）：两向量归一化后求内积
-- 汉明距离（Hamming Distance），编辑距离（Levenshtein Distance），欧氏距离（Euclidean Distance），曼哈顿距离（Manhattan Distance）等
-
-#### 语义模型
-- [CoSENT文本匹配模型](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L79)[推荐]
-- BERT模型（文本向量表征）
-- SentenceBERT文本匹配模型
-
-
-#### 字面模型
-- [Word2Vec文本浅层语义表征](https://github.com/shibing624/similarities/blob/main/similarities/literalsim.py#L374)[推荐]
-- 同义词词林
-- 知网Hownet义原匹配
-- BM25、RankBM25
-- TFIDF
-- SimHash
-
-### 图像相似度计算（图像匹配）
-#### 语义模型
-- [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
-- VGG(doing)
-- ResNet(doing)
-
-#### 特征提取
-- [pHash](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L164)[推荐], dHash, wHash, aHash
-- SIFT, Scale Invariant Feature Transform(SIFT)
-- SURF, Speeded Up Robust Features(SURF)(doing)
-
-### 图文相似度计算
-- [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
-
-### 匹配搜索
-- [SemanticSearch](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L185)：向量相似检索，使用Cosine
-  Similarty + topk高效计算，比一对一暴力计算快一个数量级
-
-# Demo
-
-Compute similarity score Demo: https://huggingface.co/spaces/shibing624/text2vec
-
-Semantic Search Demo: https://huggingface.co/spaces/shibing624/similarities
-
-![](docs/hf_search.png)
-
-
-# Evaluation
-### 文本匹配和文本检索
-#### 中文文本匹配模型评测结果
-
-| Model | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
-| :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-| Word2Vec | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 10283 |
-| SBERT-multi | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 2371 |
-| Text2vec | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 2572 |
-
-> 结果值使用spearman系数
-
-Model(doing):
-- Cilin
-- Hownet
-- SimHash
-- TFIDF
-
-#### 文本检索评测结果
-
-| Model | MS MARCO | QPS |
-| :---- | :-: | :-: |
-| Word2Vec | - | - |
-| SBERT-multi | - | - |
-| Text2vec | - | - |
-| BM25 | - | - |
-| ColBERT | - | - |
-
-> 结果值使用MRR@10、nDCG@10
-### 图像匹配和图像检索
-#### 图像匹配模型评测结果
-
-缺标准评估数据集
-
-> 结果值使用F1
-#### 图像检索评测结果
-
-缺标准评估数据集
-
-> 结果值使用MRR@10、nDCG@10
-
-
-# Install
-
-```
-pip3 install torch # conda install pytorch
-pip3 install -U similarities
-```
-
-or
-
-```
-git clone https://github.com/shibing624/similarities.git
-cd similarities
-python3 setup.py install
-```
-
-# Usage
-
-### 1. 文本语义相似度计算
-
-```python
-from similarities import Similarity
-
-m = Similarity()
-r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
-print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
-```
-
-Similarity的默认方法：
-```python
-Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
-           model_name_or_path="shibing624/text2vec-base-chinese",
-           max_seq_length=128)
-```
-
-> 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
-
-> corpus表示搜索的doc集，仅搜索时需要，输入doc格式兼容：句子列表和{corpus_id: sentence}的dict格式
-
-> model_name_or_path表示模型，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言
-表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
-
-> max_seq_length表示输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
-
-### 2. 文本语义匹配搜索
-
-一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
-
-example: [examples/base_demo.py](./examples/base_demo.py)
-
-```python
-import sys
-
-sys.path.append('..')
-from similarities import Similarity
-
-# 1.Compute cosine similarity between two sentences.
-sentences = ['如何更换花呗绑定银行卡',
-             '花呗更改绑定银行卡']
-corpus = [
-    '花呗更改绑定银行卡',
-    '我什么时候开通了花呗',
-    '俄罗斯警告乌克兰反对欧盟协议',
-    '暴风雨掩埋了东北部；新泽西16英寸的降雪',
-    '中央情报局局长访问以色列叙利亚会谈',
-    '人在巴基斯坦基地的炸弹袭击中丧生',
-]
-model = Similarity(model_name_or_path="shibing624/text2vec-base-chinese")
-print(model)
-similarity_score = model.similarity(sentences[0], sentences[1])
-print(f"{sentences[0]} vs {sentences[1]}, score: {float(similarity_score):.4f}")
-
-print('-' * 50 + '\n')
-# 2.Compute similarity between two list
-similarity_scores = model.similarity(sentences, corpus)
-print(similarity_scores.numpy())
-for i in range(len(sentences)):
-    for j in range(len(corpus)):
-        print(f"{sentences[i]} vs {corpus[j]}, score: {similarity_scores.numpy()[i][j]:.4f}")
-
-print('-' * 50 + '\n')
-# 3.Semantic Search
-model.add_corpus(corpus)
-res = model.most_similar(queries=sentences, topn=3)
-print(res)
-for q_id, c in res.items():
-    print('query:', sentences[q_id])
-    print("search top 3:")
-    for corpus_id, s in c.items():
-        print(f'\t{model.corpus[corpus_id]}: {s:.4f}')
-```
-
-output:
-
-```shell
-如何更换花呗绑定银行卡 vs 花呗更改绑定银行卡, score: 0.8551
-...
-
-如何更换花呗绑定银行卡 vs 花呗更改绑定银行卡, score: 0.8551
-如何更换花呗绑定银行卡 vs 我什么时候开通了花呗, score: 0.7212
-如何更换花呗绑定银行卡 vs 俄罗斯警告乌克兰反对欧盟协议, score: 0.1450
-如何更换花呗绑定银行卡 vs 暴风雨掩埋了东北部；新泽西16英寸的降雪, score: 0.2167
-如何更换花呗绑定银行卡 vs 中央情报局局长访问以色列叙利亚会谈, score: 0.2517
-如何更换花呗绑定银行卡 vs 人在巴基斯坦基地的炸弹袭击中丧生, score: 0.0809
-花呗更改绑定银行卡 vs 花呗更改绑定银行卡, score: 1.0000
-花呗更改绑定银行卡 vs 我什么时候开通了花呗, score: 0.6807
-花呗更改绑定银行卡 vs 俄罗斯警告乌克兰反对欧盟协议, score: 0.1714
-花呗更改绑定银行卡 vs 暴风雨掩埋了东北部；新泽西16英寸的降雪, score: 0.2162
-花呗更改绑定银行卡 vs 中央情报局局长访问以色列叙利亚会谈, score: 0.2728
-花呗更改绑定银行卡 vs 人在巴基斯坦基地的炸弹袭击中丧生, score: 0.1279
-
-query: 如何更换花呗绑定银行卡
-search top 3:
-	花呗更改绑定银行卡: 0.8551
-	我什么时候开通了花呗: 0.7212
-	中央情报局局长访问以色列叙利亚会谈: 0.2517
-```
-
-> 余弦`score`的值范围[-1, 1]，值越大，表示该query与corpus的文本越相似。
-
-
-#### 英文语义相似度计算和匹配搜索
-
-example: [examples/base_english_demo.py](./examples/base_english_demo.py)
-
-### 3. 快速近似语义匹配搜索
-
-支持Annoy、Hnswlib的近似语义匹配搜索，常用于百万数据集的匹配搜索任务。
-
-example: [examples/fast_sim_demo.py](./examples/fast_sim_demo.py)
-
-### 4. 基于字面的文本相似度计算和匹配搜索
-
-支持同义词词林（Cilin）、知网Hownet、词向量（WordEmbedding）、Tfidf、SimHash、BM25等算法的相似度计算和字面匹配搜索，常用于文本匹配冷启动。
-
-example: [examples/literal_sim_demo.py](./examples/literal_sim_demo.py)
-
-```python
-from similarities.literalsim import SimHashSimilarity, TfidfSimilarity, BM25Similarity, \
-    WordEmbeddingSimilarity, CilinSimilarity, HownetSimilarity
-
-text1 = "如何更换花呗绑定银行卡"
-text2 = "花呗更改绑定银行卡"
-
-corpus = [
-    '花呗更改绑定银行卡',
-    '我什么时候开通了花呗',
-    '俄罗斯警告乌克兰反对欧盟协议',
-    '暴风雨掩埋了东北部；新泽西16英寸的降雪',
-    '中央情报局局长访问以色列叙利亚会谈',
-    '人在巴基斯坦基地的炸弹袭击中丧生',
-]
-
-queries = [
-    '我的花呗开通了？',
-    '乌克兰被俄罗斯警告'
-]
-m = TfidfSimilarity()
-print(text1, text2, ' sim score: ', m.similarity(text1, text2))
-
-m.add_corpus(corpus)
-res = m.most_similar(queries, topn=3)
-print('sim search: ', res)
-for q_id, c in res.items():
-    print('query:', queries[q_id])
-    print("search top 3:")
-    for corpus_id, s in c.items():
-        print(f'\t{m.corpus[corpus_id]}: {s:.4f}')
-```
-
-output:
-
-```shell
-如何更换花呗绑定银行卡 花呗更改绑定银行卡  sim score:  0.8203384355246909
-
-sim search:  {0: {2: 0.9999999403953552, 1: 0.43930041790008545, 0: 0.0}, 1: {0: 0.7380483150482178, 1: 0.0, 2: 0.0}}
-query: 我的花呗开通了？
-search top 3:
-	我什么时候开通了花呗: 1.0000
-	花呗更改绑定银行卡: 0.4393
-	俄罗斯警告乌克兰反对欧盟协议: 0.0000
-...
-```
-
-### 5. 图像相似度计算和匹配搜索
-
-支持[CLIP](similarities/imagesim.py)、pHash、SIFT等算法的图像相似度计算和匹配搜索。
-
-example: [examples/image_demo.py](./examples/image_demo.py)
-
-```python
-import sys
-import glob
-from PIL import Image
-
-sys.path.append('..')
-from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
-
-
-def sim_and_search(m):
-    print(m)
-    # similarity
-    sim_scores = m.similarity(imgs1, imgs2)
-    print('sim scores: ', sim_scores)
-    for (idx, i), j in zip(enumerate(image_fps1), image_fps2):
-        s = sim_scores[idx] if isinstance(sim_scores, list) else sim_scores[idx][idx]
-        print(f"{i} vs {j}, score: {s:.4f}")
-    # search
-    m.add_corpus(corpus_imgs)
-    queries = imgs1
-    res = m.most_similar(queries, topn=3)
-    print('sim search: ', res)
-    for q_id, c in res.items():
-        print('query:', image_fps1[q_id])
-        print("search top 3:")
-        for corpus_id, s in c.items():
-            print(f'\t{m.corpus[corpus_id].filename}: {s:.4f}')
-    print('-' * 50 + '\n')
-
-image_fps1 = ['data/image1.png', 'data/image3.png']
-image_fps2 = ['data/image12-like-image1.png', 'data/image10.png']
-imgs1 = [Image.open(i) for i in image_fps1]
-imgs2 = [Image.open(i) for i in image_fps2]
-corpus_fps = glob.glob('data/*.jpg') + glob.glob('data/*.png')
-corpus_imgs = [Image.open(i) for i in corpus_fps]
-
-# 2. image and image similarity score
-sim_and_search(ClipSimilarity())  # the best result
-sim_and_search(ImageHashSimilarity(hash_function='phash'))
-sim_and_search(SiftSimilarity())
-```
-
-output:
-
-```shell
-Similarity: ClipSimilarity, matching_model: CLIPModel
-sim scores:  tensor([[0.9580, 0.8654],
-        [0.6558, 0.6145]])
-
-data/image1.png vs data/image12-like-image1.png, score: 0.9580
-data/image3.png vs data/image10.png, score: 0.6145
-
-sim search:  {0: {6: 0.9999999403953552, 0: 0.9579654932022095, 4: 0.9326782822608948}, 1: {8: 0.9999997615814209, 4: 0.6729235649108887, 0: 0.6558331847190857}}
-
-query: data/image1.png
-search top 3:
-	data/image1.png: 1.0000
-	data/image12-like-image1.png: 0.9580
-	data/image8-like-image1.png: 0.9327
-```
-
-![image_sim](docs/image_sim.png)
-
-### 6. 图文互搜
-
-CLIP 模型不仅支持以图搜图，还支持图文互搜：
-```python
-import sys
-import glob
-from PIL import Image
-sys.path.append('..')
-from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
-
-m = ClipSimilarity()
-print(m)
-# similarity score between text and image
-image_fps = ['data/image3.png',  # yellow flower image
-             'data/image1.png']  # tiger image
-texts = ['a yellow flower', 'a tiger']
-imgs = [Image.open(i) for i in image_fps]
-sim_scores = m.similarity(imgs, texts)
-
-print('sim scores: ', sim_scores)
-for (idx, i), j in zip(enumerate(image_fps), texts):
-    s = sim_scores[idx][idx]
-    print(f"{i} vs {j}, score: {s:.4f}")
-```
-
-output:
-
-```shell
-sim scores:  tensor([[0.3220, 0.2409],
-        [0.1677, 0.2959]])
-data/image3.png vs a yellow flower, score: 0.3220
-data/image1.png vs a tiger, score: 0.2959
-```
-
-# Contact
-
-- Issue(建议)
-  ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/similarities.svg)](https://github.com/shibing624/similarities/issues)
-- 邮件我：xuming: xuming624@qq.com
-- 微信我： 加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
-
-<img src="docs/wechat.jpeg" width="200" />
-
-# Citation
-
-如果你在研究中使用了similarities，请按如下格式引用：
-
-APA:
-
-```
-Xu, M. Similarities: Compute similarity score for humans (Version 1.0.1) [Computer software]. https://github.com/shibing624/similarities
-```
-
-BibTeX:
-
-```
-@misc{Xu_Similarities_Compute_similarity,
-  title={Similarities: similarity calculation and semantic search toolkit},
-  author={Xu Ming},
-  year={2022},
-  howpublished={\url{https://github.com/shibing624/similarities}},
-}
-```
-
-# License
-
-授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加similarities的链接和授权协议。
-
-# Contribute
-
-项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
-
-- 在`tests`添加相应的单元测试
-- 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
-
-之后即可提交PR。
-
-# Reference
-
-- [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
-- [liuhuanyong/SentenceSimilarity](https://github.com/liuhuanyong/SentenceSimilarity)
-- [shibing624/text2vec](https://github.com/shibing624/text2vec)
-- [qwertyforce/image_search](https://github.com/qwertyforce/image_search)
-- [ImageHash - Official Github repository](https://github.com/JohannesBuchner/imagehash)
-- [openai/CLIP](https://github.com/openai/CLIP)
+Metadata-Version: 2.1
+Name: similarities
+Version: 1.0.5
+Summary: Similarities is a toolkit for compute similarity scores between two sets of strings.
+Home-page: https://github.com/shibing624/similarities
+Author: XuMing
+Author-email: xuming624@qq.com
+License: Apache License 2.0
+Description: [![PyPI version](https://badge.fury.io/py/similarities.svg)](https://badge.fury.io/py/similarities)
+        [![Downloads](https://pepy.tech/badge/similarities)](https://pepy.tech/project/similarities)
+        [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
+        [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
+        [![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
+        [![GitHub issues](https://img.shields.io/github/issues/shibing624/similarities.svg)](https://github.com/shibing624/similarities/issues)
+        [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
+        
+        # Similarities
+        
+        Similarities is a toolkit for similarity calculation and semantic search, supports text and image.
+        
+        similarities：相似度计算、语义匹配搜索工具包。
+        
+        **similarities** 实现了多种相似度计算、匹配搜索算法，支持文本、图像，python3开发，pip安装，开箱即用。
+        
+        **Guide**
+        
+        - [Feature](#Feature)
+        - [Evaluation](#Evaluation)
+        - [Install](#install)
+        - [Usage](#usage)
+        - [Contact](#Contact)
+        - [Reference](#reference)
+        
+        # Feature
+        
+        ### 文本相似度计算（文本匹配）
+        - 余弦相似（Cosine Similarity）：两向量求余弦
+        - 点积（Dot Product）：两向量归一化后求内积
+        - 汉明距离（Hamming Distance），编辑距离（Levenshtein Distance），欧氏距离（Euclidean Distance），曼哈顿距离（Manhattan Distance）等
+        
+        #### 语义模型
+        - [CoSENT文本匹配模型](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L79)【推荐】
+        - BERT模型（文本向量表征）
+        - SentenceBERT文本匹配模型
+        
+        
+        #### 字面模型
+        - [Word2Vec文本浅层语义表征](https://github.com/shibing624/similarities/blob/main/similarities/literalsim.py#L374)【推荐】
+        - 同义词词林
+        - 知网Hownet义原匹配
+        - BM25、RankBM25
+        - TFIDF
+        - SimHash
+        
+        ### 图像相似度计算（图像匹配）
+        #### 语义模型
+        - [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
+        - VGG(doing)
+        - ResNet(doing)
+        
+        #### 特征提取
+        - [pHash](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L164)【推荐】, dHash, wHash, aHash
+        - SIFT, Scale Invariant Feature Transform(SIFT)
+        - SURF, Speeded Up Robust Features(SURF)(doing)
+        
+        ### 图文相似度计算
+        - [CLIP(Contrastive Language-Image Pre-Training)](https://github.com/shibing624/similarities/blob/main/similarities/imagesim.py#L25)
+        
+        ### 匹配搜索
+        - [SemanticSearch](https://github.com/shibing624/similarities/blob/main/similarities/similarity.py#L185)：向量相似检索，使用Cosine
+          Similarty + topk高效计算，比一对一暴力计算快一个数量级
+        
+        # Demo
+        
+        Compute similarity score Demo: https://huggingface.co/spaces/shibing624/text2vec
+        
+        Semantic Search Demo: https://huggingface.co/spaces/shibing624/similarities
+        
+        ![](docs/hf_search.png)
+        
+        
+        # Evaluation
+        ### 文本匹配和文本检索
+        #### 中文文本匹配模型评测结果
+        
+        | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
+        | :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+        | Word2Vec | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 10283 |
+        | SBERT-multi | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 2371 |
+        | Text2vec | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 2572 |
+        
+        > 结果值使用spearman系数
+        
+        Model:
+        - Cilin
+        - Hownet
+        - SimHash
+        - TFIDF
+        
+        
+        
+        # Install
+        
+        ```
+        pip3 install torch # conda install pytorch
+        pip3 install -U similarities
+        ```
+        
+        or
+        
+        ```
+        git clone https://github.com/shibing624/similarities.git
+        cd similarities
+        python3 setup.py install
+        ```
+        
+        # Usage
+        
+        ### 1. 文本语义相似度计算
+        
+        ```python
+        from similarities import Similarity
+        
+        m = Similarity()
+        r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
+        print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
+        ```
+        
+        Similarity的默认方法：
+        ```python
+        Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
+                   model_name_or_path="shibing624/text2vec-base-chinese",
+                   max_seq_length=128)
+        ```
+        
+        > 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
+        
+        > corpus表示：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
+        
+        > model_name_or_path表示：模型名称或者模型路径，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
+        
+        > max_seq_length表示：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
+        
+        ### 2. 文本语义匹配搜索
+        
+        一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
+        
+        example: [examples/base_demo.py](./examples/base_demo.py)
+        
+        ```python
+        import sys
+        
+        sys.path.append('..')
+        from similarities import Similarity
+        
+        # 1.Compute cosine similarity between two sentences.
+        sentences = ['如何更换花呗绑定银行卡',
+                     '花呗更改绑定银行卡']
+        corpus = [
+            '花呗更改绑定银行卡',
+            '我什么时候开通了花呗',
+            '俄罗斯警告乌克兰反对欧盟协议',
+            '暴风雨掩埋了东北部；新泽西16英寸的降雪',
+            '中央情报局局长访问以色列叙利亚会谈',
+            '人在巴基斯坦基地的炸弹袭击中丧生',
+        ]
+        model = Similarity(model_name_or_path="shibing624/text2vec-base-chinese")
+        print(model)
+        similarity_score = model.similarity(sentences[0], sentences[1])
+        print(f"{sentences[0]} vs {sentences[1]}, score: {float(similarity_score):.4f}")
+        
+        print('-' * 50 + '\n')
+        # 2.Compute similarity between two list
+        similarity_scores = model.similarity(sentences, corpus)
+        print(similarity_scores.numpy())
+        for i in range(len(sentences)):
+            for j in range(len(corpus)):
+                print(f"{sentences[i]} vs {corpus[j]}, score: {similarity_scores.numpy()[i][j]:.4f}")
+        
+        print('-' * 50 + '\n')
+        # 3.Semantic Search
+        model.add_corpus(corpus)
+        res = model.most_similar(queries=sentences, topn=3)
+        print(res)
+        for q_id, c in res.items():
+            print('query:', sentences[q_id])
+            print("search top 3:")
+            for corpus_id, s in c.items():
+                print(f'\t{model.corpus[corpus_id]}: {s:.4f}')
+        ```
+        
+        output:
+        
+        ```shell
+        如何更换花呗绑定银行卡 vs 花呗更改绑定银行卡, score: 0.8551
+        ...
+        
+        如何更换花呗绑定银行卡 vs 花呗更改绑定银行卡, score: 0.8551
+        如何更换花呗绑定银行卡 vs 我什么时候开通了花呗, score: 0.7212
+        如何更换花呗绑定银行卡 vs 俄罗斯警告乌克兰反对欧盟协议, score: 0.1450
+        如何更换花呗绑定银行卡 vs 暴风雨掩埋了东北部；新泽西16英寸的降雪, score: 0.2167
+        如何更换花呗绑定银行卡 vs 中央情报局局长访问以色列叙利亚会谈, score: 0.2517
+        如何更换花呗绑定银行卡 vs 人在巴基斯坦基地的炸弹袭击中丧生, score: 0.0809
+        花呗更改绑定银行卡 vs 花呗更改绑定银行卡, score: 1.0000
+        花呗更改绑定银行卡 vs 我什么时候开通了花呗, score: 0.6807
+        花呗更改绑定银行卡 vs 俄罗斯警告乌克兰反对欧盟协议, score: 0.1714
+        花呗更改绑定银行卡 vs 暴风雨掩埋了东北部；新泽西16英寸的降雪, score: 0.2162
+        花呗更改绑定银行卡 vs 中央情报局局长访问以色列叙利亚会谈, score: 0.2728
+        花呗更改绑定银行卡 vs 人在巴基斯坦基地的炸弹袭击中丧生, score: 0.1279
+        
+        query: 如何更换花呗绑定银行卡
+        search top 3:
+        	花呗更改绑定银行卡: 0.8551
+        	我什么时候开通了花呗: 0.7212
+        	中央情报局局长访问以色列叙利亚会谈: 0.2517
+        ```
+        
+        > 余弦`score`的值范围[-1, 1]，值越大，表示该query与corpus的文本越相似。
+        
+        
+        #### 英文语义相似度计算和匹配搜索
+        
+        example: [examples/base_english_demo.py](./examples/base_english_demo.py)
+        
+        ### 3. 快速近似语义匹配搜索
+        
+        支持Annoy、Hnswlib的近似语义匹配搜索，常用于百万数据集的匹配搜索任务。
+        
+        example: [examples/fast_sim_demo.py](./examples/fast_sim_demo.py)
+        
+        ### 4. 基于字面的文本相似度计算和匹配搜索
+        
+        支持同义词词林（Cilin）、知网Hownet、词向量（WordEmbedding）、Tfidf、SimHash、BM25等算法的相似度计算和字面匹配搜索，常用于文本匹配冷启动。
+        
+        example: [examples/literal_sim_demo.py](./examples/literal_sim_demo.py)
+        
+        ```python
+        from similarities.literalsim import SimHashSimilarity, TfidfSimilarity, BM25Similarity, \
+            WordEmbeddingSimilarity, CilinSimilarity, HownetSimilarity
+        
+        text1 = "如何更换花呗绑定银行卡"
+        text2 = "花呗更改绑定银行卡"
+        
+        corpus = [
+            '花呗更改绑定银行卡',
+            '我什么时候开通了花呗',
+            '俄罗斯警告乌克兰反对欧盟协议',
+            '暴风雨掩埋了东北部；新泽西16英寸的降雪',
+            '中央情报局局长访问以色列叙利亚会谈',
+            '人在巴基斯坦基地的炸弹袭击中丧生',
+        ]
+        
+        queries = [
+            '我的花呗开通了？',
+            '乌克兰被俄罗斯警告'
+        ]
+        m = TfidfSimilarity()
+        print(text1, text2, ' sim score: ', m.similarity(text1, text2))
+        
+        m.add_corpus(corpus)
+        res = m.most_similar(queries, topn=3)
+        print('sim search: ', res)
+        for q_id, c in res.items():
+            print('query:', queries[q_id])
+            print("search top 3:")
+            for corpus_id, s in c.items():
+                print(f'\t{m.corpus[corpus_id]}: {s:.4f}')
+        ```
+        
+        output:
+        
+        ```shell
+        如何更换花呗绑定银行卡 花呗更改绑定银行卡  sim score:  0.8203384355246909
+        
+        sim search:  {0: {2: 0.9999999403953552, 1: 0.43930041790008545, 0: 0.0}, 1: {0: 0.7380483150482178, 1: 0.0, 2: 0.0}}
+        query: 我的花呗开通了？
+        search top 3:
+        	我什么时候开通了花呗: 1.0000
+        	花呗更改绑定银行卡: 0.4393
+        	俄罗斯警告乌克兰反对欧盟协议: 0.0000
+        ...
+        ```
+        
+        ### 5. 图像相似度计算和匹配搜索
+        
+        支持[CLIP](similarities/imagesim.py)、pHash、SIFT等算法的图像相似度计算和匹配搜索。
+        
+        example: [examples/image_demo.py](./examples/image_demo.py)
+        
+        ```python
+        import sys
+        import glob
+        from PIL import Image
+        
+        sys.path.append('..')
+        from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
+        
+        
+        def sim_and_search(m):
+            print(m)
+            # similarity
+            sim_scores = m.similarity(imgs1, imgs2)
+            print('sim scores: ', sim_scores)
+            for (idx, i), j in zip(enumerate(image_fps1), image_fps2):
+                s = sim_scores[idx] if isinstance(sim_scores, list) else sim_scores[idx][idx]
+                print(f"{i} vs {j}, score: {s:.4f}")
+            # search
+            m.add_corpus(corpus_imgs)
+            queries = imgs1
+            res = m.most_similar(queries, topn=3)
+            print('sim search: ', res)
+            for q_id, c in res.items():
+                print('query:', image_fps1[q_id])
+                print("search top 3:")
+                for corpus_id, s in c.items():
+                    print(f'\t{m.corpus[corpus_id].filename}: {s:.4f}')
+            print('-' * 50 + '\n')
+        
+        image_fps1 = ['data/image1.png', 'data/image3.png']
+        image_fps2 = ['data/image12-like-image1.png', 'data/image10.png']
+        imgs1 = [Image.open(i) for i in image_fps1]
+        imgs2 = [Image.open(i) for i in image_fps2]
+        corpus_fps = glob.glob('data/*.jpg') + glob.glob('data/*.png')
+        corpus_imgs = [Image.open(i) for i in corpus_fps]
+        
+        # 2. image and image similarity score
+        sim_and_search(ClipSimilarity())  # the best result
+        sim_and_search(ImageHashSimilarity(hash_function='phash'))
+        sim_and_search(SiftSimilarity())
+        ```
+        
+        output:
+        
+        ```shell
+        Similarity: ClipSimilarity, matching_model: CLIPModel
+        sim scores:  tensor([[0.9580, 0.8654],
+                [0.6558, 0.6145]])
+        
+        data/image1.png vs data/image12-like-image1.png, score: 0.9580
+        data/image3.png vs data/image10.png, score: 0.6145
+        
+        sim search:  {0: {6: 0.9999999403953552, 0: 0.9579654932022095, 4: 0.9326782822608948}, 1: {8: 0.9999997615814209, 4: 0.6729235649108887, 0: 0.6558331847190857}}
+        
+        query: data/image1.png
+        search top 3:
+        	data/image1.png: 1.0000
+        	data/image12-like-image1.png: 0.9580
+        	data/image8-like-image1.png: 0.9327
+        ```
+        
+        ![image_sim](docs/image_sim.png)
+        
+        ### 6. 图文互搜
+        
+        CLIP 模型不仅支持以图搜图，还支持图文互搜：
+        ```python
+        import sys
+        import glob
+        from PIL import Image
+        sys.path.append('..')
+        from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
+        
+        m = ClipSimilarity()
+        print(m)
+        # similarity score between text and image
+        image_fps = ['data/image3.png',  # yellow flower image
+                     'data/image1.png']  # tiger image
+        texts = ['a yellow flower', 'a tiger']
+        imgs = [Image.open(i) for i in image_fps]
+        sim_scores = m.similarity(imgs, texts)
+        
+        print('sim scores: ', sim_scores)
+        for (idx, i), j in zip(enumerate(image_fps), texts):
+            s = sim_scores[idx][idx]
+            print(f"{i} vs {j}, score: {s:.4f}")
+        ```
+        
+        output:
+        
+        ```shell
+        sim scores:  tensor([[0.3220, 0.2409],
+                [0.1677, 0.2959]])
+        data/image3.png vs a yellow flower, score: 0.3220
+        data/image1.png vs a tiger, score: 0.2959
+        ```
+        
+        # Contact
+        
+        - Issue(建议)
+          ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/similarities.svg)](https://github.com/shibing624/similarities/issues)
+        - 邮件我：xuming: xuming624@qq.com
+        - 微信我： 加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
+        
+        <img src="docs/wechat.jpeg" width="200" />
+        
+        # Citation
+        
+        如果你在研究中使用了similarities，请按如下格式引用：
+        
+        APA:
+        
+        ```
+        Xu, M. Similarities: Compute similarity score for humans (Version 1.0.1) [Computer software]. https://github.com/shibing624/similarities
+        ```
+        
+        BibTeX:
+        
+        ```
+        @misc{Xu_Similarities_Compute_similarity,
+          title={Similarities: similarity calculation and semantic search toolkit},
+          author={Xu Ming},
+          year={2022},
+          howpublished={\url{https://github.com/shibing624/similarities}},
+        }
+        ```
+        
+        # License
+        
+        授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加similarities的链接和授权协议。
+        
+        # Contribute
+        
+        项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
+        
+        - 在`tests`添加相应的单元测试
+        - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
+        
+        之后即可提交PR。
+        
+        # Reference
+        
+        - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
+        - [liuhuanyong/SentenceSimilarity](https://github.com/liuhuanyong/SentenceSimilarity)
+        - [shibing624/text2vec](https://github.com/shibing624/text2vec)
+        - [qwertyforce/image_search](https://github.com/qwertyforce/image_search)
+        - [ImageHash - Official Github repository](https://github.com/JohannesBuchner/imagehash)
+        - [openai/CLIP](https://github.com/openai/CLIP)
+Keywords: similarities,Chinese Text Similarity Calculation Tool,similarity,word2vec
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
```

### Comparing `similarities-1.0.4/setup.py` & `similarities-1.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import sys
 
 from setuptools import setup, find_packages
 
 # Avoids IDE errors, but actual version is read from version.py
-__version__ = None
+__version__ = ""
 exec(open('similarities/version.py').read())
 
 if sys.version_info < (3,):
     sys.exit('Sorry, Python3 is required.')
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
@@ -29,18 +29,14 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords='similarities,Chinese Text Similarity Calculation Tool,similarity,word2vec',
     install_requires=[
         "text2vec>=1.1.5",
         "transformers",
         "jieba>=0.39",
```

### Comparing `similarities-1.0.4/similarities/__init__.py` & `similarities-1.0.5/similarities/__init__.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/clip_model.py` & `similarities-1.0.5/similarities/clip_model.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/data_loader.py` & `similarities-1.0.5/similarities/data_loader.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/evaluation.py` & `similarities-1.0.5/similarities/evaluation.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/fastsim.py` & `similarities-1.0.5/similarities/fastsim.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,71 +15,81 @@
     similar query for a given docs with Annoy.
     """
 
     def __init__(
             self,
             corpus: Union[List[str], Dict[str, str]] = None,
             model_name_or_path="shibing624/text2vec-base-chinese",
-            embedding_size: int = 768,
             n_trees: int = 256
     ):
         super().__init__(corpus, model_name_or_path)
         self.index = None
-        self.embedding_size = embedding_size
+        self.embedding_size = self.get_sentence_embedding_dimension()
         self.n_trees = n_trees
         if corpus is not None and self.corpus_embeddings:
             self.build_index()
 
     def __str__(self):
         base = f"Similarity: {self.__class__.__name__}, matching_model: {self.sentence_model}"
         if self.corpus:
             base += f", corpus size: {len(self.corpus)}"
         return base
 
-    def build_index(self):
-        """Build Annoy index after add new documents."""
-        # Create Annoy Index
+    def create_index(self):
+        """Create Annoy Index."""
         try:
             from annoy import AnnoyIndex
         except ImportError:
             raise ImportError("Annoy is not installed. Please install it first, e.g. with `pip install annoy`.")
 
         # Creating the annoy index
         self.index = AnnoyIndex(self.embedding_size, 'angular')
+        logger.debug(f"Init Annoy index, embedding_size: {self.embedding_size}")
 
-        logger.info(f"Init Annoy index, embedding_size: {self.embedding_size}")
+    def build_index(self):
+        """Build Annoy index after add new documents."""
+        self.create_index()
         logger.debug(f"Building index with {self.n_trees} trees.")
 
         for i in range(len(self.corpus_embeddings)):
             self.index.add_item(i, self.corpus_embeddings[i])
         self.index.build(self.n_trees)
 
-    def save_index(self, index_path: str):
+    def save_index(self, index_path: str = "annoy_index.bin"):
         """Save the annoy index to disk."""
-        if self.index and index_path:
-            logger.info(f"Saving index to: {index_path}")
+        if index_path:
+            if self.index is None:
+                self.build_index()
             self.index.save(index_path)
+            corpus_emb_json_path = index_path + ".json"
+            super().save_index(corpus_emb_json_path)
+            logger.info(f"Saving Annoy index to: {index_path}, corpus embedding to: {corpus_emb_json_path}")
         else:
             logger.warning("No index path given. Index not saved.")
 
-    def load_index(self, index_path: str):
+    def load_index(self, index_path: str = "annoy_index.bin"):
         """Load Annoy Index from disc."""
         if index_path and os.path.exists(index_path):
-            logger.info(f"Loading index from: {index_path}")
+            corpus_emb_json_path = index_path + ".json"
+            logger.info(f"Loading index from: {index_path}, corpus embedding from: {corpus_emb_json_path}")
+            super().load_index(corpus_emb_json_path)
+            if self.index is None:
+                self.create_index()
             self.index.load(index_path)
         else:
             logger.warning("No index path given. Index not loaded.")
 
-    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10):
+    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10,
+                     score_function: str = "cos_sim"):
         """Find the topn most similar texts to the query against the corpus."""
         result = {}
         if self.corpus_embeddings and self.index is None:
             logger.warning(f"No index found. Please add corpus and build index first, e.g. with `build_index()`."
                            f"Now returning slow search result.")
-            return super().most_similar(queries, topn)
+            return super().most_similar(queries, topn, score_function=score_function)
         if not self.corpus_embeddings:
             logger.error("No corpus_embeddings found. Please add corpus first, e.g. with `add_corpus()`.")
             return result
         if isinstance(queries, str) or not hasattr(queries, '__len__'):
             queries = [queries]
         if isinstance(queries, list):
             queries = {id: query for id, query in enumerate(queries)}
@@ -87,92 +97,104 @@
         queries_texts = list(queries.values())
         queries_embeddings = self._get_vector(queries_texts)
         # Annoy get_nns_by_vector can only search for one vector at a time
         for idx, (qid, query) in enumerate(queries.items()):
             corpus_ids, distances = self.index.get_nns_by_vector(queries_embeddings[idx], topn, include_distances=True)
             for corpus_id, distance in zip(corpus_ids, distances):
                 score = 1 - (distance ** 2) / 2
-                result[qid][self.corpus_ids_map[corpus_id]] = score
+                result[qid][corpus_id] = score
 
         return result
 
 
 class HnswlibSimilarity(Similarity):
     """
     Computes cosine similarities between word embeddings and retrieves most
     similar query for a given docs with Hnswlib.
     """
 
     def __init__(
             self,
             corpus: Union[List[str], Dict[str, str]] = None,
             model_name_or_path="shibing624/text2vec-base-chinese",
-            embedding_size: int = 768, ef_construction: int = 400, M: int = 64, ef: int = 50
+            ef_construction: int = 400, M: int = 64, ef: int = 50
     ):
         super().__init__(corpus, model_name_or_path)
-        self.embedding_size = embedding_size
+        self.embedding_size = self.get_sentence_embedding_dimension()
         self.ef_construction = ef_construction
         self.M = M
         self.ef = ef
         self.index = None
         if corpus is not None and self.corpus_embeddings:
             self.build_index()
 
     def __str__(self):
         base = f"Similarity: {self.__class__.__name__}, matching_model: {self.sentence_model}"
         if self.corpus:
             base += f", corpus size: {len(self.corpus)}"
         return base
 
-    def build_index(self):
-        """Build Hnswlib index after add new documents."""
-        # Create hnswlib Index
+    def create_index(self):
+        """Create Hnswlib Index."""
         try:
             import hnswlib
         except ImportError:
             raise ImportError("Hnswlib is not installed. Please install it first, e.g. with `pip install hnswlib`.")
 
-        # We use Inner Product (dot-product) as Index. We will normalize our vectors to unit length,
-        # then is Inner Product equal to cosine similarity
+        # Creating the hnswlib index
         self.index = hnswlib.Index(space='cosine', dim=self.embedding_size)
+        self.index.init_index(max_elements=len(self.corpus_embeddings), ef_construction=self.ef_construction, M=self.M)
+        # Controlling the recall by setting ef:
+        self.index.set_ef(self.ef)  # ef should always be > top_k_hits
+        logger.debug(f"Init Hnswlib index, embedding_size: {self.embedding_size}")
+
+    def build_index(self):
+        """Build Hnswlib index after add new documents."""
         # Init the HNSWLIB index
-        logger.info(f"Creating HNSWLIB index, max_elements: {len(self.corpus)}")
+        self.create_index()
+        logger.info(f"Building HNSWLIB index, max_elements: {len(self.corpus)}")
         logger.debug(f"Parameters Required: M: {self.M}")
         logger.debug(f"Parameters Required: ef_construction: {self.ef_construction}")
         logger.debug(f"Parameters Required: ef(>topn): {self.ef}")
 
-        self.index.init_index(max_elements=len(self.corpus_embeddings), ef_construction=self.ef_construction, M=self.M)
         # Then we train the index to find a suitable clustering
         self.index.add_items(self.corpus_embeddings, list(range(len(self.corpus_embeddings))))
-        # Controlling the recall by setting ef:
-        self.index.set_ef(self.ef)  # ef should always be > top_k_hits
 
-    def save_index(self, index_path: str):
-        """Save the annoy index to disk."""
-        if self.index and index_path:
-            logger.info(f"Saving index to: {index_path}")
+    def save_index(self, index_path: str = "hnswlib_index.bin"):
+        """Save the index to disk."""
+        if index_path:
+            if self.index is None:
+                self.build_index()
             self.index.save_index(index_path)
+            corpus_emb_json_path = index_path + ".json"
+            super().save_index(corpus_emb_json_path)
+            logger.info(f"Saving hnswlib index to: {index_path}, corpus embedding to: {corpus_emb_json_path}")
         else:
             logger.warning("No index path given. Index not saved.")
 
-    def load_index(self, index_path: str):
-        """Load Annoy Index from disc."""
+    def load_index(self, index_path: str = "hnswlib_index.bin"):
+        """Load Index from disc."""
         if index_path and os.path.exists(index_path):
-            logger.info(f"Loading index from: {index_path}")
+            corpus_emb_json_path = index_path + ".json"
+            logger.info(f"Loading index from: {index_path}, corpus embedding from: {corpus_emb_json_path}")
+            super().load_index(corpus_emb_json_path)
+            if self.index is None:
+                self.create_index()
             self.index.load_index(index_path)
         else:
             logger.warning("No index path given. Index not loaded.")
 
-    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10):
+    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10,
+                     score_function: str = "cos_sim"):
         """Find the topn most similar texts to the query against the corpus."""
         result = {}
         if self.corpus_embeddings and self.index is None:
             logger.warning(f"No index found. Please add corpus and build index first, e.g. with `build_index()`."
                            f"Now returning slow search result.")
-            return super().most_similar(queries, topn)
+            return super().most_similar(queries, topn, score_function=score_function)
         if not self.corpus_embeddings:
             logger.error("No corpus_embeddings found. Please add corpus first, e.g. with `add_corpus()`.")
             return result
         if isinstance(queries, str) or not hasattr(queries, '__len__'):
             queries = [queries]
         if isinstance(queries, list):
             queries = {id: query for id, query in enumerate(queries)}
@@ -182,10 +204,10 @@
         # We use hnswlib knn_query method to find the top_k_hits
         corpus_ids, distances = self.index.knn_query(queries_embeddings, k=topn)
         # We extract corpus ids and scores for each query
         for i, (qid, query) in enumerate(queries.items()):
             hits = [{'corpus_id': id, 'score': 1 - distance} for id, distance in zip(corpus_ids[i], distances[i])]
             hits = sorted(hits, key=lambda x: x['score'], reverse=True)
             for hit in hits:
-                result[qid][self.corpus_ids_map[hit['corpus_id']]] = hit['score']
+                result[qid][hit['corpus_id']] = hit['score']
 
         return result
```

### Comparing `similarities-1.0.4/similarities/imagesim.py` & `similarities-1.0.5/similarities/imagesim.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             self,
             corpus: Union[List[Image.Image], Dict[str, Image.Image]] = None,
             model_name_or_path='openai/clip-vit-base-patch32'
     ):
         self.clip_model = CLIPModel(model_name_or_path)  # load the CLIP model
         self.score_functions = {'cos_sim': cos_sim, 'dot': dot_score}
         self.corpus = {}
-        self.corpus_ids_map = {}
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
@@ -55,28 +54,34 @@
 
     def _convert_to_rgb(self, img):
         """Convert image to RGB mode."""
         if img.mode != 'RGB':
             img = img.convert('RGB')
         return img
 
-    def _get_vector(self, text_or_img: Union[List[Image.Image], Image.Image, str, List[str]],
-                    show_progress_bar: bool = False):
+    def _get_vector(
+            self,
+            text_or_img: Union[List[Image.Image], Image.Image, str, List[str]],
+            batch_size: int = 128,
+            show_progress_bar: bool = False,
+    ):
         """
         Returns the embeddings for a batch of images.
-        :param text_or_img: list of str or str or Image.Image or image list
+        :param text_or_img: list of str or Image.Image or image list
+        :param batch_size: batch size
+        :param show_progress_bar: show progress bar
         :return: np.ndarray, embeddings for the given images
         """
         if isinstance(text_or_img, str):
             text_or_img = [text_or_img]
         if isinstance(text_or_img, Image.Image):
             text_or_img = [text_or_img]
         if isinstance(text_or_img, list) and isinstance(text_or_img[0], Image.Image):
             text_or_img = [self._convert_to_rgb(i) for i in text_or_img]
-        return self.clip_model.encode(text_or_img, batch_size=128, show_progress_bar=show_progress_bar)
+        return self.clip_model.encode(text_or_img, batch_size=batch_size, show_progress_bar=show_progress_bar)
 
     def add_corpus(self, corpus: Union[List[Image.Image], Dict[str, Image.Image]]):
         """
         Extend the corpus with new documents.
 
         Parameters
         ----------
@@ -89,15 +94,14 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_embeddings = self._get_vector(list(corpus_new.values()), show_progress_bar=True).tolist()
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
         else:
             self.corpus_embeddings = corpus_embeddings
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}, emb size: {len(self.corpus_embeddings)}")
@@ -143,15 +147,15 @@
         queries_ids_map = {i: id for i, id in enumerate(list(queries.keys()))}
         queries_texts = list(queries.values())
         queries_embeddings = self._get_vector(queries_texts)
         corpus_embeddings = np.array(self.corpus_embeddings, dtype=np.float32)
         all_hits = semantic_search(queries_embeddings, corpus_embeddings, top_k=topn)
         for idx, hits in enumerate(all_hits):
             for hit in hits[0:topn]:
-                result[queries_ids_map[idx]][self.corpus_ids_map[hit['corpus_id']]] = hit['score']
+                result[queries_ids_map[idx]][hit['corpus_id']] = hit['score']
 
         return result
 
 
 class ImageHashSimilarity(SimilarityABC):
     """
     Compute Phash similarity between two images and retrieves most
@@ -197,15 +201,14 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_embeddings = []
         for doc_fp in tqdm(list(corpus_new.values()), desc="Calculating corpus image hash"):
             doc_seq = str(self.hash_function(doc_fp, self.hash_size))
             corpus_embeddings.append(doc_seq)
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
@@ -313,15 +316,14 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_embeddings = []
         for img in tqdm(list(corpus_new.values()), desc="Calculating corpus image SIFT"):
             _, descriptors = self.calculate_descr(img)
             if len(descriptors.shape) > 0 and descriptors.shape[0] > 0:
                 corpus_embeddings.append(descriptors.tolist())
         if self.corpus_embeddings:
```

### Comparing `similarities-1.0.4/similarities/literalsim.py` & `similarities-1.0.5/similarities/literalsim.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Compute SimHash similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
@@ -67,15 +67,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = []
         for sentence in tqdm(corpus_texts, desc="Computing corpus SimHash"):
             corpus_embeddings.append(self.simhash(sentence))
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
@@ -194,15 +194,15 @@
     Compute TFIDF similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         self.corpus_embeddings = []
         self.tfidf = TFIDF()
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
@@ -230,15 +230,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = []
         for sentence in tqdm(corpus_texts, desc="Computing corpus TFIDF"):
             corpus_embeddings.append(self.tfidf.get_tfidf(sentence))
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
@@ -276,29 +276,29 @@
         queries_texts = list(queries.values())
 
         queries_embeddings = np.array([self.tfidf.get_tfidf(query) for query in queries_texts], dtype=np.float32)
         corpus_embeddings = np.array(self.corpus_embeddings, dtype=np.float32)
         all_hits = semantic_search(queries_embeddings, corpus_embeddings, top_k=topn)
         for idx, hits in enumerate(all_hits):
             for hit in hits[0:topn]:
-                result[queries_ids_map[idx]][self.corpus_ids_map[hit['corpus_id']]] = hit['score']
+                result[queries_ids_map[idx]][hit['corpus_id']] = hit['score']
 
         return result
 
 
 class BM25Similarity(SimilarityABC):
     """
     Compute BM25OKapi similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         self.bm25 = None
         self.default_stopwords = load_stopwords(default_stopwords_file)
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
@@ -326,15 +326,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_seg = [jieba.lcut(d) for d in corpus_texts]
         corpus_seg = [[w for w in doc if (w.strip().lower() not in self.default_stopwords) and
                        len(w.strip()) > 0] for doc in corpus_seg]
         self.bm25 = BM25Okapi(corpus_seg)
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
@@ -356,15 +356,15 @@
         for qid, query in queries.items():
             tokens = jieba.lcut(query)
             scores = self.bm25.get_scores(tokens)
 
             q_res = [{'corpus_id': corpus_id, 'score': score} for corpus_id, score in enumerate(scores)]
             q_res = sorted(q_res, key=lambda x: x['score'], reverse=True)[:topn]
             for res in q_res:
-                corpus_id = self.corpus_ids_map[res['corpus_id']]
+                corpus_id = res['corpus_id']
                 result[qid][corpus_id] = res['score']
 
         return result
 
 
 class WordEmbeddingSimilarity(SimilarityABC):
     """
@@ -381,15 +381,15 @@
         if isinstance(model_name_or_path, str):
             self.keyedvectors = Word2Vec(model_name_or_path)
         elif hasattr(model_name_or_path, "encode"):
             self.keyedvectors = model_name_or_path
         else:
             raise ValueError("model_name_or_path must be ~text2vec.Word2Vec or Word2Vec model name")
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
@@ -416,15 +416,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = self._get_vector(corpus_texts, show_progress_bar=True).tolist()
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
         else:
             self.corpus_embeddings = corpus_embeddings
@@ -459,15 +459,15 @@
         queries_texts = list(queries.values())
 
         queries_embeddings = np.array([self._get_vector(query) for query in queries_texts], dtype=np.float32)
         corpus_embeddings = np.array(self.corpus_embeddings, dtype=np.float32)
         all_hits = semantic_search(queries_embeddings, corpus_embeddings, top_k=topn)
         for idx, hits in enumerate(all_hits):
             for hit in hits[0:topn]:
-                result[queries_ids_map[idx]][self.corpus_ids_map[hit['corpus_id']]] = hit['score']
+                result[queries_ids_map[idx]][hit['corpus_id']] = hit['score']
 
         return result
 
 
 class CilinSimilarity(SimilarityABC):
     """
     Compute Cilin similarity between two sentences and retrieves most
@@ -475,15 +475,15 @@
     """
     default_cilin_path = os.path.join(pwd_path, 'data/cilin.txt')
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None, cilin_path: str = default_cilin_path):
         super().__init__()
         self.cilin_dict = self.load_cilin_dict(cilin_path)  # Cilin(词林) semantic dictionary
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -509,15 +509,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     @staticmethod
     def load_cilin_dict(path):
         """加载词林语义词典"""
         sem_dict = {}
@@ -632,15 +632,15 @@
     similar sentence for a given corpus.
     """
     default_hownet_path = os.path.join(pwd_path, 'data/hownet.txt')
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None, hownet_path: str = default_hownet_path):
         self.hownet_dict = self.load_hownet_dict(hownet_path)  # semantic dictionary
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -666,15 +666,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     @staticmethod
     def load_hownet_dict(path):
         """加载Hownet语义词典"""
         hownet_dict = {}
@@ -762,15 +762,15 @@
     similar sentence for a given corpus.
     不考虑文本字符位置顺序，基于相同字符数占比计算相似度
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -796,15 +796,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     def similarity(self, a: Union[str, List[str]], b: Union[str, List[str]]):
         """
         Compute Chars similarity between two texts.
         :param a:
@@ -858,15 +858,15 @@
     similar sentence for a given corpus.
     考虑文本字符位置顺序，基于最长公共子串占比计算相似度
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        self.corpus_ids_map = {}
+        
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -892,15 +892,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
+        
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     def similarity(self, a: Union[str, List[str]], b: Union[str, List[str]],
                    min_same_len: int = 70, min_same_len_score: float = 0.9):
         """
         Compute Chars similarity between two texts.
```

### Comparing `similarities-1.0.4/similarities/similarity.py` & `similarities-1.0.5/similarities/similarity.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Compute similarity:
 1. Compute the similarity between two sentences
 2. Retrieves most similar sentence of a query against a corpus of documents.
 """
 
 import os
+import json
 from typing import List, Union, Dict
 
 import numpy as np
 from loguru import logger
 from text2vec import SentenceModel
 
 from similarities.utils.util import cos_sim, semantic_search, dot_score
@@ -62,92 +63,106 @@
         :return: Dict[str, Dict[str, float]], {query_id: {corpus_id: similarity_score}, ...}
         """
         raise NotImplementedError("cannot instantiate Abstract Base Class")
 
 
 class Similarity(SimilarityABC):
     """
-    Bert similarity:
+    Sentence Similarity:
     1. Compute the similarity between two sentences
     2. Retrieves most similar sentence of a query against a corpus of documents.
 
     The index supports adding new documents dynamically.
     """
 
     def __init__(
             self,
             corpus: Union[List[str], Dict[str, str]] = None,
-            model_name_or_path="shibing624/text2vec-base-chinese",
+            model_name_or_path="sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
             max_seq_length=128,
     ):
         """
         Initialize the similarity object.
-        :param model_name_or_path: bert model name or path, can be: ['bert-base-uncased', 'bert-base-chinese', ...]
-            default "shibing624/text2vec-base-chinese", refer: https://github.com/shibing624/text2vec
+        :param model_name_or_path: Transformer model name or path, like:
+            'sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2', 'bert-base-uncased', 'bert-base-chinese',
+             'shibing624/text2vec-base-chinese', ...
+            model in HuggingFace Model Hub and release from https://github.com/shibing624/text2vec
         :param corpus: Corpus of documents to use for similarity queries.
+        :param max_seq_length: Max sequence length for sentence model.
         """
         if isinstance(model_name_or_path, str):
             self.sentence_model = SentenceModel(model_name_or_path, max_seq_length=max_seq_length)
         elif hasattr(model_name_or_path, "encode"):
             self.sentence_model = model_name_or_path
         else:
             raise ValueError("model_name_or_path is transformers model name or path")
         self.score_functions = {'cos_sim': cos_sim, 'dot': dot_score}
         self.corpus = {}
-        self.corpus_ids_map = {}
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
     def __str__(self):
         base = f"Similarity: {self.__class__.__name__}, matching_model: {self.sentence_model}"
         if self.corpus:
             base += f", corpus size: {len(self.corpus)}"
         return base
 
+    def get_sentence_embedding_dimension(self):
+        """
+        Get the dimension of the sentence embeddings.
+
+        Returns
+        -------
+        int or None
+            The dimension of the sentence embeddings, or None if it cannot be determined.
+        """
+        if hasattr(self.sentence_model, "get_sentence_embedding_dimension"):
+            return self.sentence_model.get_sentence_embedding_dimension()
+        else:
+            return getattr(self.sentence_model.bert.pooler.dense, "out_features", None)
+
     def add_corpus(self, corpus: Union[List[str], Dict[str, str]]):
         """
         Extend the corpus with new documents.
-
-        Parameters
-        ----------
-        corpus : list of str or dict
+        :param corpus: corpus of documents to use for similarity queries.
+        :return: self.corpus, self.corpus embeddings
         """
-        corpus_new = {}
+        new_corpus = {}
         start_id = len(self.corpus) if self.corpus else 0
-        if isinstance(corpus, list):
-            corpus = list(set(corpus))
-            for id, doc in enumerate(corpus):
-                if doc not in list(self.corpus.values()):
-                    corpus_new[start_id + id] = doc
-        else:
-            for id, doc in corpus.items():
-                if doc not in list(self.corpus.values()):
-                    corpus_new[id] = doc
-        self.corpus.update(corpus_new)
-        self.corpus_ids_map = {i: id for i, id in enumerate(list(self.corpus.keys()))}
-        logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
-        corpus_embeddings = self._get_vector(list(corpus_new.values()), show_progress_bar=True).tolist()
-        if self.corpus_embeddings:
-            self.corpus_embeddings += corpus_embeddings
-        else:
-            self.corpus_embeddings = corpus_embeddings
-        logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}, emb size: {len(self.corpus_embeddings)}")
+        for id, doc in enumerate(corpus):
+            if isinstance(corpus, list):
+                if doc not in self.corpus.values():
+                    new_corpus[start_id + id] = doc
+            else:
+                if doc not in self.corpus.values():
+                    new_corpus[id] = doc
+        self.corpus.update(new_corpus)
+        logger.info(f"Start computing corpus embeddings, new docs: {len(new_corpus)}")
+        corpus_embeddings = self._get_vector(list(new_corpus.values()), show_progress_bar=True).tolist()
+        self.corpus_embeddings = self.corpus_embeddings + corpus_embeddings \
+            if self.corpus_embeddings else corpus_embeddings
+        logger.info(f"Add {len(new_corpus)} docs, total: {len(self.corpus)}, emb len: {len(self.corpus_embeddings)}")
 
-    def _get_vector(self, sentences: Union[str, List[str]], show_progress_bar: bool = False) -> np.ndarray:
+    def _get_vector(
+            self,
+            sentences: Union[str, List[str]],
+            batch_size: int = 64,
+            show_progress_bar: bool = False,
+    ) -> np.ndarray:
         """
         Returns the embeddings for a batch of sentences.
         :param sentences:
         :return:
         """
-        return self.sentence_model.encode(sentences, show_progress_bar=show_progress_bar)
+        return self.sentence_model.encode(sentences, batch_size=batch_size, show_progress_bar=show_progress_bar)
 
     def similarity(self, a: Union[str, List[str]], b: Union[str, List[str]], score_function: str = "cos_sim"):
         """
         Compute similarity between two texts.
         :param a: list of str or str
         :param b: list of str or str
         :param score_function: function to compute similarity, default cos_sim
@@ -162,29 +177,64 @@
 
         return score_function(text_emb1, text_emb2)
 
     def distance(self, a: Union[str, List[str]], b: Union[str, List[str]]):
         """Compute cosine distance between two texts."""
         return 1 - self.similarity(a, b)
 
-    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10):
+    def most_similar(self, queries: Union[str, List[str], Dict[str, str]], topn: int = 10,
+                     score_function: str = "cos_sim"):
         """
         Find the topn most similar texts to the queries against the corpus.
         :param queries: str or list of str
         :param topn: int
+        :param score_function: function to compute similarity, default cos_sim
         :return: Dict[str, Dict[str, float]], {query_id: {corpus_id: similarity_score}, ...}
         """
         if isinstance(queries, str) or not hasattr(queries, '__len__'):
             queries = [queries]
         if isinstance(queries, list):
             queries = {id: query for id, query in enumerate(queries)}
+        if score_function not in self.score_functions:
+            raise ValueError(f"score function: {score_function} must be either (cos_sim) for cosine similarity"
+                             " or (dot) for dot product")
+        score_function = self.score_functions[score_function]
         result = {qid: {} for qid, query in queries.items()}
         queries_ids_map = {i: id for i, id in enumerate(list(queries.keys()))}
         queries_texts = list(queries.values())
         queries_embeddings = self._get_vector(queries_texts)
         corpus_embeddings = np.array(self.corpus_embeddings, dtype=np.float32)
-        all_hits = semantic_search(queries_embeddings, corpus_embeddings, top_k=topn)
+        all_hits = semantic_search(queries_embeddings, corpus_embeddings, top_k=topn, score_function=score_function)
         for idx, hits in enumerate(all_hits):
             for hit in hits[0:topn]:
-                result[queries_ids_map[idx]][self.corpus_ids_map[hit['corpus_id']]] = hit['score']
+                result[queries_ids_map[idx]][hit['corpus_id']] = hit['score']
 
         return result
+
+    def save_index(self, index_path: str = "corpus_emb.json"):
+        """
+        Save corpus embeddings to json file.
+        :param index_path: json file path
+        :return:
+        """
+        corpus_emb = {id: {"doc": self.corpus[id], "doc_emb": emb} for id, emb in
+                      zip(self.corpus.keys(), self.corpus_embeddings)}
+        with open(index_path, "w", encoding="utf-8") as f:
+            json.dump(corpus_emb, f)
+        logger.debug(f"Save corpus embeddings to file: {index_path}.")
+
+    def load_index(self, index_path: str = "corpus_emb.json"):
+        """
+        Load corpus embeddings from json file.
+        :param index_path: json file path
+        :return: list of corpus embeddings, dict of corpus ids map, dict of corpus
+        """
+        try:
+            with open(index_path, "r", encoding="utf-8") as f:
+                corpus_emb = json.load(f)
+            corpus_embeddings = []
+            for id, corpus_dict in corpus_emb.items():
+                self.corpus[int(id)] = corpus_dict["doc"]
+                corpus_embeddings.append(corpus_dict["doc_emb"])
+            self.corpus_embeddings = corpus_embeddings
+        except (IOError, json.JSONDecodeError):
+            logger.error("Error: Could not load corpus embeddings from file.")
```

### Comparing `similarities-1.0.4/similarities/utils/distance.py` & `similarities-1.0.5/similarities/utils/distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     try:
         # very fast
         # http://stackoverflow.com/questions/14260126/how-python-levenshtein-ratio-is-computed
         import Levenshtein
         d = Levenshtein.distance(str1, str2) / float(max(len(str1), len(str2)))
     except:
         # https://docs.python.org/2/library/difflib.html
-        d = 1. - SequenceMatcher(lambda x: x == " ", str1, str2).ratio()
+        d = 1.0 - SequenceMatcher(lambda x: x == " ", str1, str2).ratio()
     return d
 
 
 def pearson_correlation_distance(v1, v2):  # 皮尔逊相关系数（Pearson correlation）
     v1_v2 = np.vstack([v1, v2])
     return np.corrcoef(v1_v2)[0][1]
 
@@ -105,15 +105,15 @@
 
 
 def is_str_match(str1, str2, threshold=1.0):
     assert 0.0 <= threshold <= 1.0, "Wrong threshold."
     if float(threshold) == 1.0:
         return str1 == str2
     else:
-        return (1. - edit_distance(str1, str2)) >= threshold
+        return (1.0 - edit_distance(str1, str2)) >= threshold
 
 
 def longest_match_size(str1, str2):
     """最长公共子串长度"""
     sq = SequenceMatcher(None, str1, str2)
     match = sq.find_longest_match(0, len(str1), 0, len(str2))
     return match.size
@@ -201,19 +201,26 @@
 
     print(euclidean_distance(vec1_test, vec2_test))
     print(cosine_distance(vec1_test, vec2_test))
     print(manhattan_distance(vec1_test, vec2_test))
 
     str1_test = "你到底是谁?"
     str2_test = "没想到我是谁，是真样子"
-    print('strs:', str1_test, str2_test)
-    print(edit_distance(str1_test, str2_test))
+    print('strs:', str1_test, ' vs ', str2_test)
+    print('edit_dist', edit_distance(str1_test, str2_test))
+    print('edit_sim:', 1 - edit_distance(str1_test, str2_test))
+
+    str1_test = "private Thread currentThread;"
+    str2_test = "private volatile Thread currentThread;"
+    print('strs:', str1_test, ' vs ', str2_test)
+    print('edit_dist', edit_distance(str1_test, str2_test))
+    print('edit_sim:', 1 - edit_distance(str1_test, str2_test))
+
     print(num_of_common_sub_str(str1_test, str2_test))
     print(max_min_normalize(vec1_test))  # 归一化（0-1）
     print(z_score(vec1_test))  # 标准化（0附近，正负）
 
     str1 = '刘若英是演员和歌手'
     str2 = '刘若英是演员吗？'
     print(f"{str1} vs {str2} common sub str: {num_of_common_sub_str(str1, str2)}")
     print(f"{str1} vs {str2} longest match size: {longest_match_size(str1, str2)}")
     print(f"{str1} vs {str2} longest match ratio: {longest_match_ratio(str1, str2)}")
-
```

### Comparing `similarities-1.0.4/similarities/utils/get_file.py` & `similarities-1.0.5/similarities/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/utils/imagehash.py` & `similarities-1.0.5/similarities/utils/imagehash.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/utils/rank_bm25.py` & `similarities-1.0.5/similarities/utils/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/utils/tfidf.py` & `similarities-1.0.5/similarities/utils/tfidf.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.4/similarities/utils/util.py` & `similarities-1.0.5/similarities/utils/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         top_k: int = 10,
         score_function=cos_sim
 ):
     """
     This function performs a cosine similarity search between a list of query embeddings and a list of corpus embeddings.
     It can be used for Information Retrieval / Semantic Search for corpora up to about 1 Million entries.
 
-    :param query_embeddings: A 2 dimensional tensor with the query embeddings.
-    :param corpus_embeddings: A 2 dimensional tensor with the corpus embeddings.
+    :param query_embeddings: A 2-dimensional tensor with the query embeddings.
+    :param corpus_embeddings: A 2-dimensional tensor with the corpus embeddings.
     :param query_chunk_size: Process 100 queries simultaneously. Increasing that value increases the speed, but
         requires more memory.
     :param corpus_chunk_size: Scans the corpus 100k entries at a time. Increasing that value increases the speed,
         but requires more memory.
     :param top_k: Retrieve top k matching entries.
     :param score_function: Funtion for computing scores. By default, cosine similarity.
     :return: Returns a sorted list with decreasing cosine similarity scores. Entries are dictionaries with the
```

### Comparing `similarities-1.0.4/similarities.egg-info/SOURCES.txt` & `similarities-1.0.5/similarities.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,12 +15,10 @@
 similarities.egg-info/not-zip-safe
 similarities.egg-info/requires.txt
 similarities.egg-info/top_level.txt
 similarities/utils/__init__.py
 similarities/utils/distance.py
 similarities/utils/get_file.py
 similarities/utils/imagehash.py
-similarities/utils/ngram_util.py
 similarities/utils/rank_bm25.py
 similarities/utils/tfidf.py
-similarities/utils/tokenizer.py
 similarities/utils/util.py
```

