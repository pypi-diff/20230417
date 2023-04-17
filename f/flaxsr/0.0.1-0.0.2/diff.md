# Comparing `tmp/flaxsr-0.0.1-py3-none-any.whl.zip` & `tmp/flaxsr-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,20 @@
-Zip file size: 11035 bytes, number of entries: 15
+Zip file size: 14541 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx       42 b- defN 23-Apr-16 13:04 FlaxSR/__init__.py
 -rw-rw-r--  2.0 unx      179 b- defN 23-Apr-16 09:21 FlaxSR/layers/__init__.py
--rw-rw-r--  2.0 unx     1478 b- defN 23-Apr-16 09:03 FlaxSR/layers/stochastic.py
--rw-rw-r--  2.0 unx     1564 b- defN 23-Apr-16 13:04 FlaxSR/layers/upscale.py
--rw-rw-r--  2.0 unx      194 b- defN 23-Apr-16 13:13 FlaxSR/models/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-17 07:28 FlaxSR/layers/stochastic.py
+-rw-rw-r--  2.0 unx     1567 b- defN 23-Apr-17 07:13 FlaxSR/layers/upscale.py
+-rw-rw-r--  2.0 unx      355 b- defN 23-Apr-17 07:49 FlaxSR/models/__init__.py
 -rw-rw-r--  2.0 unx     3658 b- defN 23-Apr-16 13:12 FlaxSR/models/edsr.py
 -rw-rw-r--  2.0 unx      858 b- defN 23-Apr-16 12:22 FlaxSR/models/espcn.py
 -rw-rw-r--  2.0 unx     1072 b- defN 23-Apr-16 12:04 FlaxSR/models/fsrcnn.py
+-rw-rw-r--  2.0 unx     6283 b- defN 23-Apr-17 07:46 FlaxSR/models/nafssr.py
+-rw-rw-r--  2.0 unx      930 b- defN 23-Apr-17 06:11 FlaxSR/models/ncnet.py
 -rw-rw-r--  2.0 unx     1013 b- defN 23-Apr-16 13:13 FlaxSR/models/srcnn.py
+-rw-rw-r--  2.0 unx     2138 b- defN 23-Apr-17 06:39 FlaxSR/models/srgan.py
 -rw-rw-r--  2.0 unx      890 b- defN 23-Apr-16 12:47 FlaxSR/models/vdsr.py
--rw-rw-r--  2.0 unx    11313 b- defN 23-Apr-16 14:03 flaxsr-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1193 b- defN 23-Apr-16 14:03 flaxsr-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-16 14:03 flaxsr-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-16 14:03 flaxsr-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1173 b- defN 23-Apr-16 14:03 flaxsr-0.0.1.dist-info/RECORD
-15 files, 24726 bytes uncompressed, 9109 bytes compressed:  63.2%
+-rw-rw-r--  2.0 unx    11313 b- defN 23-Apr-17 07:53 flaxsr-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-17 07:53 flaxsr-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 07:53 flaxsr-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-17 07:53 flaxsr-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1410 b- defN 23-Apr-17 07:53 flaxsr-0.0.2.dist-info/RECORD
+18 files, 34583 bytes uncompressed, 12253 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -18,29 +18,38 @@
 
 Filename: FlaxSR/models/espcn.py
 Comment: 
 
 Filename: FlaxSR/models/fsrcnn.py
 Comment: 
 
+Filename: FlaxSR/models/nafssr.py
+Comment: 
+
+Filename: FlaxSR/models/ncnet.py
+Comment: 
+
 Filename: FlaxSR/models/srcnn.py
 Comment: 
 
+Filename: FlaxSR/models/srgan.py
+Comment: 
+
 Filename: FlaxSR/models/vdsr.py
 Comment: 
 
-Filename: flaxsr-0.0.1.dist-info/LICENSE
+Filename: flaxsr-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: flaxsr-0.0.1.dist-info/METADATA
+Filename: flaxsr-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: flaxsr-0.0.1.dist-info/WHEEL
+Filename: flaxsr-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: flaxsr-0.0.1.dist-info/top_level.txt
+Filename: flaxsr-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: flaxsr-0.0.1.dist-info/RECORD
+Filename: flaxsr-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## FlaxSR/layers/stochastic.py

```diff
@@ -47,8 +47,7 @@
                 survival_state = jax.random.bernoulli(key, self.survival_prob, ())
                 if survival_state:
                     residual = (self.module(inputs) - inputs) / self.survival_prob
                 else:
                     residual = jnp.zeros_like(inputs)
 
                 return inputs + residual
-
```

## FlaxSR/layers/upscale.py

```diff
@@ -46,15 +46,15 @@
         input_c = inputs.shape[-1]
         out_c = self.out_c or input_c
 
         nc_kernel = self.variable(
             'nearest_conv', 'kernel', lambda: _nearest_conv_init(input_c, out_c, self.scale)
         )
 
-        output = lax.conv_general_dilated(
+        outputs = lax.conv_general_dilated(
             inputs, nc_kernel, (1, 1), 'VALID',
             dimension_numbers=('NHWC', 'HWIO', 'NHWC'),
         )
         if self.return_upscaled:
-            return _pixel_shuffle(output, self.scale)
+            return _pixel_shuffle(outputs, self.scale)
         else:
-            return output
+            return outputs
```

## FlaxSR/models/__init__.py

