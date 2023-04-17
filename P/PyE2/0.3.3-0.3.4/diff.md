# Comparing `tmp/pye2-0.3.3.tar.gz` & `tmp/pye2-0.3.4.tar.gz`

## Comparing `pye2-0.3.3.tar` & `pye2-0.3.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.3/TODOs.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pye2-0.3.3/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.3/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.3/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/__init__.py
--rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/logger.py
--rw-r--r--   0        0        0    18391 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/pipeline.py
--rw-r--r--   0        0        0    18533 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/tmpeb3hj3eh
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/default/__init__.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.3/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/attach_example.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/ex1.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/hello.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/remote_exec.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.3/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.3/LICENSE
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 pye2-0.3.3/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 pye2-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.4/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.3.4/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.4/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.4/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    21174 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.4/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/.example_env
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/ex1.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/hello.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.4/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.4/LICENSE
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.3.4/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.3.4/PKG-INFO
```

### Comparing `pye2-0.3.3/.github/workflows/python-publish.yml` & `pye2-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/base/__init__.py` & `pye2-0.3.4/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/base/generic_session.py` & `pye2-0.3.4/PyE2/base/generic_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 from ..io_formatter import IOFormatterManager
 from .logger import Logger
 from .payload import Payload
 from .pipeline import Pipeline
 
 
 class GenericSession(object):
+  """
+  A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
+  A Session manages `Pipelines` and handles all messages received from the communication server.
+  The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
+  """
   default_config = {
       "CONFIG_CHANNEL": {
           "TOPIC": "lummetry/{}/config"
       },
       "CTRL_CHANNEL": {
           "TOPIC": "lummetry/ctrl"
       },
@@ -43,27 +48,53 @@
       "PAYLOADS_CHANNEL": {
           "TOPIC": "lummetry/payloads"
       },
       "QOS": 0
   }
 
   def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
-    """Create a session object that allows to connect to a communication server and to interact with nodes from the AiXp network.
+    """
+  A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
+  A Session manages `Pipelines` and handles all messages received from the communication server.
+  The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
 
-    Args:
-        host (str): Hostname of the server
-        port (int): port
-        user (str): username
-        pwd (str): password
-        name (str, optional): Will be used as `SESSION_ID` when communicating with AiXp nodes. Defaults to 'pySDK'.
-        config (dict, optional): Configures the names of the channels this session will connect to. Defaults to {}.
-        log (Logger, optional): instance of a Logger class that provides utility functions and prettier logs. Useful for Hyperfy devs. Defaults to None.
-        on_notification (Callable[[Session, dict], None], optional): Callback that handles the notification received by this session. Defaults to None.
-        on_heartbeat (Callable[[Session, dict], None], optional): Callback that handles the heartbeat received by this session. Defaults to None.
-        silent (bool, optional): This flag controlls if the `.D` method dumps text to the stdout. Defaults to True.
+    Parameters
+    ----------
+    host : str
+        The hostname of the server
+    port : int
+        The port
+    user : str
+        The user name
+    pwd : str
+        The password
+    name : str, optional
+        The name of this connection, used to identify owned pipelines on a specific AiXpand node.
+        The name will be used as `INITIATOR_ID` and `SESSION_ID` when communicating with AiXp nodes, by default 'pySDK'
+    config : dict, optional
+        Configures the names of the channels this session will connect to.
+        If using a Mqtt server, these channels are in fact topics.
+        Modify this if you are absolutely certain of what you are doing.
+        By default {}
+    log : Logger, optional
+        A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
+        In the future, the documentation for the Logger base class will be available and developers will be able to use
+        custom-made Loggers. 
+    on_notification : Callable[[Session, dict], None], optional
+        Callback that handles notifications received from this network. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+        This callback will be called when there are notifications related to the node itself, e.g. when the node runs
+        low on memory. 
+        Defaults to None.
+    on_heartbeat : Callable[[Session, dict], None], optional
+        Callback that handles heartbeats received from this network, by default None
+    silent : bool, optional
+        This flag will disable debug logs, set to 'False` for a more verbose log, by default True
     """
     if log is None:
       log = Logger()
 
     super(GenericSession, self).__init__()
 
     self.silent = silent
@@ -230,47 +261,121 @@
   def send_command_delete_pipeline(self, worker, stream_name):
     self._send_command_to_box('ARCHIVE_CONFIG', worker, stream_name)
 
   def _send_payload(self, to, payload):
     raise NotImplementedError
 
   def P(self, *args, **kwargs):
-    """Print info to stdout
+    """
+    Call the `Logger.P` method. If using the default Logger, this call will print
+    info to stdout.
+
+    Parameters
+    ----------
+    *args :
+
+    msg : obj
+        The message to pass to the `Logger.P` method. If using the default Logger, this
+        will be the message displayed at the stdout.
+
+    **kwargs :
+
+
+    Returns
+    -------
+
     """
     self.log.P(*args, **kwargs)
 
   def D(self, *args, **kwargs):
-    """Print debug info to stdout if the session was created with the silent argument set to `False`
+    """
+    Call the `Logger.P` method if the session was created with the silent argument set to `False`.
+    If using the default Logger, this call will print debug info to stdout if `silent` is set to `False`.
+
+    Parameters
+    ----------
+    *args :
+
+    msg : obj
+        The message to pass to the `Logger.P` method. If using the default Logger, this
+        will be the message displayed at the stdout.
+
+    **kwargs :
+
+
+    Returns
+    -------
+
     """
     if not self.silent:
       self.log.P(*args, **kwargs)
     return
 
   def connect(self) -> None:
-    """Connect to the communication server using the credentials provided when creating this instance
+    """
+    Connect to the communication server using the credentials provided when creating this instance.
     """
     raise NotImplementedError
 
   def create_pipeline(self, *, e2id, name, data_source, config={}, plugins=[], on_data, on_notification=None, max_wait_time=0, **kwargs) -> Pipeline:
