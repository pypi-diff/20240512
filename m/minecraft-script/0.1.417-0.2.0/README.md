# Comparing `tmp/minecraft_script-0.1.417.tar.gz` & `tmp/minecraft_script-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.417.tar", last modified: Wed Aug 30 15:16:31 2023, max compression
+gzip compressed data, was "minecraft_script-0.2.0.tar", last modified: Sun May 12 12:02:50 2024, max compression
```

## Comparing `minecraft_script-0.1.417.tar` & `minecraft_script-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 15:16:31.023906 minecraft_script-0.1.417/
--rw-rw-rw-   0        0        0     1927 2023-08-30 15:16:31.022906 minecraft_script-0.1.417/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-30 15:16:30.993721 minecraft_script-0.1.417/minecraft_script/
--rw-rw-rw-   0        0        0     1728 2023-08-11 12:01:38.000000 minecraft_script-0.1.417/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      438 2023-08-11 09:34:51.000000 minecraft_script-0.1.417/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     3856 2023-08-11 19:18:37.000000 minecraft_script-0.1.417/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-08-30 15:16:31.019902 minecraft_script-0.1.417/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.417/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-08-05 21:39:09.000000 minecraft_script-0.1.417/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0      331 2023-08-05 21:31:25.000000 minecraft_script-0.1.417/minecraft_script/build_templates/pack.png
--rw-rw-rw-   0        0        0     1020 2023-08-11 21:00:02.000000 minecraft_script-0.1.417/minecraft_script/build_types.py
--rw-rw-rw-   0        0        0     3673 2023-08-11 19:00:48.000000 minecraft_script-0.1.417/minecraft_script/builder.py
--rw-rw-rw-   0        0        0     1080 2023-08-30 15:14:53.000000 minecraft_script-0.1.417/minecraft_script/common.py
--rw-rw-rw-   0        0        0     2208 2023-08-20 23:37:48.000000 minecraft_script-0.1.417/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-08-30 15:16:31.021905 minecraft_script-0.1.417/minecraft_script/grammar/
--rw-rw-rw-   0        0        0      376 2023-08-30 14:10:40.000000 minecraft_script-0.1.417/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      865 2023-08-21 22:24:11.000000 minecraft_script-0.1.417/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     9501 2023-08-30 14:55:33.000000 minecraft_script-0.1.417/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     8277 2023-08-21 22:33:24.000000 minecraft_script-0.1.417/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     7695 2023-08-30 14:20:17.000000 minecraft_script-0.1.417/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0    17075 2023-08-30 14:59:01.000000 minecraft_script-0.1.417/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2338 2023-08-11 12:11:47.000000 minecraft_script-0.1.417/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.417/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.417/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0    16852 2023-08-30 15:01:55.000000 minecraft_script-0.1.417/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-08-30 15:16:31.006069 minecraft_script-0.1.417/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     1927 2023-08-30 15:16:30.000000 minecraft_script-0.1.417/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      837 2023-08-30 15:16:30.000000 minecraft_script-0.1.417/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 15:16:30.000000 minecraft_script-0.1.417/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-30 15:16:30.000000 minecraft_script-0.1.417/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 15:16:31.023906 minecraft_script-0.1.417/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-08-10 23:28:44.000000 minecraft_script-0.1.417/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.814597 minecraft_script-0.2.0/
+-rw-rw-rw-   0        0        0     2670 2024-05-12 12:02:50.813596 minecraft_script-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.714612 minecraft_script-0.2.0/minecraft_script/
+-rw-rw-rw-   0        0        0     1169 2024-05-12 10:23:12.000000 minecraft_script-0.2.0/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-05-10 15:07:03.000000 minecraft_script-0.2.0/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0      575 2024-05-09 19:42:35.000000 minecraft_script-0.2.0/minecraft_script/common.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.744746 minecraft_script-0.2.0/minecraft_script/compiler/
+-rw-rw-rw-   0        0        0      223 2024-05-09 18:22:05.000000 minecraft_script-0.2.0/minecraft_script/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.747749 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.759784 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/
+-rw-rw-rw-   0        0        0        7 2024-03-23 20:02:41.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/command.mcfunction
+-rw-rw-rw-   0        0        0       40 2024-05-05 13:37:43.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/give_item.mcfunction
+-rw-rw-rw-   0        0        0      266 2024-03-25 19:24:47.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/log.mcfunction
+-rw-rw-rw-   0        0        0       33 2024-03-28 19:55:27.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/set_block.mcfunction
+-rw-rw-rw-   0        0        0       41 2023-08-30 16:13:30.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/function_tags.json
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.776980 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/
+-rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/add.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/divide.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-03-23 17:55:14.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/equals.mcfunction
+-rw-rw-rw-   0        0        0      126 2024-03-23 18:00:46.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/greater_equals_than.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-03-23 17:57:51.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/greater_than.mcfunction
+-rw-rw-rw-   0        0        0      126 2024-03-23 17:58:24.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/less_equals_than.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-03-23 17:57:13.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/less_than.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-03-17 10:03:02.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/modulus.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/multiply.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/subtract.mcfunction
+-rw-rw-rw-   0        0        0      140 2024-05-05 12:13:11.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0      487 2024-02-11 19:12:12.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/pack.png
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.702881 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.779982 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/blocks/
+-rw-rw-rw-   0        0        0      248 2024-03-29 21:11:25.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/blocks/no_collision.json
+-rw-rw-rw-   0        0        0    17022 2024-05-11 21:25:07.000000 minecraft_script-0.2.0/minecraft_script/compiler/builtin_functions.py
+-rw-rw-rw-   0        0        0    21509 2024-05-11 17:21:20.000000 minecraft_script-0.2.0/minecraft_script/compiler/compile_interpreter.py
+-rw-rw-rw-   0        0        0     4874 2024-05-09 10:44:09.000000 minecraft_script-0.2.0/minecraft_script/compiler/compile_types.py
+-rw-rw-rw-   0        0        0     9822 2024-05-11 19:24:42.000000 minecraft_script-0.2.0/minecraft_script/compiler/compiler.py
+-rw-rw-rw-   0        0        0       21 2024-05-09 20:04:29.000000 minecraft_script-0.2.0/minecraft_script/config.json
+-rw-rw-rw-   0        0        0      954 2024-03-20 20:07:01.000000 minecraft_script-0.2.0/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.796579 minecraft_script-0.2.0/minecraft_script/interpreter/
+-rw-rw-rw-   0        0        0        0 2024-03-17 11:19:20.000000 minecraft_script-0.2.0/minecraft_script/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     9127 2024-05-12 10:29:42.000000 minecraft_script-0.2.0/minecraft_script/interpreter/builtin_functions.py
+-rw-rw-rw-   0        0        0    12773 2024-03-27 19:37:34.000000 minecraft_script-0.2.0/minecraft_script/interpreter/interpreter.py
+-rw-rw-rw-   0        0        0    10427 2024-03-20 20:31:18.000000 minecraft_script-0.2.0/minecraft_script/interpreter/types.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.799583 minecraft_script-0.2.0/minecraft_script/lexer/
+-rw-rw-rw-   0        0        0        0 2024-03-17 11:19:09.000000 minecraft_script-0.2.0/minecraft_script/lexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.801585 minecraft_script-0.2.0/minecraft_script/lexer/grammar/
+-rw-rw-rw-   0        0        0      427 2024-01-28 16:27:27.000000 minecraft_script-0.2.0/minecraft_script/lexer/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0     2489 2024-03-27 19:31:59.000000 minecraft_script-0.2.0/minecraft_script/lexer/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5954 2024-03-27 19:15:41.000000 minecraft_script-0.2.0/minecraft_script/lexer/lexer.py
+-rw-rw-rw-   0        0        0      929 2024-03-17 11:32:14.000000 minecraft_script-0.2.0/minecraft_script/lexer/tokens.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.811594 minecraft_script-0.2.0/minecraft_script/parser/
+-rw-rw-rw-   0        0        0        0 2024-03-17 11:19:14.000000 minecraft_script-0.2.0/minecraft_script/parser/__init__.py
+-rw-rw-rw-   0        0        0    11327 2024-03-27 19:33:03.000000 minecraft_script-0.2.0/minecraft_script/parser/nodes.py
+-rw-rw-rw-   0        0        0    20952 2024-05-12 11:25:10.000000 minecraft_script-0.2.0/minecraft_script/parser/parser.py
+-rw-rw-rw-   0        0        0     3882 2024-05-10 15:07:03.000000 minecraft_script-0.2.0/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-08-30 16:13:30.000000 minecraft_script-0.2.0/minecraft_script/text_additions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.812594 minecraft_script-0.2.0/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     2670 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:02:50.814597 minecraft_script-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-12 12:02:09.000000 minecraft_script-0.2.0/setup.py
```

### Comparing `minecraft_script-0.1.417/PKG-INFO` & `minecraft_script-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.417
+Version: 0.2.0
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
-Author-email: <thisis@notarealemail.com>
+Author-email: <christophe@dronne.fr>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
@@ -19,29 +19,49 @@
 purpose is to allow you to validate your code before building it into a full datapack.
 
 Be sure to check out the [documentation](https://github.com/Bard-Gaming/Minecraft-Script/tree/main/documentation) and the provided [examples](https://github.com/Bard-Gaming/Minecraft-Script/tree/main/examples)!
 
 ## Installation
 MCS can be installed using [Python's pip module](https://pip.pypa.io/en/stable/installation/).
 
-```cmd
+```commandline
 pip install minecraft-script
 ```
 or
-```cmd
+```commandline
 python -m pip install minecraft-script
 ```
 _Note: The package's name in pip is written with a hyphen ``-``,
 whilst the actual Python package is written with an underscore ``_``._
 
 
-## Usage
+## Using Minecraft Script to make Datapacks
+### Debugging your program
+To debug your program, you can first run your file like any other programming language.
+To do this, use the following command:
+```commandline
+python -m minecraft_script run [file]
+```
+_where [file] is a relative or absolute path to your mcs file_
+
+### Building your datapack
+To actually build your minecraft datapack, which you can then simply drag & drop into your
+minecraft worlds, use the following command:
+```commandline
+python -m minecraft_script build [file]
+```
+_where [file] is a relative or absolute path to your mcs file_
+
+### More info
 For a list of all shell commands, you can use the following command:
-```cmd
+```commandline
 python -m minecraft_script help
 ```
 If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/installations.md).
 
 ## GitHub
 [**Link to GitHub Repository**](https://github.com/Bard-Gaming/Minecraft-Script)
 
-Source code, documentation, and examples, can all be found on the GitHub.
+Source code, documentation, and examples, can all be found on the GitHub.
+
+## Compatibility
+This python package **does not work on Linux / macOS**.
```

### Comparing `minecraft_script-0.1.417/minecraft_script/text_additions.py` & `minecraft_script-0.2.0/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.417/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.2.0/minecraft_script.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: minecraft-script
-Version: 0.1.417
+Name: minecraft_script
+Version: 0.2.0
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
-Author-email: <thisis@notarealemail.com>
+Author-email: <christophe@dronne.fr>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
@@ -19,29 +19,49 @@
 purpose is to allow you to validate your code before building it into a full datapack.
 
 Be sure to check out the [documentation](https://github.com/Bard-Gaming/Minecraft-Script/tree/main/documentation) and the provided [examples](https://github.com/Bard-Gaming/Minecraft-Script/tree/main/examples)!
 
 ## Installation
 MCS can be installed using [Python's pip module](https://pip.pypa.io/en/stable/installation/).
 
-```cmd
+```commandline
 pip install minecraft-script
 ```
 or
-```cmd
+```commandline
 python -m pip install minecraft-script
 ```
 _Note: The package's name in pip is written with a hyphen ``-``,
 whilst the actual Python package is written with an underscore ``_``._
 
 
-## Usage
+## Using Minecraft Script to make Datapacks
+### Debugging your program
+To debug your program, you can first run your file like any other programming language.
+To do this, use the following command:
+```commandline
+python -m minecraft_script run [file]
+```
+_where [file] is a relative or absolute path to your mcs file_
+
+### Building your datapack
+To actually build your minecraft datapack, which you can then simply drag & drop into your
+minecraft worlds, use the following command:
+```commandline
+python -m minecraft_script build [file]
+```
+_where [file] is a relative or absolute path to your mcs file_
+
+### More info
 For a list of all shell commands, you can use the following command:
-```cmd
+```commandline
 python -m minecraft_script help
 ```
 If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/installations.md).
 
 ## GitHub
 [**Link to GitHub Repository**](https://github.com/Bard-Gaming/Minecraft-Script)
 
-Source code, documentation, and examples, can all be found on the GitHub.
+Source code, documentation, and examples, can all be found on the GitHub.
+
+## Compatibility
+This python package **does not work on Linux / macOS**.
```

