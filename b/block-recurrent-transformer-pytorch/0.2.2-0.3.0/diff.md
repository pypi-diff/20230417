# Comparing `tmp/block-recurrent-transformer-pytorch-0.2.2.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.2.2.tar", last modified: Tue Apr  4 14:47:35 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.0.tar", last modified: Mon Apr 17 21:23:56 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.2.2.tar` & `block-recurrent-transformer-pytorch-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:47:35.678092 block-recurrent-transformer-pytorch-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-04 14:47:24.000000 block-recurrent-transformer-pytorch-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 14:47:35.678092 block-recurrent-transformer-pytorch-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-04 14:47:24.000000 block-recurrent-transformer-pytorch-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:47:35.678092 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-04 14:47:24.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30859 2023-04-04 14:47:24.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:47:35.678092 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 14:47:35.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-04 14:47:35.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:47:35.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 14:47:35.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 14:47:35.000000 block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:47:35.678092 block-recurrent-transformer-pytorch-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-04 14:47:24.000000 block-recurrent-transformer-pytorch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 21:23:56.000000 block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:23:56.123081 block-recurrent-transformer-pytorch-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 21:23:39.000000 block-recurrent-transformer-pytorch-0.3.0/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.2.2/LICENSE` & `block-recurrent-transformer-pytorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.2.2/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.2.2
+Version: 0.3.0
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.2.2/README.md` & `block-recurrent-transformer-pytorch-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     num_tokens = 20000,             # vocab size
     dim = 512,                      # model dimensions
     depth = 6,                      # depth
     dim_head = 64,                  # attention head dimensions
     heads = 8,                      # number of attention heads
     max_seq_len = 1024,             # the total receptive field of the transformer, in the paper this was 2 * block size
     block_width = 512,              # block size - total receptive field is max_seq_len, 2 * block size in paper. the block furthest forwards becomes the new cached xl memories, which is a block size of 1 (please open an issue if i am wrong)
-    xl_memories_layers = (5, 6),    # which layers to use xl memories. very old deepmind papers have shown you only need the last penultimate layers to have cached key values to see majority of benefit
     num_state_vectors = 512,        # number of state vectors, i believe this was a single block size in the paper, but can be any amount
     recurrent_layers = (4,),        # where to place the recurrent layer(s) for states with fixed simple gating
     enhanced_recurrence = True,     # enhanced recurrence from ernie-doc paper, i have seen it to work well on my local machine
     use_flash_attn = True           # use flash attention, if on pytorch 2.0
 )
 
 seq = torch.randint(0, 2000, (1, 1024))
@@ -66,14 +65,15 @@
 - [x] make sure attention allow for single head key / values too
 - [x] run a few experiments of fixed gating in regular transformers - does not work
 - [x] integrate <a href="https://github.com/hazyresearch/flash-attention">flash attention</a>
 - [x] cache attention mask + rotary embeddings
 
 - [ ] revisit <a href="https://github.com/lucidrains/memformer">memformer</a>
 - [ ] add ability to gate in memorizing transformers knn attention layers
+- [ ] add <a href="https://github.com/lucidrains/compressive-transformer-pytorch">compressed memories</a>
 
 ## Citations
 
 ```bibtex
 @article{Hutchins2022BlockRecurrentT,
     title   = {Block-Recurrent Transformers},
     author  = {DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam Neyshabur},
@@ -100,27 +100,14 @@
     journal = {ArXiv},
     year    = {2019},
     volume  = {abs/1911.02150}
 }
 ```
 
 ```bibtex
-@inproceedings{rae-razavi-2020-transformers,
-    title   = "Do Transformers Need Deep Long-Range Memory?",
-    author  = "Rae, Jack  and Razavi, Ali",
-    booktitle = "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics",
-    month   = jul,
-    year    = "2020",
-    address = "Online",
-    publisher = "Association for Computational Linguistics",
-    url     = "https://www.aclweb.org/anthology/2020.acl-main.672"
-}
-```
-
-```bibtex
 @inproceedings{Sun2022ALT,
     title     = {A Length-Extrapolatable Transformer},
     author    = {Yutao Sun and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary and Xia Song and Furu Wei},
     year      = {2022}
 }
 ```