-    """Create a new pipeline on a box. A pipeline is the equivalent of the "config file" used by the Hyperfy dev team internaly.
-    A pipeline allows one to define what is the data acquisition type and source, and what plugins will run on that data.
-    `max_wait_time` controls how much to wait for the given node to be indexed by the session before creating the pipeline.
-    A node is indexed if it sent any heartbeats since the session connected.
-
-    Args:
-        e2id (str): Name of the AiXp node.
-        name (str): Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
-        data_source (str): Name of the DataCaptureThread plugin to be used for acquisition.
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this pipeline. As arguments, it has a reference to this Pipeline object, the name of the Signature and the name of the Instance that sent the message, along with the payload itself.
-        plugins (list): List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box. Defaults to []. Should be left [], and instances should be created with the api.
-        config (dict, optional): Data acquisition specific parameters. Defaults to {}.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this pipeline. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-        max_wait_time(float, optional): Max wait time before creating the pipeline. Defaults to 0.
-    Returns:
-        Pipeline: a Pipeline object which can be used to control plugin instances.
+    """
+    Create a new pipeline on a node. A pipeline is the equivalent of the "config file" used by the Hyperfy dev team internaly.
+
+    A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
+
+    A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
+    processing units, usually named `Plugins`. 
+
+    An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
+
+    As such, one will work with `Instances`, by reffering to them with the unique identifier (Pipeline, Plugin, Instance).
+
+    In the documentation, the following reffer to the same thing:
+      `Pipeline` == `Stream`
+
+      `Plugin` == `Signature`
+
+    This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an AiXpand node is online or not.
+    If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
+    creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
+
+    Parameters
+    ----------
+    e2id : str
+        Name of the AiXpand node that will handle this pipeline.  
+    name : str
+        Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
+    data_source : str
+        This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from any plugin instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+    plugins : list
+        List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box. Defaults to []. Should be left [], and instances should be created with the api.
+    config : dict, optional
+        This is the dictionary that contains the configuration of the acquisition source, by default {}
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from any plugin instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+        Defaults to None.
+    max_wait_time : int, optional
+        The maximum time to busy-wait, allowing the Session object to listen to node heartbeats
+        and to check if the desired node is online in the network, by default 0.
+    **kwargs :
+        The user can provide the configuration of the acquisition source directly as kwargs.
+
+    Returns
+    -------
+    Pipeline
+        A `Pipeline` object.
+
     """
     _start = tm()
     found = False
     while (tm() - _start) < max_wait_time:
       avail_workers = self.get_active_nodes()
       if e2id in avail_workers:
         found = True
@@ -294,67 +399,127 @@
         silent=self.silent,
         **kwargs
     )
     self.own_pipelines.append(pipeline)
     return pipeline
 
   def close_own_pipelines(self):
+    """
+    Close all pipelines that were created by or attached to this session.
+    """
     # iterate through all CREATED pipelines from this session and close them
     for pipeline in self.own_pipelines:
       pipeline.close()
     return
 
   def close(self, close_pipelines=False, **kwargs):
-    """Close the session, releasing all resources and closing all threads
     """
-    # TODO: Stefan: here we need to change from abstract to concrete - all pipelines MUST
-    #       be deallocated. The child re-implementations must call self().__close__ beforehand
+    Close the session, releasing all resources and closing all threads
+
+    Parameters
+    ----------
+    close_pipelines : bool, optional
+        close all the pipelines created by or attached to this session (basically calling `.close_own_pipelines()` for you), by default False
+    """
     if close_pipelines:
       self.close_own_pipelines()
     return
 
   def get_active_nodes(self):
-    """Get the list of all AiXp nodes that sent a message since this session was created, and that are considered online
+    """
+    Get the list of all AiXp nodes that sent a message since this session was created, and that are considered online
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    list
+        List of names of all the AiXp nodes that are considered online
 
-    Returns:
-        list: List of names of all the AiXp nodes that are considered online
     """
     return list(self._online_boxes.keys())
 
   def get_active_pipelines(self, e2id):
-    """Get a dictionary with all the pipelines that are active on this AiXp node
+    """
+    Get a dictionary with all the pipelines that are active on this AiXp node
+
+    Parameters
+    ----------
+    e2id : str
+        name of the AiXp node
 
-    Args:
-        e2id (str): name of the AiXp node
+    Returns
+    -------
+    dict
+        The key is the name of the pipeline, and the value is the entire config dictionary of that pipeline.
 
-    Returns:
-        dict: The key is the name of the pipeline, and the value is the entire config dictionary of that pipeline.
     """
     return self._online_boxes.get(e2id, None)
 
   def attach_to_pipeline(self, e2id, pipeline_name, on_data, on_notification=None, max_wait_time=0, **kwargs) -> Pipeline:
-    """Create a Pipeline object and attach to an existing pipeline on a box.
-    Useful when one wants to treat an existing pipeline as one of his own, 
-    or when one wants to attach callbacks to various events (on_data, on_notification). 
-    `max_wait_time` controls how much to wait for the given node to be indexed by the session before attaching to the pipeline.
-    A node is indexed if it sent any heartbeats since the session connected.
-
-    Args:
-        e2id (str): Name of the AiXp node.
-        pipeline_name (str): Name of the pipeline
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this pipeline. As arguments, it has a reference to this Pipeline object, the name of the Signature and the name of the Instance that sent the message, along with the payload itself.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this pipeline. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-        max_wait_time(float, optional): Max wait time before creating the pipeline. Defaults to 0.
+    """
+    Create a Pipeline object and attach to an existing pipeline on an AiXpand node.
+    Useful when one wants to treat an existing pipeline as one of his own,
+    or when one wants to attach callbacks to various events (on_data, on_notification).
 
-    Raises:
-        Exception: The session does not consider the node online or the pipeline does not exist on that box.
+    A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
-    Returns:
-        Pipeline: a Pipeline object which can be used to control plugin instances.
+    A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
+    processing units, usually named `Plugins`. 
+
+    An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
+
+    As such, one will work with `Instances`, by reffering to them with the unique identifier (Pipeline, Plugin, Instance).
+
+    In the documentation, the following reffer to the same thing:
+      `Pipeline` == `Stream`
+
+      `Plugin` == `Signature`
+
+    This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an AiXpand node is online or not.
+    If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
+    creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
+
+
+    Parameters
+    ----------
+    e2id : str
+        Name of the AiXpand node that handles this pipeline.  
+    pipeline_name : str
+        Name of the existing pipeline.
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from any plugin instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from any plugin instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+    max_wait_time : int, optional
+        The maximum time to busy-wait, allowing the Session object to listen to node heartbeats
+        and to check if the desired node is online in the network, by default 0.
+    **kwargs :
+        The user can provide the configuration of the acquisition source directly as kwargs.
+
+    Returns
+    -------
+    Pipeline
+        A `Pipeline` object.
+
+    Raises
+    ------
+    Exception
+        Node does not exist (it is considered offline because the session did not receive any heartbeat)
+    Exception
+        Node does not host the desired pipeline 
     """
+
     _start = tm()
     while (tm() - _start) < max_wait_time:
       avail_workers = self.get_active_nodes()
       if e2id in avail_workers:
         break
       sleep(0.1)
 
@@ -373,29 +538,22 @@
     """
     This simple method will lock the main thread in a loop.
     This method can call `self.connect()`.
     This method can close the session and can close all pipelines when doing so.
 
     Parameters
     ----------
