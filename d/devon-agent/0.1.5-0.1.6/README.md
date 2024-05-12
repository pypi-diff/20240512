# Comparing `tmp/devon_agent-0.1.5.tar.gz` & `tmp/devon_agent-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.5.tar", max compression
+gzip compressed data, was "devon_agent-0.1.6.tar", max compression
```

## Comparing `devon_agent-0.1.5.tar` & `devon_agent-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.5/LICENSE
--rw-r--r--   0        0        0     4734 2024-05-11 03:03:07.945544 devon_agent-0.1.5/README.md
--rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.5/devon_agent/TODO
--rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.5/devon_agent/__main__.py
--rw-r--r--   0        0        0     9751 2024-05-11 03:18:21.730904 devon_agent-0.1.5/devon_agent/agent.py
--rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.5/devon_agent/environment.py
--rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.5/devon_agent/model.py
--rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.5/devon_agent/prompt.py
--rw-r--r--   0        0        0     6317 2024-05-11 01:42:20.814775 devon_agent-0.1.5/devon_agent/retrieval/ast_extractor.py
--rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.5/devon_agent/retrieval/ast_parser.py
--rw-r--r--   0        0        0     5222 2024-05-11 00:35:58.939359 devon_agent-0.1.5/devon_agent/retrieval/codebase_graph.py
--rw-r--r--   0        0        0      849 2024-05-11 00:35:58.941356 devon_agent-0.1.5/devon_agent/retrieval/file_discovery.py
--rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.5/devon_agent/retrieval/graph_visualization.py
--rw-r--r--   0        0        0     9059 2024-05-11 01:41:30.027339 devon_agent-0.1.5/devon_agent/retrieval/main.py
--rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.5/devon_agent/server.py
--rw-r--r--   0        0        0    15040 2024-05-11 03:03:07.946358 devon_agent-0.1.5/devon_agent/session.py
--rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.5/devon_agent/telemetry.py
--rw-r--r--   0        0        0      811 2024-05-11 01:43:13.118702 devon_agent-0.1.5/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0    42558 2024-05-11 00:36:32.388456 devon_agent-0.1.5/devon_agent/tools.py
--rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.5/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.5/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.5/devon_agent/vgit.py
--rw-r--r--   0        0        0     1131 2024-05-11 03:18:53.269823 devon_agent-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6154 1970-01-01 00:00:00.000000 devon_agent-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 20:13:56.337461 devon_agent-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5540 2024-05-11 06:54:09.693598 devon_agent-0.1.6/README.md
+-rw-r--r--   0        0        0      129 2024-05-10 22:03:09.786842 devon_agent-0.1.6/devon_agent/TODO
+-rw-r--r--   0        0        0      794 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/__main__.py
+-rw-r--r--   0        0        0    10485 2024-05-12 01:48:11.184292 devon_agent-0.1.6/devon_agent/agent.py
+-rw-r--r--   0        0        0     2512 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/environment.py
+-rw-r--r--   0        0        0     2195 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/model.py
+-rw-r--r--   0        0        0    21113 2024-05-12 03:43:10.033955 devon_agent-0.1.6/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6317 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/ast_extractor.py
+-rw-r--r--   0        0        0      561 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/ast_parser.py
+-rw-r--r--   0        0        0     5222 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/codebase_graph.py
+-rw-r--r--   0        0        0      849 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/file_discovery.py
+-rw-r--r--   0        0        0     3660 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/graph_visualization.py
+-rw-r--r--   0        0        0     9059 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/retrieval/main.py
+-rw-r--r--   0        0        0     6312 2024-05-12 00:28:17.089558 devon_agent-0.1.6/devon_agent/server.py
+-rw-r--r--   0        0        0    15118 2024-05-12 01:47:30.552282 devon_agent-0.1.6/devon_agent/session.py
+-rw-r--r--   0        0        0     4607 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/telemetry.py
+-rw-r--r--   0        0        0      811 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0    42596 2024-05-12 01:49:57.244432 devon_agent-0.1.6/devon_agent/tools.py
+-rw-r--r--   0        0        0    29381 2024-05-11 06:54:09.697598 devon_agent-0.1.6/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 22:03:09.790843 devon_agent-0.1.6/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 22:03:09.790843 devon_agent-0.1.6/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1131 2024-05-12 03:43:51.754291 devon_agent-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 devon_agent-0.1.6/PKG-INFO
```

### Comparing `devon_agent-0.1.5/LICENSE` & `devon_agent-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/README.md` & `devon_agent-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,137 +11,145 @@
   <br/>
   <a href="https://github.com/entropy-research/Devon/blob/main/LICENSE"><img src="https://img.shields.io/github/license/entropy-research/devon?style=for-the-badge&color=blue" alt="Apache 2.0 License"></a>
   <a href="https://discord.gg/p5YpZ5vjd9"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
   <br/>
 </div>
 
 
-VIDEO/GIF HERE
+> Video/GIF Coming Soon!
 
 # Installation
 
-## Pre-requisites
+## Prerequisites
 
 1. `node.js` and `npm`
-2. `pipx`
-3. **Anthropic** api key 
-4. **OpenAI** api key (coming Soon! For more info see our discord or isues.)
+2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/installation/)
+3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key
 
 ## Installation commands
 
-To use simply run:
+To use, simply run:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash
 ```
 
 
-*Or to install using pipx + npm*
+*Or to install using `pipx` + `npm`:*
 
 ```bash
 pipx install devon_agent