```

#### html2text {}

```diff
@@ -9,54 +9,46 @@
 block_recurrent_transformer_pytorch import BlockRecurrentTransformer model =
 BlockRecurrentTransformer( num_tokens = 20000, # vocab size dim = 512, # model
 dimensions depth = 6, # depth dim_head = 64, # attention head dimensions heads
 = 8, # number of attention heads max_seq_len = 1024, # the total receptive
 field of the transformer, in the paper this was 2 * block size block_width =
 512, # block size - total receptive field is max_seq_len, 2 * block size in
 paper. the block furthest forwards becomes the new cached xl memories, which is
-a block size of 1 (please open an issue if i am wrong) xl_memories_layers = (5,
-6), # which layers to use xl memories. very old deepmind papers have shown you
-only need the last penultimate layers to have cached key values to see majority
-of benefit num_state_vectors = 512, # number of state vectors, i believe this
-was a single block size in the paper, but can be any amount recurrent_layers =
-(4,), # where to place the recurrent layer(s) for states with fixed simple
-gating enhanced_recurrence = True, # enhanced recurrence from ernie-doc paper,
-i have seen it to work well on my local machine use_flash_attn = True # use
-flash attention, if on pytorch 2.0 ) seq = torch.randint(0, 2000, (1, 1024))
-out, mems1, states1 = model(seq) out, mems2, states2 = model(seq, xl_memories =
-mems1, states = states1) out, mems3, states3 = model(seq, xl_memories = mems2,
-states = states2) ``` ## Test on Enwik8 First `pip install -
-r requirements.txt`, then ```bash $ python train.py ``` ## Todo - [x] use
-dynamic positional bias - [x] add enhanced recurrence - [x] setup local
-attention blocks, as in the paper - [x] wrapper transformer class for training
-- [x] take care of generation with recurrence in `RecurrentTrainWrapper` - [x]
-add ability to dropout to entire memories and states during each segment step
-during trainng - [x] test full system on enwik8 locally and ablate states and
-memories and see effects first hand - [x] make sure attention allow for single
-head key / values too - [x] run a few experiments of fixed gating in regular
-transformers - does not work - [x] integrate flash_attention - [x] cache
-attention mask + rotary embeddings - [ ] revisit memformer - [ ] add ability to
-gate in memorizing transformers knn attention layers ## Citations ```bibtex
-@article{Hutchins2022BlockRecurrentT, title = {Block-Recurrent Transformers},
-author = {DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer
-and Behnam Neyshabur}, journal = {ArXiv}, year = {2022}, volume = {abs/
-2203.07852} } ``` ```bibtex @article{Ding2021ERNIEDocAR, title = {ERNIE-Doc: A
-Retrospective Long-Document Modeling Transformer}, author = {Siyu Ding and
-Junyuan Shang and Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng
-Wang}, journal = {ArXiv}, year = {2021}, volume = {abs/2012.15688} } ```
-```bibtex @article{Shazeer2019FastTD, title = {Fast Transformer Decoding: One
-Write-Head is All You Need}, author = {Noam M. Shazeer}, journal = {ArXiv},
-year = {2019}, volume = {abs/1911.02150} } ``` ```bibtex @inproceedings{rae-
-razavi-2020-transformers, title = "Do Transformers Need Deep Long-Range
-Memory?", author = "Rae, Jack and Razavi, Ali", booktitle = "Proceedings of the
-58th Annual Meeting of the Association for Computational Linguistics", month =
-jul, year = "2020", address = "Online", publisher = "Association for
-Computational Linguistics", url = "https://www.aclweb.org/anthology/2020.acl-
-main.672" } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A Length-
-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun Patra
-and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary and Xia
-Song and Furu Wei}, year = {2022} } ``` ```bibtex @inproceedings
+a block size of 1 (please open an issue if i am wrong) num_state_vectors = 512,
+# number of state vectors, i believe this was a single block size in the paper,
+but can be any amount recurrent_layers = (4,), # where to place the recurrent
+layer(s) for states with fixed simple gating enhanced_recurrence = True, #
+enhanced recurrence from ernie-doc paper, i have seen it to work well on my
+local machine use_flash_attn = True # use flash attention, if on pytorch 2.0 )
+seq = torch.randint(0, 2000, (1, 1024)) out, mems1, states1 = model(seq) out,
+mems2, states2 = model(seq, xl_memories = mems1, states = states1) out, mems3,
+states3 = model(seq, xl_memories = mems2, states = states2) ``` ## Test on
+Enwik8 First `pip install -r requirements.txt`, then ```bash $ python train.py
+``` ## Todo - [x] use dynamic positional bias - [x] add enhanced recurrence -
+[x] setup local attention blocks, as in the paper - [x] wrapper transformer
+class for training - [x] take care of generation with recurrence in
+`RecurrentTrainWrapper` - [x] add ability to dropout to entire memories and
+states during each segment step during trainng - [x] test full system on enwik8
+locally and ablate states and memories and see effects first hand - [x] make
+sure attention allow for single head key / values too - [x] run a few
+experiments of fixed gating in regular transformers - does not work - [x]
+integrate flash_attention - [x] cache attention mask + rotary embeddings - [ ]
+revisit memformer - [ ] add ability to gate in memorizing transformers knn
+attention layers - [ ] add compressed_memories ## Citations ```bibtex @article
+{Hutchins2022BlockRecurrentT, title = {Block-Recurrent Transformers}, author =
+{DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam
+Neyshabur}, journal = {ArXiv}, year = {2022}, volume = {abs/2203.07852} } ```
+```bibtex @article{Ding2021ERNIEDocAR, title = {ERNIE-Doc: A Retrospective
+Long-Document Modeling Transformer}, author = {Siyu Ding and Junyuan Shang and
+Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang}, journal =
+{ArXiv}, year = {2021}, volume = {abs/2012.15688} } ``` ```bibtex @article
+{Shazeer2019FastTD, title = {Fast Transformer Decoding: One Write-Head is All
+You Need}, author = {Noam M. Shazeer}, journal = {ArXiv}, year = {2019}, volume
+= {abs/1911.02150} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
+Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
+Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
+and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex @inproceedings
 {dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
 Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
 Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
 in Neural Information Processing Systems}, year = {2022} } ``` *Memory is
 Attention through Time* - Alex Graves
```

