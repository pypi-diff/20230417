# Comparing `tmp/kpops-1.1.0.tar.gz` & `tmp/kpops-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.1.0.tar", max compression
+gzip compressed data, was "kpops-1.1.1.tar", max compression
```

## Comparing `kpops-1.1.0.tar` & `kpops-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1064 2023-04-11 16:18:00.214327 kpops-1.1.0/LICENSE
--rw-r--r--   0        0        0     2370 2023-04-11 16:18:00.214327 kpops-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/exception.py
--rw-r--r--   0        0        0    11186 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/main.py
--rw-r--r--   0        0        0     4226 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9371 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2161 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     2913 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8202 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      182 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5890 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1470 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      788 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      180 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9588 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6937 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      444 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     4552 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    11549 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     4546 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1553 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     1754 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     7196 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      402 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2244 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     4575 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3072 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    10755 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     4407 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      291 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1107 2023-04-11 16:18:00.218327 kpops-1.1.0/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1840 2023-04-11 16:18:16.890552 kpops-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.0/setup.py
--rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 08:26:24.653158 kpops-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2370 2023-04-17 08:26:24.653158 kpops-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11186 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/main.py
+-rw-r--r--   0        0        0     4226 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1711 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     9371 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2161 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     2913 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8202 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      182 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5890 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1470 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      788 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9588 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6937 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     4552 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    11549 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     4546 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     1553 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     1754 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     7401 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0      402 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2244 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     4575 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3072 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    10755 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     4407 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      291 2023-04-17 08:26:24.657158 kpops-1.1.1/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     1107 2023-04-17 08:26:24.661158 kpops-1.1.1/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1840 2023-04-17 08:26:43.429217 kpops-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.1/setup.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.1/PKG-INFO
```

### Comparing `kpops-1.1.0/LICENSE` & `kpops-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/README.md` & `kpops-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/cli/custom_formatter.py` & `kpops-1.1.1/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/cli/main.py` & `kpops-1.1.1/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/cli/pipeline_config.py` & `kpops-1.1.1/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/cli/registry.py` & `kpops-1.1.1/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/__init__.py` & `kpops-1.1.1/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.1.1/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.1.1/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.1.1/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.1.1/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.1.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.1.1/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.1.1/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.1.1/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/topic/handler.py` & `kpops-1.1.1/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/topic/model.py` & `kpops-1.1.1/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.1.1/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/topic/utils.py` & `kpops-1.1.1/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/component_handlers/utils/exception.py` & `kpops-1.1.1/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/base_defaults_component.py` & `kpops-1.1.1/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/kafka_app.py` & `kpops-1.1.1/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/kafka_connector.py` & `kpops-1.1.1/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/kubernetes_app.py` & `kpops-1.1.1/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/models/from_section.py` & `kpops-1.1.1/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/models/to_section.py` & `kpops-1.1.1/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/base_components/pipeline_component.py` & `kpops-1.1.1/kpops/components/base_components/pipeline_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import os
 from functools import cached_property
+from typing import Literal
 
 from pydantic import BaseConfig, Extra, Field
 
 from kpops.components.base_components.base_defaults_component import (
     BaseDefaultsComponent,
 )
 from kpops.components.base_components.models.from_section import (
@@ -18,14 +19,18 @@
     TopicConfig,
     ToSection,
 )
 from kpops.utils.yaml_loading import substitute
 
 
 class PipelineComponent(BaseDefaultsComponent):
+    type: str = "pipeline-component"
+    schema_type: Literal["pipeline-component"] = Field(  # type: ignore[assignment]
+        default="pipeline-component", exclude=True
+    )
     name: str
     from_: FromSection | None = Field(default=None, alias="from", title="From")
     app: object | None = None
     to: ToSection | None = None
     prefix: str = Field(
         default="${pipeline_name}-",
         description="Pipeline prefix that will prefix every component name. If you wish to not have any prefix you can specify an empty string.",
```

### Comparing `kpops-1.1.0/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.1.1/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.1.1/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.1.1/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/pipeline_generator/pipeline.py` & `kpops-1.1.1/kpops/pipeline_generator/pipeline.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/utils/dict_differ.py` & `kpops-1.1.1/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/utils/gen_schema.py` & `kpops-1.1.1/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/kpops/utils/yaml_loading.py` & `kpops-1.1.1/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.0/pyproject.toml` & `kpops-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.1.0"
+version = "1.1.1"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-1.1.0/setup.py` & `kpops-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['kpops = kpops.cli.main:app']}
 
 setup_kwargs = {
     'name': 'kpops',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'KPOps is a tool to deploy Kafka pipelines to Kubernetes',
     'long_description': '# KPOps\n\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)\n[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)\n[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
     'author': 'bakdata',
     'author_email': 'opensource@bakdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/kpops',
```

### Comparing `kpops-1.1.0/PKG-INFO` & `kpops-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.1.0
+Version: 1.1.1
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
```

