# Comparing `tmp/dooth-1.0.1-py3-none-any.whl.zip` & `tmp/dooth-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 4448 bytes, number of entries: 10
+Zip file size: 5522 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 24-May-10 18:16 doot/__init__.py
--rw-r--r--  2.0 unx     4639 b- defN 24-May-12 12:35 doot/bot.py
--rw-r--r--  2.0 unx      371 b- defN 24-May-10 19:21 doot/command_handler.py
+-rw-r--r--  2.0 unx     8186 b- defN 24-May-12 15:11 doot/bot.py
+-rw-r--r--  2.0 unx      454 b- defN 24-May-12 14:37 doot/command_handler.py
 -rw-r--r--  2.0 unx      232 b- defN 24-May-12 12:24 doot/exception.py
 -rw-r--r--  2.0 unx     4255 b- defN 24-May-11 09:22 doot/message.py
--rw-r--r--  2.0 unx      352 b- defN 24-May-10 19:17 doot/message_handler.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      728 b- defN 24-May-12 12:37 dooth-1.0.1.dist-info/RECORD
-10 files, 10748 bytes uncompressed, 3216 bytes compressed:  70.1%
+-rw-r--r--  2.0 unx      444 b- defN 24-May-12 14:37 doot/message_handler.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-May-12 15:15 doot/response.py
+-rw-r--r--  2.0 unx       74 b- defN 24-May-12 15:22 dooth-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:22 dooth-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-12 15:22 dooth-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      801 b- defN 24-May-12 15:22 dooth-1.1.0.dist-info/RECORD
+11 files, 17070 bytes uncompressed, 4182 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -12,20 +12,23 @@
 
 Filename: doot/message.py
 Comment: 
 
 Filename: doot/message_handler.py
 Comment: 
 
-Filename: dooth-1.0.1.dist-info/METADATA
+Filename: doot/response.py
 Comment: 
 
-Filename: dooth-1.0.1.dist-info/WHEEL
+Filename: dooth-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: dooth-1.0.1.dist-info/top_level.txt
+Filename: dooth-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: dooth-1.0.1.dist-info/RECORD
+Filename: dooth-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: dooth-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doot/bot.py