### Comparing `block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -401,37 +401,39 @@
         self.attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
 
         self.block_width = block_width
         self.is_recurrent_layer = num_state_vectors > 0
 
         self.to_out = nn.Linear(inner_dim * (2 if self.is_recurrent_layer else 1), dim, bias = False)
 
-        if self.is_recurrent_layer:
-            self.state_norm = LayerNorm(dim)
+        if not self.is_recurrent_layer:
+            return
 
-            self.q_to_state = nn.Linear(dim, inner_dim, bias = False)
-            self.q_from_state = nn.Linear(dim, inner_dim, bias = False)
+        self.state_norm = LayerNorm(dim)
 
-            self.state_to_q = nn.Linear(dim, inner_dim, bias = False)
-            self.state_to_kv = nn.Linear(dim, dim_head * 2, bias = False)
+        self.q_to_state = nn.Linear(dim, inner_dim, bias = False)
+        self.q_from_state = nn.Linear(dim, inner_dim, bias = False)
 
-            self.init_state = nn.Parameter(torch.randn(num_state_vectors, dim))
-            self.state_pos_ids = nn.Parameter(torch.randn(num_state_vectors, dim))
+        self.state_to_q = nn.Linear(dim, inner_dim, bias = False)
+        self.state_to_kv = nn.Linear(dim, dim_head * 2, bias = False)
 
-            self.to_state_out = nn.Linear(inner_dim * 2, dim, bias = False)
+        self.init_state = nn.Parameter(torch.randn(num_state_vectors, dim))
+        self.state_pos_ids = nn.Parameter(torch.randn(num_state_vectors, dim))
 
-            self.to_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+        self.to_state_out = nn.Linear(inner_dim * 2, dim, bias = False)
 
-            self.state_self_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
-            self.from_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+        self.to_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
 
-            # gating related parameters - using the fixed simple config
+        self.state_self_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
+        self.from_state_cross_attn = Attention(dim_head, qk_rmsnorm = qk_rmsnorm, qk_rmsnorm_scale = qk_rmsnorm_scale, use_flash_attn = use_flash_attn)
 
-            self.state_out_to_gate = nn.Linear(dim, dim)
-            self.learned_ema_beta = nn.Parameter(torch.randn(dim))
+        # gating related parameters - using the fixed simple config
+
+        self.state_out_to_gate = nn.Linear(dim, dim)
+        self.learned_ema_beta = nn.Parameter(torch.randn(dim))
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     def forward(
         self,
@@ -441,172 +443,141 @@
         attn_mask = None,
         return_memories_and_states = None,
         xl_memories: Optional[torch.Tensor] = None,
         states: Optional[torch.Tensor] = None
     ):
         batch, seq_len, _, width, device = *x.shape, self.block_width, self.device
 
