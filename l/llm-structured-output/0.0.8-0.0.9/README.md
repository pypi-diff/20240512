# Comparing `tmp/llm_structured_output-0.0.8.tar.gz` & `tmp/llm_structured_output-0.0.9.tar.gz`

## Comparing `llm_structured_output-0.0.8.tar` & `llm_structured_output-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/.vscode/launch.json
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_build.sh
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_eval.sh
--rwxr-xr-x   0        0        0     1995 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_reluctance.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_server.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_test_number_array.sh
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_upload.sh
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/x.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/json_schema_cli.py
--rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/llm_schema.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/reluctance.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/server.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    23923 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21209 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/LICENSE
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/.vscode/launch.json
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_build.sh
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_eval.sh
+-rwxr-xr-x   0        0        0     2047 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_reluctance.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_server.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_test_number_array.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/_upload.sh
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/_/x.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/examples/json_schema_cli.py
+-rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/examples/llm_schema.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/examples/reluctance.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    23923 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/LICENSE
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.9/PKG-INFO
```

### Comparing `llm_structured_output-0.0.8/_/_eval.sh` & `llm_structured_output-0.0.9/_/_eval.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cd `dirname $0`/../src
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=mlx-community/Mistral-7B-Instruct-v0.2
-#MODEL=mlx-community/Mistral-7B-v0.2-4bit
+MODEL=mlx-community/Mistral-7B-v0.2-4bit
 #MODEL=mistralai/Mistral-7B-Instruct-v0.2
 #MODEL=mlx-community/Mixtral-8x22B-4bit
-MODEL=mlx-community/Meta-Llama-3-8B-Instruct-8bit
+#MODEL=mlx-community/Meta-Llama-3-8B-Instruct-8bit
 #EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/single_turn-00000-of-00001.json
 EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/multi_turn-00000-of-00001.json
 python3 -m tests.eval --model $MODEL --dataset $EVAL_FILE $@
```

### Comparing `llm_structured_output-0.0.8/_/_mistral_schema.sh` & `llm_structured_output-0.0.9/_/_mistral_schema.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 cd `dirname $0`/../src
 
 LLM=examples.llm_schema
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=./mistral/mlx_model_q4
-MODEL=mistralai/Mistral-7B-Instruct-v0.2
+#MODEL=mistralai/Mistral-7B-Instruct-v0.2
 #MODEL=mlx-community/Mistral-7B-v0.2-4bit
 #MODEL=mlx-community/Mixtral-8x22B-4bit
-MODEL=mlx-community/Meta-Llama-3-8B-Instruct-4bit
+#MODEL=mlx-community/Meta-Llama-3-8B-Instruct-4bit
+MODEL=mlx-community/Meta-Llama-3-8B-Instruct-8bit
 OPTIONS="--max-tokens 1000 --repeat-prompt --temp 0.8"
 
 PROMPT='[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}. Do not explain the result, just output it. Do not add any additional information. [/INST]'
 
 if [ "$1" == "--mixtral" ]; then
   shift
   MODEL=./mixtral/mlx_model_q4