```diff
@@ -1,57 +1,111 @@
 import asyncio
 import datetime
 import json
 import logging
+import os
 import threading
 import time
 
 import requests
 from urllib.parse import quote
 
 from doot.command_handler import CommandHandler, DefaultCommandHandler
 from doot.exception import CommandProcessingError, MessageProcessingError
 from doot.message import Mapper, Update
 from doot.message_handler import MessageHandler, DefaultMessageHandler
+from doot.response import HandlerResponse
 
 
 class Bot:
 
     def __init__(self, token: str):
         self.__logger = logging.getLogger(self.__class__.__name__)
         self.__base_url = f'https://api.telegram.org/bot{token}'
         self.__send_msg_url = f'{self.__base_url}/sendMessage'
         self.__get_updates_url = f'{self.__base_url}/getUpdates'
+        self.__send_photo_url = f'{self.__base_url}/sendPhoto'
+        self.__send_doc_url = f'{self.__base_url}/sendDocument'
         self.__next_update_id = -1
 
         self.command_handler: CommandHandler = DefaultCommandHandler()
         self.message_handler: MessageHandler = DefaultMessageHandler()
 
-    def send_notification(self, message: str, chat_id: int,
-                          disable_web_page_preview: bool = False,
-                          parse_mode: str = 'HTML'):
+    def send_notification(self, response: HandlerResponse, chat_id: int, disable_web_page_preview: bool = False):
 
         params = {
             'chat_id': chat_id,
-            'text': message,
-            'parse_mode': parse_mode,
+            'text': response.get_message(),
+            'parse_mode': response.get_message_parse_mode(),
             'disable_web_page_preview': str(disable_web_page_preview)
         }
         try:
             response = requests.post(self.__send_msg_url, params=params, timeout=5)
             response.raise_for_status()  # Raise an error if response status code is not 200
         except requests.exceptions.RequestException as e:
             logging.error(f"Error sending message: {e}")
             raise e
         else:
             if response.status_code != 200:
                 logging.error(f"Error: {response.text}")
             else:
                 logging.info("Message sent successfully.")
 
+    def send_photo(self, response: HandlerResponse, chat_id: int, disable_web_page_preview: bool = False):
+
+        files = {
+            'photo': open(response.get_photo_path(), 'rb'),
+        }
+
+        form_data = {
+            'chat_id': chat_id,
+            'caption': response.get_message(),
+            'parse_mode': response.get_message_parse_mode(),
+            'disable_web_page_preview': str(disable_web_page_preview)
+        }
+        try:
+            response = requests.post(self.__send_photo_url, data=form_data, files=files, timeout=5)
+            response.raise_for_status()  # Raise an error if response status code is not 200
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Error sending message: {e}")
+            raise e
+        else:
+            if response.status_code != 200:
+                logging.error(f"Error: {response.text}")
+            else:
+                logging.info("Message sent successfully.")
+        finally:
+            files['photo'].close()
+
+    def send_doc(self, response: HandlerResponse, chat_id: int, disable_web_page_preview: bool = False):
+
+        files = {
+            'document': open(response.get_document_path(), 'rb'),
+        }
+
+        form_data = {
+            'chat_id': chat_id,
+            'caption': response.get_message(),
+            'parse_mode': response.get_message_parse_mode(),
+            'disable_web_page_preview': str(disable_web_page_preview)
+        }
+        try:
+            response = requests.post(self.__send_doc_url, data=form_data, files=files, timeout=5)
+            response.raise_for_status()  # Raise an error if response status code is not 200
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Error sending message: {e}")
+            raise e
+        else:
+            if response.status_code != 200:
+                logging.error(f"Error: {response.text}")
+            else:
+                logging.info("Message sent successfully.")
+        finally:
+            files['document'].close()
+
     def _fetch_updates(self):
         params = {
             'offset': self.__next_update_id
         }
         try:
             response = requests.post(self.__get_updates_url, params=params, timeout=5)
             response.raise_for_status()  # Raise an error if response status code is not 200
@@ -72,26 +126,58 @@
     def _process_command(self, update: Update):
         args = []
         for e in update.message.text.split(' '):
             if e != '':
                 args.append(e)
         command = args.pop(0)
 
+        response = None
         try:
-            reply = self.command_handler.handle_command(command, args)
-            self.send_notification(reply, update.message.chat.id)
+            response = self.command_handler.handle_command(command, args)
+            self.respond(response, update)
         except Exception as e:
             raise CommandProcessingError(e)
+        finally:
+            self._delete_files_in_response(response)
 
     def _process_message(self, update: Update):
+        response = None
         try:
-            reply = self.message_handler.handle_message(update.message.text)
-            self.send_notification(reply, update.message.chat.id)
+            response = self.message_handler.handle_message(update.message.text)
+            self.respond(response, update)
         except Exception as e:
             raise MessageProcessingError(e)
+        finally:
+            self._delete_files_in_response(response)
+
+    def respond(self, response: HandlerResponse, update: Update):
+        if response.get_type() == 'text':
+            self.send_notification(response, update.message.chat.id)
+        elif response.get_type() == 'photo':
+            self.send_photo(response, update.message.chat.id)
+        elif response.get_type() == 'document':
+            self.send_doc(response, update.message.chat.id)
+
+    def _delete_files_in_response(self, response: HandlerResponse):
+        if response is None:
+            return
+
+        if response.get_photo_path() is not None:
+            try:
+                os.remove(response.get_photo_path())
+            except Exception as e:
+                self.__logger.warning(f'Failed to delete file: {response.get_photo_path()}: {e}',
+                                      stack_info=True, exc_info=True)
+
+        if response.get_document_path() is not None:
+            try:
+                os.remove(response.get_document_path())
+            except Exception as e:
+                self.__logger.warning(f'Failed to delete file: {response.get_photo_path()}: {e}',
+                                      stack_info=True, exc_info=True)
 
     def __drive(self, poll_delay: float):
         while True:
             try:
 
                 updates = self._fetch_updates()
                 for u in updates:
@@ -100,19 +186,21 @@
                             self._process_command(u)
                         else:
                             self._process_message(u)
                     except MessageProcessingError as e:
                         self.__logger.error(f'Exception in processing update: {e}:\n{u}',
                                             stack_info=True, exc_info=True)
                         # just so we can move on
-                        self.send_notification('Error in processing', u.message.chat.id)
+                        self.send_notification(HandlerResponse(message='Error in processing.'), u.message.chat.id)
                     time.sleep(poll_delay)
 
             except (ConnectionError, TimeoutError) as e:
                 self.__logger.error(f'Error ==> {e}', stack_info=True, exc_info=True)
                 time.sleep(15)  # To let systems recover
             except Exception as e:
                 self.__logger.error(f'Error ==> {e}', stack_info=True, exc_info=True)
 
     def start(self, poll_delay: float = 5):
         my_thread = threading.Thread(target=self.__drive, args=[poll_delay])
         my_thread.start()
+
+
```

