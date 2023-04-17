# Comparing `tmp/verifiNN-0.0.0.dev7-py3-none-any.whl.zip` & `tmp/verifiNN-0.0.0.dev8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5031 bytes, number of entries: 12
+Zip file size: 5306 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 06:13 verifiNN/__init__.py
--rw-r--r--  2.0 unx      554 b- defN 23-Apr-16 23:28 verifiNN/examples.py
--rw-r--r--  2.0 unx     4902 b- defN 23-Apr-16 23:28 verifiNN/verifier.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Apr-17 00:56 verifiNN/examples.py
+-rw-r--r--  2.0 unx     5681 b- defN 23-Apr-17 00:51 verifiNN/verifier.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 06:14 verifiNN/algorithms/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 06:15 verifiNN/models/__init__.py
 -rw-r--r--  2.0 unx      637 b- defN 23-Apr-14 19:47 verifiNN/models/network.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 06:15 verifiNN/utils/__init__.py
 -rw-r--r--  2.0 unx      188 b- defN 23-Apr-14 19:56 verifiNN/utils/utils.py
--rw-r--r--  2.0 unx      703 b- defN 23-Apr-16 23:35 verifiNN-0.0.0.dev7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 23:35 verifiNN-0.0.0.dev7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-16 23:35 verifiNN-0.0.0.dev7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      954 b- defN 23-Apr-16 23:35 verifiNN-0.0.0.dev7.dist-info/RECORD
-12 files, 8039 bytes uncompressed, 3407 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx      703 b- defN 23-Apr-17 01:00 verifiNN-0.0.0.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 01:00 verifiNN-0.0.0.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-17 01:00 verifiNN-0.0.0.dev8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      955 b- defN 23-Apr-17 01:00 verifiNN-0.0.0.dev8.dist-info/RECORD
+12 files, 9316 bytes uncompressed, 3682 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: verifiNN/utils/__init__.py
 Comment: 
 
 Filename: verifiNN/utils/utils.py
 Comment: 
 
-Filename: verifiNN-0.0.0.dev7.dist-info/METADATA
+Filename: verifiNN-0.0.0.dev8.dist-info/METADATA
 Comment: 
 
-Filename: verifiNN-0.0.0.dev7.dist-info/WHEEL
+Filename: verifiNN-0.0.0.dev8.dist-info/WHEEL
 Comment: 
 
-Filename: verifiNN-0.0.0.dev7.dist-info/top_level.txt
+Filename: verifiNN-0.0.0.dev8.dist-info/top_level.txt
 Comment: 
 
-Filename: verifiNN-0.0.0.dev7.dist-info/RECORD
+Filename: verifiNN-0.0.0.dev8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## verifiNN/examples.py

```diff
@@ -1,27 +1,42 @@
 import numpy as np
 
 from verifiNN.models.network import Network
+from verifiNN.verifier import LPVerifier
 
 
 # Defining a network
 W1 = np.array([[1, 0],
 			  [0, 1]])
 b1 = np.array([1, 1])
 W2 = np.array([[0, 1],
 			  [1, 0]])
 b2 = np.array([2, 2])
 
 weights = [W1, W2]
 biases = [b1, b2]
 network = Network(weights, biases, activation='ReLU', labeler='argmax')
 
-# Classifying an input using a network
+# Classifying an input with a network
 x_0 = np.array([1, 2])
-l_0 = network.classify(x_0) # returns 0
+l_0 = network.classify(x_0) # class 0
+assert l_0 == 0
 
 x_1 = np.array([2, 1])
-l_1 = network.classify(x_1) # returns 1
+l_1 = network.classify(x_1) # class 1
+assert l_1 == 1
 
-# verifying the epsilon robustness of a network at a reference point
+# Compute the pointwise robustness of a network at a reference point
+x_0 = np.array([1, 2]); epsilon = 1.5
 
+vf = LPVerifier()
+result = vf.compute_pointwise_robustness(network, x_0, epsilon)
+assert result['verification_status'] == 'verified'
+assert result['robustness_status'] == 'not_robust'
+
+rho = np.round(result['pointwise_robustness'], decimals=5)
+assert rho == 0.5
+
+x_hat = result['adversarial_example']
+assert np.round(x_hat[0], decimals=5) == 1.5
+assert np.round(x_hat[1], decimals=5) == 1.5
```

