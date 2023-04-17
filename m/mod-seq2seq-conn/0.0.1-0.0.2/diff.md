# Comparing `tmp/mod_seq2seq_conn-0.0.1.tar.gz` & `tmp/mod_seq2seq_conn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mod_seq2seq_conn-0.0.1.tar", last modified: Mon Apr 17 15:52:26 2023, max compression
+gzip compressed data, was "mod_seq2seq_conn-0.0.2.tar", last modified: Mon Apr 17 16:47:29 2023, max compression
```

## Comparing `mod_seq2seq_conn-0.0.1.tar` & `mod_seq2seq_conn-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:52:26.408955 mod_seq2seq_conn-0.0.1/
--rw-rw-rw-   0        0        0     1072 2023-04-17 15:21:08.000000 mod_seq2seq_conn-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      837 2023-04-17 15:52:26.408955 mod_seq2seq_conn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-17 15:50:59.000000 mod_seq2seq_conn-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 15:52:26.401975 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/
--rw-rw-rw-   0        0        0      333 2023-04-17 11:37:56.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-04-17 14:27:53.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/configs_init.py
--rw-rw-rw-   0        0        0    12392 2023-04-17 15:43:19.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/model_tfp.py
--rw-rw-rw-   0        0        0    23732 2023-04-17 14:29:43.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/model_tfp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:52:26.405964 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn.egg-info/
--rw-rw-rw-   0        0        0      837 2023-04-17 15:52:26.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-17 15:52:26.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:52:26.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-17 15:52:26.000000 mod_seq2seq_conn-0.0.1/mod_seq2seq_conn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-17 15:28:45.000000 mod_seq2seq_conn-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      622 2023-04-17 15:52:26.409960 mod_seq2seq_conn-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 15:52:26.407959 mod_seq2seq_conn-0.0.1/tests_usage/
--rw-rw-rw-   0        0        0     1456 2023-04-17 15:37:53.000000 mod_seq2seq_conn-0.0.1/tests_usage/RUN_MODELONLY.py
--rw-rw-rw-   0        0        0        0 2023-04-14 15:10:52.000000 mod_seq2seq_conn-0.0.1/tests_usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:47:29.341354 mod_seq2seq_conn-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-17 16:47:29.341354 mod_seq2seq_conn-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:47:29.337354 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/configs_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/model_tfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/model_tfp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:47:29.337354 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-17 16:47:29.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-17 16:47:29.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:47:29.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 16:47:29.000000 mod_seq2seq_conn-0.0.2/mod_seq2seq_conn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 16:47:29.341354 mod_seq2seq_conn-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:47:29.341354 mod_seq2seq_conn-0.0.2/tests_usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/tests_usage/RUN_MODELONLY.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:47:18.000000 mod_seq2seq_conn-0.0.2/tests_usage/__init__.py
```

### Comparing `mod_seq2seq_conn-0.0.1/LICENSE` & `mod_seq2seq_conn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mod_seq2seq_conn-0.0.1/PKG-INFO` & `mod_seq2seq_conn-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-Metadata-Version: 2.1
-Name: mod_seq2seq_conn
-Version: 0.0.1
-Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
-Home-page: https://github.com/gaurav306/mod_seq2seq_conn
-Author: Gaurav Chaudhary
-Author-email: gaurav.chaudhary@ntnu.no
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# mod_seq2seq_conn
-
-mod_seq2seq_conn = modular sequence to sequence control oriented neural networks
-
-## Instructions
-
-1. Install:
-
-```
-pip install mod_seq2seq_conn
-```
-
-2. Usage:
-Download congifuration file from tests_usage\ in the github repository https://github.com/gaurav306/mod_seq2seq_conn
-
+Metadata-Version: 2.1
+Name: mod_seq2seq_conn
+Version: 0.0.2
+Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
+Home-page: https://github.com/gaurav306/mod_seq2seq_conn
+Author: Gaurav Chaudhary
+Author-email: gaurav.chaudhary@ntnu.no
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mod_seq2seq_conn
+
+[![image](https://img.shields.io/pypi/v/mod_seq2seq_conn?style=plastic)](https://pypi.org/project/mod-seq2seq-conn/)
+
+mod_seq2seq_conn = modular sequence to sequence control oriented neural networks
+
+## Instructions
+
+1. Install:
+
+```
+pip install mod_seq2seq_conn
+```
+
+2. Usage:
+Download congifuration file from tests_usage\ in the github repository https://github.com/gaurav306/mod_seq2seq_conn
+
+```python
+from mod_seq2seq_conn.configs_init import get_configs
+from mod_seq2seq_conn.model_tfp import ModelClass_tfp
+
+configs = get_configs('config_model.yaml')
+model = ModelClass_tfp(configs_data, time_dt)
+```
+
+## Credits
+packaging instructions from https://towardsdatascience.com/how-to-package-your-python-code-df5a7739ab2e
```

### Comparing `mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/configs_init.py` & `mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/configs_init.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import ruamel.yaml
-yaml = ruamel.yaml.YAML()
-
-def read_write_yaml(filename, mode, data_yaml):
-	# Read the yaml file
-	if mode == 'r':
-		with open(filename) as file:
-			yaml_configs = yaml.load(file)
-		return yaml_configs
-
-	# Write to the yaml file
-	if mode == 'w':
-		with open(filename, 'w') as yamlfile:
-			yaml.dump(data_yaml, yamlfile)
-
-
-def assert_check_configs(configs):
-	assert configs['model']['optimizer'] == 'Adam' or configs['model']['optimizer'] == 'SGD', 'Adam must be either Adam or SGD'
-	assert configs['model']['model_type_prob'] == 'prob' or configs['model'][
-		'model_type_prob'] == 'nonprob', 'model_type_prob must be either prob or nonprob'
-	assert configs['model']['loss_prob'] == 'nonparametric' or configs['model'][
-		'loss_prob'] == 'parametric', 'loss_prob must be either nonparametric or parametric'
-	assert configs['model']['control_future_cells'] == 1 or configs['model']['control_future_cells'] == 6, 'control_future_cells must be either 1 or 6'
-	assert configs['model']['all_layers_neurons'] % 8 == 0 and configs['model'][
-		'all_layers_neurons'] >= 8, 'all_layers_neurons must be divisible by 8 and greater than or equal to 8'
-	assert configs['model']['mha_head'] % 8 == 0 and configs['model'][
-		'mha_head'] >= 8, 'mha_head must be divisible by 8 and greater than or equal to 8'
-	assert configs['rnn_units']['rnn_type'] in ['LSTM', 'GRU', 'RNN'], 'rnn_type must be either LSTM, GRU or RNN'
-	assert configs['rnn_units']['input_enc_rnn_depth'] <= 5, 'max depth of RNN units is 5'
-
-
-def get_configs(config_filename):
-	configs = read_write_yaml(config_filename, 'r', None)
-	assert_check_configs(configs)
-	return configs
+import ruamel.yaml
+yaml = ruamel.yaml.YAML()
+
+def read_write_yaml(filename, mode, data_yaml):
+	# Read the yaml file
+	if mode == 'r':
+		with open(filename) as file:
+			yaml_configs = yaml.load(file)
+		return yaml_configs
+
+	# Write to the yaml file
+	if mode == 'w':
+		with open(filename, 'w') as yamlfile:
+			yaml.dump(data_yaml, yamlfile)
+
+
+def assert_check_configs(configs):
+	assert configs['model']['optimizer'] == 'Adam' or configs['model']['optimizer'] == 'SGD', 'Adam must be either Adam or SGD'
+	assert configs['model']['model_type_prob'] == 'prob' or configs['model'][
+		'model_type_prob'] == 'nonprob', 'model_type_prob must be either prob or nonprob'
+	assert configs['model']['loss_prob'] == 'nonparametric' or configs['model'][
+		'loss_prob'] == 'parametric', 'loss_prob must be either nonparametric or parametric'
+	assert configs['model']['control_future_cells'] == 1 or configs['model']['control_future_cells'] == 6, 'control_future_cells must be either 1 or 6'
+	assert configs['model']['all_layers_neurons'] % 8 == 0 and configs['model'][
+		'all_layers_neurons'] >= 8, 'all_layers_neurons must be divisible by 8 and greater than or equal to 8'
+	assert configs['model']['mha_head'] % 8 == 0 and configs['model'][
+		'mha_head'] >= 8, 'mha_head must be divisible by 8 and greater than or equal to 8'
+	assert configs['rnn_units']['rnn_type'] in ['LSTM', 'GRU', 'RNN'], 'rnn_type must be either LSTM, GRU or RNN'
+	assert configs['rnn_units']['input_enc_rnn_depth'] <= 5, 'max depth of RNN units is 5'
+
+
+def get_configs(config_filename):
+	configs = read_write_yaml(config_filename, 'r', None)
+	assert_check_configs(configs)
+	return configs
```

### Comparing `mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/model_tfp.py` & `mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/model_tfp.py`

 * *Files identical despite different names*

### Comparing `mod_seq2seq_conn-0.0.1/mod_seq2seq_conn/model_tfp_utils.py` & `mod_seq2seq_conn-0.0.2/mod_seq2seq_conn/model_tfp_utils.py`

 * *Files identical despite different names*

### Comparing `mod_seq2seq_conn-0.0.1/tests_usage/RUN_MODELONLY.py` & `mod_seq2seq_conn-0.0.2/tests_usage/RUN_MODELONLY.py`

 * *Files identical despite different names*