```

### Comparing `llm_structured_output-0.0.8/_/_reluctance.sh` & `llm_structured_output-0.0.9/_/_reluctance.sh`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/_/x.py` & `llm_structured_output-0.0.9/_/x.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/examples/json_schema_cli.py` & `llm_structured_output-0.0.9/src/examples/json_schema_cli.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/examples/llm_schema.py` & `llm_structured_output-0.0.9/src/examples/llm_schema.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/examples/reluctance.py` & `llm_structured_output-0.0.9/src/examples/reluctance.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/examples/server.py` & `llm_structured_output-0.0.9/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.9/src/llm_structured_output/acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.9/src/llm_structured_output/json_acceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     def from_trie(cls, trie):
         """
         Create a StringCharTokenTrie given a full trie.
         """
         if isinstance(trie, StringCharTokenTrie):
             return trie
 
-        def _string_char_acceptor_collapse_fn(char):
+        def _string_char_acceptor_collapse_fn(char, _level):
             if char in ['"', "\\"]:
                 return True
             if char in StringCharAcceptor.INVALID_CHARS:
                 return None
             return "."
 
         # pylint: disable-next=protected-access
@@ -288,14 +288,37 @@
         def get_value(self):
             if self.in_accepted_state():
                 return self.value
             else:
                 return f"{self.text}👉"
 
 
+class NumberTokenTrie(TokenTrie):
+    """
+    Create a smaller trie by collapsing digit sequences.
+    """
+
+    @classmethod
+    def from_trie(cls, trie):
+        """
+        Create a NumberTokenTrie given a full trie.
+        """
+        if isinstance(trie, NumberTokenTrie):
+            return trie
+
+        def _number_acceptor_collapse_fn(char, level):
+            if char in "0123456789":
+                return "9"
+            # Only store branches that start with a digit.
+            return level > 0
+
+        # pylint: disable-next=protected-access
+        return trie._map(_number_acceptor_collapse_fn, StringCharTokenTrie())
+
+
 class NumberAcceptor(StateMachineAcceptor):
     """
     Accepts a well-formed JSON number
     """
 
     STATES = {
         0: [(CharAcceptor("-"), 1), (StateMachineAcceptor.EmptyTransition, 1)],  # Sign
@@ -312,28 +335,48 @@
         ],  # More decimals
         6: [(CharAcceptor("eE"), 7)],
         7: [(CharAcceptor("+-"), 8), (StateMachineAcceptor.EmptyTransition, 8)],
         8: [(DigitAcceptor, 9)],  # Exponential, first digit
         9: [(DigitAcceptor, 9)],  # Exponential, more digits
         "$": [2, 3, 5, 9],
     }
+    _cached_tries = {}
+
+    @classmethod
+    def prepare_trie(cls, trie: TokenTrie):
+        """
+        Build a collapsed trie that reduces the search space for valid tokens.
+        """
+        trie_id = id(trie)
+        if trie_id in cls._cached_tries:
+            return cls._cached_tries[trie_id]
+        collapsed_trie = NumberTokenTrie().from_trie(trie)
+        cls._cached_tries[trie_id] = collapsed_trie
+        return collapsed_trie
 
     def __init__(self):
         super().__init__(self.STATES, 0, self.STATES["$"])
 
     class Cursor(StateMachineAcceptor.Cursor):
         """
         Cursor for NumberAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.text = ""
             self.value = None
 
+        def prune(self, trie):
+            """
+            Use a custom matching trie to avoid an explosion of valid options that
+            are equivalent from the point of view of token matching.
+            """
+            return super().prune(NumberAcceptor.prepare_trie(trie))
+
         def complete_transition(self, transition_value, target_state, is_end_state):
             self.text += transition_value
             if is_end_state:
                 self.value = json.loads(self.text)
             return True
 
         def get_value(self):
@@ -482,10 +525,11 @@
 
 
 def prepare_json_acceptor_tries(trie: TokenTrie):
     """
     Pre-cache custom acceptor tries.
     """
     WhitespaceAcceptor.prepare_trie(trie)
+    NumberAcceptor.prepare_trie(trie)
     StringCharAcceptor.prepare_trie(trie)
     if '"' in trie.children:
         StringCharAcceptor.prepare_trie(trie.children['"'])
```

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.9/src/llm_structured_output/json_schema_acceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,24 @@
     Accept a JSON number that conforms to a JSON schema
     """
 
     def __init__(self, schema):
         super().__init__()
         self.schema = schema
         self.is_integer = schema["type"] == "integer"
+        self.requires_validation = any(
+            constraint in schema
+            for constraint in [
+                "minimum",
+                "exclusiveMinimum",
+                "maximum",
+                "exclusiveMaximum",
+                "multipleOf",
+            ]
+        )
 
     def validate_value(self, value):
         """
         Validate the number value according to the schema
         """
         if "minimum" in self.schema and value < self.schema["minimum"]:
             return False
@@ -157,14 +167,33 @@
         Cursor for NumberAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
+        def prune(self, trie):
+            """
+            The parent class uses a collapsed trie and this means in the token-matching
+            phase we are always getting numbers made up of the digit "9", which prevents
+            correct validation. If we actually have anything to validate, we disable it.
+            """
+            if self.acceptor.requires_validation:
+                return super(NumberAcceptor.Cursor, self).prune(trie)
+            return super().prune(trie)
+
+        def start_transition(self, transition_acceptor, target_state):
+            if (
+                self.acceptor.is_integer
+                and self.current_state == 3
+                and target_state == 4
+            ):
+                return False
+            return super().start_transition(transition_acceptor, target_state)
+
         def complete_transition(self, transition_value, target_state, is_end_state):
             if not super().complete_transition(
                 transition_value, target_state, is_end_state
             ):
                 return False
             if is_end_state:
                 return self.acceptor.validate_value(self.get_value())
```

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.9/src/llm_structured_output/util/bitmap.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.9/src/llm_structured_output/util/output.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/util/tokenization.py` & `llm_structured_output-0.0.9/src/llm_structured_output/util/tokenization.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.9/src/llm_structured_output/util/tokentrie.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,36 +78,46 @@
             yield from child.dfs(prefix + char)
 
     def map(self, map_fn) -> TokenTrie:
         """
         Return a trie where the characters are mapped to other characters using a
         function. This is useful for example to collapse a tree into a smaller one
         by pruning or merging branches where the characters are equivalent for a
