# Comparing `tmp/kernel_sidecar-0.5.2.tar.gz` & `tmp/kernel_sidecar-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernel_sidecar-0.5.2.tar", max compression
+gzip compressed data, was "kernel_sidecar-0.5.3.tar", max compression
```

## Comparing `kernel_sidecar-0.5.2.tar` & `kernel_sidecar-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/LICENSE
--rw-r--r--   0        0        0     9197 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/README.md
--rw-r--r--   0        0        0     1174 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/__init__.py
--rw-r--r--   0        0        0     4209 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/actions.py
--rw-r--r--   0        0        0     2678 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/cli.py
--rw-r--r--   0        0        0    24262 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/client.py
--rw-r--r--   0        0        0     5207 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/comms.py
--rw-r--r--   0        0        0        0 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/__init__.py
--rw-r--r--   0        0        0      902 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/base.py
--rw-r--r--   0        0        0     1580 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/debug.py
--rw-r--r--   0        0        0     5919 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/output.py
--rw-r--r--   0        0        0     4395 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/log_utils.py
--rw-r--r--   0        0        0        0 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/__init__.py
--rw-r--r--   0        0        0    14883 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/messages.py
--rw-r--r--   0        0        0     2334 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/notebook.py
--rw-r--r--   0        0        0     9369 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/models/requests.py
--rw-r--r--   0        0        0     4707 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/nb_builder.py
--rw-r--r--   0        0        0      261 2023-04-14 13:45:14.486303 kernel_sidecar-0.5.2/src/kernel_sidecar/settings.py
--rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.2/setup.py
--rw-r--r--   0        0        0    10019 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/LICENSE
+-rw-r--r--   0        0        0     8256 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/README.md
+-rw-r--r--   0        0        0     1089 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/__init__.py
+-rw-r--r--   0        0        0     4325 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/actions.py
+-rw-r--r--   0        0        0     2678 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/cli.py
+-rw-r--r--   0        0        0    24262 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/client.py
+-rw-r--r--   0        0        0     5207 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/comms.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/__init__.py
+-rw-r--r--   0        0        0     1054 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/base.py
+-rw-r--r--   0        0        0     1580 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/debug.py
+-rw-r--r--   0        0        0     5919 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/output.py
+-rw-r--r--   0        0        0     4395 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/log_utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/__init__.py
+-rw-r--r--   0        0        0    14883 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/messages.py
+-rw-r--r--   0        0        0     2334 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/notebook.py
+-rw-r--r--   0        0        0     9369 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/requests.py
+-rw-r--r--   0        0        0     5284 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/nb_builder.py
+-rw-r--r--   0        0        0      261 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/settings.py
+-rw-r--r--   0        0        0     9080 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.3/PKG-INFO
```

### Comparing `kernel_sidecar-0.5.2/LICENSE` & `kernel_sidecar-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/README.md` & `kernel_sidecar-0.5.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,48 +6,50 @@
 <img alt="Pypi" src="https://img.shields.io/pypi/v/kernel-sidecar">
 <a href="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml">
     <img src="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml/badge.svg" alt="Tests" />
 </a>
 <img alt="Python versions" src="https://img.shields.io/pypi/pyversions/kernel-sidecar">
 </p>
 
-# Kernel-Sidecar
+# Overview
 
-This package offers the building blocks for creating a "Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture, one or many frontends manage the document model (code cells, outputs, metadata, etc) and send requests to a single Kernel. Each frontend observes responses on different ZMQ channels (`iopub`, `shell`, etc) but may end up with some inconsistency based on the Kernel only sending certain responses to the client that made the request.
+`kernel-sidecar` provides the building blocks for creating applications that run alongside Jupyter Kernels, keeping the Notebook document model in memory and acting as a middle-man between the Kernel and all other clients. There are many potential features that can be built into a Sidecar application:
+
+ - __Persisting Outputs__ for cell execution even when no clients are connected (e.g. run a cell, close your browser, come back later and see the output)
+ - __Code Cell Linting__ such as `black` or `isort`
+ - __Variable Explorer__ that can be sent to newly connected clients without needing to execute code in the Kernel
+ - __Custom Execution Managers__ to handle DAG/dependent cell execution or to dequeue queued cells without sending an interrupt to the Kernel which dequeues all queued cells
 
-In a `kernel-sidecar` architecture, all frontend clients talk to the `kernel-sidecar` client, and only the `kernel-sidecar` client communicates with the Kernel over ZMQ. That pattern offers several potential features:
- - Keep a document model within `kernel-sidecar` or the backend architecture
- - Add "extension"-esque capabilities on the backend such as auto-linting code on execute
- - Eliminate inconsistencies in what messages individual frontends receive because of Kernel replies
- - Model all requests, replies, and the Notebook document with Pydantic
 
 ## Installation
 
 ```bash
 pip install kernel-sidecar
 ```
 
+
 # Key Concepts
-## KernelSidecarClient
 