-    wait: bool, float
-      If `True`, will wait forever.
-      If `False`, will not wait at all
-      If type `float`, will wait said amount of seconds
-
+    wait : bool, float
+        If `True`, will wait forever.
+        If `False`, will not wait at all
+        If type `float`, will wait said amount of seconds (Default value = True)
     close_session : bool, optional
-      If `True` will close the session when the loop is exited. The default is True.
-
+        If `True` will close the session when the loop is exited. The default is True.
     close_pipelines : bool, optional
-      If `True` will close all pipelines initiated by this session when the loop is exited. The default is True.
-
-    Returns
-    -------
-    None.
-
+        If `True` will close all pipelines initiated by this session when the loop is exited. The default is True.
     """
     if not self.connected:
       self.connect()
 
     _start_timer = tm()
     try:
       while (isinstance(wait, bool) and wait) or (tm() - _start_timer) < wait:
```

### Comparing `pye2-0.3.3/PyE2/base/logger.py` & `pye2-0.3.4/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/base/pipeline.py` & `pye2-0.3.4/PyE2/base/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,85 @@
 from ..utils.code_exec import code_to_base64
 
 
 WAIT_FOR_WORKER = 15
 
 
 class Pipeline(object):
+  """
+  A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
+
+  A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
+  processing units, usually named `Plugins`. 
+
+  An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
+
+  As such, one will work with `Instances`, by reffering to them with the unique identifier (Pipeline, Plugin, Instance).
+
+  In the documentation, the following reffer to the same thing:
+    `Pipeline` == `Stream`
+
+    `Plugin` == `Signature`
+  """
+
   def __init__(self, session, log, *, e2id, name, data_source, config={}, plugins, on_data, silent=True, on_notification=None, **kwargs) -> None:
+    """
+    A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
+
+    A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
+    processing units, usually named `Plugins`. 
+
+    An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
+
+    As such, one will work with `Instances`, by reffering to them with the unique identifier (Pipeline, Plugin, Instance).
+
+    In the documentation, the following reffer to the same thing:
+      `Pipeline` == `Stream`
+
+      `Plugin` == `Signature`
+
+    Parameters
+    ----------
+    session : Session
+        The Session object which owns this pipeline. A pipeline must be attached to a Session beacause that is the only
+        way the `on_X` callbacks are called
+    log : Logger
+        A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
+        In the future, the documentation for the Logger base class will be available and developers will be able to use
+        custom-made Loggers. 
+    e2id : str
+        Name of the AiXpand node that will handle this pipeline.  
+    name : str
+        The name of this pipeline.
+    data_source : str
+        This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
+    plugins : List | None, optional
+        This is the list with manually configured business plugins that will be in the pipeline at creation time.
+        We recommend to leave this as `[]` or as `None` and use the API to create plugin instances. 
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from any plugin instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+    config : dict, optional
+        This is the dictionary that contains the configuration of the acquisition source, by default {}
+    silent : bool, optional
+        This flag will disable debug logs, set to 'False` for a more verbose log, by default True
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from this instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+        This callback acts as a default payload processor and will be called even if for a given instance
+        the user has defined a specific callback.
+        Defaults to None.
+    create_pipeline : bool
+        This is used internally to allow the user to create or attach to a pipeline, and then use the same
+        objects in the same way, by default True
+    **kwargs : dict
+        The user can provide the configuration of the acquisition source directly as kwargs.
+    """
     self.log = log
     self.session = session
     self.e2id = e2id
     self.name = name
     self.data_source = data_source
     self.config = config
     self.plugins = plugins
@@ -82,29 +152,44 @@
     self.session.payload_pipeline_callbacks.append((self, callback))
 
   def _add_notification_pipeline_callback_to_session(self, callback):
     self.session.notification_pipeline_callbacks.append((self, callback))
 
   # TODO: maybe wait for a confirmation?
   def start_plugin_instance(self, *, signature, instance_id, params, on_data, on_notification=None, **kwargs):
-    """Create a new instance of a desired plugin, with a given configuration. This instance is attached to this pipeline, 
+    """
+    Create a new instance of a desired plugin, with a given configuration. This instance is attached to this pipeline, 
     meaning it processes data from this pipelines data source. Parameters can be passed either in the params dict, or as kwargs.
 
-    Args:
-        signature (str): name of the plugin signature. This is the name of the desired overall functionality.
-        instance_id (str): name of the instance. There can be multiple instances of the same plugin, mostly with different prameters
-        params (dict): parameters used to customize the functionality. One can change the AI engine used for object detection, or finetune alerter parameters to better fit a camera located in a low light environment.
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-
-    Raises:
-        Exception: Plugin instance already exists. 
-
-    Returns:
-        str: An identifier for this instance, useful for stopping an instance.
+    Parameters
+    ----------
+    signature : str
+        The name of the plugin signature. This is the name of the desired overall functionality.
+    instance_id : str
+        The name of the instance. There can be multiple instances of the same plugin, mostly with different prameters
+    params : dict
+        parameters used to customize the functionality. One can change the AI engine used for object detection, 
+        or finetune alerter parameters to better fit a camera located in a low light environment.
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from this instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from this instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itsel. 
+        Defaults to None
+
+    Returns
+    -------
+    str
+        An identifier for this instance, useful for stopping an instance.
+
+    Raises
+    ------
+    Exception
+        Plugin instance already exists. 
     """
     plugins = self.payload['PLUGINS']
     found_plugin_signature = False
     to_update_plugin = {
         'INSTANCES': [],
         'SIGNATURE': signature
     }