-        # first make sure to pad the sequence length to multiple of the block widths
-        # for local attention
-
-        if not divisible_by(seq_len, width):
-            padding_to_width_multiple = math.ceil(seq_len / width) * width - seq_len
-            x = pad_at_dim(x, (0, padding_to_width_multiple), dim = -2, value = 0)
-
         # pre normalization
 
         x = self.norm(x)
 
         # queries, keys, values and split out heads
 
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
 
         split_head = partial(rearrange, pattern = 'b n (h d) -> b h n d', h = self.heads)
         q = split_head(q)
 
-        # bucket the queries, keys, values by block width
-
-        bq, bk, bv = map(lambda t: rearrange(t, 'b ... (w n) d -> b w ... n d', n = width), (q, k, v))
-
         # save the last key / values as memories for recurrence
 
         memories = None
 
         if return_memories_and_states:
-            memories = torch.stack((bk[:, -1], bv[:, -1]))
+            memories = torch.stack((k, v))
+
+        mem_len = 0
 
         if exists(xl_memories):
             # if past memories are passed in, concat as the first bucket
+            mem_len = xl_memories.shape[-2]
             past_k, past_v = xl_memories
-            past_k, past_v = map(lambda t: rearrange(t, 'b ... n d -> b 1 ... n d'), (past_k, past_v))
-            bk = torch.cat((past_k, bk), dim = 1)
-            bv = torch.cat((past_v, bv), dim = 1)
-        else:
-            # otherwise add padding
-            bk = pad_at_dim(bk, (1, 0), value = 0., dim = 1)
-            bv = pad_at_dim(bv, (1, 0), value = 0., dim = 1)
+            k = torch.cat((past_k, k), dim = 1)
+            v = torch.cat((past_v, v), dim = 1)
 
-        # alter attention mask so that the first window looking back would either attend to nothing (in the case of padding), or everything (in the case of xl memories)
+        # handle cropping of attention mask and positional embeddings
 
         if exists(attn_mask):
-            attn_mask = repeat(attn_mask, 'i j -> w 1 i j', w = bq.shape[1])
-            attn_mask[0, 0, :, :width] = exists(xl_memories)
-
-        # local attention with look back of one bucket - in paper they did total receptive field of 2 * block_width, with 1 block_width worth of memories, seems like a more efficient transformer-xl design?
-
-        bk = torch.cat((bk[:, :-1], bk[:, 1:]), dim = -2)
-        bv = torch.cat((bv[:, :-1], bv[:, 1:]), dim = -2)
+            attn_mask = attn_mask[:seq_len, (width - mem_len):(width + seq_len)]
 
         # attention, but of course
 
         out = self.attn(
-            bq, bk, bv,
+            q, k, v,
             rotary_pos_emb = rotary_pos_emb,
             xpos_scale = xpos_scale,
             mask = attn_mask
         )
 
-        # merge the heads as well as the buckets
+        new_states = None
 
-        out = rearrange(out, 'b w h n d -> b (w n) (h d)')
+        # merge heads
 
-        # in case there is padding during sampling, splice it out
+        out = rearrange(out, 'b h n d -> b n (h d)')
 
-        out = out[:, :seq_len]
+        # early return if not a recurrent layer
 
-        new_states = None
+        if not self.is_recurrent_layer:
+            return self.to_out(out), memories, new_states
 
         # if designated a recurrent layer, do all the state logic
         # it was hard moving this to a separate module, as the attention is closely intertwined between the current tokens and state tokens
 
-        if self.is_recurrent_layer:
-            # process input in blocks
-
-            x_blocks, k_blocks, v_blocks = map(lambda t: t[:, :seq_len].split(width, dim = -2), (x, k, v))
-
-            # ready attended output of the input to the state, concatted block by block
-
-            to_state_out = torch.empty((batch, 0, out.shape[-1]), device = device, dtype = out.dtype)
-
-            # use initial state if no states were passed in
+        # ready attended output of the input to the state, concatted block by block
 
-            if not exists(states):
-                states = self.init_state
+        to_state_out = torch.empty((batch, 0, out.shape[-1]), device = device, dtype = out.dtype)
 