+npm install -g devon-tui 
 ```
 
-```bash
-npm install -g devon-tui
-```
+This installs the Python backend, and the cli command to run the tool
 
 ### Thats it! Happy building :)
 
 
 # Usage
-Prior to running, set your Anthropic API key as an environment variable
+Navigate to your project folder and open the terminal.
+
+Set your Anthropic API key as an environment variable:
 
 ```bash
 export ANTHROPIC_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 ```
 
 Then to *run*, the command is:
 ```bash
-devon-tui
+devon
 ```
 
 It's as easy as that.
 
+> [!NOTE]
+> Don't worry, the agent will be able to only access files and folders in the directory you started it from. You can also correct it while it's performing actions.
+
 # Features
-- Multi file editing
-- Code base exploration
+- Multi-file editing
+- Codebase exploration
 - Config writing
 - Test writing
 - Bug fixing
 - Architecture exploration
 
+### Limitations
+- Minimal functionality for non-Python languages
+- Sometimes have to specify the file where you want the change to happen
+
 # Progress
 
 
-### This project is still super early and we need your help to make it great!
+### This project is still super early and <ins>we would love your help</ins> to make it great!
 
 ### Current goals
+- Multi-model support
 - Launch plugin system for tool and agent builders
-- Create self hostable electron app
-- Set SOTA on swebench-lite
+- Create self-hostable Electron app
+- Set SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html)
 
+> View our current thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-1vTjLCQcWE_n-uUHFhtBkxTCIJ4FFe5ftY_E4_q69SjXhuEZv_CYpLaQDh3HqrJlAxsgikUx0sTzf9le/pub)
 
 ### Star history
 <p align="center">
   <a href="https://star-history.com/#entropy-research/Devon&Date">
     <img src="https://api.star-history.com/svg?repos=entropy-research/Devon&type=Date" width="500" alt="Star History Chart">
   </a>
 </p>
 
-### Past Milestones
+### Past milestones
 
-- May 10, 2024, ~~Complete interactive agent v0.1.0~~
-- May 10, 2024, ~~Add steerability features~~
-- May 8, 2024, ~~Beat AutoCodeRover on SWE-Bench Lite~~
-- Mid April, 2024, ~~Add repo level code search tooling~~
-- April 2, 2024, ~~Begin development of v0.1.0 interactive agent~~
-- March 17, 2024 ~~Launch non-interactive agent v0.0.1~~
+- [x] **May 10, 2024** - Complete interactive agent v0.1.0
+- [x] **May 10, 2024** - Add steerability features
+- [x] **May 8, 2024** - Beat AutoCodeRover on SWE-Bench Lite
+- [x] **Mid April, 2024** - Add repo level code search tooling
+- [x] **April 2, 2024** - Begin development of v0.1.0 interactive agent
+- [x] **March 17, 2024** - Launch non-interactive agent v0.0.1
 
 
 ## Current development priorities
 
 1. Improve context gathering and code indexing abilities ex:
     - Adding memory modules
     - Improved code indexing
-    - 
 2. Add alternative models and agents to:
     - a) Reduce end user cost and
     - b) Reduce end user latency
-3. Introduce electron app and new UI
+3. Introduce Electron app and new UI
 
 
 
 # How can I contribute?
 
 Devon and the entropy-research org are community-driven, and we welcome contributions from everyone!
 From tackling issues to building features to creating datasets, there are many ways to get involved:
 
 - **Core functionality:** Help us develop the core agents, user experience, tool integrations, plugins, etc.
 - **Research:** Help us research agent performance (including benchmarks!), build data pipelines, and finetune models.
 - **Feedback and Testing:** Use Devon, report bugs, suggest features, or provide feedback on usability.
 
 For details, please check [CONTRIBUTING.md](./CONTRIBUTING.md).
 
-If you would like to contribute to the project, please fill out our [contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9)
+If you would like to contribute to the project, please fill out our [Contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9)
 
 
 # Feedback
 
-We would love feedback! Feel free to drop us a note on our [discord](https://discord.gg/p5YpZ5vjd9) in the feedback channel, or create issues!
+We would love feedback! Feel free to drop us a note on our [Discord](https://discord.gg/p5YpZ5vjd9) in the #feedback channel, or [create issues](https://github.com/entropy-research/Devon/issues)!
 
 We collect basic event type (i.e. "tool call") and failure telemetry to solve bugs and improve the user experience, but if you want to reach out, we would love to hear from you!
 
-To disable telemtry, set the environment variable `DEVON_TELEMETRY_DISABLED` to `true` 
+To disable telemetry, set the environment variable `DEVON_TELEMETRY_DISABLED` to `true` 
 ```bash
 export DEVON_TELEMETRY_DISABLED=true
 ```
 
 # Community
 
-Join our discord server and say hi!
-[discord](https://discord.gg/p5YpZ5vjd9)
+Join our Discord server and say hi!
+[Discord](https://discord.gg/p5YpZ5vjd9)
 
 
 # License
 
 Distributed under the Apache 2.0 License. See [`LICENSE`](./LICENSE) for more information.
```

#### html2text {}