@@ -145,22 +230,28 @@
           signature, instance_id, on_notification)
     self.P("Starting plugin {}:{}".format(
         signature, instance_id))
     self.D("with params {}".format(params))
     return "##".join([self.e2id, self.name, signature, instance_id])
 
   def stop_plugin_instance(self, signature, instance_id=None, /):
-    """Stop a plugin instance from this pipeline. The function can accept either the signature and the instance_id of the desired instance,
+    """
+    Stop a plugin instance from this pipeline. The function can accept either the signature and the instance_id of the desired instance,
     or the identifier returned from `start_plugin_instance` or `start_custom_instance` or `attach_to_instance` or `attach_to_custom_instance`.
 
-    Args:
-        signature (str): Signature of a plugin (name of the plugin type) or instance identifier
-        instance_id (str, optional): Name of the instance. Defaults to None.
+
+    Parameters
+    ----------
+    signature : str
+        Signature of a plugin (name of the plugin type) or instance identifier
+    instance_id : str, optional
+        Name of the instance, by default None
 
     """
+
     if instance_id is None:
       try:
         e2id, pipeline_name, signature, instance_id = tuple(
             signature.split('##'))
       except:
         raise ("Unknown format of instance_id. Please provide the return value of a 'start_plugin_instance' call")
 
@@ -199,31 +290,50 @@
         stream_config=self.payload
     )
     self.session.remove_instance_callback(self, signature, instance_id)
 
     return
 
   def start_custom_plugin(self, *, instance_id, plain_code: str = None, plain_code_path: str = None, params, on_data, on_notification=None, **kwargs):
-    """Create a new custom execution instance, with a given configuration. This instance is attached to this pipeline, 
-    meaning it processes data from this pipelines data source. The code used for the custom instance must be provided either as a string, or as a path to a file. Parameters can be passed either in the params dict, or as kwargs.
+    """
+    Create a new custom execution instance, with a given configuration. This instance is attached to this pipeline, 
+    meaning it processes data from this pipelines data source. The code used for the custom instance must be provided
+    either as a string, or as a path to a file. Parameters can be passed either in the params dict, or as kwargs.
     The custom plugin instance will run periodically. If one desires to execute a custom code only once, use `wait_exec`.
 
-    Args:
-        instance_id (str): name of the instance. There can be multiple instances of the same plugin, mostly with different prameters
-        params (dict): parameters used to customize the functionality.
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
-        plain_code (str, optional): A string containing the entire code that is to be executed remotely on an AiXp node. Defaults to None.
-        plain_code_path (str, optional): A string containing the path to the code that is to be executed remotely on an AiXp node. Defaults to None.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-
-    Raises:
-        Exception: The code was not provided.
-
-    Returns:
-        str: An identifier for this instance, useful for stopping an instance.
+    Parameters
+    ----------
+    `instance_id` : str
+        The name of the instance. There can be multiple instances of the same plugin, mostly with different prameters
+    `plain_code` : str, optional
+        A string containing the entire code that is to be executed remotely on an AiXp node. Defaults to None.
+    `plain_code_path` : str, optional
+        A string containing the path to the code that is to be executed remotely on an AiXp node. Defaults to None.
+    `params` : dict
+        parameters used to customize the functionality. One can change the AI engine used for object detection, 
+        or finetune alerter parameters to better fit a camera located in a low light environment.
+    `on_data` : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from this instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+    `on_notification` : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from this instance. 
+        As arguments, it has a reference to this Pipeline object, along with the payload itsel. 
+        Defaults to None
+
+    Returns
+    -------
+    str
+        An identifier for this instance, useful for stopping an instance.
+
+    Raises
+    ------
+    Exception
+        The code was not provided.
+    Exception
+        Plugin instance already exists. 
     """
 
     def custom_exec_on_data(self, data):
       exec_data = None
       if "SB_IMPLEMENTATION" in data or "EE_FORMATTER" in data:
         exec_data = data.get('EXEC_RESULT', data.get('EXEC_INFO'))
         exec_error = data.get('EXEC_ERRORS', 'no keyword error')
@@ -264,39 +374,54 @@
         },
         on_data=custom_exec_on_data,
         on_notification=on_notification,
         **kwargs
     )
 
   def stop_custom_instance(self, instance_id):
-    """Stop a custom execution instance from this pipeline.
+    """
+    Stop a custom execution instance from this pipeline.
 
-    Args:
-        instance_id (str, optional): Name of the custom instance. Defaults to None.
+    Parameters
+    ----------
+    instance_id : str
+        Name of the custom instance.
 
     """
     self.stop_plugin_instance('CUSTOM_EXEC_01', instance_id)
 
   def wait_exec(self, *, plain_code: str = None, plain_code_path: str = None, params={}):
-    """Create a new REST-like custom execution instance, with a given configuration. This instance is attached to this pipeline, 
+    """
+    Create a new REST-like custom execution instance, with a given configuration. This instance is attached to this pipeline, 
     meaning it processes data from this pipelines data source. The code used for the custom instance must be provided either as a string, or as a path to a file. Parameters can be passed either in the params dict, or as kwargs.
     The REST-like custom plugin instance will execute only once. If one desires to execute a custom code periodically, use `start_custom_plugin`.
 
-    Args:
-        params (dict, optional): parameters used to customize the functionality. Defaults to {}.
-        plain_code (str, optional): A string containing the entire code that is to be executed remotely on an AiXp node. Defaults to None.
-        plain_code_path (str, optional): A string containing the path to the code that is to be executed remotely on an AiXp node. Defaults to None.
-
-    Raises:
-        Exception: The code was not provided.
-
-    Returns:
-        Tuple[Any, Any]: a tuple containing the result of the execution and the error, if any. 
+    Parameters
+    ----------
+    plain_code : str, optional
+        A string containing the entire code that is to be executed remotely on an AiXp node, by default None
+    plain_code_path : str, optional
+        A string containing the path to the code that is to be executed remotely on an AiXp node, by default None
+    params : dict, optional
+        parameters used to customize the functionality, by default {}
+
+    Returns
+    -------
+    Tuple[Any, Any]
+        a tuple containing the result of the execution and the error, if any. 
         If the execution completed succesfully, the `error` is None, and the `result` is the returned value of the custom code.
+
+    Raises
+    ------
+    Exception
+        The code was not provided.
+    Exception
+        Plugin instance already exists. 
     """