## verifiNN/verifier.py

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 
 from verifiNN.models.network import Network
 
 
 class AbstractVerifier:
 
-
 	def __init__(self, network=None):
 		self.network = network
 		self.variables = {}
 		self.var_name_to_id_map = {}
 		self.constraints = []
 
 	def get_var(self, name)-> cp.Variable:
@@ -121,15 +120,15 @@
 		e_l = np.eye(1, m, l)[0] # unit basis vector with 1 at index l
 
 		z_H_plus_1 = self.get_var(f'z_{self.network.H + 1}')
 		ss_cons = ((e_0 - e_l) @ z_H_plus_1 <= 0)
 
 		return ss_cons
 
-	def _solve(self, network: Network, x_0: np.array, epsilon: float,
+	def _solve(self, x_0: np.array, epsilon: float,
 		obj: cp.problems.objective.Minimize) -> dict:
 
 		# Constraints
 		constraints = []
 		region_cons = self.generate_region_constraints(x_0, epsilon) # region const
 		aff_cons = self.generate_affine_constraints() # affine const
 		ReLU_cons = self.generate_ReLU_constraints(x_0) # ReLU const
@@ -158,18 +157,40 @@
 		epsilon: float) -> dict:
 		"""Verify epsilon-robustness of the network via LP satisfiability."""
 
 		self.network = network
 		self.generate_decision_variables()
 
 		obj = cp.Minimize(1)
-		return self._solve(network, x_0, epsilon, obj)
+		result = self._solve(x_0, epsilon, obj)
+
+		if result['problem_status'] == 'optimal':
+			result.update({'verification_status': 'verified'})
+			result.update({'robustness_status': 'not_robust'})
+			result.update({'pointwise_robustness': 'unavailable'})
+		else:
+			result.update({'verification_status': 'unverified'})
+			result.update({'robustness_status': 'unknown'})
+			result.update({'pointwise_robustness': 'unavailable'})
+
+		return result
 
 	def compute_pointwise_robustness(self, network: Network, x_0: np.array,
 		epsilon: float) -> dict:
 		"""Compute the distance to the nearest adversarial example."""
 
 		self.network = network
 		self.generate_decision_variables()
 
 		obj = cp.Minimize(cp.norm_inf(x_0 - self.get_var('z_0'))) # hack
-		return self._solve(network, x_0, epsilon, obj)
+		result = self._solve(x_0, epsilon, obj)
+
+		if result['problem_status'] == 'optimal':
+			result.update({'verification_status': 'verified'})
+			result.update({'robustness_status': 'not_robust'})
+			result.update({'pointwise_robustness': result['optimal_value']})
+		else:
+			result.update({'verification_status': 'unverified'})
+			result.update({'robustness_status': 'unknown'})
+			result.update({'pointwise_robustness': 'unavailable'})
+
+		return result
```

## Comparing `verifiNN-0.0.0.dev7.dist-info/METADATA` & `verifiNN-0.0.0.dev8.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifiNN
-Version: 0.0.0.dev7
+Version: 0.0.0.dev8
 Summary: A package for optimization based neural network verification.
 Author-email: Ayush Bharadwaj <ayush.bharadwaj@gmail.com>, Harsh Bolakani <harshbolakani@gmail.com>
 Maintainer-email: Ayush Bharadwaj <ayush.bharadwaj@gmail.com>
 Project-URL: homepage, https://github.com/ayusbhar2/verifiNN
 Keywords: neural networks,verification,convex optimization,semidefinit programming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