-            for ind, (x_block, xk_block, xv_block) in enumerate(zip(x_blocks, k_blocks, v_blocks)):
-                is_last = ind == (len(x_blocks) - 1)
+        # use initial state if no states were passed in
 
-                residual_states = states
+        if not exists(states):
+            states = self.init_state
 
-                # pre norm state for attention
+        # state residual
 
-                states = self.state_norm(states)
+        residual_states = states
 
-                # add the positional ids, as stated in the paper critical for it to work
+        # pre norm state for attention
 
-                states = states + self.state_pos_ids
+        states = self.state_norm(states)
 
-                # get queries for cross attention, which they do not share, although they share key / values. another intriguing detail
+        # add the positional ids, as stated in the paper critical for it to work
 
-                q_to_state = self.q_to_state(x_block)
-                q_from_state = self.q_from_state(states)
+        states = states + self.state_pos_ids
 
-                q_to_state, q_from_state = map(lambda t: rearrange(t, '... n (h d) -> ... h n d', h = self.heads), (q_to_state, q_from_state))
+        # get queries for cross attention, which they do not share, although they share key / values. another intriguing detail
 
-                # self attention qkv for states
+        q_to_state = self.q_to_state(x)
+        q_from_state = self.q_from_state(states)
 
-                state_q, state_k, state_v = (self.state_to_q(states), *self.state_to_kv(states).chunk(2, dim = -1))
+        q_to_state, q_from_state = map(lambda t: rearrange(t, '... n (h d) -> ... h n d', h = self.heads), (q_to_state, q_from_state))
 
-                state_q_einsum = 'n (h d)' if state_q.ndim == 2 else 'b n (h d)'
-                state_q = repeat(state_q, f'{state_q_einsum} -> b h n d', h = self.heads, b = batch)
+        # self attention qkv for states
 
-                # cross attend to the past states key values
+        state_q, state_k, state_v = (self.state_to_q(states), *self.state_to_kv(states).chunk(2, dim = -1))
 
-                to_state_out_block = self.to_state_cross_attn(q_to_state, state_k, state_v)
+        state_q_einsum = 'n (h d)' if state_q.ndim == 2 else 'b n (h d)'
+        state_q = repeat(state_q, f'{state_q_einsum} -> b h n d', h = self.heads, b = batch)
 
-                to_state_out_block = rearrange(to_state_out_block, 'b h n d -> b n (h d)')
+        # cross attend to the past states key values
 
-                to_state_out = torch.cat((to_state_out, to_state_out_block), dim = -2)
+        to_state_out_block = self.to_state_cross_attn(q_to_state, state_k, state_v)
 
-                # if need to return states, or is not the last block, calculate state update
+        to_state_out_block = rearrange(to_state_out_block, 'b h n d -> b n (h d)')
 
-                if return_memories_and_states or not is_last:
+        to_state_out = torch.cat((to_state_out, to_state_out_block), dim = -2)
 
-                    # states must also undergo self attention
+        # states must also undergo self attention
 
-                    if q_from_state.ndim == 3:
-                        q_from_state = repeat(q_from_state, '... -> b ...', b = batch)
+        if q_from_state.ndim == 3:
+            q_from_state = repeat(q_from_state, '... -> b ...', b = batch)
 
-                    state_out = self.state_self_attn(state_q, state_k, state_v)
+        state_out = self.state_self_attn(state_q, state_k, state_v)
 
-                    from_state_out = self.from_state_cross_attn(q_from_state, xk_block, xv_block)
+        from_state_out = self.from_state_cross_attn(q_from_state, k, v)
 
-                    state_out = torch.cat((state_out, from_state_out), dim = -1)
-                    state_out = rearrange(state_out, 'b h n d -> b n (h d)')
+        state_out = torch.cat((state_out, from_state_out), dim = -1)
+        state_out = rearrange(state_out, 'b h n d -> b n (h d)')
 
-                    state_out = self.to_state_out(state_out)
+        state_out = self.to_state_out(state_out)
 
-                    # use the best performing configuration
-                    # fixed simple gate - nothing more than a learned EMA with some resemblance to highway networks
+        # use the best performing configuration
+        # fixed simple gate - nothing more than a learned EMA with some resemblance to highway networks
 
-                    z = self.state_out_to_gate(state_out)
-                    learned_ema_decay = self.learned_ema_beta.sigmoid()
+        z = self.state_out_to_gate(state_out)
+        learned_ema_decay = self.learned_ema_beta.sigmoid()
 