+
     if plain_code is None and plain_code_path is None:
       raise Exception(
           "Need to specify at least one of the following: plain_code, plain_code_path")
 
     if plain_code is None:
       with open(plain_code_path, "r") as fd:
         plain_code = "".join(fd.readlines())
@@ -341,50 +466,66 @@
 
     # stop the stream
     self.stop_plugin_instance('REST_CUSTOM_EXEC_01', instance_id)
 
     return result, error
 
   def close(self):
-    """Close the pipeline, stopping all the instances associated with it.
+    """
+    Close the pipeline, stopping all the instances associated with it.
     """
     # remove callbacks
     self.session.send_command_delete_pipeline(self.e2id, self.name)
     self.session.remove_pipeline_callbacks(self)
     return
 
   def P(self, *args, **kwargs):
-    """Print info to stdout.
+    """
+    Print info to stdout.
     """
     return self.log.P(*args, **kwargs)
 
   def D(self, *args, **kwargs):
-    """Print debug info to stdout if the session was created with the silent argument set to `False`. 
+    """
+    Print debug info to stdout if the session was created with the silent argument set to `False`. 
     The silent argument is passed to the Pipeline object when creating it with `create_pipeline` or `attach_to_pipeline`.
     """
     if not self.silent:
       return self.log.P(*args, **kwargs)
 
   def attach_to_instance(self, signature, instance_id, on_data, on_notification=None):
-    """Attach to an existing instance on this pipeline. 
+    """
+    Attach to an existing instance on this pipeline. 
     This method is useful when one wishes to attach an 
     `on_data` and `on_notification` callbacks to said instance.
 
-    Args:
-        signature (str): name of the plugin signature.
-        instance_id (str): name of the instance.
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-
-    Raises:
-        Exception: the pipeline does not contain plugins with a given signature or it does not contain the desired instance.
-
-    Returns:
-        str: An identifier for this instance, useful for stopping an instance.
+    Parameters
+    ----------
+    signature : str
+        name of the plugin signature.
+    instance_id : str
+        name of the instance.
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
+
+    Returns
+    -------
+    str
+        An identifier for this instance, useful for stopping an instance.
+
+    Raises
+    ------
+    Exception
+        the pipeline does not contain plugins with a given signature.
+    Exception
+        The pipeline does not contain the desired instance.
     """
+
     plugins = self.payload['PLUGINS']
     found_plugin_signature = False
 
     for plugin in plugins:
       if plugin['SIGNATURE'] == signature:
         found_plugin_signature = True
         break
@@ -400,28 +541,39 @@
           self._add_notification_instance_callback_to_session(
               signature, instance_id, on_notification)
         return "##".join([self.e2id, self.name, signature, instance_id])
 
     raise Exception("Unable to attach to instance. Instance does not exist")
 
   def attach_to_custom_instance(self, instance_id, on_data, on_notification=None):
-    """Attach to an existing custom execution instance on this pipeline. 
+    """
+    Attach to an existing custom execution instance on this pipeline. 
     This method is useful when one wishes to attach an 
     `on_data` and `on_notification` callbacks to said instance.
 
-    Args:
-        instance_id (str): name of the instance.
-        on_data (Callable[[Pipeline, str, str, dict], None]): Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
-        on_notification (Callable[[Pipeline, dict], None], optional): Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
-
-    Raises:
-        Exception: the pipeline does not contain plugins with a given signature or it does not contain the desired instance.
-
-    Returns:
-        str: An identifier for this instance, useful for stopping an instance.
+    Parameters
+    ----------
+    instance_id : str
+        name of the instance.
+    on_data : Callable[[Pipeline, str, str, dict], None]
+        Callback that handles messages received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself.
+    on_notification : Callable[[Pipeline, dict], None], optional
+        Callback that handles notifications received from this instance. As arguments, it has a reference to this Pipeline object, along with the payload itself. Defaults to None.
+
+    Returns
+    -------
+    str
+        An identifier for this instance, useful for stopping an instance.
+
+    Raises
+    ------
+    Exception
+        the pipeline does not contain any custom plugin.
+    Exception
+        The pipeline does not contain the desired instance.
     """
 
     def custom_exec_on_data(self, data):
       exec_data = None
       if "SB_IMPLEMENTATION" in data or "EE_FORMATTER" in data:
         exec_data = data.get('EXEC_RESULT', data.get('EXEC_INFO'))
         exec_error = data.get('EXEC_ERRORS', 'no keyword error')
```

### Comparing `pye2-0.3.3/PyE2/base/payload/payload.py` & `pye2-0.3.4/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/comm/__init__.py` & `pye2-0.3.4/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/comm/amqp_wrapper.py` & `pye2-0.3.4/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/comm/mqtt_wrapper.py` & `pye2-0.3.4/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/__init__.py` & `pye2-0.3.4/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/base.py` & `pye2-0.3.4/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/comms.py` & `pye2-0.3.4/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/heartbeat.py` & `pye2-0.3.4/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/misc.py` & `pye2-0.3.4/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/const/payload.py` & `pye2-0.3.4/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/default/mqtt_session.py` & `pye2-0.3.4/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/__init__.py` & `pye2-0.3.4/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/consts.py` & `pye2-0.3.4/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.3.4/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/base/__init__.py` & `pye2-0.3.4/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.3.4/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/default/__init__.py` & `pye2-0.3.4/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.3.4/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/default/cavi2.py` & `pye2-0.3.4/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.3.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/utils/code.py` & `pye2-0.3.4/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/PyE2/utils/code_exec.py` & `pye2-0.3.4/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/xperimental/attach_example.py` & `pye2-0.3.4/xperimental/attach_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 @description:
 Created on Thu Jan 26 14:57:44 2023
 """
 
 import os
 from time import sleep, time
 
+from dotenv import load_dotenv
+
 from PyE2 import Payload, Pipeline, Session
 
+load_dotenv()
 print(os.environ['PYTHONPATH'].split(os.pathsep))
 
 boxes = {}
 
 
 def instance_on_data(pipeline, data: Payload):
   global boxes
