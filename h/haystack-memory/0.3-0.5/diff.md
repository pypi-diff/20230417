# Comparing `tmp/haystack_memory-0.3.tar.gz` & `tmp/haystack_memory-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haystack_memory-0.3.tar", last modified: Thu Apr  6 21:48:10 2023, max compression
+gzip compressed data, was "haystack_memory-0.5.tar", last modified: Mon Apr 17 00:10:14 2023, max compression
```

## Comparing `haystack_memory-0.3.tar` & `haystack_memory-0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-04-06 20:01:18.510222 haystack_memory-0.3/LICENSE
--rw-r--r--   0        0        0     4233 2023-04-06 21:42:59.413119 haystack_memory-0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-06 20:01:18.510922 haystack_memory-0.3/haystack_memory/__init__.py
--rw-r--r--   0        0        0     2083 2023-04-06 20:01:18.511075 haystack_memory-0.3/haystack_memory/memory.py
--rw-r--r--   0        0        0     2111 2023-04-06 20:01:18.511237 haystack_memory-0.3/haystack_memory/prompt_templates.py
--rw-r--r--   0        0        0     2453 2023-04-06 20:01:18.511394 haystack_memory-0.3/haystack_memory/utils.py
--rw-r--r--   0        0        0      766 2023-04-06 21:48:10.602041 haystack_memory-0.3/pyproject.toml
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 haystack_memory-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-06 20:01:18.510222 haystack_memory-0.5/LICENSE
+-rw-r--r--   0        0        0     4569 2023-04-17 00:08:49.813401 haystack_memory-0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 20:01:18.510922 haystack_memory-0.5/haystack_memory/__init__.py
+-rw-r--r--   0        0        0     2083 2023-04-06 20:01:18.511075 haystack_memory-0.5/haystack_memory/memory.py
+-rw-r--r--   0        0        0     1985 2023-04-16 19:46:09.913105 haystack_memory-0.5/haystack_memory/prompt_templates.py
+-rw-r--r--   0        0        0     2541 2023-04-16 19:51:16.596401 haystack_memory-0.5/haystack_memory/utils.py
+-rw-r--r--   0        0        0      766 2023-04-17 00:10:14.877375 haystack_memory-0.5/pyproject.toml
+-rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 haystack_memory-0.5/PKG-INFO
```

### Comparing `haystack_memory-0.3/LICENSE` & `haystack_memory-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_memory-0.3/README.md` & `haystack_memory-0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Haystack Memory
 