```diff
@@ -2,7 +2,13 @@
 from .fsrcnn import FSRCNN as FSRCNN
 from .espcn import ESPCN as ESPCN
 from .vdsr import VDSR as VDSR
 from .edsr import (
     EDSR as EDSR,
     MDSR as MDSR,
 )
+from .ncnet import NCNet as NCNet
+from .srgan import (
+    SRResNet as SRResNet,
+    # SRGAN as SRGAN,  will be added in the future
+)
+from .nafssr import NAFSSR
```

## Comparing `flaxsr-0.0.1.dist-info/LICENSE` & `flaxsr-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flaxsr-0.0.1.dist-info/METADATA` & `flaxsr-0.0.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Super Resolution models with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy (>=1.12)
-Requires-Dist: jax (>=0.4.2)
-Requires-Dist: flax (>=0.6.0)
 
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
 ## HOW TO USE
 
+### Install
+```shell
+pip install flaxsr
+```
+
+### Usage
 ```python
 from FlaxSR.models import VDSR
 import jax
 import jax.numpy as jnp
 
 inputs = jnp.ones((16, 256, 256, 3))
 key = jax.random.PRNGKey(42)
 model = VDSR(n_filters=64, n_blocks=20, scale=4)
 params = model.init(key, inputs)
 outputs = model.apply(params, inputs)
 print(outputs.shape)
 ```
 
-## Feats will be added
-
- - [ ] More models
- - [ ] Pre-trained parameters
- - [ ] Training states(includes Generative-sr models)
+## Models implemented
+ - SRCNN
+ - FSRCNN
+ - ESPCN
+ - VDSR
+ - EDSR, MDSR,
+ - NCNet
+ - SRResNet(SRGAN will be implemented in future)
+ - NAFSSR
+
+## Feats will be added in future
+
+ - More models
+ - Pre-trained parameters
+ - Training states(includes Generative-sr models)
```

## Comparing `flaxsr-0.0.1.dist-info/RECORD` & `flaxsr-0.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 FlaxSR/__init__.py,sha256=NyPxSO4MYTgfwqOgTihLlwIpKmwqYmUyeQ8wR_IkJ9A,42
 FlaxSR/layers/__init__.py,sha256=XmEUQ7GU5L6FawKfgU3PajHfOKFeOWMZPzatpkk06Ps,179
-FlaxSR/layers/stochastic.py,sha256=a52I_HHA_ZiTI0cKC3O6moOd1o5zgQldnMLu_SzyqOI,1478
-FlaxSR/layers/upscale.py,sha256=he1-pNl9zS1tYEiJgeCVuHXTep5sCFzTQvnppTiwJQI,1564
-FlaxSR/models/__init__.py,sha256=kLCfhxPdjoZs7HvTiLDhK5VgLNYUnTxP6B-nUBg_EUw,194
+FlaxSR/layers/stochastic.py,sha256=7zgAyUABe22eoytFPMCz9deJ6eXAHoK0ckskzywcMEs,1477
+FlaxSR/layers/upscale.py,sha256=C09bRf84h6OmQpxZcXMpwgAgol7foE6uAIAvgPJN7sQ,1567
+FlaxSR/models/__init__.py,sha256=oBFwirA_wQD9q9_gPSki3j8PqGf4tF4omMSWz66If2I,355
 FlaxSR/models/edsr.py,sha256=-LNKF8Jn2nrpVhacyy0XL30aOptXiEXshg2zvb76wqw,3658
 FlaxSR/models/espcn.py,sha256=rafsA-ICXjnxDunc8vTFOmA_5t4xoxP1VOpF9c-zAmA,858
 FlaxSR/models/fsrcnn.py,sha256=JR2R51ywYz5OrimyTwgd5mkDzM4drh-21vaof5jEtBA,1072
+FlaxSR/models/nafssr.py,sha256=um3sGqr1eTs3YpY91mM1PvjqUxdUfqgkeWntWNtaX9E,6283
+FlaxSR/models/ncnet.py,sha256=MI47Cdb1zu6LMeCszWaP2gvbzZchpQI7sjb06LkAEJM,930
 FlaxSR/models/srcnn.py,sha256=667uOj9YYl8JIiGFA__yx51AHT6_aRpiWDV180b32lw,1013
+FlaxSR/models/srgan.py,sha256=r203sU9EiWv5QLiQI4b9IXdcBDNsXSiBVATIZ6roYuk,2138
 FlaxSR/models/vdsr.py,sha256=OJIm13inZU7OuS7AeytvxOlgasxB-IwbkbL7Sy52AxM,890
-flaxsr-0.0.1.dist-info/LICENSE,sha256=UeuGtONxLyJHg6LVfV_8F_rV8oCPKaBRpwlgDixQCO4,11313
-flaxsr-0.0.1.dist-info/METADATA,sha256=9LOOHyMTwlEbHQJ_LyHa3Cfm3GqxK8GA8dVJs5vOZNg,1193
-flaxsr-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-flaxsr-0.0.1.dist-info/top_level.txt,sha256=MVm6sMxEshMxPdjXtT9zH_BEQEqfThUdXHoNEId4NeE,7
-flaxsr-0.0.1.dist-info/RECORD,,
+flaxsr-0.0.2.dist-info/LICENSE,sha256=UeuGtONxLyJHg6LVfV_8F_rV8oCPKaBRpwlgDixQCO4,11313
+flaxsr-0.0.2.dist-info/METADATA,sha256=wkST4xzW1QCTYsJlte7S5BmynC63J3h0ATwVDgJ2anw,1299
+flaxsr-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+flaxsr-0.0.2.dist-info/top_level.txt,sha256=MVm6sMxEshMxPdjXtT9zH_BEQEqfThUdXHoNEId4NeE,7
+flaxsr-0.0.2.dist-info/RECORD,,
```