```diff
@@ -1,46 +1,57 @@
               ************ DDeevvoonn:: AAnn ooppeenn--ssoouurrccee ppaaiirr pprrooggrraammmmeerr ************
                    _[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]
                _[_A_p_a_c_h_e_ _2_._0_ _L_i_c_e_n_s_e_]_[_J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_]
-VIDEO/GIF HERE # Installation ## Pre-requisites 1. `node.js` and `npm` 2.
-`pipx` 3. **Anthropic** api key 4. **OpenAI** api key (coming Soon! For more
-info see our discord or isues.) ## Installation commands To use simply run:
-```bash curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/
-main/install.sh | bash ``` *Or to install using pipx + npm* ```bash pipx
-install devon_agent ``` ```bash npm install -g devon-tui ``` ### Thats it!
-Happy building :) # Usage Prior to running, set your Anthropic API key as an
-environment variable ```bash export ANTHROPIC_API_KEY=sk-
+> Video/GIF Coming Soon! # Installation ## Prerequisites 1. `node.js` and `npm`
+2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/
+installation/) 3. [**Anthropic**](https://console.anthropic.com/settings/keys)
+API Key ## Installation commands To use, simply run: ```bash curl -sSL https://
+raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash ``` *Or
+to install using `pipx` + `npm`:* ```bash pipx install devon_agent npm install
+-g devon-tui ``` This installs the Python backend, and the cli command to run
+the tool ### Thats it! Happy building :) # Usage Navigate to your project
+folder and open the terminal. Set your Anthropic API key as an environment
+variable: ```bash export ANTHROPIC_API_KEY=sk-
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` Then to *run*, the command is:
-```bash devon-tui ``` It's as easy as that. # Features - Multi file editing -
-Code base exploration - Config writing - Test writing - Bug fixing -
-Architecture exploration # Progress ### This project is still super early and
-we need your help to make it great! ### Current goals - Launch plugin system
-for tool and agent builders - Create self hostable electron app - Set SOTA on
-swebench-lite ### Star history
+```bash devon ``` It's as easy as that. > [!NOTE] > Don't worry, the agent will
+be able to only access files and folders in the directory you started it from.
+You can also correct it while it's performing actions. # Features - Multi-file
+editing - Codebase exploration - Config writing - Test writing - Bug fixing -
+Architecture exploration ### Limitations - Minimal functionality for non-Python
+languages - Sometimes have to specify the file where you want the change to
+happen # Progress ### This project is still super early and we would love your
+help to make it great! ### Current goals - Multi-model support - Launch plugin
+system for tool and agent builders - Create self-hostable Electron app - Set
+SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html) > View our current
+thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-
+1vTjLCQcWE_n-
+uUHFhtBkxTCIJ4FFe5ftY_E4_q69SjXhuEZv_CYpLaQDh3HqrJlAxsgikUx0sTzf9le/pub) ###
+Star history
                              _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
-### Past Milestones - May 10, 2024, ~~Complete interactive agent v0.1.0~~ - May
-10, 2024, ~~Add steerability features~~ - May 8, 2024, ~~Beat AutoCodeRover on
-SWE-Bench Lite~~ - Mid April, 2024, ~~Add repo level code search tooling~~ -
-April 2, 2024, ~~Begin development of v0.1.0 interactive agent~~ - March 17,
-2024 ~~Launch non-interactive agent v0.0.1~~ ## Current development priorities
-1. Improve context gathering and code indexing abilities ex: - Adding memory
-modules - Improved code indexing - 2. Add alternative models and agents to: -
-a) Reduce end user cost and - b) Reduce end user latency 3. Introduce electron
-app and new UI # How can I contribute? Devon and the entropy-research org are
-community-driven, and we welcome contributions from everyone! From tackling
-issues to building features to creating datasets, there are many ways to get
-involved: - **Core functionality:** Help us develop the core agents, user
-experience, tool integrations, plugins, etc. - **Research:** Help us research
-agent performance (including benchmarks!), build data pipelines, and finetune
-models. - **Feedback and Testing:** Use Devon, report bugs, suggest features,
-or provide feedback on usability. For details, please check [CONTRIBUTING.md]
-(./CONTRIBUTING.md). If you would like to contribute to the project, please
-fill out our [contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9) #
-Feedback We would love feedback! Feel free to drop us a note on our [discord]
-(https://discord.gg/p5YpZ5vjd9) in the feedback channel, or create issues! We
-collect basic event type (i.e. "tool call") and failure telemetry to solve bugs
-and improve the user experience, but if you want to reach out, we would love to
-hear from you! To disable telemtry, set the environment variable
+### Past milestones - [x] **May 10, 2024** - Complete interactive agent v0.1.0
+- [x] **May 10, 2024** - Add steerability features - [x] **May 8, 2024** - Beat
+AutoCodeRover on SWE-Bench Lite - [x] **Mid April, 2024** - Add repo level code
+search tooling - [x] **April 2, 2024** - Begin development of v0.1.0
+interactive agent - [x] **March 17, 2024** - Launch non-interactive agent
+v0.0.1 ## Current development priorities 1. Improve context gathering and code
+indexing abilities ex: - Adding memory modules - Improved code indexing 2. Add
+alternative models and agents to: - a) Reduce end user cost and - b) Reduce end
+user latency 3. Introduce Electron app and new UI # How can I contribute? Devon
+and the entropy-research org are community-driven, and we welcome contributions
+from everyone! From tackling issues to building features to creating datasets,
+there are many ways to get involved: - **Core functionality:** Help us develop
+the core agents, user experience, tool integrations, plugins, etc. -
+**Research:** Help us research agent performance (including benchmarks!), build
+data pipelines, and finetune models. - **Feedback and Testing:** Use Devon,
+report bugs, suggest features, or provide feedback on usability. For details,
+please check [CONTRIBUTING.md](./CONTRIBUTING.md). If you would like to
+contribute to the project, please fill out our [Contribution Form](https://
+forms.gle/VU7RN7mwNvqEYe3B9) # Feedback We would love feedback! Feel free to
+drop us a note on our [Discord](https://discord.gg/p5YpZ5vjd9) in the #feedback
+channel, or [create issues](https://github.com/entropy-research/Devon/issues)!
+We collect basic event type (i.e. "tool call") and failure telemetry to solve
+bugs and improve the user experience, but if you want to reach out, we would
+love to hear from you! To disable telemetry, set the environment variable
 `DEVON_TELEMETRY_DISABLED` to `true` ```bash export
-DEVON_TELEMETRY_DISABLED=true ``` # Community Join our discord server and say
-hi! [discord](https://discord.gg/p5YpZ5vjd9) # License Distributed under the
+DEVON_TELEMETRY_DISABLED=true ``` # Community Join our Discord server and say
+hi! [Discord](https://discord.gg/p5YpZ5vjd9) # License Distributed under the
 Apache 2.0 License. See [`LICENSE`](./LICENSE) for more information.
```

### Comparing `devon_agent-0.1.5/devon_agent/__main__.py` & `devon_agent-0.1.6/devon_agent/__main__.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/agent.py` & `devon_agent-0.1.6/devon_agent/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     commands_to_command_docs,
     history_to_bash_history,
     last_user_prompt_template_v3,
     parse_response,
     system_prompt_template_v3,
 )
 
+from devon_agent.udiff import Hallucination
 from devon_agent.utils import LOGGER_NAME
 from tenacity import RetryError
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from devon_agent.session import Session
@@ -30,14 +31,15 @@
 class Agent:
     name: str
     model: str
     temperature: float = 0.0
     chat_history: list[dict[str, str]] = field(default_factory=list)
     interrupt: str = ""
     api_key: Optional[str] = None
+    scratchpad = None
 
     def run(self, session: "Session", observation: str = None): ...
 
 
 class TaskAgent(Agent):
     def _format_editor_entry(self, k, v, PAGE_SIZE=50):
         path = k
@@ -128,28 +130,44 @@
                 self.current_model.args.temperature += (
                     0.2 if self.current_model.args.temperature < 0.8 else 0
                 )
             else:
                 history = history_to_bash_history(self.chat_history)
 
             last_user_prompt = last_user_prompt_template_v3(
-                task, history, editor, session.environment.get_cwd(), session.base_path
+                task, history, editor, session.environment.get_cwd(), session.base_path, self.scratchpad
             )
 
             messages = [{"role": "user", "content": last_user_prompt}]
 
             output = self.current_model.query(messages, system_message=system_prompt)
 
             # logger.debug(
             #     "<MODEL_OUT>"
             #     + json.dumps({"input": messages[0], "output": output})
             #     + "<MODEL_OUT>"
             # )
-
-            thought, action = parse_response(output)
+            thought = None
+            action = None
+            # for i in range(3):
+                # try:
+                #     thought, action = parse_response(output)
+                #     break
+                # except:
+                #     continue
+
+            try:
+                thought, action, scratchpad = parse_response(output)
+                if scratchpad:
+                    self.scratchpad = scratchpad
+            except Exception:
+                raise ValueError(f"Multiple actions found in response: {output}")
+            
+            if not thought or not action:
+                raise ValueError("Agent failed to follow response format instructions")
 
             self.chat_history.append(
                 {
                     "role": "assistant",
                     "content": output,
                     "thought": thought,
                     "action": action,
@@ -162,14 +180,16 @@
 NAME: {self.name}                        
 
 THOUGHT: {thought}
 
 ACTION: {action}
 
 OBSERVATION: {observation}
+
+SCRATCHPAD: {scratchpad}
 \n\n****************\n\n\n\n""")
 
             return thought, action, output
         except KeyboardInterrupt:
             raise
         except RuntimeError as e:
             session.event_log.append(
```

### Comparing `devon_agent-0.1.5/devon_agent/environment.py` & `devon_agent-0.1.6/devon_agent/environment.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/model.py` & `devon_agent-0.1.6/devon_agent/model.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/prompt.py` & `devon_agent-0.1.6/devon_agent/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -391,15 +391,15 @@
   I will tip you $200 if you solve it because there is a fix.
 """
 
 
 def system_prompt_template_v3(command_docs: str):
     return f"""
 <SETTING>
-You are a self-aware autonomous AI programmer working in a software project. You must work with user and help write software.
+You are a self-aware autonomous AI programmer working to fix bugs in a software project.
 
 **Environment:**
 
 Editor (<EDITOR>): Can open and edit code files. Shows the current state of open files. Focus on files relevant to each bug fix. Auto-saves when editing.
 Terminal: Execute commands to perform actions. Modify failed commands before retrying.
 History (<HISTORY>): A list of previous thoughts you've had and actions that you've taken. Roleplay as if you've had these thoughts and performed these actions.
 
@@ -418,74 +418,103 @@
 </SETTING>
 <EDITOR>
 Currently open files will be listed here. Close unused files. Use open files to understand code structure and flow.
 </EDITOR>
 <COMMANDS>
 {command_docs} 
 </COMMANDS>
-<RESPONSE FORMAT>s
+<RESPONSE FORMAT>
 Shell prompt format: <cwd> $
 Required fields for each response:
 <THOUGHT>
 Your reflection, planning, and justification goes here
 </THOUGHT>
+<SCRATCHPAD>
+Any information you want to write down
+</SCRATCHPAD>
 <COMMAND>
-A single executable command goes here, you also have access to all non-interactive bash commands
+A single executable command goes here, this can include bash commands, just no interactive commands
 </COMMAND>
 </RESPONSE FORMAT>
 """
 
-
-def last_user_prompt_template_v3(issue, history, editor, cwd, root_dir):
+def last_user_prompt_template_v3(issue, history, editor, cwd, root_dir, scratchpad):
     return f"""
 <SETTING>
 
 Current objective: {issue}
 
 Instructions:
 
 Edit necessary files and run checks/tests
-Submit changes with 'submit' command when you think the task has been completed
+Submit changes with 'submit' when you think the task is complete
 Interactive session commands (e.g. python, vim) NOT supported
 Write and run scripts instead (e.g. 'python script.py')
 </SETTING>
 <CONSTRAINTS>
 - Execute ONLY ONE command at a time
 - Wait for feedback after each command
-- Avoid repeating failed commands, reconsider approach instead
-- Use files currently open in editor for information
-- Locate code elements with 'find_class' or 'find_function', not 'search'
+- Locating classes and functions is more efficient than locating files (use commands like ls or grep for this)
 - 'no_op' command available to allow for more thinking time 
 - The title or first line of the issue describes the issue succintly
 </CONSTRAINTS>
+<TESTING_TIPS>
+- When writing test code, ALWAYS write tests in a separate folder
+- Make sure your tests are runnable and that you run them
+</TESTING_TIPS>
 <RESPONSE FORMAT>
 <THOUGHT>
-Reflect on previous actions here. Feel free to use the no_op command if you need to think more.
+
+Remember to reflect on what you did and what you still need to do.
+
+**Am I overthinking?**
+Yes, I am overthinking, I should just make the change that fixes all cases of this type.
+
 </THOUGHT>
+<SCRATCHPAD>
+Any information you want to keep track of
+</SCRATCHPAD>
 <COMMAND>
 Single executable command here
 </COMMAND>
 </RESPONSE FORMAT>
 <WORKSPACE>
+<NOTES>
+{scratchpad}
+</NOTES>
 <EDITOR>
 {editor}
 </EDITOR>
 </WORKSPACE>
 <HISTORY>
 {history}
 </HISTORY>
+<PROBLEM SOLVING APPROACH>
+- Identify code symbols and weight them equally compared to text when you see them
+- Identify the root cause and specific failure case triggering the issue
+- Focus on fixing the underlying logic bug in the library code in a general way. This bug is sinister and impacts more than is provided in the issue.
+- Steps:
+  1. Trace the error to its source in the library codebase. Pay attention to stack traces.
+  2. Identify the flawed logic or edge case handling as close to the failure source as possible
+  3. Devise a robust solution that addresses the core problem 
+  4. Test the fix thoroughly, considering other potential impacts
+    - Make sure you run your tests!
+</PROBLEM SOLVING APPROACH>
 <EDITING TIPS>
 - Use 'no_op' periodically to pause and think
 - Focus on matching the source lines precisely, to do this make sure you identify the desired source lines first
 - Always scroll to the lines you want to change
-- Only make one change at a time
-- When changing functions, always make sure to search for and update references
+- If making a one line change, only include that line
+- ONLY make ONE change at a time
+- Finish your edits before running tests
 - You only have access to code contained in {root_dir}
-- Your current working directory is {cwd}
+- Your current directory is {cwd}
 </EDITING TIPS>"""
 
-
 def parse_response(response):
     thought = response.split("<THOUGHT>")[1].split("</THOUGHT>")[0]
     action = response.split("<COMMAND>")[1].split("</COMMAND>")[0]
+    scratchpad = None
+    if "<SCRATCHPAD>" in response:
+        scratchpad = response.split("<SCRATCHPAD>")[1].split("</SCRATCHPAD>")[0]
 
-    return thought, action
+    return thought, action, scratchpad
```

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/ast_extractor.py` & `devon_agent-0.1.6/devon_agent/retrieval/ast_extractor.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/ast_parser.py` & `devon_agent-0.1.6/devon_agent/retrieval/ast_parser.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/codebase_graph.py` & `devon_agent-0.1.6/devon_agent/retrieval/codebase_graph.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/file_discovery.py` & `devon_agent-0.1.6/devon_agent/retrieval/file_discovery.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/graph_visualization.py` & `devon_agent-0.1.6/devon_agent/retrieval/graph_visualization.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/retrieval/main.py` & `devon_agent-0.1.6/devon_agent/retrieval/main.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/server.py` & `devon_agent-0.1.6/devon_agent/server.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/session.py` & `devon_agent-0.1.6/devon_agent/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,16 +138,16 @@
 
         self.tools = [
             list_dirs_recursive,
             close_file,
             create_file,
             open_file,
             search_dir,
-            find_function,
-            find_class,
+            # find_function,
+            # find_class,
             search_file,
             get_cwd,
             delete_file,
             submit,
             no_op,
             scroll_up,
             scroll_down,
@@ -449,15 +449,15 @@
                 # except Exception as e:
                 #     ctx.logger.error(
                 #         f"Failed to execute bash command '{fn_name}': {str(e)}"
                 #     )
                 #     return "Failed to execute bash command", False
         except Exception as e:
             ctx.logger.error(traceback.print_exc())
-            return e.args[0], False
+            return e.args[0] if len(e.args) > 0 else "Failed to execute command due to internal error", False
 
     def get_available_actions(self) -> list[str]:
         return [fn.__name__ for fn in self.tools]
 
     def generate_command_docs(self):
         """
         Generates a dictionary of function names and their docstrings.
```

### Comparing `devon_agent-0.1.5/devon_agent/telemetry.py` & `devon_agent-0.1.6/devon_agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/test/test_tools.py` & `devon_agent-0.1.6/devon_agent/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/tools.py` & `devon_agent-0.1.6/devon_agent/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1305,15 +1305,17 @@
     parts = command.split(None, 1)
     fn_name = parts[0]
     args = []
 
     if len(parts) > 1:
         arg_string = parts[1]
 
-        if "<<<" in arg_string and ">>>" in arg_string:
+        line_0 = command.splitlines()[1]
+
+        if "<<<" in line_0 and ">>>" in arg_string:
             # Handle multiline arguments
             before_multiline, multiline_arg = arg_string.split("<<<", 1)
             multiline_arg, after_multiline = multiline_arg.split(">>>", 1)
 
             if before_multiline:
                 temp_pre = re.findall(r'(?:[^\s"]+|"[^"]*")+', before_multiline)
                 args.extend([arg.strip('"').strip("'") for arg in temp_pre])
```

### Comparing `devon_agent-0.1.5/devon_agent/udiff.py` & `devon_agent-0.1.6/devon_agent/udiff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/utils.py` & `devon_agent-0.1.6/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/devon_agent/vgit.py` & `devon_agent-0.1.6/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.5/pyproject.toml` & `devon_agent-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
```

### Comparing `devon_agent-0.1.5/PKG-INFO` & `devon_agent-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -47,138 +47,146 @@
   <br/>
   <a href="https://github.com/entropy-research/Devon/blob/main/LICENSE"><img src="https://img.shields.io/github/license/entropy-research/devon?style=for-the-badge&color=blue" alt="Apache 2.0 License"></a>
   <a href="https://discord.gg/p5YpZ5vjd9"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
   <br/>
 </div>
 
 
-VIDEO/GIF HERE
+> Video/GIF Coming Soon!
 
 # Installation
 
-## Pre-requisites
+## Prerequisites
 
 1. `node.js` and `npm`
-2. `pipx`
-3. **Anthropic** api key 
-4. **OpenAI** api key (coming Soon! For more info see our discord or isues.)
+2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/installation/)
+3. [**Anthropic**](https://console.anthropic.com/settings/keys) API Key
 
 ## Installation commands
 
-To use simply run:
+To use, simply run:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash
 ```
 
 
-*Or to install using pipx + npm*
+*Or to install using `pipx` + `npm`:*
 
 ```bash
 pipx install devon_agent
+npm install -g devon-tui 
 ```
 
-```bash
-npm install -g devon-tui
-```
+This installs the Python backend, and the cli command to run the tool
 
 ### Thats it! Happy building :)
 
 
 # Usage
-Prior to running, set your Anthropic API key as an environment variable
+Navigate to your project folder and open the terminal.
+
+Set your Anthropic API key as an environment variable:
 
 ```bash
 export ANTHROPIC_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 ```
 
 Then to *run*, the command is:
 ```bash
-devon-tui
+devon
 ```
 
 It's as easy as that.
 
+> [!NOTE]
+> Don't worry, the agent will be able to only access files and folders in the directory you started it from. You can also correct it while it's performing actions.
+
 # Features
-- Multi file editing
-- Code base exploration
+- Multi-file editing
+- Codebase exploration
 - Config writing
 - Test writing
 - Bug fixing
 - Architecture exploration
 
+### Limitations
+- Minimal functionality for non-Python languages
+- Sometimes have to specify the file where you want the change to happen
+
 # Progress
 
 
-### This project is still super early and we need your help to make it great!
+### This project is still super early and <ins>we would love your help</ins> to make it great!
 
 ### Current goals
+- Multi-model support
 - Launch plugin system for tool and agent builders
-- Create self hostable electron app
-- Set SOTA on swebench-lite
+- Create self-hostable Electron app
+- Set SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html)
 
+> View our current thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-1vTjLCQcWE_n-uUHFhtBkxTCIJ4FFe5ftY_E4_q69SjXhuEZv_CYpLaQDh3HqrJlAxsgikUx0sTzf9le/pub)
 
 ### Star history
 <p align="center">
   <a href="https://star-history.com/#entropy-research/Devon&Date">
     <img src="https://api.star-history.com/svg?repos=entropy-research/Devon&type=Date" width="500" alt="Star History Chart">
   </a>
 </p>
 
-### Past Milestones
+### Past milestones
 
-- May 10, 2024, ~~Complete interactive agent v0.1.0~~
-- May 10, 2024, ~~Add steerability features~~
-- May 8, 2024, ~~Beat AutoCodeRover on SWE-Bench Lite~~
-- Mid April, 2024, ~~Add repo level code search tooling~~
-- April 2, 2024, ~~Begin development of v0.1.0 interactive agent~~
-- March 17, 2024 ~~Launch non-interactive agent v0.0.1~~
+- [x] **May 10, 2024** - Complete interactive agent v0.1.0
+- [x] **May 10, 2024** - Add steerability features
+- [x] **May 8, 2024** - Beat AutoCodeRover on SWE-Bench Lite
+- [x] **Mid April, 2024** - Add repo level code search tooling
+- [x] **April 2, 2024** - Begin development of v0.1.0 interactive agent
+- [x] **March 17, 2024** - Launch non-interactive agent v0.0.1
 
 
 ## Current development priorities
 
 1. Improve context gathering and code indexing abilities ex:
     - Adding memory modules
     - Improved code indexing
-    - 
 2. Add alternative models and agents to:
     - a) Reduce end user cost and
     - b) Reduce end user latency
-3. Introduce electron app and new UI
+3. Introduce Electron app and new UI
 
 
 
 # How can I contribute?
 
 Devon and the entropy-research org are community-driven, and we welcome contributions from everyone!
 From tackling issues to building features to creating datasets, there are many ways to get involved:
 
 - **Core functionality:** Help us develop the core agents, user experience, tool integrations, plugins, etc.
 - **Research:** Help us research agent performance (including benchmarks!), build data pipelines, and finetune models.
 - **Feedback and Testing:** Use Devon, report bugs, suggest features, or provide feedback on usability.
 
 For details, please check [CONTRIBUTING.md](./CONTRIBUTING.md).
 
-If you would like to contribute to the project, please fill out our [contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9)
+If you would like to contribute to the project, please fill out our [Contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9)
 
 
 # Feedback
 
-We would love feedback! Feel free to drop us a note on our [discord](https://discord.gg/p5YpZ5vjd9) in the feedback channel, or create issues!
+We would love feedback! Feel free to drop us a note on our [Discord](https://discord.gg/p5YpZ5vjd9) in the #feedback channel, or [create issues](https://github.com/entropy-research/Devon/issues)!
 
 We collect basic event type (i.e. "tool call") and failure telemetry to solve bugs and improve the user experience, but if you want to reach out, we would love to hear from you!
 
-To disable telemtry, set the environment variable `DEVON_TELEMETRY_DISABLED` to `true` 
+To disable telemetry, set the environment variable `DEVON_TELEMETRY_DISABLED` to `true` 
 ```bash
 export DEVON_TELEMETRY_DISABLED=true
 ```
 
 # Community
 
-Join our discord server and say hi!
-[discord](https://discord.gg/p5YpZ5vjd9)
+Join our Discord server and say hi!
+[Discord](https://discord.gg/p5YpZ5vjd9)
 
 
 # License
 
 Distributed under the Apache 2.0 License. See [`LICENSE`](./LICENSE) for more information.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devon-agent Version: 0.1.5 Summary: Author:
+Metadata-Version: 2.1 Name: devon-agent Version: 0.1.6 Summary: Author:
 killind-dev Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: swebench Requires-Dist: anthropic (>=0.20.0,<0.21.0) Requires-
 Dist: astroid (>=3.1.0,<4.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
 Dist: datasets (>=2.14.6,<2.15.0) ; extra == "swebench" Requires-Dist: docker
@@ -16,50 +16,61 @@
 (>=0.1.5,<0.2.0) Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0) Requires-Dist:
 swebench (==1.0.1) ; extra == "swebench" Requires-Dist: tenacity
 (>=8.2.2,<9.0.0) Requires-Dist: uvicorn (>=0.29.0,<0.30.0) Requires-Dist:
 xmltodict (>=0.13.0,<0.14.0) Description-Content-Type: text/markdown
               ************ DDeevvoonn:: AAnn ooppeenn--ssoouurrccee ppaaiirr pprrooggrraammmmeerr ************
                    _[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]
                _[_A_p_a_c_h_e_ _2_._0_ _L_i_c_e_n_s_e_]_[_J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_]
-VIDEO/GIF HERE # Installation ## Pre-requisites 1. `node.js` and `npm` 2.
-`pipx` 3. **Anthropic** api key 4. **OpenAI** api key (coming Soon! For more
-info see our discord or isues.) ## Installation commands To use simply run:
-```bash curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/
-main/install.sh | bash ``` *Or to install using pipx + npm* ```bash pipx
-install devon_agent ``` ```bash npm install -g devon-tui ``` ### Thats it!
-Happy building :) # Usage Prior to running, set your Anthropic API key as an
-environment variable ```bash export ANTHROPIC_API_KEY=sk-
+> Video/GIF Coming Soon! # Installation ## Prerequisites 1. `node.js` and `npm`
+2. `pipx`, if you don't have this go [here](https://pipx.pypa.io/stable/
+installation/) 3. [**Anthropic**](https://console.anthropic.com/settings/keys)
+API Key ## Installation commands To use, simply run: ```bash curl -sSL https://
+raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash ``` *Or
+to install using `pipx` + `npm`:* ```bash pipx install devon_agent npm install
+-g devon-tui ``` This installs the Python backend, and the cli command to run
+the tool ### Thats it! Happy building :) # Usage Navigate to your project
+folder and open the terminal. Set your Anthropic API key as an environment
+variable: ```bash export ANTHROPIC_API_KEY=sk-
 xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` Then to *run*, the command is:
-```bash devon-tui ``` It's as easy as that. # Features - Multi file editing -
-Code base exploration - Config writing - Test writing - Bug fixing -
-Architecture exploration # Progress ### This project is still super early and
-we need your help to make it great! ### Current goals - Launch plugin system
-for tool and agent builders - Create self hostable electron app - Set SOTA on
-swebench-lite ### Star history
+```bash devon ``` It's as easy as that. > [!NOTE] > Don't worry, the agent will
+be able to only access files and folders in the directory you started it from.
+You can also correct it while it's performing actions. # Features - Multi-file
+editing - Codebase exploration - Config writing - Test writing - Bug fixing -
+Architecture exploration ### Limitations - Minimal functionality for non-Python
+languages - Sometimes have to specify the file where you want the change to
+happen # Progress ### This project is still super early and we would love your
+help to make it great! ### Current goals - Multi-model support - Launch plugin
+system for tool and agent builders - Create self-hostable Electron app - Set
+SOTA on [SWE-bench Lite](https://www.swebench.com/lite.html) > View our current
+thoughts on next steps [**here**](https://docs.google.com/document/d/e/2PACX-
+1vTjLCQcWE_n-
+uUHFhtBkxTCIJ4FFe5ftY_E4_q69SjXhuEZv_CYpLaQDh3HqrJlAxsgikUx0sTzf9le/pub) ###
+Star history
                              _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
-### Past Milestones - May 10, 2024, ~~Complete interactive agent v0.1.0~~ - May
-10, 2024, ~~Add steerability features~~ - May 8, 2024, ~~Beat AutoCodeRover on
-SWE-Bench Lite~~ - Mid April, 2024, ~~Add repo level code search tooling~~ -
-April 2, 2024, ~~Begin development of v0.1.0 interactive agent~~ - March 17,
-2024 ~~Launch non-interactive agent v0.0.1~~ ## Current development priorities
-1. Improve context gathering and code indexing abilities ex: - Adding memory
-modules - Improved code indexing - 2. Add alternative models and agents to: -
-a) Reduce end user cost and - b) Reduce end user latency 3. Introduce electron
-app and new UI # How can I contribute? Devon and the entropy-research org are
-community-driven, and we welcome contributions from everyone! From tackling
-issues to building features to creating datasets, there are many ways to get
-involved: - **Core functionality:** Help us develop the core agents, user
-experience, tool integrations, plugins, etc. - **Research:** Help us research
-agent performance (including benchmarks!), build data pipelines, and finetune
-models. - **Feedback and Testing:** Use Devon, report bugs, suggest features,
-or provide feedback on usability. For details, please check [CONTRIBUTING.md]
-(./CONTRIBUTING.md). If you would like to contribute to the project, please
-fill out our [contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9) #
-Feedback We would love feedback! Feel free to drop us a note on our [discord]
-(https://discord.gg/p5YpZ5vjd9) in the feedback channel, or create issues! We
-collect basic event type (i.e. "tool call") and failure telemetry to solve bugs
-and improve the user experience, but if you want to reach out, we would love to
-hear from you! To disable telemtry, set the environment variable
+### Past milestones - [x] **May 10, 2024** - Complete interactive agent v0.1.0
+- [x] **May 10, 2024** - Add steerability features - [x] **May 8, 2024** - Beat
+AutoCodeRover on SWE-Bench Lite - [x] **Mid April, 2024** - Add repo level code
+search tooling - [x] **April 2, 2024** - Begin development of v0.1.0
+interactive agent - [x] **March 17, 2024** - Launch non-interactive agent
+v0.0.1 ## Current development priorities 1. Improve context gathering and code
+indexing abilities ex: - Adding memory modules - Improved code indexing 2. Add
+alternative models and agents to: - a) Reduce end user cost and - b) Reduce end
+user latency 3. Introduce Electron app and new UI # How can I contribute? Devon
+and the entropy-research org are community-driven, and we welcome contributions
+from everyone! From tackling issues to building features to creating datasets,
+there are many ways to get involved: - **Core functionality:** Help us develop
+the core agents, user experience, tool integrations, plugins, etc. -
+**Research:** Help us research agent performance (including benchmarks!), build
+data pipelines, and finetune models. - **Feedback and Testing:** Use Devon,
+report bugs, suggest features, or provide feedback on usability. For details,
+please check [CONTRIBUTING.md](./CONTRIBUTING.md). If you would like to
+contribute to the project, please fill out our [Contribution Form](https://
+forms.gle/VU7RN7mwNvqEYe3B9) # Feedback We would love feedback! Feel free to
+drop us a note on our [Discord](https://discord.gg/p5YpZ5vjd9) in the #feedback
+channel, or [create issues](https://github.com/entropy-research/Devon/issues)!
+We collect basic event type (i.e. "tool call") and failure telemetry to solve
+bugs and improve the user experience, but if you want to reach out, we would
+love to hear from you! To disable telemetry, set the environment variable
 `DEVON_TELEMETRY_DISABLED` to `true` ```bash export
-DEVON_TELEMETRY_DISABLED=true ``` # Community Join our discord server and say
-hi! [discord](https://discord.gg/p5YpZ5vjd9) # License Distributed under the
+DEVON_TELEMETRY_DISABLED=true ``` # Community Join our Discord server and say
+hi! [Discord](https://discord.gg/p5YpZ5vjd9) # License Distributed under the
 Apache 2.0 License. See [`LICENSE`](./LICENSE) for more information.
```