-        particular use case.
+        particular use case. The mapping function is passed a character to map, and
+        the recursion level in the tree, and it can return True to preserve the
+        branch of the tree as is, None to prune it, or a replacement character.
+        If the latter, the branch will be recursed upon and stored under the
+        replacement branch.
         """
         return self._map(map_fn, self.__class__())
 
-    def _map(self, map_fn: Callable[[str], str], mapped_trie: TokenTrie) -> TokenTrie:
+    def _map(
+        self, map_fn: Callable[[str, int], str], mapped_trie: TokenTrie, level: int = 0
+    ) -> TokenTrie:
         """
         Internal implementation of map()
         """
         mapped_trie.ids |= self.ids
         for char, child in self.children.items():
-            mapped_char = map_fn(char)
+            mapped_char = map_fn(char, level)
             if mapped_char is True:
                 # If the mapping function returns True, preserve the original branch
                 mapped_trie.children[char] = child
             elif mapped_char is None:
                 # If the mapping function returns None, prune the original branch
                 pass
             else:
                 # Map the branch to a new character, e.g. merge several chars into one
-                mapped_child = mapped_trie.children.get(mapped_char, mapped_trie.__class__())
+                mapped_child = mapped_trie.children.get(
+                    mapped_char, mapped_trie.__class__()
+                )
                 # pylint: disable-next=protected-access
-                mapped_trie.children[mapped_char] = child._map(map_fn, mapped_child)
+                mapped_trie.children[mapped_char] = child._map(
+                    map_fn, mapped_child, level + 1
+                )
         return mapped_trie
 
     def _id_count(self) -> int:
         """
         Returns the number of ids in this node
         """
         # FUTURE: self.ids.bit_count() available from Python 3.10 is said to be 6x faster
```

### Comparing `llm_structured_output-0.0.8/src/tests/eval.py` & `llm_structured_output-0.0.9/src/tests/eval.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/LICENSE` & `llm_structured_output-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/README.md` & `llm_structured_output-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.8/pyproject.toml` & `llm_structured_output-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.8/PKG-INFO` & `llm_structured_output-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.8
+Version: 0.0.9
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