-A manager that uses `jupyter_client` under the hood to create ZMQ connections and watch for messages coming in over different ZMQ channels (`iopub`, `shell`, etc. An important assumption here is that `kernel-sidecar` is the only client talking to the Kernel, which means every message observed coming from the Kernel should be a reply (based on `parent_header_msg.msg_id`) to a request sent from this client.
+![Architecture overview diagram](docs/overview_arch_diagram.png)
 
-When the `KernelSidecarClient` send a request to the Kernel, it is wrapped in an `KernelAction` class. Every message received from the Kernel is delegated to the requesting Action and triggers callbacks attached to the Action class.
+## KernelSidecarClient
 
-## Actions
+The `KernelSidecarClient` class manages the ZMQ connections to the Kernel, sending execute request or other messages to the Kernel, and processing messages coming back from the Kernel on `iopub`, `shell`, `control`, and `stdin` channels. All messages sent and received are modeled with Pydantic. When preparing to send a request to the Kernel, it's structured as a `KernelAction` which connects the request with zero-to-many callbacks for responses to that specific request.
 
-Actions in `kernel-sidecar` encompass a request-reply cycle, including an `await action` syntax, where the Action is complete when the Kernel has reported its status returning to `idle` and optionally emitted a reply appropriate for the request. For instance, an `execute_request` is "done" when the `status` has been reported as `idle` *and* the Kernel has emitted an `execute_reply`, both with the `parent_header_msg.msg_id` the same as the `execute_request` `header.msg_id`.
 
-In a nutshell, an `actions.KernelAction` takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses (or just `async functions`) and creates an `awaitable` instance. `kernel.send(action)` submits the Request over ZMQ, and registers the Action so that all observed messages get routed to that Action to be handled by the Handlers/callbacks.
+## KernelAction
 
-Most of the time, you should be able to just use convience functions in the `KernelSidecarClient` class to create the actions. See `tests/test_actions.py` for many examples of using Actions and Handlers.
+`KernelAction` connects three key pieces of the request-reply flow between the sidecar application and the Kernel:
+ - Store the sent Request message
+ - Delegate messages to callbacks based on the request message
+ - Make the flow "awaitable" based on the Request type, e.g. an `execute_request` is done when `execute_reply` or `error` is received and `status` has gone to `idle`.
 
 ## Handlers
 
-When the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods `handle_<msg_type>`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.
+When the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods named for the message type, e.g. `async def handle_display_data`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.
 
 ## Comms
 
 Comms are a flexible way for a client and the Kernel to send messages outside of the `execute_request` format. The most widely used package that utilizes Comms is probably `ipywidgets`, but Comms in general are a very powerful tool for a Sidecar application. A Comm can be opened by either the Sidecar or the Kernel. A target for that Comm should be registered on the other side before the open happens. It's probably most typical to register a Comm target in the Kernel by sending an `execute_request`, then sending a `comm_open` from the Sidecar side. See `tests/test_comms.py` for examples.
 
 Once a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will automatically route all `comm_msg` messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but it's necessary because `comm_msg` can come in as a result of `execute_request`'s or `comm_msg`'s or potentially other messages. So the `CommManager` -> `CommHandler` routing basically needs to be applied to every message the `KernelSidecarClient` receives over ZMQ.
```

#### html2text {}

```diff
@@ -1,95 +1,83 @@
                                 Kernel Sidecar
                        [Pypi] [Tests] [Python versions]
-# Kernel-Sidecar This package offers the building blocks for creating a "Kernel
-Sidecar" Jupyter framework. In normal Jupyter Notebook architecture, one or
-many frontends manage the document model (code cells, outputs, metadata, etc)
-and send requests to a single Kernel. Each frontend observes responses on
-different ZMQ channels (`iopub`, `shell`, etc) but may end up with some
-inconsistency based on the Kernel only sending certain responses to the client
-that made the request. In a `kernel-sidecar` architecture, all frontend clients
-talk to the `kernel-sidecar` client, and only the `kernel-sidecar` client
-communicates with the Kernel over ZMQ. That pattern offers several potential
-features: - Keep a document model within `kernel-sidecar` or the backend
-architecture - Add "extension"-esque capabilities on the backend such as auto-
-linting code on execute - Eliminate inconsistencies in what messages individual
-frontends receive because of Kernel replies - Model all requests, replies, and
-the Notebook document with Pydantic ## Installation ```bash pip install kernel-
-sidecar ``` # Key Concepts ## KernelSidecarClient A manager that uses
-`jupyter_client` under the hood to create ZMQ connections and watch for
-messages coming in over different ZMQ channels (`iopub`, `shell`, etc. An
-important assumption here is that `kernel-sidecar` is the only client talking
-to the Kernel, which means every message observed coming from the Kernel should
-be a reply (based on `parent_header_msg.msg_id`) to a request sent from this
-client. When the `KernelSidecarClient` send a request to the Kernel, it is
-wrapped in an `KernelAction` class. Every message received from the Kernel is
-delegated to the requesting Action and triggers callbacks attached to the
-Action class. ## Actions Actions in `kernel-sidecar` encompass a request-reply
-cycle, including an `await action` syntax, where the Action is complete when
-the Kernel has reported its status returning to `idle` and optionally emitted a
-reply appropriate for the request. For instance, an `execute_request` is "done"
-when the `status` has been reported as `idle` *and* the Kernel has emitted an
-`execute_reply`, both with the `parent_header_msg.msg_id` the same as the
-`execute_request` `header.msg_id`. In a nutshell, an `actions.KernelAction`
-takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses
-(or just `async functions`) and creates an `awaitable` instance. `kernel.send
-(action)` submits the Request over ZMQ, and registers the Action so that all
-observed messages get routed to that Action to be handled by the Handlers/
-callbacks. Most of the time, you should be able to just use convience functions
-in the `KernelSidecarClient` class to create the actions. See `tests/
-test_actions.py` for many examples of using Actions and Handlers. ## Handlers
-When the `KernelSidecarClient` receives a message over ZMQ, parses it into a
-Pydantic model, and delegates it to the appropriate `Action` to be handled, it
-passes on that message to every `Handler` attached to the `Action` and awaits
-all of them to handle that message. `Handler` objects can define handling
-different message types by creating methods `handle_`. See
-`handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.
-## Comms Comms are a flexible way for a client and the Kernel to send messages
-outside of the `execute_request` format. The most widely used package that
-utilizes Comms is probably `ipywidgets`, but Comms in general are a very
-powerful tool for a Sidecar application. A Comm can be opened by either the
-Sidecar or the Kernel. A target for that Comm should be registered on the other
-side before the open happens. It's probably most typical to register a Comm
-target in the Kernel by sending an `execute_request`, then sending a
-`comm_open` from the Sidecar side. See `tests/test_comms.py` for examples. Once
-a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will
-automatically route all `comm_msg` messages to a `CommHandler` instance by
-`comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as
-it overlaps the `Handler` / `Action` pattern, but it's necessary because
-`comm_msg` can come in as a result of `execute_request`'s or `comm_msg`'s or
-potentially other messages. So the `CommManager` -> `CommHandler` routing
-basically needs to be applied to every message the `KernelSidecarClient`
-receives over ZMQ. ## Models `kernel-sidecar` has Pydantic models for: - The
-Jupyter Notebook document (`models/notebook.py`), which should be consistent
-with `nbformat` parsing / structure - Request messages sent to the Kernel over
-ZMQ (`models/requests.py`) - Messages received over ZMQ from the Kernel
-(`models/messages.py`) ## CLI `kernel-sidecar` ships a small CLI for testing a
-connection to a Kernel. ```bash â¯ sidecar --help Usage: sidecar [OPTIONS]
-Options: -f FILE Kernel connection file [required] --debug / --no-debug Turn on
-DEBUG logging [default: no-debug] --execute TEXT Execute code string instead of
-sending kernel info request --tail / --no-tail Continue tailing ZMQ after
-connecting or executing code [default: no-tail] --install-completion
-[bash|zsh|fish|powershell|pwsh] Install completion for the specified shell. --
-show-completion [bash|zsh|fish|powershell|pwsh] Show completion for the
-specified shell, to copy it or customize the installation. --help Show this
-message and exit. ``` Try it out by starting an IPython kernel in one terminal
-and using the CLI in another. ```bash python -m ipykernel_launcher --debug -f /
-tmp/kernel.json ``` ```bash kernel-sidecar on î  release-0.3.2 [$?] is ð¦
-v0.3.1 via ð v3.11.0 (kernel-sidecar-py3.11) â¯ sidecar -f /tmp/kernel.json
-2023-03-10T14:31:59.992235Z [info ] Attempting to connect: {'control_port':
-34897, 'hb_port': 49821, 'iopub_port': 40577, 'ip': '127.0.0.1', 'kernel_name':
-'', 'key': '615bcebc-baf2e28abad1f6c017dc71dc', 'shell_port': 37421,
-'signature_scheme': 'hmac-sha256', 'stdin_port': 41405, 'transport': 'tcp'}
-[kernel_sidecar.cli] filename=cli.py func_name=main lineno=62 2023-03-10T14:32:
-00.026503Z [info ] {'banner': 'Python 3.11.0 (main, Nov 7 2022, 09:38:45) [GCC
-9.4.0]\n' "Type 'copyright', 'credits' or 'license' for more information\n"
-"IPython 8.10.0 -- An enhanced Interactive Python. Type '?' for " 'help.\n',
-'debugger': None, 'help_links': [{'text': 'Python Reference', 'url': 'https://
-docs.python.org/3.11'}, {'text': 'IPython Reference', 'url': 'https://
-ipython.org/documentation.html'}, {'text': 'NumPy Reference', 'url': 'https://
+# Overview `kernel-sidecar` provides the building blocks for creating
+applications that run alongside Jupyter Kernels, keeping the Notebook document
+model in memory and acting as a middle-man between the Kernel and all other
+clients. There are many potential features that can be built into a Sidecar
+application: - __Persisting Outputs__ for cell execution even when no clients
+are connected (e.g. run a cell, close your browser, come back later and see the
+output) - __Code Cell Linting__ such as `black` or `isort` - __Variable
+Explorer__ that can be sent to newly connected clients without needing to
+execute code in the Kernel - __Custom Execution Managers__ to handle DAG/
+dependent cell execution or to dequeue queued cells without sending an
+interrupt to the Kernel which dequeues all queued cells ## Installation ```bash
+pip install kernel-sidecar ``` # Key Concepts ![Architecture overview diagram]
+(docs/overview_arch_diagram.png) ## KernelSidecarClient The
+`KernelSidecarClient` class manages the ZMQ connections to the Kernel, sending
+execute request or other messages to the Kernel, and processing messages coming
+back from the Kernel on `iopub`, `shell`, `control`, and `stdin` channels. All
+messages sent and received are modeled with Pydantic. When preparing to send a
+request to the Kernel, it's structured as a `KernelAction` which connects the
+request with zero-to-many callbacks for responses to that specific request. ##
+KernelAction `KernelAction` connects three key pieces of the request-reply flow
+between the sidecar application and the Kernel: - Store the sent Request
+message - Delegate messages to callbacks based on the request message - Make
+the flow "awaitable" based on the Request type, e.g. an `execute_request` is
+done when `execute_reply` or `error` is received and `status` has gone to
+`idle`. ## Handlers When the `KernelSidecarClient` receives a message over ZMQ,
+parses it into a Pydantic model, and delegates it to the appropriate `Action`
+to be handled, it passes on that message to every `Handler` attached to the
+`Action` and awaits all of them to handle that message. `Handler` objects can
+define handling different message types by creating methods named for the
+message type, e.g. `async def handle_display_data`. See `handlers.DebugHandler`
+or `cli.OutputHandler` for examples of custom Handlers. ## Comms Comms are a
+flexible way for a client and the Kernel to send messages outside of the
+`execute_request` format. The most widely used package that utilizes Comms is
+probably `ipywidgets`, but Comms in general are a very powerful tool for a
+Sidecar application. A Comm can be opened by either the Sidecar or the Kernel.
+A target for that Comm should be registered on the other side before the open
+happens. It's probably most typical to register a Comm target in the Kernel by
+sending an `execute_request`, then sending a `comm_open` from the Sidecar side.
+See `tests/test_comms.py` for examples. Once a Comm is open, it has a unique
+`comm_id`. `KernelSidecarClient` will automatically route all `comm_msg`
+messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content.
+That routing pattern is a bit confusing as it overlaps the `Handler` / `Action`
+pattern, but it's necessary because `comm_msg` can come in as a result of
+`execute_request`'s or `comm_msg`'s or potentially other messages. So the
+`CommManager` -> `CommHandler` routing basically needs to be applied to every
+message the `KernelSidecarClient` receives over ZMQ. ## Models `kernel-sidecar`
+has Pydantic models for: - The Jupyter Notebook document (`models/
+notebook.py`), which should be consistent with `nbformat` parsing / structure -
+Request messages sent to the Kernel over ZMQ (`models/requests.py`) - Messages
+received over ZMQ from the Kernel (`models/messages.py`) ## CLI `kernel-
+sidecar` ships a small CLI for testing a connection to a Kernel. ```bash â¯
+sidecar --help Usage: sidecar [OPTIONS] Options: -f FILE Kernel connection file
+[required] --debug / --no-debug Turn on DEBUG logging [default: no-debug] --
+execute TEXT Execute code string instead of sending kernel info request --tail
+/ --no-tail Continue tailing ZMQ after connecting or executing code [default:
+no-tail] --install-completion [bash|zsh|fish|powershell|pwsh] Install
+completion for the specified shell. --show-completion
+[bash|zsh|fish|powershell|pwsh] Show completion for the specified shell, to
+copy it or customize the installation. --help Show this message and exit. ```
+Try it out by starting an IPython kernel in one terminal and using the CLI in
+another. ```bash python -m ipykernel_launcher --debug -f /tmp/kernel.json ```
+```bash kernel-sidecar on î  release-0.3.2 [$?] is ð¦ v0.3.1 via ð
+v3.11.0 (kernel-sidecar-py3.11) â¯ sidecar -f /tmp/kernel.json 2023-03-10T14:
+31:59.992235Z [info ] Attempting to connect: {'control_port': 34897, 'hb_port':
+49821, 'iopub_port': 40577, 'ip': '127.0.0.1', 'kernel_name': '', 'key':
+'615bcebc-baf2e28abad1f6c017dc71dc', 'shell_port': 37421, 'signature_scheme':
+'hmac-sha256', 'stdin_port': 41405, 'transport': 'tcp'} [kernel_sidecar.cli]
+filename=cli.py func_name=main lineno=62 2023-03-10T14:32:00.026503Z [info ]
+{'banner': 'Python 3.11.0 (main, Nov 7 2022, 09:38:45) [GCC 9.4.0]\n' "Type
+'copyright', 'credits' or 'license' for more information\n" "IPython 8.10.0 -
+- An enhanced Interactive Python. Type '?' for " 'help.\n', 'debugger': None,
+'help_links': [{'text': 'Python Reference', 'url': 'https://docs.python.org/
+3.11'}, {'text': 'IPython Reference', 'url': 'https://ipython.org/
+documentation.html'}, {'text': 'NumPy Reference', 'url': 'https://
 docs.scipy.org/doc/numpy/reference/'}, {'text': 'SciPy Reference', 'url':
 'https://docs.scipy.org/doc/scipy/reference/'}, {'text': 'Matplotlib
 Reference', 'url': 'https://matplotlib.org/contents.html'}, {'text': 'SymPy
 Reference', 'url': 'http://docs.sympy.org/latest/index.html'}, {'text': 'pandas
 Reference', 'url': 'https://pandas.pydata.org/pandas-docs/stable/'}],
 'implementation': 'ipython', 'implementation_version': '8.10.0',
 'language_info': {'codemirror_mode': {'name': 'ipython', 'version': 3},
```

### Comparing `kernel_sidecar-0.5.2/pyproject.toml` & `kernel_sidecar-0.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kernel-sidecar"
-version = "0.5.2"
+version = "0.5.3"
 description = "A sidecar "
 authors = ["Matt Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "kernel_sidecar", from = "src"}]
 repository = "https://github.com/kafonek/kernel-sidecar"
 
@@ -27,18 +27,14 @@
 notebook = "^6.5.2"
 ipywidgets = "^8.0.4"
 jupyterlab = "^3.6.1"
 pytest-rerunfailures = "^11.1.1"
 structlog = "^22.3.0"
 
 
-[tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.0.12"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sidecar = "kernel_sidecar.cli:app"
```

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/actions.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,35 +71,37 @@
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.msg_type} {self.msg_id}>"
 
     def __await__(self) -> asyncio.Event:
         """Support 'await action' syntax"""
         return self.done.wait().__await__()
 
-    def maybe_set_done(self):
+    async def maybe_set_done(self):
         """
         Set the Action as "done", meaning we've seen all expected replies from the Kernel
          - always wait until Kernel has reported being Idle with our parent header msg id
          - Depending on the request type, also wait for an expected reply type, e.g.
            execute_request isn't "complete" until we get execute_reply
         """
         if self.kernel_idle.is_set():
             if self.reply_seen.is_set() or not self.expected_reply_msg_type:
                 self.done.set()
                 self.running = False
+                for handler in self.handlers:
+                    await handler.action_complete()
 
     async def handle_message(self, msg: messages.Message):
         """Delegate message to the appropriate handler defined in subclasses"""
         # Delegate the message to any attached handlers, in the order they were attached
         for handler in self.handlers:
             await handler(msg)
 
         # Checking for status / special reply type in order to maybe set "done"
         if msg.msg_type == "status":
             if msg.content.execution_state == "busy":
                 self.running = True
             elif msg.content.execution_state == "idle":
                 self.kernel_idle.set()
-                self.maybe_set_done()
+                await self.maybe_set_done()
         elif msg.msg_type == self.expected_reply_msg_type:
             self.reply_seen.set()
-            self.maybe_set_done()
+            await self.maybe_set_done()
```

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/cli.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/cli.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/client.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/client.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/comms.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/comms.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/base.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,13 @@
             await self.unhandled_message(msg)
 
     async def unhandled_message(self, msg: messages.Message):
         """
         Called when a message is delegated to this Action but no handler is defined for the msg_type
         """
         pass
+
+    async def action_complete(self):
+        """
+        Called when the KernelAction this Handler is attached to is complete
+        """
+        pass
```

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/debug.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/debug.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/handlers/output.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/output.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/log_utils.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/log_utils.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/models/messages.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/models/messages.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/models/notebook.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/models/notebook.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/models/requests.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/models/requests.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.2/src/kernel_sidecar/nb_builder.py` & `kernel_sidecar-0.5.3/src/kernel_sidecar/nb_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,31 +31,39 @@
         data = {"id": id or str(uuid.uuid4()), "source": source, "cell_type": cell_type}
         if self.get_cell(data["id"]):
             data["id"] = str(uuid.uuid4())
         cell = pydantic.parse_obj_as(notebook.NotebookCell, data)
         self.nb.cells.append(cell)
         return cell
 
-    def add_cell_output(
-        self,
-        cell_id: str,
-        content: ContentType,
-    ):
+    def add_cell_output(self, cell_id: str, content: ContentType):
         cell = self.get_cell(cell_id)
         if not cell:
             logger.warning(f"Cell not found: {cell_id}")
             return
         cell.outputs.append(content)
 
+    def set_execution_count(self, cell_id: str, execution_count: int):
+        cell = self.get_cell(cell_id)
+        if not cell:
+            logger.warning(f"Cell not found: {cell_id}")
+            return
+        if cell.cell_type != "code":
+            logger.warning(f"Cell is not a code cell: {cell_id}")
+            return
+        cell.execution_count = execution_count
+
     def clear_cell_output(self, cell_id: str):
         cell = self.get_cell(cell_id)
         if not cell:
             logger.warning(f"Cell not found: {cell_id}")
             return
         cell.outputs = []
+        if cell.cell_type == "code":
+            cell.execution_count = None
 
     def replace_display_data(
         self, content: Union[messages.DisplayDataContent, messages.UpdateDisplayDataContent]
     ):
         for cell in self.nb.cells:
             for idx, output in enumerate(cell.outputs):
                 if isinstance(output, messages.DisplayDataContent):
@@ -108,7 +116,10 @@
     async def clear_output_widget_content(self, handler: WidgetHandler):
         self.builder.output_widget_state[handler.comm_id] = handler.state["outputs"]
 
     async def sync_display_data(
         self, content: Union[messages.DisplayDataContent, messages.UpdateDisplayDataContent]
     ):
         self.builder.replace_display_data(content)
+
+    async def handle_execute_input(self, msg: messages.ExecuteInput):
+        self.builder.set_execution_count(self.cell_id, msg.content.execution_count)
```

### Comparing `kernel_sidecar-0.5.2/setup.py` & `kernel_sidecar-0.5.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,180 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kernel-sidecar
+Version: 0.5.3
+Summary: A sidecar 
+Home-page: https://github.com/kafonek/kernel-sidecar
+License: MIT
+Author: Matt Kafonek
+Author-email: matt.kafonek@noteable.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cli
+Requires-Dist: jupyter-client (>=7.3.4)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: structlog ; extra == "cli"
+Requires-Dist: typer ; extra == "cli"
+Project-URL: Repository, https://github.com/kafonek/kernel-sidecar
+Description-Content-Type: text/markdown
+
+<p align="center">
+Kernel Sidecar
+</p>
+
+<p align="center">
+<img alt="Pypi" src="https://img.shields.io/pypi/v/kernel-sidecar">
+<a href="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml">
+    <img src="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml/badge.svg" alt="Tests" />
+</a>
+<img alt="Python versions" src="https://img.shields.io/pypi/pyversions/kernel-sidecar">
+</p>
+
+# Overview
+
+`kernel-sidecar` provides the building blocks for creating applications that run alongside Jupyter Kernels, keeping the Notebook document model in memory and acting as a middle-man between the Kernel and all other clients. There are many potential features that can be built into a Sidecar application:
+
+ - __Persisting Outputs__ for cell execution even when no clients are connected (e.g. run a cell, close your browser, come back later and see the output)
+ - __Code Cell Linting__ such as `black` or `isort`
+ - __Variable Explorer__ that can be sent to newly connected clients without needing to execute code in the Kernel
+ - __Custom Execution Managers__ to handle DAG/dependent cell execution or to dequeue queued cells without sending an interrupt to the Kernel which dequeues all queued cells
+
+
+## Installation
+
+```bash
+pip install kernel-sidecar
+```
+
+
+# Key Concepts
+
+![Architecture overview diagram](docs/overview_arch_diagram.png)
+
+## KernelSidecarClient
+
+The `KernelSidecarClient` class manages the ZMQ connections to the Kernel, sending execute request or other messages to the Kernel, and processing messages coming back from the Kernel on `iopub`, `shell`, `control`, and `stdin` channels. All messages sent and received are modeled with Pydantic. When preparing to send a request to the Kernel, it's structured as a `KernelAction` which connects the request with zero-to-many callbacks for responses to that specific request.
+
+
+## KernelAction
+
+`KernelAction` connects three key pieces of the request-reply flow between the sidecar application and the Kernel:
+ - Store the sent Request message
+ - Delegate messages to callbacks based on the request message
+ - Make the flow "awaitable" based on the Request type, e.g. an `execute_request` is done when `execute_reply` or `error` is received and `status` has gone to `idle`.
+
+## Handlers
+
+When the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods named for the message type, e.g. `async def handle_display_data`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.
+
+## Comms
+
+Comms are a flexible way for a client and the Kernel to send messages outside of the `execute_request` format. The most widely used package that utilizes Comms is probably `ipywidgets`, but Comms in general are a very powerful tool for a Sidecar application. A Comm can be opened by either the Sidecar or the Kernel. A target for that Comm should be registered on the other side before the open happens. It's probably most typical to register a Comm target in the Kernel by sending an `execute_request`, then sending a `comm_open` from the Sidecar side. See `tests/test_comms.py` for examples.
+
+Once a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will automatically route all `comm_msg` messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but it's necessary because `comm_msg` can come in as a result of `execute_request`'s or `comm_msg`'s or potentially other messages. So the `CommManager` -> `CommHandler` routing basically needs to be applied to every message the `KernelSidecarClient` receives over ZMQ.
+
+
+## Models
+
+`kernel-sidecar` has Pydantic models for:
+ - The Jupyter Notebook document (`models/notebook.py`), which should be consistent with `nbformat` parsing / structure
+ - Request messages sent to the Kernel over ZMQ (`models/requests.py`)
+ - Messages received over ZMQ from the Kernel (`models/messages.py`)
+
+
+## CLI
+
+`kernel-sidecar` ships a small CLI for testing a connection to a Kernel.
+
+```bash
+❯ sidecar --help
+Usage: sidecar [OPTIONS]
+
+Options:
+  -f FILE                         Kernel connection file  [required]
+  --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]
+  --execute TEXT                  Execute code string instead of sending
+                                  kernel info request
+  --tail / --no-tail              Continue tailing ZMQ after connecting or
+                                  executing code  [default: no-tail]
+  --install-completion [bash|zsh|fish|powershell|pwsh]
+                                  Install completion for the specified shell.
+  --show-completion [bash|zsh|fish|powershell|pwsh]
+                                  Show completion for the specified shell, to
+                                  copy it or customize the installation.
+  --help                          Show this message and exit.
+```
+
+Try it out by starting an IPython kernel in one terminal and using the CLI in another.
+
+```bash
+python -m ipykernel_launcher --debug -f /tmp/kernel.json
+```
+
+```bash
+kernel-sidecar on  release-0.3.2 [$?] is 📦 v0.3.1 via 🐍 v3.11.0 (kernel-sidecar-py3.11) 
+❯ sidecar -f /tmp/kernel.json
+2023-03-10T14:31:59.992235Z [info     ] Attempting to connect:
+{'control_port': 34897,
+ 'hb_port': 49821,
+ 'iopub_port': 40577,
+ 'ip': '127.0.0.1',
+ 'kernel_name': '',
+ 'key': '615bcebc-baf2e28abad1f6c017dc71dc',
+ 'shell_port': 37421,
+ 'signature_scheme': 'hmac-sha256',
+ 'stdin_port': 41405,
+ 'transport': 'tcp'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62
+2023-03-10T14:32:00.026503Z [info     ] {'banner': 'Python 3.11.0 (main, Nov  7 2022, 09:38:45) [GCC 9.4.0]\n'
+           "Type 'copyright', 'credits' or 'license' for more information\n"
+           "IPython 8.10.0 -- An enhanced Interactive Python. Type '?' for "
+           'help.\n',
+ 'debugger': None,
+ 'help_links': [{'text': 'Python Reference',
+                 'url': 'https://docs.python.org/3.11'},
+                {'text': 'IPython Reference',
+                 'url': 'https://ipython.org/documentation.html'},
+                {'text': 'NumPy Reference',
+                 'url': 'https://docs.scipy.org/doc/numpy/reference/'},
+                {'text': 'SciPy Reference',
+                 'url': 'https://docs.scipy.org/doc/scipy/reference/'},
+                {'text': 'Matplotlib Reference',
+                 'url': 'https://matplotlib.org/contents.html'},
+                {'text': 'SymPy Reference',
+                 'url': 'http://docs.sympy.org/latest/index.html'},
+                {'text': 'pandas Reference',
+                 'url': 'https://pandas.pydata.org/pandas-docs/stable/'}],
+ 'implementation': 'ipython',
+ 'implementation_version': '8.10.0',
+ 'language_info': {'codemirror_mode': {'name': 'ipython', 'version': 3},
+                   'file_extension': '.py',
+                   'mimetype': 'text/x-python',
+                   'name': 'python',
+                   'nbconvert_exporter': 'python',
+                   'pygments_lexer': 'ipython3',
+                   'version': '3.11.0'},
+ 'protocol_version': '5.3',
+ 'status': 'ok'} [kernel_sidecar.cli] filename=cli.py func_name=connect lineno=44
+```
+
+```bash
+❯ sidecar -f /tmp/kernel.json --execute "print('Hello, World'); 1/0"
+2023-03-10T14:33:27.394935Z [info     ] Attempting to connect:
+{'control_port': 34897,
+ 'hb_port': 49821,
+ 'iopub_port': 40577,
+ 'ip': '127.0.0.1',
+ 'kernel_name': '',
+ 'key': '615bcebc-baf2e28abad1f6c017dc71dc',
+ 'shell_port': 37421,
+ 'signature_scheme': 'hmac-sha256',
+ 'stdin_port': 41405,
+ 'transport': 'tcp'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62
+2023-03-10T14:33:27.629630Z [info     ] Hello, World
+                  [kernel_sidecar.cli] filename=cli.py func_name=handle_stream lineno=23
+2023-03-10T14:33:27.702700Z [error    ] division by zero               [kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31
+```
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['kernel_sidecar', 'kernel_sidecar.handlers', 'kernel_sidecar.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['jupyter-client>=7.3.4', 'pydantic>=1.10.4,<2.0.0']
-
-extras_require = \
-{'cli': ['structlog', 'typer']}
-
-entry_points = \
-{'console_scripts': ['sidecar = kernel_sidecar.cli:app']}
-
-setup_kwargs = {
-    'name': 'kernel-sidecar',
-    'version': '0.5.2',
-    'description': 'A sidecar ',
-    'long_description': '<p align="center">\nKernel Sidecar\n</p>\n\n<p align="center">\n<img alt="Pypi" src="https://img.shields.io/pypi/v/kernel-sidecar">\n<a href="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml">\n    <img src="https://github.com/kafonek/kernel-sidecar/actions/workflows/tests.yaml/badge.svg" alt="Tests" />\n</a>\n<img alt="Python versions" src="https://img.shields.io/pypi/pyversions/kernel-sidecar">\n</p>\n\n# Kernel-Sidecar\n\nThis package offers the building blocks for creating a "Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture, one or many frontends manage the document model (code cells, outputs, metadata, etc) and send requests to a single Kernel. Each frontend observes responses on different ZMQ channels (`iopub`, `shell`, etc) but may end up with some inconsistency based on the Kernel only sending certain responses to the client that made the request.\n\nIn a `kernel-sidecar` architecture, all frontend clients talk to the `kernel-sidecar` client, and only the `kernel-sidecar` client communicates with the Kernel over ZMQ. That pattern offers several potential features:\n - Keep a document model within `kernel-sidecar` or the backend architecture\n - Add "extension"-esque capabilities on the backend such as auto-linting code on execute\n - Eliminate inconsistencies in what messages individual frontends receive because of Kernel replies\n - Model all requests, replies, and the Notebook document with Pydantic\n\n## Installation\n\n```bash\npip install kernel-sidecar\n```\n\n# Key Concepts\n## KernelSidecarClient\n\nA manager that uses `jupyter_client` under the hood to create ZMQ connections and watch for messages coming in over different ZMQ channels (`iopub`, `shell`, etc. An important assumption here is that `kernel-sidecar` is the only client talking to the Kernel, which means every message observed coming from the Kernel should be a reply (based on `parent_header_msg.msg_id`) to a request sent from this client.\n\nWhen the `KernelSidecarClient` send a request to the Kernel, it is wrapped in an `KernelAction` class. Every message received from the Kernel is delegated to the requesting Action and triggers callbacks attached to the Action class.\n\n## Actions\n\nActions in `kernel-sidecar` encompass a request-reply cycle, including an `await action` syntax, where the Action is complete when the Kernel has reported its status returning to `idle` and optionally emitted a reply appropriate for the request. For instance, an `execute_request` is "done" when the `status` has been reported as `idle` *and* the Kernel has emitted an `execute_reply`, both with the `parent_header_msg.msg_id` the same as the `execute_request` `header.msg_id`.\n\nIn a nutshell, an `actions.KernelAction` takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses (or just `async functions`) and creates an `awaitable` instance. `kernel.send(action)` submits the Request over ZMQ, and registers the Action so that all observed messages get routed to that Action to be handled by the Handlers/callbacks.\n\nMost of the time, you should be able to just use convience functions in the `KernelSidecarClient` class to create the actions. See `tests/test_actions.py` for many examples of using Actions and Handlers.\n\n## Handlers\n\nWhen the `KernelSidecarClient` receives a message over ZMQ, parses it into a Pydantic model, and delegates it to the appropriate `Action` to be handled, it passes on that message to every `Handler` attached to the `Action` and awaits all of them to handle that message. `Handler` objects can define handling different message types by creating methods `handle_<msg_type>`. See `handlers.DebugHandler` or `cli.OutputHandler` for examples of custom Handlers.\n\n## Comms\n\nComms are a flexible way for a client and the Kernel to send messages outside of the `execute_request` format. The most widely used package that utilizes Comms is probably `ipywidgets`, but Comms in general are a very powerful tool for a Sidecar application. A Comm can be opened by either the Sidecar or the Kernel. A target for that Comm should be registered on the other side before the open happens. It\'s probably most typical to register a Comm target in the Kernel by sending an `execute_request`, then sending a `comm_open` from the Sidecar side. See `tests/test_comms.py` for examples.\n\nOnce a Comm is open, it has a unique `comm_id`. `KernelSidecarClient` will automatically route all `comm_msg` messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content. That routing pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but it\'s necessary because `comm_msg` can come in as a result of `execute_request`\'s or `comm_msg`\'s or potentially other messages. So the `CommManager` -> `CommHandler` routing basically needs to be applied to every message the `KernelSidecarClient` receives over ZMQ.\n\n\n## Models\n\n`kernel-sidecar` has Pydantic models for:\n - The Jupyter Notebook document (`models/notebook.py`), which should be consistent with `nbformat` parsing / structure\n - Request messages sent to the Kernel over ZMQ (`models/requests.py`)\n - Messages received over ZMQ from the Kernel (`models/messages.py`)\n\n\n## CLI\n\n`kernel-sidecar` ships a small CLI for testing a connection to a Kernel.\n\n```bash\n❯ sidecar --help\nUsage: sidecar [OPTIONS]\n\nOptions:\n  -f FILE                         Kernel connection file  [required]\n  --debug / --no-debug            Turn on DEBUG logging  [default: no-debug]\n  --execute TEXT                  Execute code string instead of sending\n                                  kernel info request\n  --tail / --no-tail              Continue tailing ZMQ after connecting or\n                                  executing code  [default: no-tail]\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n```\n\nTry it out by starting an IPython kernel in one terminal and using the CLI in another.\n\n```bash\npython -m ipykernel_launcher --debug -f /tmp/kernel.json\n```\n\n```bash\nkernel-sidecar on \ue0a0 release-0.3.2 [$?] is 📦 v0.3.1 via 🐍 v3.11.0 (kernel-sidecar-py3.11) \n❯ sidecar -f /tmp/kernel.json\n2023-03-10T14:31:59.992235Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:32:00.026503Z [info     ] {\'banner\': \'Python 3.11.0 (main, Nov  7 2022, 09:38:45) [GCC 9.4.0]\\n\'\n           "Type \'copyright\', \'credits\' or \'license\' for more information\\n"\n           "IPython 8.10.0 -- An enhanced Interactive Python. Type \'?\' for "\n           \'help.\\n\',\n \'debugger\': None,\n \'help_links\': [{\'text\': \'Python Reference\',\n                 \'url\': \'https://docs.python.org/3.11\'},\n                {\'text\': \'IPython Reference\',\n                 \'url\': \'https://ipython.org/documentation.html\'},\n                {\'text\': \'NumPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/numpy/reference/\'},\n                {\'text\': \'SciPy Reference\',\n                 \'url\': \'https://docs.scipy.org/doc/scipy/reference/\'},\n                {\'text\': \'Matplotlib Reference\',\n                 \'url\': \'https://matplotlib.org/contents.html\'},\n                {\'text\': \'SymPy Reference\',\n                 \'url\': \'http://docs.sympy.org/latest/index.html\'},\n                {\'text\': \'pandas Reference\',\n                 \'url\': \'https://pandas.pydata.org/pandas-docs/stable/\'}],\n \'implementation\': \'ipython\',\n \'implementation_version\': \'8.10.0\',\n \'language_info\': {\'codemirror_mode\': {\'name\': \'ipython\', \'version\': 3},\n                   \'file_extension\': \'.py\',\n                   \'mimetype\': \'text/x-python\',\n                   \'name\': \'python\',\n                   \'nbconvert_exporter\': \'python\',\n                   \'pygments_lexer\': \'ipython3\',\n                   \'version\': \'3.11.0\'},\n \'protocol_version\': \'5.3\',\n \'status\': \'ok\'} [kernel_sidecar.cli] filename=cli.py func_name=connect lineno=44\n```\n\n```bash\n❯ sidecar -f /tmp/kernel.json --execute "print(\'Hello, World\'); 1/0"\n2023-03-10T14:33:27.394935Z [info     ] Attempting to connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:33:27.629630Z [info     ] Hello, World\n                  [kernel_sidecar.cli] filename=cli.py func_name=handle_stream lineno=23\n2023-03-10T14:33:27.702700Z [error    ] division by zero               [kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31\n```\n',
-    'author': 'Matt Kafonek',
-    'author_email': 'matt.kafonek@noteable.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kafonek/kernel-sidecar',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,129 +1,107 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['kernel_sidecar', 'kernel_sidecar.handlers',
-'kernel_sidecar.models'] package_data = \ {'': ['*']} install_requires = \
-['jupyter-client>=7.3.4', 'pydantic>=1.10.4,<2.0.0'] extras_require = \ {'cli':
-['structlog', 'typer']} entry_points = \ {'console_scripts': ['sidecar =
-kernel_sidecar.cli:app']} setup_kwargs = { 'name': 'kernel-sidecar', 'version':
-'0.5.2', 'description': 'A sidecar ', 'long_description': '
-                              \nKernel Sidecar\n
-\n\n
-                  \n[Pypi]\n\n_[Tests]\n\n[Python versions]\n
-\n\n# Kernel-Sidecar\n\nThis package offers the building blocks for creating a
-"Kernel Sidecar" Jupyter framework. In normal Jupyter Notebook architecture,
-one or many frontends manage the document model (code cells, outputs, metadata,
-etc) and send requests to a single Kernel. Each frontend observes responses on
-different ZMQ channels (`iopub`, `shell`, etc) but may end up with some
-inconsistency based on the Kernel only sending certain responses to the client
-that made the request.\n\nIn a `kernel-sidecar` architecture, all frontend
-clients talk to the `kernel-sidecar` client, and only the `kernel-sidecar`
-client communicates with the Kernel over ZMQ. That pattern offers several
-potential features:\n - Keep a document model within `kernel-sidecar` or the
-backend architecture\n - Add "extension"-esque capabilities on the backend such
-as auto-linting code on execute\n - Eliminate inconsistencies in what messages
-individual frontends receive because of Kernel replies\n - Model all requests,
-replies, and the Notebook document with Pydantic\n\n##
-Installation\n\n```bash\npip install kernel-sidecar\n```\n\n# Key Concepts\n##
-KernelSidecarClient\n\nA manager that uses `jupyter_client` under the hood to
-create ZMQ connections and watch for messages coming in over different ZMQ
-channels (`iopub`, `shell`, etc. An important assumption here is that `kernel-
-sidecar` is the only client talking to the Kernel, which means every message
-observed coming from the Kernel should be a reply (based on
-`parent_header_msg.msg_id`) to a request sent from this client.\n\nWhen the
-`KernelSidecarClient` send a request to the Kernel, it is wrapped in an
-`KernelAction` class. Every message received from the Kernel is delegated to
-the requesting Action and triggers callbacks attached to the Action
-class.\n\n## Actions\n\nActions in `kernel-sidecar` encompass a request-reply
-cycle, including an `await action` syntax, where the Action is complete when
-the Kernel has reported its status returning to `idle` and optionally emitted a
-reply appropriate for the request. For instance, an `execute_request` is "done"
-when the `status` has been reported as `idle` *and* the Kernel has emitted an
-`execute_reply`, both with the `parent_header_msg.msg_id` the same as the
-`execute_request` `header.msg_id`.\n\nIn a nutshell, an `actions.KernelAction`
-takes in a `requests.Request` and zero-to-many `handlers.Handler` subclasses
-(or just `async functions`) and creates an `awaitable` instance. `kernel.send
-(action)` submits the Request over ZMQ, and registers the Action so that all
-observed messages get routed to that Action to be handled by the Handlers/
-callbacks.\n\nMost of the time, you should be able to just use convience
-functions in the `KernelSidecarClient` class to create the actions. See `tests/
-test_actions.py` for many examples of using Actions and Handlers.\n\n##
-Handlers\n\nWhen the `KernelSidecarClient` receives a message over ZMQ, parses
-it into a Pydantic model, and delegates it to the appropriate `Action` to be
-handled, it passes on that message to every `Handler` attached to the `Action`
-and awaits all of them to handle that message. `Handler` objects can define
-handling different message types by creating methods `handle_`. See
-`handlers.DebugHandler` or `cli.OutputHandler` for examples of custom
-Handlers.\n\n## Comms\n\nComms are a flexible way for a client and the Kernel
-to send messages outside of the `execute_request` format. The most widely used
-package that utilizes Comms is probably `ipywidgets`, but Comms in general are
-a very powerful tool for a Sidecar application. A Comm can be opened by either
-the Sidecar or the Kernel. A target for that Comm should be registered on the
-other side before the open happens. It\'s probably most typical to register a
-Comm target in the Kernel by sending an `execute_request`, then sending a
-`comm_open` from the Sidecar side. See `tests/test_comms.py` for
-examples.\n\nOnce a Comm is open, it has a unique `comm_id`.
-`KernelSidecarClient` will automatically route all `comm_msg` messages to a
-`CommHandler` instance by `comm_id` in the `comm_msg` content. That routing
-pattern is a bit confusing as it overlaps the `Handler` / `Action` pattern, but
-it\'s necessary because `comm_msg` can come in as a result of
-`execute_request`\'s or `comm_msg`\'s or potentially other messages. So the
+Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.3 Summary: A sidecar
+Home-page: https://github.com/kafonek/kernel-sidecar License: MIT Author: Matt
+Kafonek Author-email: matt.kafonek@noteable.io Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cli Requires-Dist: jupyter-client (>=7.3.4) Requires-Dist:
+pydantic (>=1.10.4,<2.0.0) Requires-Dist: structlog ; extra == "cli" Requires-
+Dist: typer ; extra == "cli" Project-URL: Repository, https://github.com/
+kafonek/kernel-sidecar Description-Content-Type: text/markdown
+                                Kernel Sidecar
+                       [Pypi] [Tests] [Python versions]
+# Overview `kernel-sidecar` provides the building blocks for creating
+applications that run alongside Jupyter Kernels, keeping the Notebook document
+model in memory and acting as a middle-man between the Kernel and all other
+clients. There are many potential features that can be built into a Sidecar
+application: - __Persisting Outputs__ for cell execution even when no clients
+are connected (e.g. run a cell, close your browser, come back later and see the
+output) - __Code Cell Linting__ such as `black` or `isort` - __Variable
+Explorer__ that can be sent to newly connected clients without needing to
+execute code in the Kernel - __Custom Execution Managers__ to handle DAG/
+dependent cell execution or to dequeue queued cells without sending an
+interrupt to the Kernel which dequeues all queued cells ## Installation ```bash
+pip install kernel-sidecar ``` # Key Concepts ![Architecture overview diagram]
+(docs/overview_arch_diagram.png) ## KernelSidecarClient The
+`KernelSidecarClient` class manages the ZMQ connections to the Kernel, sending
+execute request or other messages to the Kernel, and processing messages coming
+back from the Kernel on `iopub`, `shell`, `control`, and `stdin` channels. All
+messages sent and received are modeled with Pydantic. When preparing to send a
+request to the Kernel, it's structured as a `KernelAction` which connects the
+request with zero-to-many callbacks for responses to that specific request. ##
+KernelAction `KernelAction` connects three key pieces of the request-reply flow
+between the sidecar application and the Kernel: - Store the sent Request
+message - Delegate messages to callbacks based on the request message - Make
+the flow "awaitable" based on the Request type, e.g. an `execute_request` is
+done when `execute_reply` or `error` is received and `status` has gone to
+`idle`. ## Handlers When the `KernelSidecarClient` receives a message over ZMQ,
+parses it into a Pydantic model, and delegates it to the appropriate `Action`
+to be handled, it passes on that message to every `Handler` attached to the
+`Action` and awaits all of them to handle that message. `Handler` objects can
+define handling different message types by creating methods named for the
+message type, e.g. `async def handle_display_data`. See `handlers.DebugHandler`
+or `cli.OutputHandler` for examples of custom Handlers. ## Comms Comms are a
+flexible way for a client and the Kernel to send messages outside of the
+`execute_request` format. The most widely used package that utilizes Comms is
+probably `ipywidgets`, but Comms in general are a very powerful tool for a
+Sidecar application. A Comm can be opened by either the Sidecar or the Kernel.
+A target for that Comm should be registered on the other side before the open
+happens. It's probably most typical to register a Comm target in the Kernel by
+sending an `execute_request`, then sending a `comm_open` from the Sidecar side.
+See `tests/test_comms.py` for examples. Once a Comm is open, it has a unique
+`comm_id`. `KernelSidecarClient` will automatically route all `comm_msg`
+messages to a `CommHandler` instance by `comm_id` in the `comm_msg` content.
+That routing pattern is a bit confusing as it overlaps the `Handler` / `Action`
+pattern, but it's necessary because `comm_msg` can come in as a result of
+`execute_request`'s or `comm_msg`'s or potentially other messages. So the
 `CommManager` -> `CommHandler` routing basically needs to be applied to every
-message the `KernelSidecarClient` receives over ZMQ.\n\n\n## Models\n\n`kernel-
-sidecar` has Pydantic models for:\n - The Jupyter Notebook document (`models/
-notebook.py`), which should be consistent with `nbformat` parsing / structure\n
-- Request messages sent to the Kernel over ZMQ (`models/requests.py`)\n -
-Messages received over ZMQ from the Kernel (`models/messages.py`)\n\n\n##
-CLI\n\n`kernel-sidecar` ships a small CLI for testing a connection to a
-Kernel.\n\n```bash\nâ¯ sidecar --help\nUsage: sidecar [OPTIONS]\n\nOptions:\n
--f FILE Kernel connection file [required]\n --debug / --no-debug Turn on DEBUG
-logging [default: no-debug]\n --execute TEXT Execute code string instead of
-sending\n kernel info request\n --tail / --no-tail Continue tailing ZMQ after
-connecting or\n executing code [default: no-tail]\n --install-completion
-[bash|zsh|fish|powershell|pwsh]\n Install completion for the specified shell.\n
---show-completion [bash|zsh|fish|powershell|pwsh]\n Show completion for the
-specified shell, to\n copy it or customize the installation.\n --help Show this
-message and exit.\n```\n\nTry it out by starting an IPython kernel in one
-terminal and using the CLI in another.\n\n```bash\npython -m ipykernel_launcher
---debug -f /tmp/kernel.json\n```\n\n```bash\nkernel-sidecar on \ue0a0 release-
-0.3.2 [$?] is ð¦ v0.3.1 via ð v3.11.0 (kernel-sidecar-py3.11) \nâ¯
-sidecar -f /tmp/kernel.json\n2023-03-10T14:31:59.992235Z [info ] Attempting to
-connect:\n{\'control_port\': 34897,\n \'hb_port\': 49821,\n \'iopub_port\':
-40577,\n \'ip\': \'127.0.0.1\',\n \'kernel_name\': \'\',\n \'key\': \'615bcebc-
-baf2e28abad1f6c017dc71dc\',\n \'shell_port\': 37421,\n \'signature_scheme\':
-\'hmac-sha256\',\n \'stdin_port\': 41405,\n \'transport\': \'tcp\'}
-[kernel_sidecar.cli] filename=cli.py func_name=main lineno=62\n2023-03-10T14:
-32:00.026503Z [info ] {\'banner\': \'Python 3.11.0 (main, Nov 7 2022, 09:38:45)
-[GCC 9.4.0]\\n\'\n "Type \'copyright\', \'credits\' or \'license\' for more
-information\\n"\n "IPython 8.10.0 -- An enhanced Interactive Python. Type \'?\'
-for "\n \'help.\\n\',\n \'debugger\': None,\n \'help_links\': [{\'text\':
-\'Python Reference\',\n \'url\': \'https://docs.python.org/3.11\'},\n
-{\'text\': \'IPython Reference\',\n \'url\': \'https://ipython.org/
-documentation.html\'},\n {\'text\': \'NumPy Reference\',\n \'url\': \'https://
-docs.scipy.org/doc/numpy/reference/\'},\n {\'text\': \'SciPy Reference\',\n
-\'url\': \'https://docs.scipy.org/doc/scipy/reference/\'},\n {\'text\':
-\'Matplotlib Reference\',\n \'url\': \'https://matplotlib.org/
-contents.html\'},\n {\'text\': \'SymPy Reference\',\n \'url\': \'http://
-docs.sympy.org/latest/index.html\'},\n {\'text\': \'pandas Reference\',\n
-\'url\': \'https://pandas.pydata.org/pandas-docs/stable/\'}],\n
-\'implementation\': \'ipython\',\n \'implementation_version\': \'8.10.0\',\n
-\'language_info\': {\'codemirror_mode\': {\'name\': \'ipython\', \'version\':
-3},\n \'file_extension\': \'.py\',\n \'mimetype\': \'text/x-python\',\n
-\'name\': \'python\',\n \'nbconvert_exporter\': \'python\',\n
-\'pygments_lexer\': \'ipython3\',\n \'version\': \'3.11.0\'},\n
-\'protocol_version\': \'5.3\',\n \'status\': \'ok\'} [kernel_sidecar.cli]
-filename=cli.py func_name=connect lineno=44\n```\n\n```bash\nâ¯ sidecar -f /
-tmp/kernel.json --execute "print(\'Hello, World\'); 1/0"\n2023-03-10T14:33:
-27.394935Z [info ] Attempting to connect:\n{\'control_port\': 34897,\n
-\'hb_port\': 49821,\n \'iopub_port\': 40577,\n \'ip\': \'127.0.0.1\',\n
-\'kernel_name\': \'\',\n \'key\': \'615bcebc-baf2e28abad1f6c017dc71dc\',\n
-\'shell_port\': 37421,\n \'signature_scheme\': \'hmac-sha256\',\n
-\'stdin_port\': 41405,\n \'transport\': \'tcp\'} [kernel_sidecar.cli]
-filename=cli.py func_name=main lineno=62\n2023-03-10T14:33:27.629630Z [info ]
-Hello, World\n [kernel_sidecar.cli] filename=cli.py func_name=handle_stream
-lineno=23\n2023-03-10T14:33:27.702700Z [error ] division by zero
-[kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31\n```\n',
-'author': 'Matt Kafonek', 'author_email': 'matt.kafonek@noteable.io',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-kafonek/kernel-sidecar', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'entry_points': entry_points,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+message the `KernelSidecarClient` receives over ZMQ. ## Models `kernel-sidecar`
+has Pydantic models for: - The Jupyter Notebook document (`models/
+notebook.py`), which should be consistent with `nbformat` parsing / structure -
+Request messages sent to the Kernel over ZMQ (`models/requests.py`) - Messages
+received over ZMQ from the Kernel (`models/messages.py`) ## CLI `kernel-
+sidecar` ships a small CLI for testing a connection to a Kernel. ```bash â¯
+sidecar --help Usage: sidecar [OPTIONS] Options: -f FILE Kernel connection file
+[required] --debug / --no-debug Turn on DEBUG logging [default: no-debug] --
+execute TEXT Execute code string instead of sending kernel info request --tail
+/ --no-tail Continue tailing ZMQ after connecting or executing code [default:
+no-tail] --install-completion [bash|zsh|fish|powershell|pwsh] Install
+completion for the specified shell. --show-completion
+[bash|zsh|fish|powershell|pwsh] Show completion for the specified shell, to
+copy it or customize the installation. --help Show this message and exit. ```
+Try it out by starting an IPython kernel in one terminal and using the CLI in
+another. ```bash python -m ipykernel_launcher --debug -f /tmp/kernel.json ```
+```bash kernel-sidecar on î  release-0.3.2 [$?] is ð¦ v0.3.1 via ð
+v3.11.0 (kernel-sidecar-py3.11) â¯ sidecar -f /tmp/kernel.json 2023-03-10T14:
+31:59.992235Z [info ] Attempting to connect: {'control_port': 34897, 'hb_port':
+49821, 'iopub_port': 40577, 'ip': '127.0.0.1', 'kernel_name': '', 'key':
+'615bcebc-baf2e28abad1f6c017dc71dc', 'shell_port': 37421, 'signature_scheme':
+'hmac-sha256', 'stdin_port': 41405, 'transport': 'tcp'} [kernel_sidecar.cli]
+filename=cli.py func_name=main lineno=62 2023-03-10T14:32:00.026503Z [info ]
+{'banner': 'Python 3.11.0 (main, Nov 7 2022, 09:38:45) [GCC 9.4.0]\n' "Type
+'copyright', 'credits' or 'license' for more information\n" "IPython 8.10.0 -
+- An enhanced Interactive Python. Type '?' for " 'help.\n', 'debugger': None,
+'help_links': [{'text': 'Python Reference', 'url': 'https://docs.python.org/
+3.11'}, {'text': 'IPython Reference', 'url': 'https://ipython.org/
+documentation.html'}, {'text': 'NumPy Reference', 'url': 'https://
+docs.scipy.org/doc/numpy/reference/'}, {'text': 'SciPy Reference', 'url':
+'https://docs.scipy.org/doc/scipy/reference/'}, {'text': 'Matplotlib
+Reference', 'url': 'https://matplotlib.org/contents.html'}, {'text': 'SymPy
+Reference', 'url': 'http://docs.sympy.org/latest/index.html'}, {'text': 'pandas
+Reference', 'url': 'https://pandas.pydata.org/pandas-docs/stable/'}],
+'implementation': 'ipython', 'implementation_version': '8.10.0',
+'language_info': {'codemirror_mode': {'name': 'ipython', 'version': 3},
+'file_extension': '.py', 'mimetype': 'text/x-python', 'name': 'python',
+'nbconvert_exporter': 'python', 'pygments_lexer': 'ipython3', 'version':
+'3.11.0'}, 'protocol_version': '5.3', 'status': 'ok'} [kernel_sidecar.cli]
+filename=cli.py func_name=connect lineno=44 ``` ```bash â¯ sidecar -f /tmp/
+kernel.json --execute "print('Hello, World'); 1/0" 2023-03-10T14:33:27.394935Z
+[info ] Attempting to connect: {'control_port': 34897, 'hb_port': 49821,
+'iopub_port': 40577, 'ip': '127.0.0.1', 'kernel_name': '', 'key': '615bcebc-
+baf2e28abad1f6c017dc71dc', 'shell_port': 37421, 'signature_scheme': 'hmac-
+sha256', 'stdin_port': 41405, 'transport': 'tcp'} [kernel_sidecar.cli]
+filename=cli.py func_name=main lineno=62 2023-03-10T14:33:27.629630Z [info ]
+Hello, World [kernel_sidecar.cli] filename=cli.py func_name=handle_stream
+lineno=23 2023-03-10T14:33:27.702700Z [error ] division by zero
+[kernel_sidecar.cli] filename=cli.py func_name=handle_error lineno=31 ```
```