@@ -49,18 +52,18 @@
 def pipeline_on_notification(pipeline, notification):
   pipeline.P(
       "Received specific notification for pipeline {}".format(pipeline.name))
   return
 
 
 dct_server = {
-    'host': "hostname",
-    'port': 88888,
-    'user': "username",
-    'pwd': "password"
+    'host': os.getenv('PYE2_HOSTNAME'),
+    'port': int(os.getenv('PYE2_PORT')),
+    'user': os.getenv('PYE2_USERNAME'),
+    'pwd': os.getenv('PYE2_PASSWORD')
 }
 
 e2id = 'e2id'
 sess = Session(**dct_server)
 sess.connect()
 
 listener_params = {k.upper(): v for k, v in dct_server.items()}
```

### Comparing `pye2-0.3.3/xperimental/ex1.py` & `pye2-0.3.4/xperimental/ex1.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 @copyright: Lummetry.AI
 @author: Lummetry.AI - AID
 @project: 
 @description:
 Created on Thu Jan 26 14:57:44 2023
 """
 
+import os
 from time import sleep
 
+from dotenv import load_dotenv
+
 from PyE2 import Payload, Session
 
+load_dotenv()
+
 
 def instance_on_data(pipeline, data: Payload):
   # this could refresh a UI
   pipeline.P('Receive specific message from PERIMETER_VIOLATION_02:inst01 (hardcoded)', color='m')
 
 
 def another_instance_on_data(pipeline, data: Payload):
@@ -54,18 +59,18 @@
 
 
 if __name__ == '__main__':
 
   e2id = 'e2id'
 
   dct_server = {
-      'host': "hostname",
-      'port': 88888,
-      'user': "username",
-      'pwd': "password"
+      'host': os.getenv('PYE2_HOSTNAME'),
+      'port': int(os.getenv('PYE2_PORT')),
+      'user': os.getenv('PYE2_USERNAME'),
+      'pwd': os.getenv('PYE2_PASSWORD')
   }
 
   sess = Session(**dct_server)
   sess.connect()
 
   pipeline = sess.create_pipeline(
       e2id=e2id,
```

### Comparing `pye2-0.3.3/xperimental/remote_exec.py` & `pye2-0.3.4/xperimental/remote_exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 @description:
 Created on Thu Jan 26 14:57:44 2023
 """
 
 import os
 from time import sleep, time
 
+from dotenv import load_dotenv
+
 from PyE2 import Payload, Pipeline, Session
 
