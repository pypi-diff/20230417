# Comparing `tmp/chatgpt_prompt_wrapper-0.0.8.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.8.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.9.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.8.tar` & `chatgpt_prompt_wrapper-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.8/LICENSE
--rw-r--r--   0        0        0    11989 2023-04-11 03:18:50.790208 chatgpt_prompt_wrapper-0.0.8/README.md
--rw-r--r--   0        0        0     2704 2023-04-11 03:19:56.727892 chatgpt_prompt_wrapper-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3654 2023-04-11 02:53:38.594014 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6673 2023-04-11 03:12:12.225520 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7760 2023-04-11 03:10:48.348304 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     7127 2023-04-11 03:02:08.687752 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0    13379 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-10 15:06:55.587443 chatgpt_prompt_wrapper-0.0.9/LICENSE
+-rw-r--r--   0        0        0    13238 2023-04-17 13:39:14.306855 chatgpt_prompt_wrapper-0.0.9/README.md
+-rw-r--r--   0        0        0     2704 2023-04-17 13:32:37.176854 chatgpt_prompt_wrapper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3654 2023-04-12 06:22:26.340319 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      173 2023-04-17 13:30:21.056854 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2414 2023-04-15 17:20:10.900493 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     4698 2023-04-17 00:32:52.873006 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7803 2023-04-17 13:31:10.596855 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     6724 2023-04-17 13:39:06.416855 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/discuss.py
+-rw-r--r--   0        0        0     2638 2023-04-17 13:37:57.336855 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/stream.py
+-rw-r--r--   0        0        0     7538 2023-04-17 13:39:06.426855 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      966 2023-04-17 13:30:21.056854 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0    14628 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.9/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/LICENSE` & `chatgpt_prompt_wrapper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/README.md` & `chatgpt_prompt_wrapper-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 [![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage)
 
 Python CLI implementation for [ChatGPT](https://openai.com/blog/chatgpt).
 
 ## Requirements
 
 - Python 3.9, 3.10, 3.11
-- Poetry (For development)
 
 ## Installation
 
+By Homebrew:
+
+```
+$ brew install rcmdnk/rcmdnkpac/chatgpt-prompt-wrapper
+```
+
+By pip:
+
 ```
-$ pip install chatgpt-prompt-wrapper
+$ pip3 install chatgpt-prompt-wrapper
 ```
 
 ## Preparation
 
 To get an OpenAI API key, go to [Account API Keys - OpenAI API](https://platform.openai.com/account/api-keys).
 
 Set it as the environment variable `OPENAI_API_KEY`.
@@ -63,54 +70,74 @@
   --no_multiline        Use single line input for chat command.
   --vi                  Use vi mode at chat.
   --emacs               Use emacs mode at chat.
   --show_cost           Show cost used.
 ```
 
 ```
+
 $ cg commands
 Available subcommands:
   Reserved commands:
     ask       : Ask w/o predefined prompt.
     chat      : Start chat w/o predefined prompt.
+    discuss   : Start a discussion between GPTs. Give a them as a message.
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Ask, Chat
 
 `ask` and `chat` are reserved commands for running simple interaction without a predefined prompt.
 
+- `ask`
+
 `cg ask <message>` returns the answer from ChatGPT for `message`.
 
+- `chat`
+
 `cg chat` starts a chat.
 
 :memo: In `chat` mode, all messages in the past, including answers from
 ChatGPT, will be sent each time you send a new message.
 
 The oldest message will be dropped when the total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the tokens limit (`tokens_limit` or the number of max tokens (-1) for the used model).
 
 It means you will send almost the max length after a long conversation.
 Please keep the cost in mind. You may want to set `tokens_limit`.
 
+### Discuss
+
+`discuss` is another reserved command which start a discussion between two ChatGPTs.
+
+Two GPTs are ask to perform as:
+
+- Please engage in the discussion as a supporter.
+- Please engage in the discussion as a opponent.
+
+You input message will be a message and they start a discussion.
+
+Please push `Enter` to proceed a duscussion and `Ctrl-C` to quit a discussion.
+
 ### Configuration file
 
 You can define your command in the configuration files.
 
-A command can be in either `ask` mode or `chat` mode.
+A command can be in either `ask` mode, `chat` mode or \`discuss mode.
 
 - `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
 - `chat` mode: Start a chat with a predefined prompt if defined:
   - `chat` mode can be in either `multiline` mode or single (`no_multiline`) mode.
+- `discuss` mode: Start a discussion between two different ChatGPTs.
 
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
@@ -138,15 +165,17 @@
 - `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - Table of `alias`: Dictionary of role aliases. The default alias is: '`user' = 'User'`, `'system' = 'System'`, `'assistant' = 'Assistant'`.
-- List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
+- List of `messages`: Dictionary of message, which must have `role` and `content` (message text).
+  - For `ask`, `chat` modes, `role` must be one of `system`, `user` and `assistant`
+  - For `discuss` mode, three roles, `theme`, `gpt1` and `gpt2` are needed.
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
@@ -200,14 +229,32 @@
 
 [enjoy_chat]
 description = "Chat example with a predefined prompt."
 chat = true
 [[chat.messages]]
 role = "user"
 content = "Let's enjoy a chat."
+
+
+[dd]
+discuss = true
+
+[dd.names]
+gpt1 = "pros"
+gpt2 = "cons"
+
+[[dd.messages]]
+role = "theme"
+content = "Discuss whether or not to actively adopt ChatGPT in the education field. Please provide one-sentence responses."
+[[dd.messages]]
+role = "gpt1"
+content = "Please speak from the standpoint that you should actively adopt ChatGPT in the field of education."
+[[dd.messages]]
+role = "gpt2"
+content = "Please speak from the standpoint that you should not actively adopt ChatGPT in the field of education."
 ```
 
 These messages will be sent as an prompt before your input message.
 
 You can give full questions and use `cg` w/o input messages like a first example `test` command.
 
 Command examples:
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.8"
+version = "0.0.9"
 description = "CLI tool to wrap ChatGPT Python API."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/discuss.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,43 @@
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Generator, cast
 
-from prompt_toolkit import prompt
-from prompt_toolkit.formatted_text import HTML
-from prompt_toolkit.key_binding import KeyBindings
-from prompt_toolkit.key_binding.bindings.named_commands import accept_line
-from prompt_toolkit.key_binding.key_processor import KeyPressEvent
-from prompt_toolkit.styles import Style
-
-from .chatgpt import ChatGPT, Messages
+from ..chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
+from .chatgpt import Messages
+from .stream import Stream
 
 
 @dataclass
-class Chat(ChatGPT):
-    """Chat class for interacting with OpenAI's API.
+class Discuss(Stream):
+    """Discussion between ChatGPTs.
 
     Parameters
     ----------
-    multiline : bool
-        Whether to use multiline prompt.
-    vi: bool
-        If true, use the vi keybindings at input prompt (default is emacs key bindings).
-    chat_exit_cmd: list[str]
-        The command to exit the chat.
+    colors: dict[str, str]
+        The colors to use for the different roles.
+    names: dict[str, str]
+        The names to use for the different roles.
     """
 
-    multiline: bool = True
-    vi: bool = False
-    chat_exit_cmd: list[str] = field(
-        default_factory=lambda: ["bye", "bye!", "exit", "quit"]
+    colors: dict[str, str] = field(
+        default_factory=lambda: {
+            "gpt1": "blue",
+            "gpt2": "purple",
+        }
+    )
+    names: dict[str, str] = field(
+        default_factory=lambda: {
+            "gpt1": "gpt1",
+            "gpt2": "gpt2",
+        }
     )
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        self.make_prompt()
-
-    def make_prompt(self) -> None:
-        if self.multiline:
-            toolbar_text = f"Send text: <b>[Meta+Enter]</b>, <b>[Esc]</b><b>[Enter]</b>. Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>, "
-        else:
-            toolbar_text = (
-                f"Exit chat: <b>[Ctrl-C]</b>, <b>{self.chat_exit_cmd[0]}</b>,"
-            )
-        if self.vi:
-            toolbar_text += "<b>Vi mode</b>."
-        else:
-            toolbar_text += "<b>emacs mode</b>."
-        toolbar_view = HTML(toolbar_text)
-
-        def bottom_toolbar() -> HTML:
-            return toolbar_view
-
-        def prompt_continuation(
-            width: int, line_number: int, is_soft_wrap: bool
-        ) -> str:
-            return ""
-
-        style_dict = {"": ""}  # Text (normal color)
-        for k, v in self.colors.items():
-            if v in self.ansi_colors:
-                style_dict[k] = f"ansi{v} bold"
-        style = Style.from_dict(style_dict)
-
-        bindings = KeyBindings()
-
-        @bindings.add("c-c")
-        def _(event: KeyPressEvent) -> None:
-            self.finish_chat = True
-            accept_line(event)
-
-        self.prompt_params = {
-            "style": style,
-            "multiline": self.multiline,
-            "prompt_continuation": prompt_continuation,
-            "bottom_toolbar": bottom_toolbar,
-            "key_bindings": bindings,
-            "vi_mode": self.vi,
-        }
 
     def set_no_line_break_log(self) -> None:
         self.default_terminators = [
             (h, h.terminator)
             for h in self.log.handlers
             if isinstance(h, logging.StreamHandler)
         ]
@@ -95,96 +51,138 @@
             handler.terminator = ""
 
     def reset_no_line_break_log(self) -> None:
         for handler, default_terminator in self.default_terminators:
             handler.terminator = default_terminator
         del self.default_terminators
 
-    def show_stream(
-        self, response: Generator[dict[str, Any], None, None], max_size: int
-    ) -> dict[str, str]:
-        message = {"role": "", "content": ""}
-        for chunk in response:
-            delta = chunk["choices"][0]["delta"]
-            if "role" in delta:
-                self.log.info(
-                    self.get_output(
-                        {"role": delta["role"], "content": ""},
-                        max_size,
-                    )
-                )
-                message["role"] = delta["role"]
-            if "content" in delta:
-                self.log.info(delta["content"])
-                message["content"] += delta["content"]
-            finish_reason = chunk["choices"][0]["finish_reason"]
-            if finish_reason == "length":
-                self.log.warning(
-                    "The reply was truncated due to the tokens limit.\n"
-                )
-            elif finish_reason == "content_filter":
-                self.log.warning(
-                    "The reply was omitted due to the content filters.\n"
-                )
-        self.log.info("\n")
-        return message
-
-    def run(self, messages: Messages) -> float:
-        messages = self.fix_messages(messages)
-        tokens = [
-            self.num_tokens_from_message(message) for message in messages
+    def prepare_messages(
+        self, messages: Messages
+    ) -> tuple[Messages, Messages, list[int], list[int]]:
+        theme = {}
+        gpt1 = {
+            "role": "system",
+            "content": "Please engage in the discussion as a supporter.",
+        }
+        gpt2 = {
+            "role": "system",
+            "content": "Please engage in the discussion as a opponent.",
+        }
+        for message in messages:
+            if message["role"] == "theme":
+                theme = message
+                theme["role"] = "system"
+            elif message["role"] == "gpt1":
+                gpt1 = message
+                gpt1["role"] = "system"
+            elif message["role"] == "gpt2":
+                gpt2 = message
+                gpt2["role"] = "system"
+            elif message["role"] in ["user", "system"]:
+                if theme:
+                    theme["content"] += "\n" + message["content"]
+                else:
+                    theme = message
+                    theme["role"] = "system"
+        if not theme or not gpt1 or not gpt2:
+            self.reset_no_line_break_log()
+            raise ChatGPTPromptWrapperError(
+                "The discuss mode must have a theme (or given by a message from the command line), gpt1, and gpt2 roles."
+            )
+        gpt1_messages = [theme, gpt1]
+        gpt2_messages = [theme, gpt2]
+
+        tokens1 = [
+            self.num_tokens_from_message(message) for message in gpt1_messages
+        ]
+        tokens2 = [
+            self.num_tokens_from_message(message) for message in gpt2_messages
         ]
-        prompt_tokens = self.num_total_tokens(sum(tokens))
-        self.check_prompt_tokens(prompt_tokens)
 
-        max_size = (
-            max(10, max(len(self.get_name(message)) for message in messages))
-            if messages
-            else 10
+        prompt_tokens1 = self.num_total_tokens(sum(tokens1))
+        self.check_prompt_tokens(prompt_tokens1)
+        prompt_tokens2 = self.num_total_tokens(sum(tokens2))
+        self.check_prompt_tokens(prompt_tokens2)
+
+        return gpt1_messages, gpt2_messages, tokens1, tokens2
+
+    def run_main(self, messages: Messages) -> tuple[int, float]:
+
+        gpt1_messages, gpt2_messages, tokens1, tokens2 = self.prepare_messages(
+            messages
         )
-        for message in messages:
-            self.log.info(self.get_output(message, max_size))
+        max_size = max(10, *[len(x) for x in self.names])
+        self.log.info(f"Theme: {messages[0]['content']}\n")
 
-        self.set_no_line_break_log()
         cost = 0.0
-        self.finish_chat = False
-        while True:
-            user = [("class:user", f"{self.alias['user']:>{max_size}}> ")]
-            text = prompt(user, **self.prompt_params)  # type: ignore
-            if self.finish_chat:
-                break
-            message = {"role": "user", "content": text}
-            if message["content"].lower() in self.chat_exit_cmd:
-                break
-            message_tokens = self.num_tokens_from_message(message)
-            if (
-                self.num_total_tokens(message_tokens)
-                > self.tokens_limit - self.min_max_tokens
-            ):
-                self.log.warning("Input is too long, try shorter.\n")
-                continue
-            messages.append(message)
-            tokens.append(message_tokens)
-            while (
-                prompt_tokens := self.num_total_tokens(sum(tokens))
-            ) > self.tokens_limit - self.min_max_tokens:
-                messages = messages[1:]
-                tokens = tokens[1:]
-            cost += self.prices[self.model][0] * prompt_tokens / 1000.0
-            response = cast(
-                Generator[dict[str, Any], None, None],
-                self.completion(messages, stream=True),
-            )
-            new_message = self.show_stream(response, max_size)
-            messages.append(new_message)
-            cost += (
-                self.prices[self.model][1]
-                * self.num_tokens_from_message(new_message, only_content=True)
-                / 1000.0
-            )
+        try:
+            while True:
+                _ = input()
+
+                while (
+                    prompt_tokens := self.num_total_tokens(sum(tokens1))
+                ) > self.tokens_limit - self.min_max_tokens:
+                    gpt1_messages = gpt1_messages[:2] + gpt1_messages[3:]
+                    tokens1 = tokens1[:2] + tokens1[3:]
+                cost += self.prices[self.model][0] * prompt_tokens / 1000.0
+                response = cast(
+                    Generator[dict[str, Any], None, None],
+                    self.completion(gpt1_messages, stream=True),
+                )
 
-        message = {"role": "assistant", "content": "Bye!"}
-        self.log.info(self.get_output(message, max_size))
-        self.log.info("\n")
+                new_message = self.show_stream(
+                    response, max_size, name=self.names.get("gpt1", "gpt1")
+                )
+                gpt1_messages.append(new_message)
+                tokens = self.num_tokens_from_message(new_message)
+                tokens1.append(tokens)
+                user_message = {
+                    "role": "user",
+                    "content": new_message["content"],
+                }
+                gpt2_messages.append(user_message)
+                tokens = self.num_tokens_from_message(user_message)
+                tokens2.append(tokens)
+
+                cost += (
+                    self.prices[self.model][1]
+                    * self.num_tokens_from_message(
+                        new_message, only_content=True
+                    )
+                    / 1000.0
+                )
 
-        self.reset_no_line_break_log()
-        return cost
+                _ = input()
+                while (
+                    prompt_tokens := self.num_total_tokens(sum(tokens2))
+                ) > self.tokens_limit - self.min_max_tokens:
+                    gpt2_messages = gpt2_messages[:2] + gpt2_messages[3:]
+                    tokens2 = tokens2[:2] + tokens2[3:]
+                cost += self.prices[self.model][0] * prompt_tokens / 1000.0
+                response = cast(
+                    Generator[dict[str, Any], None, None],
+                    self.completion(gpt2_messages, stream=True),
+                )
+                new_message = self.show_stream(
+                    response, max_size, name=self.names.get("gpt2", "gpt2")
+                )
+                gpt2_messages.append(new_message)
+                tokens = self.num_tokens_from_message(new_message)
+                tokens2.append(tokens)
+                user_message = {
+                    "role": "user",
+                    "content": new_message["content"],
+                }
+                gpt1_messages.append(user_message)
+                tokens = self.num_tokens_from_message(user_message)
+                tokens1.append(tokens)
+
+                cost += (
+                    self.prices[self.model][1]
+                    * self.num_tokens_from_message(
+                        new_message, only_content=True
+                    )
+                    / 1000.0
+                )
+        except KeyboardInterrupt:
+            pass
+        return max_size, cost
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     top_p: float
         Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time.
     presence_penalty: float
         The penalty for the model to return the same token (-2 ~ 2).
     frequency_penalty: float
         The penalty for the model to return the same token multiple times (-2 ~ 2).
     colors: dict[str, str]
-        The colors to use for the different roles.
+        The colors to use for the different names/roles.
     alias: dict[str, str]
         The aliases of role names.
     """
 
     key: str
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 0
@@ -132,21 +132,21 @@
             raise ChatGPTPromptWrapperError(
                 f"Model: {self.model} is not supported."
             )
 
         # every reply is primed with <|start|>assistant<|message|>
         self.reply_tokens = 3
 
-    def add_color(self, text: str, role: str, size: int = 0) -> str:
+    def add_color(self, text: str, name: str, size: int = 0) -> str:
         if (
             sys.stdout.isatty()
-            and role in self.colors
-            and self.colors[role] in self.ansi_colors
+            and name in self.colors
+            and self.colors[name] in self.ansi_colors
         ):
-            text = f"\033[{self.ansi_colors[self.colors[role]]};1m{text:>{size}}\033[m"
+            text = f"\033[{self.ansi_colors[self.colors[name]]};1m{text:>{size}}\033[m"
         return text
 
     def check_prompt_tokens(self, prompt_tokens: int) -> None:
         if prompt_tokens + self.min_max_tokens > self.tokens_limit:
             raise ChatGPTPromptWrapperError(
                 f"Too much tokens: prompt tokens ({prompt_tokens}) + completion tokens ({self.min_max_tokens}) > tokens limit ({self.tokens_limit})."
             )
@@ -187,25 +187,30 @@
         if "gpt-3.5" in self.model:
             for message in messages:
                 if message["role"] == "system":
                     message["role"] = "user"
         return messages
 
     def get_name(self, message: dict[str, str]) -> str:
-        name = self.alias[message["role"]]
         if "name" in message:
-            if "gpt-3.5" in self.model:
-                name = message["name"]
-            else:
-                name = f"{message['name']} ({message['role']})"
+            name = message["name"]
+        else:
+            name = self.alias.get(message["role"], message["role"])
         return name
 
-    def get_output(self, message: dict[str, str], size: int = 0) -> str:
-        name = self.add_color(self.get_name(message), message["role"], size)
-        return f"{name}> {message['content']}"
+    def get_output(
+        self,
+        message: dict[str, str],
+        size: int = 0,
+        add_linebreak: bool = False,
+    ) -> str:
+        name = self.get_name(message)
+        name = self.add_color(name, name, size)
+        lb = "\n" if add_linebreak else ""
+        return f"{name}> {message['content']}{lb}"
 
     def completion(
         self, messages: Messages, stream: bool = False
     ) -> Generator[dict[str, Any], None, None] | dict[str, Any]:
         max_tokens = self.get_max_tokens(messages)
 
         response = openai.ChatCompletion.create(
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from .__version__ import __version__
 from .arg_parser import cli_help, parse_args, true_false_params, true_params
-from .chatgpt import Ask, Chat
+from .chatgpt import Ask, Chat, Discuss
 from .chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
 from .cmd import commands, cost, init
 from .config import get_config
 from .log_formatter import get_logger
 
 try:
     import tomllib
@@ -128,25 +128,38 @@
 
     def get_cmd_config(self, config: dict[str, Any]) -> dict[str, Any]:
         cmd_config = config.get("global", {})
         cmd_config.update(config.get(self.cmd, {}))
         cmd_config["chat"] = (
             True if self.cmd == "chat" else cmd_config.get("chat", False)
         )
+        cmd_config["discuss"] = (
+            True if self.cmd == "discuss" else cmd_config.get("discuss", False)
+        )
         self.update_cmd_config(cmd_config)
 
-        if not cmd_config["chat"] and not cmd_config["messages"]:
+        if (
+            not cmd_config["chat"]
+            and not cmd_config["discuss"]
+            and not cmd_config["messages"]
+        ):
             raise ChatGPTPromptWrapperError(
                 "This subcommand (ask mode) does not predefined prompt and need input message."
             )
 
         return cmd_config
 
     def run_chatgpt(self, config: dict[str, Any]) -> float:
-        cls: Ask | Chat = Chat if config["chat"] else Ask
+        cls: Ask | Chat | Discuss
+        if config["chat"]:
+            cls = Chat
+        elif config["discuss"]:
+            cls = Discuss
+        else:
+            cls = Ask
         accepted_args = inspect.signature(cls.__init__).parameters  # type: ignore
         params = {k: v for k, v in config.items() if k in accepted_args}
         cost_data_this = cls(**params).run(config["messages"])  # type: ignore
         return cost_data_this
 
     def update_cost(
         self, cost_file: Path, new_cost: float, show_cost: bool = False
@@ -173,15 +186,18 @@
             return
 
         if not self.args.key:
             raise ChatGPTPromptWrapperError(
                 "Set OPEN_AI_API_KEY environment variable or give it by -k (--key) argument."
             )
 
-        if self.cmd not in ["ask", "chat"] and not self.config_file.is_file():
+        if (
+            self.cmd not in ["ask", "chat", "discuss"]
+            and not self.config_file.is_file()
+        ):
             raise ChatGPTPromptWrapperError(
                 f"Configuration file {self.config_file} does not exist"
                 f"`ask` or `cht` subcommand can be used w/o configuration file."
                 f"You prepare the configuration file by `cg init` command."
             )
 
         if self.config_file.is_file():
@@ -190,15 +206,17 @@
         else:
             config = {}
 
         if self.cmd == "commands":
             commands(config, self.log)
             return
 
-        cmds = ["ask", "chat"] + [x for x in config if x != "global"]
+        cmds = ["ask", "chat", "discuss"] + [
+            x for x in config if x != "global"
+        ]
         if self.cmd == "global":
             raise ChatGPTPromptWrapperError("`global` is not a subcommand.")
         if self.cmd not in cmds:
             raise ChatGPTPromptWrapperError(
                 f"Subcommand: `{self.cmd}` is not defined."
             )
```

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.9/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.8/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI tool to wrap ChatGPT Python API.
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -38,20 +38,27 @@
 [![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/chatgpt-prompt-wrapper/tree/coverage)
 
 Python CLI implementation for [ChatGPT](https://openai.com/blog/chatgpt).
 
 ## Requirements
 
 - Python 3.9, 3.10, 3.11
-- Poetry (For development)
 
 ## Installation
 
+By Homebrew:
+
+```
+$ brew install rcmdnk/rcmdnkpac/chatgpt-prompt-wrapper
+```
+
+By pip:
+
 ```
-$ pip install chatgpt-prompt-wrapper
+$ pip3 install chatgpt-prompt-wrapper
 ```
 
 ## Preparation
 
 To get an OpenAI API key, go to [Account API Keys - OpenAI API](https://platform.openai.com/account/api-keys).
 
 Set it as the environment variable `OPENAI_API_KEY`.
@@ -97,54 +104,74 @@
   --no_multiline        Use single line input for chat command.
   --vi                  Use vi mode at chat.
   --emacs               Use emacs mode at chat.
   --show_cost           Show cost used.
 ```
 
 ```
+
 $ cg commands
 Available subcommands:
   Reserved commands:
     ask       : Ask w/o predefined prompt.
     chat      : Start chat w/o predefined prompt.
+    discuss   : Start a discussion between GPTs. Give a them as a message.
     init      : Initialize config file with an example command.
     cost      : Show estimated cost used until now.
     commands  : List up subcommands (show this).
     version   : Show version.
     help      : Show help.
   User commands:
     test      : Example command to test the OpenAI API.
     ...
 ```
 
 ### Ask, Chat
 
 `ask` and `chat` are reserved commands for running simple interaction without a predefined prompt.
 
+- `ask`
+
 `cg ask <message>` returns the answer from ChatGPT for `message`.
 
+- `chat`
+
 `cg chat` starts a chat.
 
 :memo: In `chat` mode, all messages in the past, including answers from
 ChatGPT, will be sent each time you send a new message.
 
 The oldest message will be dropped when the total tokens (including the reserved tokens for the completion defined by `max_tokens` or `min_max_tokens`) exceeds the tokens limit (`tokens_limit` or the number of max tokens (-1) for the used model).
 
 It means you will send almost the max length after a long conversation.
 Please keep the cost in mind. You may want to set `tokens_limit`.
 
+### Discuss
+
+`discuss` is another reserved command which start a discussion between two ChatGPTs.
+
+Two GPTs are ask to perform as:
+
+- Please engage in the discussion as a supporter.
+- Please engage in the discussion as a opponent.
+
+You input message will be a message and they start a discussion.
+
+Please push `Enter` to proceed a duscussion and `Ctrl-C` to quit a discussion.
+
 ### Configuration file
 
 You can define your command in the configuration files.
 
-A command can be in either `ask` mode or `chat` mode.
+A command can be in either `ask` mode, `chat` mode or \`discuss mode.
 
 - `ask` mode: Send a predefined prompt and a message from the command line and receive one answer.
 - `chat` mode: Start a chat with a predefined prompt if defined:
   - `chat` mode can be in either `multiline` mode or single (`no_multiline`) mode.
+- `discuss` mode: Start a discussion between two different ChatGPTs.
 
 #### File path
 
 The default path to the configuration file is **$XDG_CONFIG_HOME/cg/config.toml**.
 
 If **$XDG_CONFIG_HOME** is not defined, use **~/.config/cg/config.toml**.
 
@@ -172,15 +199,17 @@
 - `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
 - Table of `alias`: Dictionary of role aliases. The default alias is: '`user' = 'User'`, `'system' = 'System'`, `'assistant' = 'Assistant'`.
-- List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
+- List of `messages`: Dictionary of message, which must have `role` and `content` (message text).
+  - For `ask`, `chat` modes, `role` must be one of `system`, `user` and `assistant`
+  - For `discuss` mode, three roles, `theme`, `gpt1` and `gpt2` are needed.
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
 
 The options for chat mode:
@@ -234,14 +263,32 @@
 
 [enjoy_chat]
 description = "Chat example with a predefined prompt."
 chat = true
 [[chat.messages]]
 role = "user"
 content = "Let's enjoy a chat."
+
+
+[dd]
+discuss = true
+
+[dd.names]
+gpt1 = "pros"
+gpt2 = "cons"
+
+[[dd.messages]]
+role = "theme"
+content = "Discuss whether or not to actively adopt ChatGPT in the education field. Please provide one-sentence responses."
+[[dd.messages]]
+role = "gpt1"
+content = "Please speak from the standpoint that you should actively adopt ChatGPT in the field of education."
+[[dd.messages]]
+role = "gpt2"
+content = "Please speak from the standpoint that you should not actively adopt ChatGPT in the field of education."
 ```
 
 These messages will be sent as an prompt before your input message.
 
 You can give full questions and use `cg` w/o input messages like a first example `test` command.
 
 Command examples:
```

