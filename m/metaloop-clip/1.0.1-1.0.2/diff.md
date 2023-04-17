# Comparing `tmp/metaloop-clip-1.0.1.tar.gz` & `tmp/metaloop-clip-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metaloop-clip-1.0.1.tar", last modified: Mon Oct 31 15:29:55 2022, max compression
+gzip compressed data, was "dist/metaloop-clip-1.0.2.tar", last modified: Mon Apr 17 09:47:58 2023, max compression
```

## Comparing `metaloop-clip-1.0.1.tar` & `metaloop-clip-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/
--rw-rw-r--   0 yadda     (1000) yadda     (1000)       42 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/MANIFEST.in
--rw-rw-r--   0 yadda     (1000) yadda     (1000)      184 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/PKG-INFO
--rw-rw-r--   0 yadda     (1000) yadda     (1000)     7024 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/README.md
-drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/clip/
--rw-rw-r--   0 yadda     (1000) yadda     (1000)       20 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/clip/__init__.py
--rw-rw-r--   0 yadda     (1000) yadda     (1000)  1356917 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 yadda     (1000) yadda     (1000)     9396 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/clip/clip.py
--rw-rw-r--   0 yadda     (1000) yadda     (1000)    17374 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/clip/model.py
--rw-rw-r--   0 yadda     (1000) yadda     (1000)     4632 2022-07-27 19:42:37.000000 metaloop-clip-1.0.1/clip/simple_tokenizer.py
-drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/
--rw-rw-r--   0 yadda     (1000) yadda     (1000)      184 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/PKG-INFO
--rw-rw-r--   0 yadda     (1000) yadda     (1000)      317 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/SOURCES.txt
--rw-rw-r--   0 yadda     (1000) yadda     (1000)        1 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/dependency_links.txt
--rw-rw-r--   0 yadda     (1000) yadda     (1000)       48 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/requires.txt
--rw-rw-r--   0 yadda     (1000) yadda     (1000)        5 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/metaloop_clip.egg-info/top_level.txt
--rw-rw-r--   0 yadda     (1000) yadda     (1000)       38 2022-10-31 15:29:55.000000 metaloop-clip-1.0.1/setup.cfg
--rw-rw-r--   0 yadda     (1000) yadda     (1000)      436 2022-10-31 15:29:52.000000 metaloop-clip-1.0.1/setup.py
+drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)       42 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/MANIFEST.in
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)      184 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/PKG-INFO
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)     7024 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/README.md
+drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/clip/
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)       20 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/clip/__init__.py
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)  1356917 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)     9396 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/clip/clip.py
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)    17366 2023-04-17 09:45:39.000000 metaloop-clip-1.0.2/clip/model.py
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)     4632 2022-07-27 19:42:37.000000 metaloop-clip-1.0.2/clip/simple_tokenizer.py
+drwxrwxr-x   0 yadda     (1000) yadda     (1000)        0 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)      184 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/PKG-INFO
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)      317 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/SOURCES.txt
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)        1 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/dependency_links.txt
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)       48 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/requires.txt
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)        5 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/metaloop_clip.egg-info/top_level.txt
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)       38 2023-04-17 09:47:58.000000 metaloop-clip-1.0.2/setup.cfg
+-rw-rw-r--   0 yadda     (1000) yadda     (1000)      436 2023-04-17 09:46:20.000000 metaloop-clip-1.0.2/setup.py
```

### Comparing `metaloop-clip-1.0.1/README.md` & `metaloop-clip-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `metaloop-clip-1.0.1/clip/bpe_simple_vocab_16e6.txt.gz` & `metaloop-clip-1.0.2/clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `metaloop-clip-1.0.1/clip/clip.py` & `metaloop-clip-1.0.2/clip/clip.py`

 * *Files identical despite different names*

### Comparing `metaloop-clip-1.0.1/clip/model.py` & `metaloop-clip-1.0.2/clip/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             dropout_p=0,
             out_proj_weight=self.c_proj.weight,
             out_proj_bias=self.c_proj.bias,
             use_separate_proj_weight=True,
             training=self.training,
             need_weights=False
         )
-        return x.squeeze(0)
+        return x[0]
 
 
 class ModifiedResNet(nn.Module):
     """
     A ResNet class that is similar to torchvision's but contains the following changes:
     - There are now 3 "stem" convolutions as opposed to 1, with an average pool instead of a max pool.
     - Performs anti-aliasing strided convolutions, where an avgpool is prepended to convolutions with stride > 1
```

### Comparing `metaloop-clip-1.0.1/clip/simple_tokenizer.py` & `metaloop-clip-1.0.2/clip/simple_tokenizer.py`

 * *Files identical despite different names*

