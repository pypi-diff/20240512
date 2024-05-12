# Comparing `tmp/promptdown-0.5.0.tar.gz` & `tmp/promptdown-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptdown-0.5.0.tar", last modified: Fri May  3 03:15:29 2024, max compression
+gzip compressed data, was "promptdown-0.6.0.tar", last modified: Sun May 12 04:07:42 2024, max compression
```

## Comparing `promptdown-0.5.0.tar` & `promptdown-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-03 03:15:12.836759 promptdown-0.5.0/LICENSE
--rw-r--r--   0        0        0     5079 2024-05-03 03:15:12.836759 promptdown-0.5.0/README.md
--rw-r--r--   0        0        0     1074 2024-05-03 03:15:29.956712 promptdown-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-05-03 03:15:12.836759 promptdown-0.5.0/src/promptdown/__init__.py
--rw-r--r--   0        0        0      124 2024-05-03 03:15:28.004717 promptdown-0.5.0/src/promptdown/__init__.pyi
--rw-r--r--   0        0        0    11164 2024-05-03 03:15:12.836759 promptdown-0.5.0/src/promptdown/promptdown.py
--rw-r--r--   0        0        0     1010 2024-05-03 03:15:28.004717 promptdown-0.5.0/src/promptdown/promptdown.pyi
--rw-r--r--   0        0        0     5886 1970-01-01 00:00:00.000000 promptdown-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 04:07:31.518849 promptdown-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6288 2024-05-12 04:07:31.518849 promptdown-0.6.0/README.md
+-rw-r--r--   0        0        0     1074 2024-05-12 04:07:42.898839 promptdown-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-12 04:07:31.518849 promptdown-0.6.0/src/promptdown/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-12 04:07:41.578839 promptdown-0.6.0/src/promptdown/__init__.pyi
+-rw-r--r--   0        0        0    14952 2024-05-12 04:07:31.518849 promptdown-0.6.0/src/promptdown/promptdown.py
+-rw-r--r--   0        0        0     1010 2024-05-12 04:07:41.578839 promptdown-0.6.0/src/promptdown/promptdown.pyi
+-rw-r--r--   0        0        0     7095 1970-01-01 00:00:00.000000 promptdown-0.6.0/PKG-INFO
```

### Comparing `promptdown-0.5.0/LICENSE` & `promptdown-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptdown-0.5.0/README.md` & `promptdown-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -78,14 +78,45 @@
 | Assistant | I'd be happy to help. What seems to be the problem? |
 """
 
 structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
 print(structured_prompt)
 ```
 
+### Simplified Conversation Format
+
+For scenarios where you need to include multi-line messages or prefer a more readable format, Promptdown also supports a simplified conversation format. This alternative is particularly useful for writing extended dialogues or when the conversation involves complex instructions that span multiple lines.
+
+In the simplified format, roles are marked with bold text (**Role:**), and each message can extend over multiple lines, allowing for more expressive and detailed conversations. Here's how you can structure a conversation using this format:
+
+```markdown
+# My Prompt
+
+## System Message
+
+You are a helpful assistant.
+
+## Conversation
+
+**User:**  
+Hello, how are you doing today?  
+I need some help with a project.
+
+**Assistant:**  
+I'm here to help. What's the issue you're encountering with your project?
+
+**User:**  
+I'm trying to integrate an API, but I keep running into errors.
+
+**Assistant:**  
+Let's go through the integration process together. Can you show me the code where you're making the API calls?
+```
+
+The simplified format is especially well-suited for complex templates where multiple template values and introductory message text need to be combined.
+
 ### Loading Prompts from Package Resources
 
 For applications where prompts are bundled within Python packages, Promptdown can load prompts directly from these resources. This approach is useful for distributing prompts alongside Python libraries or applications:
 
 ```python
 from promptdown import StructuredPrompt
```

### Comparing `promptdown-0.5.0/pyproject.toml` & `promptdown-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptdown"
-version = "0.5.0"
+version = "0.6.0"
 description = "A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts"
 authors = [
     { name = "B.T. Franklin", email = "brandon.franklin@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `promptdown-0.5.0/src/promptdown/promptdown.py` & `promptdown-0.6.0/src/promptdown/promptdown.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,28 +63,31 @@
                 self.name == other.name
                 and self.system_message == other.system_message
                 and self.conversation == other.conversation
             )
         return False
 
     @classmethod
-    def _parse_conversation(cls, lines: list[str]) -> list[Message]:
+    def _parse_conversation_table(cls, lines: list[str]) -> list[Message]:
         """
-        Parse the conversation part of a promptdown string into a list of Message objects.
+        Parse the conversation from the given list of lines using the table-based format.
+
+        This method assumes that the conversation section follows a table structure,
+        where each row represents a message with columns like Role, Name (optional),
+        and Content.
 
         Args:
-            lines (list[str]): The lines of the conversation section from a promptdown string.
+            lines (list[str]): A list of lines containing the conversation section.
 
         Returns:
-            list[Message]: A list of Message instances parsed from the given lines.
+            list[Message]: A list of Message objects representing the parsed conversation.
         """
         conversation: list[Message] = []
         headers: list[str] = []
 
-        # Iterate over each line in the input lines
         for line in lines:
             # Check if the line starts with "|", indicating a conversation row
             if line.startswith("|"):
                 # Split the line by "|" and remove leading/trailing whitespace from each part
                 parts = [part.strip() for part in line.split("|") if part.strip()]
 
                 # If headers list is empty, it means we are parsing the first row which contains the headers
@@ -113,14 +116,99 @@
                         )
                     )
 
         # Return the parsed conversation list
         return conversation
 
     @classmethod
+    def _parse_conversation_simplified(cls, lines: list[str]) -> list[Message]:
+        """
+        Parse the conversation from the given list of lines using the simplified format.
+
+        In this format, each message is identified by the role specified with double asterisks
+        (**Role:**) at the beginning of the message. Each subsequent line without a new role
+        will be considered part of the message's content until the next role line is encountered.
+
+        Args:
+            lines (list[str]): A list of lines containing the conversation section.
+
+        Returns:
+            list[Message]: A list of Message objects representing the parsed conversation.
+        """
+        conversation: list[Message] = []
+        known_roles = {"User", "Assistant"}
+        role: str | None = None
+        content: list[str] = []
+
+        for line in lines:
+            # Strip leading/trailing whitespace from the current line
+            line_strip = line.strip()
+
+            # If the line starts and ends with double asterisks, it's a role indicator
+            if line_strip.startswith("**") and line_strip.endswith(":**"):
+                # If a role is already set and there is accumulated content,
+                # add the message to the conversation list
+                if role and content:
+                    conversation.append(
+                        Message(role=role, content=" ".join(content).strip())
+                    )
+                    # Clear content to start collecting the next message
+                    content = []
+
+                # Extract the role name from the asterisks and colon, e.g., "**User:**"
+                role_line = line_strip.strip("*")
+                role, _, _ = role_line.partition(":")
+
+                # If the role is one of the known roles, update the role variable
+                if role in known_roles:
+                    role = role.strip()
+                else:
+                    _LOGGER.warning(
+                        f"Unknown role '{role}' encountered in conversation."
+                    )
+                    role = None
+            else:
+                # If it's not a role indicator, consider it part of the message content
+                content.append(line)
+
+        # If there is a role set and accumulated content after the last line,
+        # append the last message to the conversation
+        if role and content:
+            conversation.append(Message(role=role, content=" ".join(content).strip()))
+
+        # Return the list of parsed messages
+        return conversation
+
+    @classmethod
+    def _parse_conversation(cls, lines: list[str]) -> list[Message]:
+        """
+        Parse the conversation part of a promptdown string into a list of Message objects.
+
+        Args:
+            lines (list[str]): The lines of the conversation section from a promptdown string.
+
+        Returns:
+            list[Message]: A list of Message instances parsed from the given lines.
+        """
+        # Skip empty lines until finding a non-whitespace character
+        for line in lines:
+            stripped_line = line.strip()
+
+            # If we find a line with non-whitespace content, check its first character
+            if stripped_line:
+                # If the first non-whitespace character is a pipe, it's a table format
+                if stripped_line[0] == "|":
+                    return cls._parse_conversation_table(lines)
+                # Otherwise, assume the simplified format
+                return cls._parse_conversation_simplified(lines)
+
+        # If no content is found, return an empty list
+        return []
+
+    @classmethod
     def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt:
         """
         Parse a structured prompt from a raw promptdown string.
 
         Args:
             promptdown_string (str): The complete promptdown formatted string to parse.
```

### Comparing `promptdown-0.5.0/src/promptdown/promptdown.pyi` & `promptdown-0.6.0/src/promptdown/promptdown.pyi`

 * *Files identical despite different names*

### Comparing `promptdown-0.5.0/PKG-INFO` & `promptdown-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptdown
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts
 Author-Email: "B.T. Franklin" <brandon.franklin@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -96,14 +96,45 @@
 | Assistant | I'd be happy to help. What seems to be the problem? |
 """
 
 structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
 print(structured_prompt)
 ```
 
+### Simplified Conversation Format
+
+For scenarios where you need to include multi-line messages or prefer a more readable format, Promptdown also supports a simplified conversation format. This alternative is particularly useful for writing extended dialogues or when the conversation involves complex instructions that span multiple lines.
+
+In the simplified format, roles are marked with bold text (**Role:**), and each message can extend over multiple lines, allowing for more expressive and detailed conversations. Here's how you can structure a conversation using this format:
+
+```markdown
+# My Prompt
+
+## System Message
+
+You are a helpful assistant.
+
+## Conversation
+
+**User:**  
+Hello, how are you doing today?  
+I need some help with a project.
+
+**Assistant:**  
+I'm here to help. What's the issue you're encountering with your project?
+
+**User:**  
+I'm trying to integrate an API, but I keep running into errors.
+
+**Assistant:**  
+Let's go through the integration process together. Can you show me the code where you're making the API calls?
+```
+
+The simplified format is especially well-suited for complex templates where multiple template values and introductory message text need to be combined.
+
 ### Loading Prompts from Package Resources
 
 For applications where prompts are bundled within Python packages, Promptdown can load prompts directly from these resources. This approach is useful for distributing prompts alongside Python libraries or applications:
 
 ```python
 from promptdown import StructuredPrompt
```