## doot/command_handler.py

```diff
@@ -1,18 +1,19 @@
-import datetime
 from abc import ABC, abstractmethod
 
+from doot.response import HandlerResponse
+
 
 class CommandHandler(ABC):
 
     def __init__(self):
         pass
 
     @abstractmethod
-    def handle_command(self, command: str, args: list) -> str:
+    def handle_command(self, command: str, args: list) -> HandlerResponse:
         pass
 
 
 class DefaultCommandHandler(CommandHandler):
 
-    def handle_command(self, command: str, args: list):
-        return f'Command: {command}\nArgs: {args}'
+    def handle_command(self, command: str, args: list) -> HandlerResponse:
+        return HandlerResponse(message=f'Command: {command}\nArgs: {args}')
```

## doot/message_handler.py

```diff
@@ -1,18 +1,20 @@
 import datetime
 from abc import ABC, abstractmethod
 
+from doot.response import HandlerResponse
+
 
 class MessageHandler(ABC):
 
     def __init__(self):
         pass
 
     @abstractmethod
-    def handle_message(self, message_text: str) -> str:
+    def handle_message(self, message_text: str) -> HandlerResponse:
         pass
 
 
 class DefaultMessageHandler(MessageHandler):
 
-    def handle_message(self, message_text: str) -> str:
-        return f'Echo: {message_text}'
+    def handle_message(self, message_text: str) -> HandlerResponse:
+        return HandlerResponse(message=f'Echo: {message_text}')
```

## Comparing `dooth-1.0.1.dist-info/RECORD` & `dooth-1.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 doot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-doot/bot.py,sha256=lgsNNCa1EO8z8PE_FKn68_gSNjlYJAtjUaYUMq4QglE,4639
-doot/command_handler.py,sha256=kTPu6R1FzDIac6j64d27OvqxuoRoYylEgDaGqZT_elU,371
+doot/bot.py,sha256=scPAe9j27N5SofW4QHt0YsfSyoi10kdEppWeyUY_8Qs,8186
+doot/command_handler.py,sha256=euFeDZeJPHBgMR8EzAzGbyPJCitdIVVtapcIrut38pI,454
 doot/exception.py,sha256=Ys10w9WqxYIyzn6QPbkxoX_ykgMf_fTUDIH7UsRAWyQ,232
 doot/message.py,sha256=hiXeJ7TOTMvF2TGXj0fqbo3LTAxPi_lW6H1bMeG6UEI,4255
-doot/message_handler.py,sha256=gyP99ss3dA7ozCckejX7GtJbOP2WvEPbcWX4J6aLqZM,352
-dooth-1.0.1.dist-info/METADATA,sha256=Yq3gmouRpiUJPOB3KUNYJl5XdAKbz8ITAl1c66oSAo8,74
-dooth-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dooth-1.0.1.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
-dooth-1.0.1.dist-info/RECORD,,
+doot/message_handler.py,sha256=KwDN7B0ig7GUXjeo6PJ-1RLehz4ilyiBHA_dSXC9zFw,444
+doot/response.py,sha256=iAFsgMb3nEJ_gRizDFG7xv-euzIbqRZYVpL6KfsnLX0,2527
+dooth-1.1.0.dist-info/METADATA,sha256=OOLHjKSrtnkCVOUG16TycqO6Ou6yfV3wiY2fYcDcgr0,74
+dooth-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dooth-1.1.0.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
+dooth-1.1.0.dist-info/RECORD,,
```