-                    # set new state with the learned EMA gating
+        # set new state with the learned EMA gating
 
-                    states = learned_ema_decay * z + (1 - learned_ema_decay) * residual_states
+        states = learned_ema_decay * z + (1 - learned_ema_decay) * residual_states
 
-            # concat the output of cross attending to the state vectors
+        # concat the output of cross attending to the state vectors
 
-            out = torch.cat((out, to_state_out), dim = -1)
+        out = torch.cat((out, to_state_out), dim = -1)
 
-            if return_memories_and_states:
-                new_states = states
-
-        return self.to_out(out), memories, new_states
+        return self.to_out(out), memories, states
 
 # classes
 
 @beartype
 class BlockRecurrentTransformer(nn.Module):
     def __init__(
         self,
@@ -616,51 +587,45 @@
         depth,
         dim_head = 64,
         heads = 8,
         all_layers_qk_rmsnorm = False,
         ff_mult = 4,
         max_seq_len = 1024,
         block_width = 512,
-        xl_memories_layers: Optional[Tuple[int, ...]] = None,
         recurrent_layers: Optional[Tuple[int, ...]] = None,
         num_state_vectors = None,
         enhanced_recurrence = False,
         ignore_index = -100,
         use_flash_attn = False
     ):
         super().__init__()
         num_state_vectors = default(num_state_vectors, block_width)