-Memory for [haystack](https://github.com/deepset-ai/haystack) Agents. Currently, the memory of agents can be used in memory or with redis. The latter supports a sliding window.
+Memory for [haystack](https://github.com/deepset-ai/haystack) Agents. Currently, the memory for agents can be used in-memory or using redis. The latter supports a sliding window.
 
 ## Installation
 
-- Python pip: ```python3 -m pip install haystack-memory``` . This package will attempt to install the dependencies (farm-haystack>=1.15.0)
-- Python pip (skip dependency installation: Use  ```python3 -m pip install haystack-memory --no-deps```
+- Python pip: ```pip install --upgrade haystack-memory``` . This method will attempt to install the dependencies (farm-haystack>=1.15.0, redis)
+- Python pip (skip dependency installation): Use  ```pip install --upgrade haystack-memory --no-deps```
 - Using git: ```pip install git+https://github.com/rolandtannous/HaystackAgentBasicMemory.git@main#egg=HaystackAgentBasicMemory```
 
 
 ## Usage
 
-To use memory in your agent, you need two parts:
-- `MemoryRecallNode`: This node is passed to the agent to be used as a tool. It will be passed to the agent to let it remember the conversation.
-- `MemoryUtils`: This class has to be used to save the query and the answers to the memory.
+To use memory in your agent, you need two components:
+- `MemoryRecallNode`: This node is added to the agent as a tool. It will allow the agent to remember the conversation and make query-memory associations.
+- `MemoryUtils`: This class should be used to save the queries and the final agent answers to the conversation memory.
+- `chat`: This is a method of the MemoryUtils class. It is used to chat with the agent. It will save the query and the answer to the memory. It also returns the full result and the updated conversation memory for further usage.
 
 ```py
 from haystack.agents import Agent, Tool
 from haystack.nodes import PromptNode
 from haystack_memory.prompt_templates import memory_template
 from haystack_memory.memory import MemoryRecallNode
 from haystack_memory.utils import MemoryUtils
@@ -34,15 +35,15 @@
                          max_length=1024,
                          stop_words=["Observation:"])
 memory_agent = Agent(prompt_node=prompt_node, prompt_template=memory_template)
 memory_agent.add_tool(memory_tool)
 
 # Initialize the utils to save the query and the answers to the memory
 memory_utils = MemoryUtils(memory_database=memory_database, agent=memory_agent)
-memory_utils.chat("<Your Question>")
+result, conversation_memory = memory_utils.chat("<Your Question>")
 ```
 
 ### Redis
 
 The memory can also be stored in a redis database which makes it possible to use different memories at the same time to be used with multiple agents. Additionally, it supports a sliding window to only utilize the last messages.
 
 ```py
@@ -67,15 +68,15 @@
 memory_agent = Agent(prompt_node=prompt_node, prompt_template=memory_template)
 # Initialize the utils to save the query and the answers to the memory
 redis_utils = RedisUtils(agent=memory_agent,
                          memory_id="agent_memory",
                          host="localhost",
                          port=6379,
                          db=0)
-redis_utils.chat("<Your Question>")
+result, conversation_memory = redis_utils.chat("<Your Question>")
 ```
 
 
 ## Examples
 
 Examples can be found in the `examples/` folder. It contains the usage for all memory types.
 To open the examples in colab, click on the following links:
```

### Comparing `haystack_memory-0.3/haystack_memory/memory.py` & `haystack_memory-0.5/haystack_memory/memory.py`

 * *Files identical despite different names*

### Comparing `haystack_memory-0.3/haystack_memory/utils.py` & `haystack_memory-0.5/haystack_memory/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     def __save_to_memory(self, result: dict):
         self.memory_database.append(result["query"])
         self.memory_database.append(result["answers"][0].answer)
 
     def chat(self, query: str):
         result = self.agent.run(query)
         self.__save_to_memory(result)
+        return result, self.memory_database
 
 
 class RedisUtils:
     def __init__(self,
                  agent: Agent,
                  memory_id: str,
                  host: str = "localhost",
@@ -62,7 +63,8 @@
              query: str):
         """
         Function to run a query with the given agent. Stores the results in the memory
         :param query: Query to run with the agent
         """
         result = self.agent.run(query)
         self.__save_to_memory(result)
+        return result, self.memory_database
```

### Comparing `haystack_memory-0.3/pyproject.toml` & `haystack_memory-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm.build]
 
 [project]
 name = "haystack_memory"
-version = "0.3"
+version = "0.5"
 description = "Basic Memory library for Haystack NLP agents"
 authors = [
     { name = "Florian Brand <github@florianbrand.de>, Roland Tannous, Tuana Celik, recrudesce" },
 ]
 dependencies = [
     "farm-haystack>=1.15.0",
     "redis",
```

### Comparing `haystack_memory-0.3/PKG-INFO` & `haystack_memory-0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haystack-memory
-Version: 0.3
+Version: 0.5
 Summary: Basic Memory library for Haystack NLP agents
 Author: Florian Brand <github@florianbrand.de>, Roland Tannous, Tuana Celik, recrudesce
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/rolandtannous/haystack-memory
@@ -12,28 +12,29 @@
 Requires-Python: >=3.9.16
 Requires-Dist: farm-haystack>=1.15.0
 Requires-Dist: redis
 Description-Content-Type: text/markdown
 
 # Haystack Memory
 
-Memory for [haystack](https://github.com/deepset-ai/haystack) Agents. Currently, the memory of agents can be used in memory or with redis. The latter supports a sliding window.
+Memory for [haystack](https://github.com/deepset-ai/haystack) Agents. Currently, the memory for agents can be used in-memory or using redis. The latter supports a sliding window.
 
 ## Installation
 
-- Python pip: ```python3 -m pip install haystack-memory``` . This package will attempt to install the dependencies (farm-haystack>=1.15.0)
-- Python pip (skip dependency installation: Use  ```python3 -m pip install haystack-memory --no-deps```
+- Python pip: ```pip install --upgrade haystack-memory``` . This method will attempt to install the dependencies (farm-haystack>=1.15.0, redis)
+- Python pip (skip dependency installation): Use  ```pip install --upgrade haystack-memory --no-deps```
 - Using git: ```pip install git+https://github.com/rolandtannous/HaystackAgentBasicMemory.git@main#egg=HaystackAgentBasicMemory```
 
 
 ## Usage
 
-To use memory in your agent, you need two parts:
-- `MemoryRecallNode`: This node is passed to the agent to be used as a tool. It will be passed to the agent to let it remember the conversation.
-- `MemoryUtils`: This class has to be used to save the query and the answers to the memory.
+To use memory in your agent, you need two components:
+- `MemoryRecallNode`: This node is added to the agent as a tool. It will allow the agent to remember the conversation and make query-memory associations.
+- `MemoryUtils`: This class should be used to save the queries and the final agent answers to the conversation memory.
+- `chat`: This is a method of the MemoryUtils class. It is used to chat with the agent. It will save the query and the answer to the memory. It also returns the full result and the updated conversation memory for further usage.
 
 ```py
 from haystack.agents import Agent, Tool
 from haystack.nodes import PromptNode
 from haystack_memory.prompt_templates import memory_template
 from haystack_memory.memory import MemoryRecallNode
 from haystack_memory.utils import MemoryUtils
@@ -50,15 +51,15 @@
                          max_length=1024,
                          stop_words=["Observation:"])
 memory_agent = Agent(prompt_node=prompt_node, prompt_template=memory_template)
 memory_agent.add_tool(memory_tool)
 
 # Initialize the utils to save the query and the answers to the memory
 memory_utils = MemoryUtils(memory_database=memory_database, agent=memory_agent)
-memory_utils.chat("<Your Question>")
+result, conversation_memory = memory_utils.chat("<Your Question>")
 ```
 
 ### Redis
 
 The memory can also be stored in a redis database which makes it possible to use different memories at the same time to be used with multiple agents. Additionally, it supports a sliding window to only utilize the last messages.
 
 ```py
@@ -83,15 +84,15 @@
 memory_agent = Agent(prompt_node=prompt_node, prompt_template=memory_template)
 # Initialize the utils to save the query and the answers to the memory
 redis_utils = RedisUtils(agent=memory_agent,
                          memory_id="agent_memory",
                          host="localhost",
                          port=6379,
                          db=0)
-redis_utils.chat("<Your Question>")
+result, conversation_memory = redis_utils.chat("<Your Question>")
 ```
 
 
 ## Examples
 
 Examples can be found in the `examples/` folder. It contains the usage for all memory types.
 To open the examples in colab, click on the following links:
```

