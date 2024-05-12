# Comparing `tmp/circular-dict-1.7.tar.gz` & `tmp/circular_dict-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular-dict-1.7.tar", last modified: Thu Aug 17 10:05:09 2023, max compression
+gzip compressed data, was "circular_dict-1.8.tar", last modified: Sun May 12 16:49:07 2024, max compression
```

## Comparing `circular-dict-1.7.tar` & `circular_dict-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-17 10:05:09.532633 circular-dict-1.7/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.7/LICENSE
--rw-rw-rw-   0        0        0     5902 2023-08-17 10:05:09.531017 circular-dict-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4258 2023-06-20 08:15:45.000000 circular-dict-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-17 10:05:09.486822 circular-dict-1.7/circular_dict/
--rw-rw-rw-   0        0        0     7784 2023-08-17 10:05:01.000000 circular-dict-1.7/circular_dict/CircularDict.py
--rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.7/circular_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-17 10:05:09.529986 circular-dict-1.7/circular_dict.egg-info/
--rw-rw-rw-   0        0        0     5902 2023-08-17 10:05:09.000000 circular-dict-1.7/circular_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-17 10:05:09.000000 circular-dict-1.7/circular_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-17 10:05:09.000000 circular-dict-1.7/circular_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-17 10:05:09.000000 circular-dict-1.7/circular_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-17 10:05:09.532633 circular-dict-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-08-17 10:04:11.000000 circular-dict-1.7/setup.py
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-05-12 16:49:07.496316 circular_dict-1.8/
+-rw-r--r--   0 haru       (501) staff       (20)     1068 2024-05-12 16:23:53.000000 circular_dict-1.8/LICENSE
+-rw-r--r--   0 haru       (501) staff       (20)     5782 2024-05-12 16:49:07.496090 circular_dict-1.8/PKG-INFO
+-rw-r--r--   0 haru       (501) staff       (20)     4167 2024-05-12 16:23:53.000000 circular_dict-1.8/README.md
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-05-12 16:49:07.495213 circular_dict-1.8/circular_dict/
+-rw-r--r--   0 haru       (501) staff       (20)     8208 2024-05-12 16:43:34.000000 circular_dict-1.8/circular_dict/CircularDict.py
+-rw-r--r--   0 haru       (501) staff       (20)       38 2024-05-12 16:23:53.000000 circular_dict-1.8/circular_dict/__init__.py
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-05-12 16:49:07.495891 circular_dict-1.8/circular_dict.egg-info/
+-rw-r--r--   0 haru       (501) staff       (20)     5782 2024-05-12 16:49:07.000000 circular_dict-1.8/circular_dict.egg-info/PKG-INFO
+-rw-r--r--   0 haru       (501) staff       (20)      230 2024-05-12 16:49:07.000000 circular_dict-1.8/circular_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 haru       (501) staff       (20)        1 2024-05-12 16:49:07.000000 circular_dict-1.8/circular_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 haru       (501) staff       (20)       14 2024-05-12 16:49:07.000000 circular_dict-1.8/circular_dict.egg-info/top_level.txt
+-rw-r--r--   0 haru       (501) staff       (20)       38 2024-05-12 16:49:07.496362 circular_dict-1.8/setup.cfg
+-rw-r--r--   0 haru       (501) staff       (20)     1827 2024-05-12 16:44:34.000000 circular_dict-1.8/setup.py
```

### Comparing `circular-dict-1.7/PKG-INFO` & `circular_dict-1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-Metadata-Version: 2.1
-Name: circular-dict
-Version: 1.7
-Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
-Home-page: https://github.com/Eric-Canas/CircularDict
-Author: Eric-Canas
-Author-email: eric@ericcanas.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: System :: Hardware
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Debuggers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CircularDict
-<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
-
-Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
-
-## Installation
-
-To install **CircularDict** simply run:
-
-```bash
-pip install circular-dict
-```
-
-## Usage
-
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
-```python
-from circular_dict import CircularDict
-# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
-my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
-```
-
-### Example with `maxlen`
-You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
-
-```python
-from circular_dict import CircularDict
-
-# Initialize a CircularDict with a maximum length of 3
-my_buffer = CircularDict(maxlen=3)
-
-# Fill it with 3 items
-my_buffer['item1'] = 'value1'
-my_buffer['item2'] = 'value2'
-my_buffer['item3'] = 'value3'
-
-print(f"When filling it: {circ_dict}")
-
-# Add another item
-my_buffer['item4'] = 'value4'
-
-print(f"After adding an element beyond maxlen: {circ_dict}")
-```
-
-Output:
-```bash
-When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
-After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
-```
-
-### Example with `maxsize_bytes`
-You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
-
-```python
-from circular_dict import CircularDict
-import numpy as np
-import sys
-
-# Initialize a CircularDict with a maximum length of 100KB
-my_buffer = CircularDict(maxsize_bytes=100*1024)
-
-# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
-my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
-my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
-my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
-too_big_array = np.ones((40, 1024), dtype=np.int32)
-try:
-  # Try to add it to the dict
-  my_buffer['item4'] = too_big_array
-except MemoryError:
-  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
-        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
-```
-
-Output
-
-```bash
-2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
-2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
-Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
-```
-
-Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
+Metadata-Version: 2.1
+Name: circular-dict
+Version: 1.8
+Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
+Home-page: https://github.com/Eric-Canas/CircularDict
+Author: Eric-Canas
+Author-email: eric@ericcanas.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: System :: Hardware
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Debuggers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CircularDict
+<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
+
+Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
+
+## Installation
+
+To install **CircularDict** simply run:
+
+```bash
+pip install circular-dict
+```
+
+## Usage
+
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
+
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+
+```python
+from circular_dict import CircularDict
+
+# Initialize a CircularDict with a maximum length of 3
+my_buffer = CircularDict(maxlen=3)
+
+# Fill it with 3 items
+my_buffer['item1'] = 'value1'
+my_buffer['item2'] = 'value2'
+my_buffer['item3'] = 'value3'
+
+print(f"When filling it: {circ_dict}")
+
+# Add another item
+my_buffer['item4'] = 'value4'
+
+print(f"After adding an element beyond maxlen: {circ_dict}")
+```
+
+Output:
+```bash
+When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
+After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
+```
+
+### Example with `maxsize_bytes`
+You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
+
+```python
+from circular_dict import CircularDict
+import numpy as np
+import sys
+
+# Initialize a CircularDict with a maximum length of 100KB
+my_buffer = CircularDict(maxsize_bytes=100*1024)
+
+# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
+my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
+my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
+my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
+too_big_array = np.ones((40, 1024), dtype=np.int32)
+try:
+  # Try to add it to the dict
+  my_buffer['item4'] = too_big_array
+except MemoryError:
+  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
+        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
+```
+
+Output
+
+```bash
+2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
+2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
+Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
+```
+
+Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
```

### Comparing `circular-dict-1.7/README.md` & `circular_dict-1.8/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# CircularDict
-<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
-
-Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
-
-## Installation
-
-To install **CircularDict** simply run:
-
-```bash
-pip install circular-dict
-```
-
-## Usage
-
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
-```python
-from circular_dict import CircularDict
-# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
-my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
-```
-
-### Example with `maxlen`
-You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
-
-```python
-from circular_dict import CircularDict
-
-# Initialize a CircularDict with a maximum length of 3
-my_buffer = CircularDict(maxlen=3)
-
-# Fill it with 3 items
-my_buffer['item1'] = 'value1'
-my_buffer['item2'] = 'value2'
-my_buffer['item3'] = 'value3'
-
-print(f"When filling it: {circ_dict}")
-
-# Add another item
-my_buffer['item4'] = 'value4'
-
-print(f"After adding an element beyond maxlen: {circ_dict}")
-```
-
-Output:
-```bash
-When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
-After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
-```
-
-### Example with `maxsize_bytes`
-You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
-
-```python
-from circular_dict import CircularDict
-import numpy as np
-import sys
-
-# Initialize a CircularDict with a maximum length of 100KB
-my_buffer = CircularDict(maxsize_bytes=100*1024)
-
-# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
-my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
-my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
-my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
-too_big_array = np.ones((40, 1024), dtype=np.int32)
-try:
-  # Try to add it to the dict
-  my_buffer['item4'] = too_big_array
-except MemoryError:
-  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
-        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
-```
-
-Output
-
-```bash
-2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
-2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
-Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
-```
-
-Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
+# CircularDict
+<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
+
+Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
+
+## Installation
+
+To install **CircularDict** simply run:
+
+```bash
+pip install circular-dict
+```
+
+## Usage
+
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
+
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+
+```python
+from circular_dict import CircularDict
+
+# Initialize a CircularDict with a maximum length of 3
+my_buffer = CircularDict(maxlen=3)
+
+# Fill it with 3 items
+my_buffer['item1'] = 'value1'
+my_buffer['item2'] = 'value2'
+my_buffer['item3'] = 'value3'
+
+print(f"When filling it: {circ_dict}")
+
+# Add another item
+my_buffer['item4'] = 'value4'
+
+print(f"After adding an element beyond maxlen: {circ_dict}")
+```
+
+Output:
+```bash
+When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
+After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
+```
+
+### Example with `maxsize_bytes`
+You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
+
+```python
+from circular_dict import CircularDict
+import numpy as np
+import sys
+
+# Initialize a CircularDict with a maximum length of 100KB
+my_buffer = CircularDict(maxsize_bytes=100*1024)
+
+# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
+my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
+my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
+my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
+too_big_array = np.ones((40, 1024), dtype=np.int32)
+try:
+  # Try to add it to the dict
+  my_buffer['item4'] = too_big_array
+except MemoryError:
+  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
+        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
+```
+
+Output
+
+```bash
+2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
+2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
+Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
+```
+
+Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
```

### Comparing `circular-dict-1.7/circular_dict/CircularDict.py` & `circular_dict-1.8/circular_dict/CircularDict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,182 @@
-"""
-CircularDict: A dictionary that operates as a circular buffer, removing the oldest item when either maxlen or
-              maxsize (in bytes) is exceeded. Useful for caching large items without using too much memory. This
-              class is an implementation of the OrderedDict from the collections module and is designed to be
-              highly efficient and scalable for use cases that require both, dictionary-like and
-              circular-queue-like operations.
-
-Author: Eric Canas
-Date: 19-06-2023
-Email: eric@ericcanas.com
-Github: https://github.com/Eric-Canas
-"""
-
-import sys
-from collections import OrderedDict
-from typing import Any, Optional, Tuple
-
-class CircularDict(OrderedDict):
-    """
-    A dictionary that operates as a circular buffer, removing the oldest item when either maxlen or
-    maxsize (in bytes) is exceeded.
-
-    :param maxlen: Optional[int]. The maximum number of items in the dictionary.
-    :param maxsize_bytes: Optional[int]. The maximum size of the dictionary in bytes.
-    """
-
-    def __init__(self, maxlen: Optional[int] = None, maxsize_bytes: Optional[int] = None, *args, **kwargs):
-        """
-        Initialize CircularDict.
-
-        :param maxlen: Optional[int]. Maximum number of items in the dictionary.
-        :param maxsize_bytes: Optional[int]. Maximum size of items in the dictionary in bytes.
-        :param args: Positional arguments passed to OrderedDict.
-        :param kwargs: Keyword arguments passed to OrderedDict.
-        """
-        assert maxlen is not None or maxsize_bytes is not None, "Either maxlen or maxsize must be set"
-        self.maxlen = maxlen
-        self.maxsize_bytes = maxsize_bytes
-        self.current_size = 0
-        super().__init__(*args, **kwargs)
-
-    def is_empty(self) -> bool:
-        """
-        Check if the dictionary is empty.
-
-        :return: bool. True if empty, False otherwise.
-        """
-        empty = len(self) == 0
-        if empty:
-            assert self.current_size == 0, f"currentsize must be 0 when the dictionary is empty. currentsize={self.current_size}"
-        return empty
-
-    def is_full(self) -> bool:
-        """
-        Check if the dictionary is full. A full dictionary will remove the oldest item when a new item is added.
-
-        :return: bool. True if full, False otherwise.
-        """
-        if self.maxsize_bytes is not None:
-            assert self.current_size <= self.maxsize_bytes, f"currentsize must be less than or equal to maxsize. currentsize={self.current_size}, maxsize={self.maxsize_bytes}"
-
-        if self.maxlen is not None:
-            assert len(self) <= self.maxlen, f"len(self) must be less than or equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
-
-        return (self.maxlen is not None and len(self) == self.maxlen) or (self.maxsize_bytes is not None and self.current_size == self.maxsize_bytes)
-
-    def clear(self):
-        """
-        Remove all items from the dictionary.
-        """
-        super().clear()
-        self.current_size = 0
-
-    def __setitem__(self, key: Any, value: Any):
-        """
-        Set an item in the dictionary. If the key already exists, it will update the value.
-        If the dictionary exceeds maxlen or maxsize, it will remove the oldest item until it no longer does.
-
-        :param key: Any. Key to set or update. (It must be hashable)
-        :param value: Any. Value to associate with the key.
-        """
-        item_size = sys.getsizeof(key) + sys.getsizeof(value)
-
-        # If the element could not fit in the empty dictionary, raise an error
-        if self.maxsize_bytes is not None:
-            if item_size > self.maxsize_bytes:
-                raise MemoryError(f"Item size {item_size} is larger than maxsize {self.maxsize_bytes}")
-
-        # Delete the previous item if it exists to update the size accurately
-        if key in self:
-            del self[key]
-
-        # Keep removing oldest items until there's enough space
-        while self.maxsize_bytes is not None and self.current_size + item_size > self.maxsize_bytes:
-            self.popitem(last=False)
-        # Keep removing oldest items until there's
-        while self.maxlen is not None and len(self) >= self.maxlen:
-            assert len(self) == self.maxlen, f"len(self) must be equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
-            self.popitem(last=False)
-
-        OrderedDict.__setitem__(self, key, value)
-        self.current_size += item_size  # add size of new item
-
-    def __delitem__(self, key: Any):
-        """
-        Delete an item from the dictionary.
-
-        :param key: Any. The key of the item to delete.
-        """
-        if key in self:
-            value = self[key]
-            self.current_size -= sys.getsizeof(key) + sys.getsizeof(value)
-            OrderedDict.__delitem__(self, key)
-
-    def pop(self, key: Any, default: Optional[Any] = None) -> Any:
-        """
-        Remove specified key and return the corresponding value. Override of the default pop method,
-        adapted to work with independently of the Python version (as Python 3.11 (and possibly later versions)
-        does not call __delitem__ when popping).
-        :param key: Any. The key of the item to pop.
-        :param default: Any. The default value to return if the key is not found.
-        :return: Any. The value associated with the key, or the default value if the key is not found.
-        """
-        # As pop doesn't work as expected with Python 3.11, this is a workaround
-        if key not in self:
-            if default is None:
-                raise KeyError(key)
-            return default
-
-        prev_size = self.current_size
-        element = super().pop(key)
-
-        element_size = sys.getsizeof(key) + sys.getsizeof(element)
-
-        # If size did not change, because __delitem__ was not called (Python 3.11), then we must remove it manually
-        if self.current_size == prev_size:
-            self.current_size -= element_size
-        else:
-            # Otherwise, just assert to make sure everything is working as expected
-            assert self.current_size == prev_size - element_size, f"currentsize must be equal to prev_size - element_size. currentsize={self.current_size}, prev_size={prev_size}, element_size={element_size}"
-
-        return element
-
-    def popitem(self, last: bool = True) -> Tuple[Any, Any]:
-        """
-        Remove and return a (key, value) pair from the dictionary.
-        Pairs are returned in LIFO order if last is true or FIFO order if false.
-        Override of the default popitem method, adapted to work independently of the
-        Python version (as Python 3.11 (and possibly later versions) does not call __delitem__
-        when popitem is used).
-
-        :param last: bool. Return the last item (LIFO) if True, and the first item (FIFO) if False.
-        :return: Tuple[Any, Any]. A key-value pair.
-        """
-
-        prev_size = self.current_size
-        key, element = super().popitem(last=last)
-        element_size = sys.getsizeof(key) + sys.getsizeof(element)
-
-        # If size did not change, because __delitem__ was not called (Python 3.11), then we must remove it manually
-        if self.current_size == prev_size:
-            self.current_size -= element_size
-        else:
-            # Otherwise, just assert to make sure everything is working as expected
-            assert self.current_size == prev_size - element_size, f"currentsize must be equal to prev_size - element_size. currentsize={self.current_size}, prev_size={prev_size}, element_size={element_size}"
-
-        return key, element
-
+"""
+CircularDict: A dictionary that operates as a circular buffer, removing the oldest item when either maxlen or
+              maxsize (in bytes) is exceeded. Useful for caching large items without using too much memory. This
+              class is an implementation of the OrderedDict from the collections module and is designed to be
+              highly efficient and scalable for use cases that require both, dictionary-like and
+              circular-queue-like operations.
+
+Author: Eric Canas
+Date: 19-06-2023
+Email: eric@ericcanas.com
+Github: https://github.com/Eric-Canas
+"""
+
+import sys
+from collections import OrderedDict
+from typing import Any, Optional, Tuple
+
+# To make sure it is compatible with PyPy environments (PyPy does not have sys.getsizeof for all types)
+try:
+    sys.getsizeof("Exist Check")
+    getsizeof_available = True
+except TypeError:
+    sys.getsizeof = lambda x: 0
+    getsizeof_available = False
+
+
+class CircularDict(OrderedDict):
+    """
+    A dictionary that operates as a circular buffer, removing the oldest item when either maxlen or
+    maxsize (in bytes) is exceeded.
+
+    :param maxlen: Optional[int]. The maximum number of items in the dictionary.
+    :param maxsize_bytes: Optional[int]. The maximum size of the dictionary in bytes.
+    """
+
+    def __init__(self, maxlen: Optional[int] = None, maxsize_bytes: Optional[int] = None, *args, **kwargs):
+        """
+        Initialize CircularDict.
+
+        :param maxlen: Optional[int]. Maximum number of items in the dictionary.
+        :param maxsize_bytes: Optional[int]. Maximum size of items in the dictionary in bytes.
+        :param args: Positional arguments passed to OrderedDict.
+        :param kwargs: Keyword arguments passed to OrderedDict.
+        """
+        assert maxlen is not None or maxsize_bytes is not None, "Either maxlen or maxsize must be set"
+        if not getsizeof_available:
+            assert maxsize_bytes is None, ("sys.getsizeof is not available for all types in this environment. "
+                                           "That's common on, for example PyPy environments."
+                                           "maxsize_bytes cannot be used. Set it to None.")
+
+        self.maxlen = maxlen
+        self.maxsize_bytes = maxsize_bytes
+        self.current_size = 0
+        super().__init__(*args, **kwargs)
+
+    def is_empty(self) -> bool:
+        """
+        Check if the dictionary is empty.
+
+        :return: bool. True if empty, False otherwise.
+        """
+        empty = len(self) == 0
+        if empty:
+            assert self.current_size == 0, f"currentsize must be 0 when the dictionary is empty. currentsize={self.current_size}"
+        return empty
+
+    def is_full(self) -> bool:
+        """
+        Check if the dictionary is full. A full dictionary will remove the oldest item when a new item is added.
+
+        :return: bool. True if full, False otherwise.
+        """
+        if self.maxsize_bytes is not None:
+            assert self.current_size <= self.maxsize_bytes, f"currentsize must be less than or equal to maxsize. currentsize={self.current_size}, maxsize={self.maxsize_bytes}"
+
+        if self.maxlen is not None:
+            assert len(self) <= self.maxlen, f"len(self) must be less than or equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
+
+        return (self.maxlen is not None and len(self) == self.maxlen) or (self.maxsize_bytes is not None and self.current_size == self.maxsize_bytes)
+
+    def clear(self):
+        """
+        Remove all items from the dictionary.
+        """
+        super().clear()
+        self.current_size = 0
+
+    def __setitem__(self, key: Any, value: Any):
+        """
+        Set an item in the dictionary. If the key already exists, it will update the value.
+        If the dictionary exceeds maxlen or maxsize, it will remove the oldest item until it no longer does.
+
+        :param key: Any. Key to set or update. (It must be hashable)
+        :param value: Any. Value to associate with the key.
+        """
+        item_size = sys.getsizeof(key) + sys.getsizeof(value)
+
+        # If the element could not fit in the empty dictionary, raise an error
+        if self.maxsize_bytes is not None:
+            if item_size > self.maxsize_bytes:
+                raise MemoryError(f"Item size {item_size} is larger than maxsize {self.maxsize_bytes}")
+
+        # Delete the previous item if it exists to update the size accurately
+        if key in self:
+            del self[key]
+
+        # Keep removing oldest items until there's enough space
+        while self.maxsize_bytes is not None and self.current_size + item_size > self.maxsize_bytes:
+            self.popitem(last=False)
+        # Keep removing oldest items until there's
+        while self.maxlen is not None and len(self) >= self.maxlen:
+            assert len(self) == self.maxlen, f"len(self) must be equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
+            self.popitem(last=False)
+
+        OrderedDict.__setitem__(self, key, value)
+        self.current_size += item_size  # add size of new item
+
+    def __delitem__(self, key: Any):
+        """
+        Delete an item from the dictionary.
+
+        :param key: Any. The key of the item to delete.
+        """
+        if key in self:
+            value = self[key]
+            self.current_size -= sys.getsizeof(key) + sys.getsizeof(value)
+            OrderedDict.__delitem__(self, key)
+
+    def pop(self, key: Any, default: Optional[Any] = None) -> Any:
+        """
+        Remove specified key and return the corresponding value. Override of the default pop method,
+        adapted to work with independently of the Python version (as Python 3.11 (and possibly later versions)
+        does not call __delitem__ when popping).
+        :param key: Any. The key of the item to pop.
+        :param default: Any. The default value to return if the key is not found.
+        :return: Any. The value associated with the key, or the default value if the key is not found.
+        """
+        # As pop doesn't work as expected with Python 3.11, this is a workaround
+        if key not in self:
+            if default is None:
+                raise KeyError(key)
+            return default
+
+        prev_size = self.current_size
+        element = super().pop(key)
+
+        element_size = sys.getsizeof(key) + sys.getsizeof(element)
+
+        # If size did not change, because __delitem__ was not called (Python 3.11), then we must remove it manually
+        if self.current_size == prev_size:
+            self.current_size -= element_size
+        else:
+            # Otherwise, just assert to make sure everything is working as expected
+            assert self.current_size == prev_size - element_size, f"currentsize must be equal to prev_size - element_size. currentsize={self.current_size}, prev_size={prev_size}, element_size={element_size}"
+
+        return element
+
+    def popitem(self, last: bool = True) -> Tuple[Any, Any]:
+        """
+        Remove and return a (key, value) pair from the dictionary.
+        Pairs are returned in LIFO order if last is true or FIFO order if false.
+        Override of the default popitem method, adapted to work independently of the
+        Python version (as Python 3.11 (and possibly later versions) does not call __delitem__
+        when popitem is used).
+
+        :param last: bool. Return the last item (LIFO) if True, and the first item (FIFO) if False.
+        :return: Tuple[Any, Any]. A key-value pair.
+        """
+
+        prev_size = self.current_size
+        key, element = super().popitem(last=last)
+        element_size = sys.getsizeof(key) + sys.getsizeof(element)
+
+        # If size did not change, because __delitem__ was not called (Python 3.11), then we must remove it manually
+        if self.current_size == prev_size:
+            self.current_size -= element_size
+        else:
+            # Otherwise, just assert to make sure everything is working as expected
+            assert self.current_size == prev_size - element_size, f"currentsize must be equal to prev_size - element_size. currentsize={self.current_size}, prev_size={prev_size}, element_size={element_size}"
+
+        return key, element
+
```

### Comparing `circular-dict-1.7/circular_dict.egg-info/PKG-INFO` & `circular_dict-1.8/circular_dict.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-Metadata-Version: 2.1
-Name: circular-dict
-Version: 1.7
-Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
-Home-page: https://github.com/Eric-Canas/CircularDict
-Author: Eric-Canas
-Author-email: eric@ericcanas.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: System :: Hardware
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Debuggers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CircularDict
-<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
-
-Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
-
-## Installation
-
-To install **CircularDict** simply run:
-
-```bash
-pip install circular-dict
-```
-
-## Usage
-
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
-```python
-from circular_dict import CircularDict
-# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
-my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
-```
-
-### Example with `maxlen`
-You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
-
-```python
-from circular_dict import CircularDict
-
-# Initialize a CircularDict with a maximum length of 3
-my_buffer = CircularDict(maxlen=3)
-
-# Fill it with 3 items
-my_buffer['item1'] = 'value1'
-my_buffer['item2'] = 'value2'
-my_buffer['item3'] = 'value3'
-
-print(f"When filling it: {circ_dict}")
-
-# Add another item
-my_buffer['item4'] = 'value4'
-
-print(f"After adding an element beyond maxlen: {circ_dict}")
-```
-
-Output:
-```bash
-When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
-After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
-```
-
-### Example with `maxsize_bytes`
-You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
-
-```python
-from circular_dict import CircularDict
-import numpy as np
-import sys
-
-# Initialize a CircularDict with a maximum length of 100KB
-my_buffer = CircularDict(maxsize_bytes=100*1024)
-
-# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
-my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
-my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
-my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
-
-print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
-
-# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
-too_big_array = np.ones((40, 1024), dtype=np.int32)
-try:
-  # Try to add it to the dict
-  my_buffer['item4'] = too_big_array
-except MemoryError:
-  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
-        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
-```
-
-Output
-
-```bash
-2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
-2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
-Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
-```
-
-Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
+Metadata-Version: 2.1
+Name: circular-dict
+Version: 1.8
+Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
+Home-page: https://github.com/Eric-Canas/CircularDict
+Author: Eric-Canas
+Author-email: eric@ericcanas.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: System :: Hardware
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Debuggers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CircularDict
+<img alt="CircularDict" title="CircularDict" src="https://raw.githubusercontent.com/Eric-Canas/CircularDict/main/resources/logo.png" width="20%" align="left"> **CircularDict** is a Python `dict` that acts as a **Circular Buffer**. This dictionary maintains a **controlled size**, limited either by a specified **number of items** (_maxlen_) or **total size in bytes** (_maxsize_bytes_). Upon reaching the defined limit, **CircularDict** automatically removes the oldest entries, maintaining **memory usage** under control.
+
+Built upon Python's `OrderedDict`, **CircularDict** inherits all **standard dictionary usage** and operations, augmented by the capability of **memory management**. It's particularly useful in scenarios such as **caching**, where limiting **memory consumption** is crucial. The class combines _dictionary_ and _circular-queue_ behaviors, providing an efficient and scalable solution for various use cases.
+
+## Installation
+
+To install **CircularDict** simply run:
+
+```bash
+pip install circular-dict
+```
+
+## Usage
+
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
+
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+
+```python
+from circular_dict import CircularDict
+
+# Initialize a CircularDict with a maximum length of 3
+my_buffer = CircularDict(maxlen=3)
+
+# Fill it with 3 items
+my_buffer['item1'] = 'value1'
+my_buffer['item2'] = 'value2'
+my_buffer['item3'] = 'value3'
+
+print(f"When filling it: {circ_dict}")
+
+# Add another item
+my_buffer['item4'] = 'value4'
+
+print(f"After adding an element beyond maxlen: {circ_dict}")
+```
+
+Output:
+```bash
+When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
+After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
+```
+
+### Example with `maxsize_bytes`
+You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
+
+```python
+from circular_dict import CircularDict
+import numpy as np
+import sys
+
+# Initialize a CircularDict with a maximum length of 100KB
+my_buffer = CircularDict(maxsize_bytes=100*1024)
+
+# Add two arrays of ~40Kb (10*1024*4 bytes (int32) + 5 bytes (chars) + 100 bytes (numpy structure) + 50 bytes (str structure))
+my_buffer['item1'] = np.zeros((10, 1024), dtype=np.int32)
+my_buffer['item2'] = np.ones((10, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Add a new element of ~32Kb will delete oldest elements ('item1') until fitting in the `dict`.
+my_buffer['item3'] = np.ones((8, 1024), dtype=np.int32)
+
+print(f"{len(my_buffer)} Elements {tuple(my_buffer.keys())}. Dict size: {my_buffer.current_size/1024} Kb")
+
+# Create an element of ~160Kb (bigger than the defined maximum storage) to trigger a MemoryError
+too_big_array = np.ones((40, 1024), dtype=np.int32)
+try:
+  # Try to add it to the dict
+  my_buffer['item4'] = too_big_array
+except MemoryError:
+  print(f"Cannot add an element with {sys.getsizeof(too_big_array)/1024}Kb in a dict with"\
+        f"maxsize_bytes of {my_buffer.maxsize_bytes/1024} Kb. Current elements {tuple(my_buffer.keys())}")
+```
+
+Output
+
+```bash
+2 Elements ('item1', 'item2'). Dict size: 80.35 Kb
+2 Elements ('item2', 'item3'). Dict size: 72.35 Kb
+Cannot add an element with 160.12Kb in a dict with maxsize_bytes of 100.0 Kb. Current elements ('item2', 'item3')
+```
+
+Please remember that the `maxsize_bytes` parameter considers the **total** memory footprint, including the sizes of _keys_ and _values_. If you try to add an item that exceeds the `maxsize_bytes`, a `MemoryError` will be raised.
```

### Comparing `circular-dict-1.7/setup.py` & `circular_dict-1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='circular-dict',
-    version='1.7',
-    author='Eric-Canas',
-    author_email='eric@ericcanas.com',
-    url='https://github.com/Eric-Canas/CircularDict',
-    description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
-                'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
-                'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
-                'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
-    long_description=open('README.md', 'r').read(),
-    long_description_content_type='text/markdown',
-    license='MIT',
-    packages=find_packages(),
-    python_requires='>=3.6',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Operating System :: OS Independent',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Topic :: System :: Hardware',
-        'Topic :: Software Development :: Testing',
-        'Topic :: Software Development :: Debuggers',
-    ],
+from setuptools import setup, find_packages
+
+setup(
+    name='circular-dict',
+    version='1.8',
+    author='Eric-Canas',
+    author_email='eric@ericcanas.com',
+    url='https://github.com/Eric-Canas/CircularDict',
+    description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
+                'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
+                'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
+                'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
+    long_description=open('README.md', 'r').read(),
+    long_description_content_type='text/markdown',
+    license='MIT',
+    packages=find_packages(),
+    python_requires='>=3.6',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Operating System :: OS Independent',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Topic :: System :: Hardware',
+        'Topic :: Software Development :: Testing',
+        'Topic :: Software Development :: Debuggers',
+    ],
 )
```