+load_dotenv()
 print(os.environ['PYTHONPATH'].split(os.pathsep))
 
 boxes = {}
 
 custom_worker_code = """
 _result=None
 payload = plugin.dataapi_struct_data()
@@ -77,18 +80,18 @@
 def pipeline_on_notification(pipeline, notification):
   pipeline.P(
       "Received specific notification for pipeline {}".format(pipeline.name))
   return
 
 
 dct_server = {
-    'host': "hostname",
-    'port': 88888,
-    'user': "username",
-    'pwd': "password"
+    'host': os.getenv('PYE2_HOSTNAME'),
+    'port': int(os.getenv('PYE2_PORT')),
+    'user': os.getenv('PYE2_USERNAME'),
+    'pwd': os.getenv('PYE2_PASSWORD')
 }
 
 e2id = 'e2id'
 sess = Session(**dct_server)
 sess.connect()
 
 listener_params = {k.upper(): v for k, v in dct_server.items()}
```

### Comparing `pye2-0.3.3/xperimental/decentralized/dedist_example.py` & `pye2-0.3.4/xperimental/decentralized/dedist_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 
 import os
+
+from dotenv import load_dotenv
+
 from PyE2 import Session, code_to_base64
 
+load_dotenv()
+
 SERVER_CONFIG = {
-    'host': "hostname",
-    'port': 88888,
-    'user': "username",
-    'pwd': "password"
+    'host': os.getenv('PYE2_HOSTNAME'),
+    'port': int(os.getenv('PYE2_PORT')),
+    'user': os.getenv('PYE2_USERNAME'),
+    'pwd': os.getenv('PYE2_PASSWORD')
 }
 
 
 def instance_on_data(pipeline, data):
   print(data)
   return
```

### Comparing `pye2-0.3.3/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.3.4/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/.gitignore` & `pye2-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/LICENSE` & `pye2-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.3.3/README.md` & `pye2-0.3.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # PyE2 SDK
 
 This Python package enables low-code development and deployment of end-to-end AI cooperative application pipelines within the AiXpand Execution Engine processing nodes ecosystem. For further information please see "AiXpand - Decentralized ubiquitous computing MLOps execution engine".
 
-
 ## Installation
 
-
-
 ## Quick start "Hello world!"
 
 Below is a simple "Hello world!" style application that creates a session by connecting to a known communication broker, listens for processing nodes heartbeats and displays the basic compute capabilities of the discovered nodes such as CPU & RAM.
 
 ### Importing and configuration
 
-```
+```python
 from PyE2 import Session
 ```
 
 ### Preparing callbacks
 
-```
+```python
 def on_hb(session, data):
   print(data['EE_ID'], " has a ", data['CPU'])
   return
 ```
 
 ### Running a simple main loop
 
-```
+```python
 if __name__ == '__main__':
   sess = Session(
     host="hostname",
     port=88888,
     user="username",
     pwd="password",
     on_heartbeat=on_hb
@@ -42,84 +39,92 @@
 ## Advanced quick-start with decentralized distributed jobs
 
 For a more advanced quick-start we are going to create a execution pipeline on a target processing node that will request a specific number of workers in the network (including itself) to run a brute prime number search job.
 The initiator job itself will create the request for the required number of discovered worker peers then will listen for results. Finally after a given configurable amount of time will close its own execution pipeline as well as each worker pipeline.
 
 ### Worker code
 
-```
+The worker will randomly generate numbers and will check if they are prime. If it finds a prime number, it sets the `_result`
+variable.
+
+```python
 _result=None
 skip = False
 for _ in range(plugin.cfg_max_tries):
+  # generate up to `max_tries` numbers in this call
   num = plugin.np.random.randint(1, 10_000)
   for n in range(2,int(num**0.5)+1):
     if num % n == 0:
+      # the generated number is not a prime
       skip=True
       break
     # endif
   # endfor
   if not skip:
     _result=num
     break
   # endif
 # endfor
 ```
 
 ### Initiator node code
 
-```
+The initiator will search for available workers in the network and will send them the custom job, then will collect data for a time,
+after which will close the worker nodes and itself
+
+```python
 result=None
 if plugin.int_cache['run_first_time'] == 0:
   # this is the first run, consider this the setup
-  
+
   plugin.int_cache['run_first_time'] = 1
 
   worker_code = plugin.cfg_worker_code
   n_workers = plugin.cfg_n_workers
   # we use DeAPI `plugin.deapi_get_wokers` call to get the needed workers
   plugin.obj_cache['lst_workers'] = plugin.deapi_get_wokers(n_workers)
   plugin.obj_cache['dct_workers'] = {}
   plugin.obj_cache['dct_worker_progress'] = {}
   plugin.P(plugin.obj_cache['lst_workers'])
-  
+
   # for each worker we symetrically launch the same job
   for worker in plugin.obj_cache['lst_workers']:
     plugin.obj_cache['dct_worker_progress'][worker] = []
     pipeline_name = plugin.cmdapi_start_simple_custom_pipeline(
-      base64code=worker_code, 
+      base64code=worker_code,
       dest=worker,
       instance_config={
-        'MAX_TRIES': plugin.cfg_max_tries, 
+        'MAX_TRIES': plugin.cfg_max_tries,
       }
     )
-    plugin.obj_cache['dct_workers'][worker] = pipeline_name 
+    plugin.obj_cache['dct_workers'][worker] = pipeline_name
   # endfor
-  
+
   plugin.obj_cache["start_time"] = plugin.datetime.now()
   # endfor
 elif (plugin.datetime.now() - plugin.obj_cache["start_time"]).seconds > plugin.cfg_max_run_time:
-  # if the configured time has elapsed we stop all the worker pipelines 
+  # if the configured time has elapsed we stop all the worker pipelines
   # as well as stop this pipeline itself
-  
+
   for ee_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
     plugin.cmdapi_archive_pipeline(dest=ee_id, name=pipeline_name)
   # now archive own pipeline
   plugin.cmdapi_archive_pipeline()
   result = {
     'STATUS'  : 'DONE',
     'RESULTS' : plugin.obj_cache['dct_worker_progress']
   }
 else:
   # here are the operations we are running periodically
   payload = plugin.dataapi_struct_data() # we use the DataAPI to get upstream data
   if payload is not None:
-    
+
     ee_id = payload.get('EE_ID', payload.get('SB_ID'))
     pipeline_name = payload.get('STREAM_NAME')
-    
+
     if (ee_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
       # now we extract result from the result key of the payload JSON
       # this also can be configured to another name
       num = payload.get('EXEC_RESULT', payload.get('EXEC_INFO'))
       if num is not None:
         plugin.obj_cache['dct_worker_progress'][ee_id].append(num)
         result = {
@@ -128,76 +133,76 @@
         }
   # endif
 # endif
 ```
 
 ### The local code
 
-```
+```python
 
 from PyE2 import Session, code_to_base64
 
 SERVER_CONFIG = {
     'host': "****************",
-    'port': 31083,
+    'port': 8888,
     'user': "****************",
     'pwd': "****************"
 }
 
 
 def instance_on_data(pipeline, data):
   print(data)
   return
 
 
 def pipeline_on_data(pipeline, signature, instance, data):
   pass
 
 if __name__ == '__main__':
-  
+
   WORKER_CODE_PATH = 'xperimental/dedist_example_worker.py'
   INITIATOR_CODE_PATH = 'xperimental/dedist_example_initiator.py'
-  
+
   with open(WORKER_CODE_PATH, 'rt') as fh:
     worker_code = fh.read()
-    
+
   e2id = 'e2id' # provide a known EE id
   sess = Session(**SERVER_CONFIG, silent=True)
   sess.connect()
-  
+
   listener_params = {k.upper(): v for k, v in SERVER_CONFIG.items()}
   listener_params["PASS"] = listener_params["PWD"]
   listener_params["TOPIC"] = "lummetry/payloads"
-  
+
   pipeline = sess.create_pipeline(
       e2id=e2id,
       name='test_dist_jobs',
       # data_source='Void',
       # config={},
       data_source='IotQueueListener', # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
       plugins=None,
       on_data=pipeline_on_data,
   )
-  
-  
+
+
   pipeline.start_custom_plugin(
       instance_id='inst02',
       plain_code_path=INITIATOR_CODE_PATH,
       params={
         'MAX_TRIES': 10, # this will be used within plugin as `plugin.cfg_max_tries`
         'MAX_RUN_TIME': 60, # this will be used within plugin as `plugin.cfg_max_run_time`
         'N_WORKERS': 2, # this will be used within plugin as `plugin.cfg_n_workers`
-        
+
         # this will be used within plugin as `plugin.cfg_worker_code`
-        'WORKER_CODE': code_to_base64(worker_code) 
+        'WORKER_CODE': code_to_base64(worker_code)
         },
       on_data=instance_on_data,
       process_delay=0.2
   )
-  
+
   sess.wait_until_sigint(close_session=True, close_pipelines=True)
-  
+
 ```
```

### Comparing `pye2-0.3.3/pyproject.toml` & `pye2-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.3.3/PKG-INFO` & `pye2-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.3.3
+Version: 0.3.4
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,40 +12,37 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # PyE2 SDK
 
 This Python package enables low-code development and deployment of end-to-end AI cooperative application pipelines within the AiXpand Execution Engine processing nodes ecosystem. For further information please see "AiXpand - Decentralized ubiquitous computing MLOps execution engine".
 
-
 ## Installation
 
-
-
 ## Quick start "Hello world!"
 
 Below is a simple "Hello world!" style application that creates a session by connecting to a known communication broker, listens for processing nodes heartbeats and displays the basic compute capabilities of the discovered nodes such as CPU & RAM.
 
 ### Importing and configuration
 
-```
+```python
 from PyE2 import Session
 ```
 
 ### Preparing callbacks
 
-```
+```python
 def on_hb(session, data):
   print(data['EE_ID'], " has a ", data['CPU'])
   return
 ```
 
 ### Running a simple main loop
 
-```
+```python
 if __name__ == '__main__':
   sess = Session(
     host="hostname",
     port=88888,
     user="username",
     pwd="password",
     on_heartbeat=on_hb
@@ -56,84 +53,92 @@
 ## Advanced quick-start with decentralized distributed jobs
 
 For a more advanced quick-start we are going to create a execution pipeline on a target processing node that will request a specific number of workers in the network (including itself) to run a brute prime number search job.
 The initiator job itself will create the request for the required number of discovered worker peers then will listen for results. Finally after a given configurable amount of time will close its own execution pipeline as well as each worker pipeline.
 
 ### Worker code
 
-```
+The worker will randomly generate numbers and will check if they are prime. If it finds a prime number, it sets the `_result`
+variable.
+
+```python
 _result=None
 skip = False
 for _ in range(plugin.cfg_max_tries):
+  # generate up to `max_tries` numbers in this call
   num = plugin.np.random.randint(1, 10_000)
   for n in range(2,int(num**0.5)+1):
     if num % n == 0:
+      # the generated number is not a prime
       skip=True
       break
     # endif
   # endfor
   if not skip:
     _result=num
     break
   # endif
 # endfor
 ```
 
 ### Initiator node code
 
-```
+The initiator will search for available workers in the network and will send them the custom job, then will collect data for a time,
+after which will close the worker nodes and itself
+
+```python
 result=None
 if plugin.int_cache['run_first_time'] == 0:
   # this is the first run, consider this the setup
-  
+
   plugin.int_cache['run_first_time'] = 1
 
   worker_code = plugin.cfg_worker_code
   n_workers = plugin.cfg_n_workers
   # we use DeAPI `plugin.deapi_get_wokers` call to get the needed workers
   plugin.obj_cache['lst_workers'] = plugin.deapi_get_wokers(n_workers)
   plugin.obj_cache['dct_workers'] = {}
   plugin.obj_cache['dct_worker_progress'] = {}
   plugin.P(plugin.obj_cache['lst_workers'])
-  
+
   # for each worker we symetrically launch the same job
   for worker in plugin.obj_cache['lst_workers']:
     plugin.obj_cache['dct_worker_progress'][worker] = []
     pipeline_name = plugin.cmdapi_start_simple_custom_pipeline(
-      base64code=worker_code, 
+      base64code=worker_code,
       dest=worker,
       instance_config={
-        'MAX_TRIES': plugin.cfg_max_tries, 
+        'MAX_TRIES': plugin.cfg_max_tries,
       }
     )
-    plugin.obj_cache['dct_workers'][worker] = pipeline_name 
+    plugin.obj_cache['dct_workers'][worker] = pipeline_name
   # endfor
-  
+
   plugin.obj_cache["start_time"] = plugin.datetime.now()
   # endfor
 elif (plugin.datetime.now() - plugin.obj_cache["start_time"]).seconds > plugin.cfg_max_run_time:
-  # if the configured time has elapsed we stop all the worker pipelines 
+  # if the configured time has elapsed we stop all the worker pipelines
   # as well as stop this pipeline itself
-  
+
   for ee_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
     plugin.cmdapi_archive_pipeline(dest=ee_id, name=pipeline_name)
   # now archive own pipeline
   plugin.cmdapi_archive_pipeline()
   result = {
     'STATUS'  : 'DONE',
     'RESULTS' : plugin.obj_cache['dct_worker_progress']
   }
 else:
   # here are the operations we are running periodically
   payload = plugin.dataapi_struct_data() # we use the DataAPI to get upstream data
   if payload is not None:
-    
+
     ee_id = payload.get('EE_ID', payload.get('SB_ID'))
     pipeline_name = payload.get('STREAM_NAME')
-    
+
     if (ee_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
       # now we extract result from the result key of the payload JSON
       # this also can be configured to another name
       num = payload.get('EXEC_RESULT', payload.get('EXEC_INFO'))
       if num is not None:
         plugin.obj_cache['dct_worker_progress'][ee_id].append(num)
         result = {
@@ -142,76 +147,76 @@
         }
   # endif
 # endif
 ```
 
 ### The local code
 
-```
+```python
 
 from PyE2 import Session, code_to_base64
 
 SERVER_CONFIG = {
     'host': "****************",
-    'port': 31083,
+    'port': 8888,
     'user': "****************",
     'pwd': "****************"
 }
 
 
 def instance_on_data(pipeline, data):
   print(data)
   return
 
 
 def pipeline_on_data(pipeline, signature, instance, data):
   pass
 
 if __name__ == '__main__':
-  
+
   WORKER_CODE_PATH = 'xperimental/dedist_example_worker.py'
   INITIATOR_CODE_PATH = 'xperimental/dedist_example_initiator.py'
-  
+
   with open(WORKER_CODE_PATH, 'rt') as fh:
     worker_code = fh.read()
-    
+
   e2id = 'e2id' # provide a known EE id
   sess = Session(**SERVER_CONFIG, silent=True)
   sess.connect()
-  
+
   listener_params = {k.upper(): v for k, v in SERVER_CONFIG.items()}
   listener_params["PASS"] = listener_params["PWD"]
   listener_params["TOPIC"] = "lummetry/payloads"
-  
+
   pipeline = sess.create_pipeline(
       e2id=e2id,
       name='test_dist_jobs',
       # data_source='Void',
       # config={},
       data_source='IotQueueListener', # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
       plugins=None,
       on_data=pipeline_on_data,
   )
-  
-  
+
+
   pipeline.start_custom_plugin(
       instance_id='inst02',
       plain_code_path=INITIATOR_CODE_PATH,
       params={
         'MAX_TRIES': 10, # this will be used within plugin as `plugin.cfg_max_tries`
         'MAX_RUN_TIME': 60, # this will be used within plugin as `plugin.cfg_max_run_time`
         'N_WORKERS': 2, # this will be used within plugin as `plugin.cfg_n_workers`
-        
+
         # this will be used within plugin as `plugin.cfg_worker_code`
-        'WORKER_CODE': code_to_base64(worker_code) 
+        'WORKER_CODE': code_to_base64(worker_code)
         },
       on_data=instance_on_data,
       process_delay=0.2
   )
-  
+
   sess.wait_until_sigint(close_session=True, close_pipelines=True)
-  
+
 ```
```