-        xl_memories_layers = default(xl_memories_layers, tuple(range(1, depth + 1)))
-        self.xl_memories_layers = set(xl_memories_layers)
-
-        assert all([0 < layer <= depth for layer in xl_memories_layers])
 
         recurrent_layers = default(recurrent_layers, (depth // 2,)) # default to one recurent layer at middle of the network
         self.recurrent_layers = set(recurrent_layers)
 
         assert all([0 < layer <= depth for layer in recurrent_layers])
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         self.rotary_pos_emb = RotaryEmbedding(dim = dim_head)
 
         self.layers = nn.ModuleList([])
 
         for layer in range(1, depth + 1):
             is_recurrent_layer = layer in self.recurrent_layers
-            is_xl_layer = layer in self.xl_memories_layers
 
             layer_num_state_vectors = num_state_vectors if is_recurrent_layer else 0
 
             # only layers with xl memories
             # or has recurrence in horizontal direction
             # use qk rmsnorm (in paper, they use cosine sim attention, but i think qk rmsnorm is more proven given Vit 22B paper)
             # one can also override to use all qk rmsnorm by setting all_layers_qk_rmsnorm = True
 
-            qk_rmsnorm = all_layers_qk_rmsnorm or is_recurrent_layer or is_xl_layer
+            qk_rmsnorm = all_layers_qk_rmsnorm or is_recurrent_layer
 
             self.layers.append(nn.ModuleList([
                 AttentionBlock(
                     dim,
                     block_width = block_width,
                     dim_head = dim_head,
                     heads = heads,
@@ -786,86 +751,113 @@
         x = self.token_emb(x)
 
         # dynamic pos bias
 
         attn_mask = self.get_causal_attn_mask(w)
         rotary_pos_emb, xpos_scale = self.rotary_pos_emb(2 * w)
 
-        # enhanced recurrence
+        # only return memories and state if at the full block width, but can be overridden
 
-        if self.enhanced_recurrence and len(xl_memories) > 1:
-            xl_memories = [*xl_memories[1:], xl_memories[0]]
+        return_memories_and_states = default(return_memories_and_states, self.max_seq_len == x.shape[-2])
 
-        # ready xl memories and states
+        # ready output tensor, to be concatted to block by block
 
-        xl_memories = iter(xl_memories)
-        states = iter(states)
+        batch, _, dim = x.shape
 
-        next_xl_memories = []
-        next_states = []
+        out = torch.empty(batch, 0, dim, dtype = x.dtype, device = self.device)
 
-        return_memories_and_states = default(return_memories_and_states, self.max_seq_len == x.shape[-2])
+        # split input into blocks of width w
 
-        # go through layers
+        input_blocks = x.split(w, dim = -2)
 
-        for ind, (attn, ff) in enumerate(self.layers):
+        # process each block at a time
 
-            # determine if the layer requires transformer xl memories
+        for input_block in input_blocks:
 
-            layer = ind + 1
+            # enhanced recurrence
 
-            is_xl_layer     = layer in self.xl_memories_layers
-            is_state_layer  = attn.is_recurrent_layer
+            if self.enhanced_recurrence and len(xl_memories) > 1:
+                xl_memories = [*xl_memories[1:], xl_memories[0]]
 
-            # whether to pass in xl memories
+            # ready xl memories and states
 
-            attn_kwargs = dict(
-                rotary_pos_emb = rotary_pos_emb,
-                xpos_scale = xpos_scale,
-                attn_mask = attn_mask,
-                return_memories_and_states = return_memories_and_states
-            )
+            xl_memories = iter(xl_memories)
+            states = iter(states)
+
+            next_xl_memories = []
+            next_states = []
+
+            # go through layers
+
+            for ind, (attn, ff) in enumerate(self.layers):
+
+                # determine if the layer requires transformer xl memories
 
-            if is_xl_layer:
-                attn_kwargs.update(xl_memories = next(xl_memories, None))
+                layer = ind + 1
+                is_state_layer  = attn.is_recurrent_layer
 
-            if is_state_layer:
-                attn_kwargs.update(states = next(states, None))
+                # whether to pass in xl memories
 
-            # attention layer
+                attn_kwargs = dict(
+                    rotary_pos_emb = rotary_pos_emb,
+                    xpos_scale = xpos_scale,
+                    attn_mask = attn_mask,
+                    xl_memories = next(xl_memories, None),
+                    return_memories_and_states = return_memories_and_states
+                )
 
-            residual = x
-            attn_branch_out, layer_xl_memories, layer_next_states = attn(x, **attn_kwargs)
+                if is_state_layer:
+                    attn_kwargs.update(states = next(states, None))
 
-            if return_memories_and_states:
-                # save states if needed
+                # attention layer
+
+                residual = input_block
+                attn_branch_out, layer_xl_memories, layer_next_states = attn(input_block, **attn_kwargs)
+
+                if exists(layer_xl_memories):
+                    next_xl_memories.append(layer_xl_memories)
 
                 if exists(layer_next_states):
-                    next_states.append(layer_next_states.detach())
+                    next_states.append(layer_next_states)
+
+                input_block = attn_branch_out + residual
+
+                # feedforward layer
+
+                input_block = ff(input_block) + input_block
 
-                # save current xl memories if needed
+            # concat to output
 
-                if is_xl_layer:
-                    next_xl_memories.append(layer_xl_memories.detach())
+            out = torch.cat((out, input_block), dim = -2)
 
-            x = attn_branch_out + residual
+            # set new xl memories and states
 
-            # feedforward layer
+            states = next_states
+            xl_memories = next_xl_memories
 
-            x = ff(x) + x
+        # project to logits
 
-        logits = self.to_logits(x)
+        logits = self.to_logits(out)
+
+        # detach the states and memories
+
+        returned_next_states = list(map(torch.detach, states)) if return_memories_and_states else None
+        returned_next_xl_memories = list(map(torch.detach, xl_memories)) if return_memories_and_states else None
+
+        # whether to return logits
 
         if not return_loss:
-            return logits, next_xl_memories, next_states
+            return logits, returned_next_xl_memories, returned_next_states
+
+        # cross entropy loss
 
         logits = rearrange(logits, 'b n c -> b c n')
         loss = F.cross_entropy(logits, labels, ignore_index = self.ignore_index)
 
-        return loss, next_xl_memories, next_states
+        return loss, returned_next_xl_memories, returned_next_states
 
 # recurrent trainer wrapper
 
 @beartype
 class RecurrentTrainerWrapper(nn.Module):
     def __init__(
         self,
@@ -925,15 +917,19 @@
             )
 
             output = torch.cat((output, segment_output), dim = -1)
             current_len = 1
 
         return output[:, start_len:]
 
-    def forward(self, x, return_memories_and_states = False):
+    def forward(
+        self,
+        x,
+        return_memories_and_states = False
+    ):
         total_seq_len, seq_len = x.shape[1], self.seq_len
 
         assert divisible_by(total_seq_len - 1, seq_len), f'length of sequence ({total_seq_len}) must be equal to a multiple of {seq_len} + 1 (one extra token) during training'
         segments = total_seq_len // seq_len
 
         total_loss = 0.
```

### Comparing `block-recurrent-transformer-pytorch-0.2.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.3.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.2.2
+Version: 0.3.0
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.2.2/setup.py` & `block-recurrent-transformer-pytorch-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.3.0',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

