# Comparing `tmp/dooth-1.0.0-py3-none-any.whl.zip` & `tmp/dooth-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 4071 bytes, number of entries: 9
+Zip file size: 4448 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 24-May-10 18:16 doot/__init__.py
--rw-r--r--  2.0 unx     3966 b- defN 24-May-11 09:21 doot/bot.py
+-rw-r--r--  2.0 unx     4639 b- defN 24-May-12 12:35 doot/bot.py
 -rw-r--r--  2.0 unx      371 b- defN 24-May-10 19:21 doot/command_handler.py
+-rw-r--r--  2.0 unx      232 b- defN 24-May-12 12:24 doot/exception.py
 -rw-r--r--  2.0 unx     4255 b- defN 24-May-11 09:22 doot/message.py
 -rw-r--r--  2.0 unx      352 b- defN 24-May-10 19:17 doot/message_handler.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-11 09:25 dooth-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 09:25 dooth-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-11 09:25 dooth-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 24-May-11 09:25 dooth-1.0.0.dist-info/RECORD
-9 files, 9770 bytes uncompressed, 2949 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx       74 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      728 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/RECORD
+10 files, 10748 bytes uncompressed, 3216 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: doot/bot.py
 Comment: 
 
 Filename: doot/command_handler.py
 Comment: 
 
+Filename: doot/exception.py
+Comment: 
+
 Filename: doot/message.py
 Comment: 
 
 Filename: doot/message_handler.py
 Comment: 
 
-Filename: dooth-1.0.0.dist-info/METADATA
+Filename: dooth-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dooth-1.0.0.dist-info/WHEEL
+Filename: dooth-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dooth-1.0.0.dist-info/top_level.txt
+Filename: dooth-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dooth-1.0.0.dist-info/RECORD
+Filename: dooth-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doot/bot.py

```diff
@@ -5,14 +5,15 @@
 import threading
 import time
 
 import requests
 from urllib.parse import quote
 
 from doot.command_handler import CommandHandler, DefaultCommandHandler
+from doot.exception import CommandProcessingError, MessageProcessingError
 from doot.message import Mapper, Update
 from doot.message_handler import MessageHandler, DefaultMessageHandler
 
 
 class Bot:
 
     def __init__(self, token: str):
@@ -71,33 +72,47 @@
     def _process_command(self, update: Update):
         args = []
         for e in update.message.text.split(' '):
             if e != '':
                 args.append(e)
         command = args.pop(0)
 
-        reply = self.command_handler.handle_command(command, args)
-        self.send_notification(reply, update.message.chat.id)
+        try:
+            reply = self.command_handler.handle_command(command, args)
+            self.send_notification(reply, update.message.chat.id)
+        except Exception as e:
+            raise CommandProcessingError(e)
 
     def _process_message(self, update: Update):
-        reply = self.message_handler.handle_message(update.message.text)
-        self.send_notification(reply, update.message.chat.id)
+        try:
+            reply = self.message_handler.handle_message(update.message.text)
+            self.send_notification(reply, update.message.chat.id)
+        except Exception as e:
+            raise MessageProcessingError(e)
 
     def __drive(self, poll_delay: float):
         while True:
-            updates = self._fetch_updates()
-            for u in updates:
-                try:
-                    if u.message.text is not None and u.message.text.startswith('/'):
-                        self._process_command(u)
-                    else:
-                        self._process_message(u)
-                except Exception as e:
-                    self.__logger.error(f'Exception in processing update: {e}:\n{u}',
-                                        stack_info=True, exc_info=True)
-                    # just so we can move on
-                    self.send_notification('Error in processing', u.message.chat.id)
-                time.sleep(poll_delay)
+            try:
+
+                updates = self._fetch_updates()
+                for u in updates:
+                    try:
+                        if u.message.text is not None and u.message.text.startswith('/'):
+                            self._process_command(u)
+                        else:
+                            self._process_message(u)
+                    except MessageProcessingError as e:
+                        self.__logger.error(f'Exception in processing update: {e}:\n{u}',
+                                            stack_info=True, exc_info=True)
+                        # just so we can move on
+                        self.send_notification('Error in processing', u.message.chat.id)
+                    time.sleep(poll_delay)
+
+            except (ConnectionError, TimeoutError) as e:
+                self.__logger.error(f'Error ==> {e}', stack_info=True, exc_info=True)
+                time.sleep(15)  # To let systems recover
+            except Exception as e:
+                self.__logger.error(f'Error ==> {e}', stack_info=True, exc_info=True)
 
-    def start(self, poll_delay: int = 5):
+    def start(self, poll_delay: float = 5):
         my_thread = threading.Thread(target=self.__drive, args=[poll_delay])
         my_thread.start()
```

