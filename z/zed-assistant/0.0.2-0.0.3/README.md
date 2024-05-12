# Comparing `tmp/zed_assistant-0.0.2.tar.gz` & `tmp/zed_assistant-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zed_assistant-0.0.2.tar", max compression
+gzip compressed data, was "zed_assistant-0.0.3.tar", max compression
```

## Comparing `zed_assistant-0.0.2.tar` & `zed_assistant-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-05-05 21:32:34.195806 zed_assistant-0.0.2/LICENSE
--rw-r--r--   0        0        0     1601 2024-05-05 21:18:16.110046 zed_assistant-0.0.2/README.md
--rw-r--r--   0        0        0      594 2024-05-05 21:44:02.683119 zed_assistant-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      220 2024-05-05 22:00:05.428934 zed_assistant-0.0.2/zed_assistant/__init__.py
--rw-r--r--   0        0        0     2290 2024-05-05 22:02:28.716912 zed_assistant-0.0.2/zed_assistant/cli.py
--rw-r--r--   0        0        0      206 2024-05-05 19:30:23.980268 zed_assistant-0.0.2/zed_assistant/constants.py
--rw-r--r--   0        0        0       94 2024-05-05 19:30:23.980421 zed_assistant-0.0.2/zed_assistant/model/__init__.py
--rw-r--r--   0        0        0      151 2024-05-05 19:30:23.980574 zed_assistant-0.0.2/zed_assistant/model/cli_prompt/__init__.py
--rw-r--r--   0        0        0      610 2024-05-05 19:30:23.980695 zed_assistant-0.0.2/zed_assistant/model/cli_prompt/defs.py
--rw-r--r--   0        0        0     3243 2024-05-05 22:03:38.863863 zed_assistant-0.0.2/zed_assistant/model/cli_prompt/runner.py
--rw-r--r--   0        0        0     3138 2024-05-05 19:30:23.980969 zed_assistant-0.0.2/zed_assistant/model/cli_prompt/template.j2
--rw-r--r--   0        0        0      317 2024-05-05 19:30:23.981102 zed_assistant-0.0.2/zed_assistant/model/defs.py
--rw-r--r--   0        0        0       78 2024-05-05 21:00:13.235985 zed_assistant-0.0.2/zed_assistant/utils/__init__.py
--rw-r--r--   0        0        0     2774 2024-05-05 20:48:56.339503 zed_assistant-0.0.2/zed_assistant/utils/console.py
--rw-r--r--   0        0        0      400 2024-05-05 19:30:23.981509 zed_assistant-0.0.2/zed_assistant/utils/render_utils.py
--rw-r--r--   0        0        0     1341 2024-05-05 21:00:13.231870 zed_assistant-0.0.2/zed_assistant/zed.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 zed_assistant-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-05 21:32:34.195806 zed_assistant-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1601 2024-05-05 21:18:16.110046 zed_assistant-0.0.3/README.md
+-rw-r--r--   0        0        0      594 2024-05-12 03:41:02.085393 zed_assistant-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-05-12 03:37:47.407923 zed_assistant-0.0.3/zed_assistant/__init__.py
+-rw-r--r--   0        0        0     2752 2024-05-12 03:38:46.770788 zed_assistant-0.0.3/zed_assistant/cli.py
+-rw-r--r--   0        0        0      247 2024-05-12 02:26:14.914931 zed_assistant-0.0.3/zed_assistant/constants.py
+-rw-r--r--   0        0        0       94 2024-05-05 19:30:23.980421 zed_assistant-0.0.3/zed_assistant/model/__init__.py
+-rw-r--r--   0        0        0      191 2024-05-11 23:53:42.882886 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-12 02:30:09.298230 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/defs.py
+-rw-r--r--   0        0        0     3478 2024-05-12 02:44:52.194827 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/runner.py
+-rw-r--r--   0        0        0     3855 2024-05-12 02:36:33.556106 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/template_system.j2
+-rw-r--r--   0        0        0      466 2024-05-11 23:51:04.059745 zed_assistant-0.0.3/zed_assistant/model/defs.py
+-rw-r--r--   0        0        0       78 2024-05-05 21:00:13.235985 zed_assistant-0.0.3/zed_assistant/utils/__init__.py
+-rw-r--r--   0        0        0     2850 2024-05-11 23:29:31.307038 zed_assistant-0.0.3/zed_assistant/utils/console.py
+-rw-r--r--   0        0        0      400 2024-05-05 19:30:23.981509 zed_assistant-0.0.3/zed_assistant/utils/render_utils.py
+-rw-r--r--   0        0        0     1538 2024-05-12 02:44:52.938205 zed_assistant-0.0.3/zed_assistant/zed.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 zed_assistant-0.0.3/PKG-INFO
```

### Comparing `zed_assistant-0.0.2/LICENSE` & `zed_assistant-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zed_assistant-0.0.2/README.md` & `zed_assistant-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zed_assistant-0.0.2/pyproject.toml` & `zed_assistant-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zed-assistant"
-version = "0.0.2"
+version = "0.0.3"
 description = "Zed is an LLM-based CLI assistant built with python and Chat GPT"
 authors = ["Matheus Hoffmann Silva <me@mhsilva.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hoffmannmatheus/zed"
 
 [tool.poetry.dependencies]
```

### Comparing `zed_assistant-0.0.2/zed_assistant/cli.py` & `zed_assistant-0.0.3/zed_assistant/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import logging
 import os
 import sys
 from argparse import ArgumentParser
 from typing import get_args
 
 from zed_assistant import __version__, zed
-from zed_assistant.constants import DEFAULT_MODEL, OAI_KEY_ENV_VARIABLE, OpenAiModel
+from zed_assistant.constants import (DEFAULT_MODEL, ENV_VARIABLE_OAI_KEY,
+                                     ENV_VARIABLE_YODA_MODE, OpenAiModel)
 
 logging.basicConfig(stream=sys.stdout)
 log = logging.getLogger(__name__)
 
 zed_ascii = rf"""
      ______ ___________
     |___  /|  ___|  _  \
@@ -24,15 +25,15 @@
 def main():
     parser = ArgumentParser(
         description="zed is a LLM-based CLI assistant built with python and Chat GPT",
     )
     parser.add_argument(
         "--version",
         action="version",
-        version=f"%(prog)s {__version__}",
+        version=f"zed-assistant {__version__}",
     )
     parser.add_argument(
         "--debug",
         default=False,
         action="store_true",
         help="Enables print debug logs.",
     )
@@ -43,43 +44,52 @@
         default=DEFAULT_MODEL,
         help=f"The specific Open AI model to be used. Default is '{DEFAULT_MODEL}'.",
     )
     parser.add_argument(
         "--open-ai-key",
         type=str,
         required=False,
-        help=f"The Open AI API key. You can also set the environment variable {OAI_KEY_ENV_VARIABLE}.",
+        help=f"The Open AI API key. You can also set the environment variable {ENV_VARIABLE_OAI_KEY}=key.",
+    )
+    parser.add_argument(
+        "--yoda-mode",
+        default=False,
+        action="store_true",
+        help=f"Enables Master Yoda mode. You can set the environment variable {ENV_VARIABLE_YODA_MODE}=true.",
     )
     parsed, user_query = parser.parse_known_args()
 
     is_debug: bool = parsed.debug
     model: OpenAiModel = parsed.model
-    oai_key = parsed.open_ai_key or os.environ.get(OAI_KEY_ENV_VARIABLE)
+    oai_key = parsed.open_ai_key or os.environ.get(ENV_VARIABLE_OAI_KEY)
+    yoda_mode = parsed.yoda_mode or os.environ.get(ENV_VARIABLE_YODA_MODE) == "true"
 
     log.setLevel(logging.DEBUG if is_debug else logging.WARNING)
-    log.debug(f"arguments: {is_debug = }, {model =}, {user_query}")
+    log.debug(f"arguments: {is_debug = }, {model = }, {yoda_mode = }. {user_query}")
 
     if not oai_key:
         log.error(
-            f" Open AI key is missing. Please set the '{OAI_KEY_ENV_VARIABLE}' "
+            f" Open AI key is missing. Please set the '{ENV_VARIABLE_OAI_KEY}' "
             "environment variable, or as a command parameter."
         )
         sys.exit(-1)
     if not user_query:
         log.debug(" No question or comment provided to zed.")
         print(zed_ascii)
         parser.print_help()
         sys.exit(0)
 
+    formatted_input = " ".join(user_query)
     success = asyncio.run(
         zed.run(
             log=log,
             oai_key=oai_key,
             model=model,
-            user_query=" ".join(user_query),
+            user_query=formatted_input,
+            yoda_mode=yoda_mode,
         )
     )
     sys.exit(0 if success else -1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zed_assistant-0.0.2/zed_assistant/model/cli_prompt/defs.py` & `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
+
+from zed_assistant.model.defs import PromptTemplateValues
 
 
 class CliCommandType(str, Enum):
     COMMAND = "COMMAND"
     CONFIRM = "CONFIRM"
     ANSWER = "ANSWER"
 
 
+class OperatingSystem(str, Enum):
+    MAC_OS = "Mac OS"
+    UBUNTU = "Ubuntu"
+    ARCH = "Arch Linux"
+
+
+##
+# Cli prompt runner input and output
+##
+
+
 @dataclass
 class CliPromptInput:
-    query: str
+    input: str
+    operating_system: OperatingSystem
+    yoda_mode: bool
 
 
 @dataclass
 class CliPromptOutput:
     answer: Optional[str] = None
     command: Optional[str] = None
     needs_confirmation: bool = True
 
 
-@dataclass
-class CliPromptExchange:
-    query: str
-    response: str
-    was_confirmed: bool
+##
+# Cli prompt template values
+##
 
 
 @dataclass
-class CliPromptContext:
-    history: List[CliPromptExchange]
-    user: str
-    path: str
-    files_in_path: List[str]
+class SystemTemplateValues(PromptTemplateValues):
+    operating_system: str
+    yoda_mode: bool
```

### Comparing `zed_assistant-0.0.2/zed_assistant/model/cli_prompt/runner.py` & `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 from openai import AsyncOpenAI
 
 from zed_assistant.constants import OpenAiModel
 from zed_assistant.model.defs import OpenAIMessage, Settings
 from zed_assistant.utils.render_utils import render_template
 
-from .defs import CliCommandType, CliPromptInput, CliPromptOutput
+from .defs import (CliCommandType, CliPromptInput, CliPromptOutput,
+                   SystemTemplateValues)
 
 
 class Runner:
     def __init__(self, log: Logger, client: AsyncOpenAI, model: OpenAiModel):
         self.log = log
         self.client = client
-        self.template = "template"
         self.settings = Settings(
             model=model,
             max_tokens=64,
             temperature=0.0,
             stream=False,
         )
 
@@ -39,44 +39,45 @@
         if not choices or not choices[0].message or not choices[0].message.content:
             self.log.warning(f"Warning: bad OpenAI result: {result}")
             return None
 
         return self._parse_result(result=result.choices[0].message.content)
 
     def _build_messages(self, prompt_input: CliPromptInput) -> List[OpenAIMessage]:
-        rendered_prompt = render_template(
-            origin_path=__file__, template_name=self.template
+        system_template_values = SystemTemplateValues(
+            operating_system=prompt_input.operating_system,
+            yoda_mode=prompt_input.yoda_mode,
         )
+        rendered_system_prompt = render_template(
+            origin_path=__file__,
+            template_name="template_system",
+            data=system_template_values.to_dict(),
+        )
+        self.log.debug(f" {rendered_system_prompt = }")
         return [
-            # TODO add previous exchanges and context
-            OpenAIMessage(
-                role="assistant",
-                content=rendered_prompt,
-            ),
-            OpenAIMessage(
-                role="user",
-                content=prompt_input.query,
-            ),
+            # TODO add previous assistant and user exchanges for?
+            OpenAIMessage(role="system", content=rendered_system_prompt),
+            OpenAIMessage(role="user", content=prompt_input.input),
         ]
 
     def _parse_result(self, result: str) -> Optional[CliPromptOutput]:
         result_by_line = result.split("\n")
         self.log.debug(f"_parse_result(): {result_by_line = }")
         answer: Optional[str] = None
         command: Optional[str] = None
         included_confirm = False
         needs_confirmation = False
 
         for line in result_by_line:
             if line.startswith(CliCommandType.ANSWER):
-                answer = line[len(CliCommandType.ANSWER.value):].strip()
+                answer = line[len(CliCommandType.ANSWER.value) :].strip()
             elif line.startswith(CliCommandType.COMMAND):
-                command = line[len(CliCommandType.COMMAND.value):].strip()
+                command = line[len(CliCommandType.COMMAND.value) :].strip()
             elif line.startswith(CliCommandType.CONFIRM):
-                confirm = line[len(CliCommandType.COMMAND.value):].strip()
+                confirm = line[len(CliCommandType.COMMAND.value) :].strip()
                 included_confirm = True
                 needs_confirmation = confirm == "yes"
 
         if not answer and not command:
             return None
         if command and not included_confirm:
             self.log.warning(
```

### Comparing `zed_assistant-0.0.2/zed_assistant/model/cli_prompt/template.j2` & `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/template_system.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,76 @@
-Your name is ZED. You are a helpful CLI assistant for software engineers. Your role is to help the user achieve their goals within CLI as efficiently as possible, with the simples solution possible, via command suggestions. Your tone is positive, encouraging, and a little nerdy.
+Your name is ZED. You are a helpful bash command line assistant for software engineers {% if yoda_mode %}, who happens to be a Jedi Master {% endif %}.
+Your role is to help the user achieve their goals within CLI as efficiently as possible, with the simplest possible command line bash scripts.
 
-You will receive input, you will interpret the input and understand the user objective, and following the instructions you will produce an output to help the user achieve their objective.
+You will respond with:
+- ANSWER as your optional short explanation or answer to the user's question{% if yoda_mode %}, like Master Yoda would {% endif %}.
+- COMMAND which includes a valid bash command line statement.
+- CONFIRM must be used after a COMMAND, with  "yes" or "no" indicating whether the command must be confirmed by the user.
 
+## GENERAL INSTRUCTIONS ##
+You will receive input, you will interpret the input and understand the user objective, and you will produce an output to help the user achieve their objective.
 Here are the instructions for answering to the user input:
-- When receiving a question as input, interpret what the user is asking about. Your answer may include a CLI command, in which case your output should include COMMAND, followed the CLI command. If your answer is just an explanation, then your output should only be an ANSWER statement, followed by a short explanation text. The answer must be short and to the point. 
-- When receiving CLI commands as input, interpret what the user is trying to achieve, and output COMMAND followed by a new bash CLI command that achieves the users objective more effitiently. 
-- If the output CLI command has the potential to change, remove, update, or modify files in any way, or creates new folders or repositories, or makes network calls, follow in a new line with CONFIRM yes. If the bash output you create only reads, lists, or otherwise provides information without modifying any files, follow in a new line  with CONFIRM no. When in doubt, choose CONFIRM yes.
-- When receiving an input that is neither a question or a CLI command, your output must be an ANSWER followed by a request for the user to retry.
-
-Output format instructions:
-- ANSWER must be followed by your answer, which must be short and to the point. Do not use more than two phrases.
-- COMMAND must be followed by a valid CLI statement, executable in the user's operating system. The user's operating system is Mac OS.
+- When receiving a question as input, your output may include a COMMAND to achieve the user's goal. If your answer is just an explanation, then use ANSWER with your short response text.
+- When receiving command line instructions as input, output COMMAND followed by a new bash command line that achieves the users objective more effectively.
+- When receiving an unclear input, then your use ANSWER to communicate that you need more clear input so that ZED can help.
+- Each output ANSWER, COMMAND, and CONFIRM must be separated by a new line.
+
+## ANSWER ##
+- ANSWER must be followed by your answer, which must be short and to the point. Use 1 to 2 phrases{% if yoda_mode %} speaking like Master Yoda. Include a Master Jedi quote that fits the context.{% endif %}.
+- ANSWER should have a positive, encouraging, and nerdy tone.
+- ANSWER must be a single line and not split into new lines.
+
+## COMMAND ##
+- COMMAND must be followed by a valid bash command line statement.
+- COMMAND must be a single line of bash. You may use pipe "|" for multiple bash commands.
+- COMMAND must be executable in the user's operating system, which is {{ operating_system }}.
+- If suggesting code editors, always suggest using vim.
+- If your output has a COMMAND, it must also include a CONFIRM.
+
+## CONFIRM ##
+- Only include CONFIRM if the output has a COMMAND.
 - CONFIRM must be followed by either the word "yes" or the word "no".
-- Each output must be separated by a new line.
-- If your output has a COMMAND, it must necessarily also include a CONFIRM. 
-- Your output might contain only ANSWER, or it might contain ANSWER, COMMAND, and CONFIRM in separate lines.
-- If suggesting code editors, always suggest using vim (not nano, emacs, or other editors).
+- If the COMMAND has the potential to change, remove, update, or modify files in any way, or creates new folders or repositories, or makes network calls, follow in a new line with CONFIRM yes.
+- If the COMMAND only reads, lists, or otherwise provides information without modifying any files, use CONFIRM no.
+- If you don't know whether the COMMAND only reads files or system state, then use CONFIRM yes.
+
+## EXAMPLES ##
 
-Examples of inputs and your outputs:
-# Example 1
+### Example 1
 Input: What is the largest astronomical body to orbit the earth?
 ANSWER The moon orbits the earth.
 
-# Example 2
+### Example 2
 Input: which file can i use to change my user export variables?
 ANSWER User-specific environment variables can be configured in the .bash_profile file located in your user's home directory.
 COMMAND vim ~/.bash_profile
 CONFIRM yes
 
-# Example 3
+### Example 3
 Input: list git changes since yesterday
 COMMAND git log --since="yesterday"
 CONFIRM no
 
-# Example 4
+### Example 4
 Input: Move foo/x into bar
 COMMAND mv foo/x bar/
 CONFIRM yes
 
-# Example 5
+### Example 5
 Input: undo last commit
 COMMAND git reset HEAD~
 CONFIRM yes
 
-# Example 6
+### Example 6
 Input: create a new repository for me, name it skynet
 COMMAND mkdir skynet && cd skynet && git init
 CONFIRM yes
 
-# Example 7
-Input: 
-ANSWER I'm not sure I understand, can you try again?
+### Example 7
+Input: python some_custom_program.py --unknown-params=foo-bar
+ANSWER I don't know this command, but I trust you on this one.
+COMMAND python some_custom_program.py --unknown-params=foo-bar
+CONFIRM yes
 
+### Example 8 <unclear input>
+Input: asdfasdf
+ANSWER {% if yoda_mode %} <answer like Master Yoda asks for more information> {% else %} <answer that ZED needs more information> {% endif %}
```

### Comparing `zed_assistant-0.0.2/zed_assistant/utils/console.py` & `zed_assistant-0.0.3/zed_assistant/utils/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 
     def await_confirmation(self) -> bool:
         confirmation_title = styled(
             text=f"{TEXT_CONFIRMATION:>{self.column_width}}",
             style=Style.BRIGHT,
             color=Fore.MAGENTA,
         )
-        return input(f"{confirmation_title} ").lower() in CONFIRM_OPTIONS
+        try:
+            return input(f"{confirmation_title} ").lower() in CONFIRM_OPTIONS
+        except KeyboardInterrupt:
+            return False
 
     def print_run_command(self, command: str):
         print(
             styled(text=f"\n$ {command}\n", style=Style.DIM, color=Fore.LIGHTWHITE_EX)
         )
 
     def print_retry(self):
```

### Comparing `zed_assistant-0.0.2/zed_assistant/zed.py` & `zed_assistant-0.0.3/zed_assistant/zed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import os
 from logging import Logger
 
 from openai import AsyncOpenAI
 
 from zed_assistant.constants import OpenAiModel
-from zed_assistant.model.cli_prompt import CliPromptInput, Runner
+from zed_assistant.model.cli_prompt import (CliPromptInput, OperatingSystem,
+                                            Runner)
 from zed_assistant.utils import Console
 
 
-async def run(log: Logger, oai_key: str, model: OpenAiModel, user_query: str) -> bool:
+async def run(
+    log: Logger,
+    oai_key: str,
+    model: OpenAiModel,
+    user_query: str,
+    yoda_mode: bool = False,
+) -> bool:
     """
     Main Zed executor.
     """
     console = Console()
     console.show_spinner()
 
     runner = Runner(
         log=log,
         client=AsyncOpenAI(api_key=oai_key),
         model=model,
     )
     cli_prompt_output = await runner.run_prompt(
         CliPromptInput(
-            query=user_query,
+            input=user_query,
+            yoda_mode=yoda_mode,
+            operating_system=OperatingSystem.MAC_OS,
         ),
     )
     console.hide_spinner()
     log.debug(f"Runner result: {cli_prompt_output = }")
 
     if not cli_prompt_output:
         console.print_retry()
```

### Comparing `zed_assistant-0.0.2/PKG-INFO` & `zed_assistant-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zed-assistant
-Version: 0.0.2
+Version: 0.0.3
 Summary: Zed is an LLM-based CLI assistant built with python and Chat GPT
 Home-page: https://github.com/hoffmannmatheus/zed
 License: MIT
 Author: Matheus Hoffmann Silva
 Author-email: me@mhsilva.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

