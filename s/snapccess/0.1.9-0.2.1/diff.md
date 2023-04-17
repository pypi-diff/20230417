# Comparing `tmp/snapccess-0.1.9.tar.gz` & `tmp/snapccess-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapccess-0.1.9.tar", max compression
+gzip compressed data, was "snapccess-0.2.1.tar", max compression
```

## Comparing `snapccess-0.1.9.tar` & `snapccess-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       15 2023-01-17 00:30:17.518742 snapccess-0.1.9/README.md
--rw-r--r--   0        0        0      421 2023-02-21 23:52:10.047296 snapccess-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-21 23:40:32.854532 snapccess-0.1.9/snapccess/__init__.py
--rw-r--r--   0        0        0     3727 2023-01-23 00:05:51.063642 snapccess-0.1.9/snapccess/model.py
--rw-r--r--   0        0        0     3302 2023-01-17 10:52:07.848132 snapccess-0.1.9/snapccess/train.py
--rw-r--r--   0        0        0     3303 2022-11-15 03:30:35.116840 snapccess-0.1.9/snapccess/util.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 snapccess-0.1.9/setup.py
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 snapccess-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-01-17 00:30:17.518742 snapccess-0.2.1/README.md
+-rw-r--r--   0        0        0      421 2023-04-17 00:54:46.183369 snapccess-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-02-22 00:18:13.161087 snapccess-0.2.1/snapccess/__init__.py
+-rw-r--r--   0        0        0     3187 2023-04-17 00:48:17.050565 snapccess-0.2.1/snapccess/model.py
+-rw-r--r--   0        0        0     3302 2023-01-17 10:52:07.848132 snapccess-0.2.1/snapccess/train.py
+-rw-r--r--   0        0        0     2993 2023-04-17 00:53:04.163149 snapccess-0.2.1/snapccess/util.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 snapccess-0.2.1/PKG-INFO
```

### Comparing `snapccess-0.1.9/snapccess/model.py` & `snapccess-0.2.1/snapccess/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         super().__init__(*layers)
 
 ## nn.module is the superclass, encoder is the subclass
 class Encoder(nn.Module):
     """Encoder for multi-modal data"""
     def __init__(self, num_features: list, num_hidden_features: list, z_dim: int=128):
         super().__init__()
-        self.features=num_features #[num_features[i] for i in range(len(num_features))]  
+        self.features=num_features
         self.encoder_eachmodal= nn.ModuleList([LinBnDrop(num_features[i], num_hidden_features[i], p=0.2, act=nn.ReLU())
                                  for i in range(len(num_hidden_features))]).to(device) 
         self.encoder = LinBnDrop(sum(num_hidden_features), z_dim, act=nn.ReLU()).to(device)
         self.weights=[]
         for i in range(len(num_features)):
             self.weights.append(nn.Parameter(torch.rand(1,num_features[i]) * 0.001, requires_grad=True).to(device))# 
         self.fc_mu =nn.Sequential( LinBnDrop(z_dim,z_dim, p=0.1),#0.1
@@ -35,51 +35,44 @@
         eps = torch.randn_like(std)
         return eps * std + mu
 
     def forward(self, x):
         X = []
         startfeature=0
         for i, eachmodal in enumerate(self.encoder_eachmodal):
-            if i == 0:
-                tmp=eachmodal(x[:,startfeature:self.features[i]]*self.weights[i])
-                startfeature=startfeature+self.features[i]
-                X.append(tmp)
-            else:
-                tmp=eachmodal(x[:,startfeature:(startfeature+self.features[i])]*self.weights[i])
-                startfeature=startfeature+self.features[i]
-                X.append(tmp)
-        #X = [self.encoder_eachmodal[i](x[:,:self.features[i]]*self.weights[i]) for i in range(len(self.features))]
+            tmp=eachmodal(x[:,startfeature:(startfeature+self.features[i])]*self.weights[i])
+            startfeature=startfeature+self.features[i]
+            X.append(tmp)
         x = torch.cat(X, 1)
         x = self.encoder(x)
         mu = self.fc_mu(x)
         var = self.fc_var(x)
         x = self.reparameterize(mu, var)
         return x,mu,var
     
     
     
 class Decoder(nn.Module):
     """Decoder for 2 modal data"""
     def __init__(self, num_features: list, z_dim: int = 128):
         super().__init__()
-        self.features=num_features #[num_features[i] for i in range(len(num_features))]  
+        self.features=num_features
         self.decoder_eachmodal= nn.ModuleList([ LinBnDrop(z_dim, num_features[i], act=nn.ReLU()) for i in range(len(num_features))]).to(device) 
 
     def forward(self, x):
-        #X = [self.decoder_eachmodal[i](x) for i in range(len(self.decoder_eachmodal))]
         X = []
         for i, deachmodal in enumerate(self.decoder_eachmodal):
             tmp=deachmodal(x)
             X.append(tmp)
         x = torch.cat(X, 1)
         return x
 
 class snapshotVAE(nn.Module):
     def __init__(self, num_features: list, num_hidden_features: list, z_dim: int = 20):
         super().__init__()
         self.encoder = Encoder(num_features, num_hidden_features, z_dim)
         self.decoder = Decoder(num_features, z_dim)
     def forward(self, x):
-        x,mu,var = self.encoder(x) #
+        x,mu,var = self.encoder(x)
         x = self.decoder(x)
         return x,mu,var
```

### Comparing `snapccess-0.1.9/snapccess/train.py` & `snapccess-0.2.1/snapccess/train.py`

 * *Files identical despite different names*

### Comparing `snapccess-0.1.9/snapccess/util.py` & `snapccess-0.2.1/snapccess/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,38 +12,22 @@
 # LongTensor = torch.cuda.LongTensor if cuda else torch.LongTensor
 
 def snapshot_lr(initial_lr, epoch, epoch_per_cycle):
     # proposed learning late function #return initial_lr * (cos(pi * epoch / epoch_per_cycle) + 1) / 2
     return initial_lr * (cos(pi * ((epoch-1)%epoch_per_cycle) / epoch_per_cycle) + 1) / 2
 
 def setup_seed(seed):
-     torch.manual_seed(seed)
-     torch.cuda.manual_seed_all(seed)
-     np.random.seed(seed)
-     random.seed(seed)
-     torch.backends.cudnn.deterministic = True
-     torch.backends.cudnn.benchmark = False
-     os.environ['PYTHONHASHSEED']=str(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+    np.random.seed(seed)
+    random.seed(seed)
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
+    os.environ['PYTHONHASHSEED']=str(seed)
 
- 
-
-from torch.utils.data import Dataset
-
-class TabularDataset(Dataset):
-    """Custome dataset for tabular data"""
-    def __init__(self, data):
-        self.data = data
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, idx):
-        x = self.data[idx]
-        return x
- 
 
 def get_encodings(model, dl):
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     model.eval()
     result = []
     with torch.no_grad():
         for x in dl:
```

### Comparing `snapccess-0.1.9/PKG-INFO` & `snapccess-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapccess
-Version: 0.1.9
+Version: 0.2.1
 Summary: Ensemble deep learning of embeddings for clustering multimodal single-cell omics data
 Author: Lijia Yu
 Author-email: yulj2010@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

