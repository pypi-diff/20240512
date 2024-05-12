# Comparing `tmp/llmail-0.1.0.tar.gz` & `tmp/llmail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmail-0.1.0.tar", max compression
+gzip compressed data, was "llmail-0.1.1.tar", max compression
```

## Comparing `llmail-0.1.0.tar` & `llmail-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.1.0/LICENSE
--rw-r--r--   0        0        0     1560 2024-05-05 21:10:00.993783 llmail-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 23:31:53.519788 llmail-0.1.0/llmail/__init__.py
--rw-r--r--   0        0        0    21045 2024-05-05 20:55:16.342536 llmail-0.1.0/llmail/__main__.py
--rw-r--r--   0        0        0        0 2024-04-29 23:49:56.280104 llmail-0.1.0/llmail/utils/__init__.py
--rw-r--r--   0        0        0     3603 2024-05-05 20:55:16.341276 llmail-0.1.0/llmail/utils/cli_args.py
--rw-r--r--   0        0        0      747 2024-05-05 17:12:56.006502 llmail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 llmail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-29 23:31:53.519788 llmail-0.1.1/llmail/__init__.py
+-rw-r--r--   0        0        0    22080 2024-05-12 03:02:00.564879 llmail-0.1.1/llmail/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:49:56.280104 llmail-0.1.1/llmail/utils/__init__.py
+-rw-r--r--   0        0        0     4681 2024-05-12 02:54:37.168425 llmail-0.1.1/llmail/utils/cli_args.py
+-rw-r--r--   0        0        0      846 2024-05-12 02:23:16.253525 llmail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1532 2024-05-12 03:11:36.325088 llmail-0.1.1/README.md
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 llmail-0.1.1/PKG-INFO
```

### Comparing `llmail-0.1.0/LICENSE` & `llmail-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmail-0.1.0/README.md` & `llmail-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 # LLMail  
 Interact with Large Language Models (LLMs) via email.
 
 ### Features  
 - Utilize any OpenAI-compatible API
+    - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) offers free access to specific models with an OpenAI-compatible API
 - Check every _n_ seconds 
 - No need for a local database - uses IMAP
 
 ## Prerequisites  
 ### Python  
-- Python ^3.11
-- Poetry <!-- (optional)  -->
-- An API key from an OpenAI-compatible API
-    - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) provides free access to select models
-        - Right now, they are the only provider that will work due to the model being hard-coded (for now)
+- Python ^3.11  
+- Poetry (optional)  
+- An API key from an OpenAI-compatible API  
+### Docker
+- Docker  
 
 ## Usage  
-### Installation  
+### Installing from PyPi with `pip` (recommended)  
+This assumes you have the correct version of Python installed
+1. `pip install llmail`  
+    a. You may need to use `pip3` instead of `pip`  
+2. `llmail`  
+
+### Installation from source or with Docker
 Cloning the repository is not required when installing from PyPi but is required when installing from source  
 1. Clone this repo with `git clone https://github.com/slashtechno/llmail`  
 2. `cd` into the cloned repository  
-3. Install with [Poetry](https://python-poetry.org/) <!-- or [Docker](https://www.docker.com/) -->
+3. Install and run with one of the following methods:
 
-<!-- 
-#### Installing from PyPi with pip (recommended)  
-This assumes you have the correct version of Python installed
-1. `pip install llmail`  
-    a. You may need to use `pip3` instead of `pip`  
-2. `llmail`   -->
 
-#### Poetry  
+
+#### Poetry
 1. `poetry install`  
 2. `poetry run -- llmail`  
 
-<!-- #### Docker  -->
+#### Docker
+1. Configure with the steps below  
+2. `docker compose up -d`
+
 ### Configuration  
-To configure the program, either use CLI flags (`--help` for more information) or environment variables.  
-It is recommended to just copy .env.example to .env and fill in the necessary information.
+To configure the program, either use CLI flags (`--help` for more information) or environment variables.
+It is recommended to just copy `.env.example` to `.env` and fill in the necessary information.
 
 ### How to uninstall  
 - If you used Poetry, just delete the virtual environment and then the cloned repository
```

### Comparing `llmail-0.1.0/llmail/__main__.py` & `llmail-0.1.1/llmail/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import yagmail
 import html2text
 from icecream import ic
 from imapclient import IMAPClient
 import imaplib
 from loguru import logger
 from openai import OpenAI
-from email.utils import getaddresses, parsedate_to_datetime
+from email.utils import getaddresses, parsedate_to_datetime, make_msgid
 from datetime import timezone
 import time
 
 
 from llmail.utils.cli_args import argparser
 
 
@@ -24,15 +24,15 @@
     def add_reply(self, reply_email):
         # If the message_id of the reply email is not in the list of messages add it
         # Also, don't do it if the email is the inital/top-level email itself
         if (
             reply_email.message_id not in [email.message_id for email in self.replies]
             and reply_email.message_id != self.initial_email.message_id
         ):
-            logger.info(
+            logger.debug(
                 f"Reply sent by {reply_email.sender} at {reply_email.timestamp} does not exist in thread. Adding it to thread for email {self.initial_email.message_id}"
             )
             self.replies.append(reply_email)
             self.sort_replies()
         else:
             logger.debug(f"Reply email {reply_email} already exists in thread")
 
@@ -63,58 +63,75 @@
     def __repr__(self):
         # return f"Email(imap_id={self.imap_id}, message_id={self.message_id}, subject={self.subject}, sender={self.sender}, timestamp={self.timestamp})"
         return f"Email(imap_id={self.imap_id}, timestamp={self.timestamp})"
 
 
 args = None
 bot_email = None
+
 email_threads = {}
+
 SUBJECT = "autoreply password"
 
 
 def main():
     """Main entry point for the script."""
     global args
     global bot_email
+    global email_threads
     args = argparser.parse_args()
 
-    bot_email = args.imap_username
 
-    # Set up logging
-    set_primary_logger(args.log_level)
-    ic(args)
-    if args.watch_interval:
-        while True:
-            fetch_and_process_emails()
-            time.sleep(args.watch_interval)
-    else:
-        fetch_and_process_emails()
+    match args.subcommand:
+        case "list-folders":
+            with IMAPClient(args.imap_host) as client:
+                client.login(args.imap_username, args.imap_password)
+                folders = client.list_folders()
+                for folder in folders:
+                    print(folder[2])
+        case None:
+            bot_email = args.imap_username
+
+            # Set up logging
+            set_primary_logger(args.log_level)
+            ic(args)
+            if args.watch_interval:
+                logger.info(f"Watching for new emails every {args.watch_interval} seconds")
+                while True:
+                    fetch_and_process_emails()
+                    time.sleep(args.watch_interval)
+                    # **EMPTY THREADS**
+                    email_threads = {}
+            else:
+                fetch_and_process_emails()
 
 
 def fetch_and_process_emails():
     """Fetch and process emails from the IMAP server."""
     global email_threads
     openai = OpenAI(api_key=args.openai_api_key, base_url=args.openai_base_url)
     with IMAPClient(args.imap_host) as client:
         client.login(args.imap_username, args.imap_password)
 
         email_threads = {}
+        folders = args.folder if args.folder else [folder[2] for folder in client.list_folders()]
         # for folder in client.list_folders():
         # Disabling fetching from all folders due it not being inefficient
         # Instead, just fetch from INBOX and get the threads later
-        for folder in [(None, None, "INBOX")]:
+        for folder in folders:
             try:
-                client.select_folder(folder[2])
+                client.select_folder(folder)
             # If the error is imaplib.IMAP4.error: select failed:...
             except imaplib.IMAP4.error:
                 logger.debug(f"Failed to select folder {folder[2]}. Skipping...")
                 continue
             # messages = client.search([f"(OR SUBJECT \"{SUBJECT}\" SUBJECT \"Re: {SUBJECT}\")"])
             messages = client.search(["OR", "SUBJECT", SUBJECT, "SUBJECT", f"Re: {SUBJECT}"])
             for msg_id in messages:
+                # TODO: It seems this will throw a KeyError if an email is sent while this for loop is running. May have been fixed by emptying email_threads at the end of the while loop? This should be tested again to confirm
                 msg_data = client.fetch([msg_id], ["ENVELOPE", "BODY[]", "RFC822.HEADER"])
                 envelope = msg_data[msg_id][b"ENVELOPE"]
                 subject = envelope.subject.decode()
                 timestamp = envelope.date
                 # Parse the headers from the email data
                 message = message_from_bytes(msg_data[msg_id][b"RFC822.HEADER"])
                 sender = get_sender(message)["email"]
@@ -174,45 +191,46 @@
                                 )
                             )
                             email_threads[parent_email_id] = email_thread
                             logger.info(
                                 f"Created new thread for email {message_id} sent at {timestamp}"
                             )
 
-        # Send replies outside of the loop
-        for email_thread in email_threads.values():
-            # Check if we're on the last email in the
-            # We don't have to use user_replies since we're checking if the bot replied to the email later
+        # ic([thread for thread in email_threads.values()])
+        ic(email_threads)
+        # Check if there are any emails wherein the last email in the thread is a user email
+        # If so, send a reply
+        for message_id, email_thread in email_threads.items():
+            # Check if the email only has an initial email
+            # If it does, then there won't be any replies and an index error will occur
             if len(email_thread.replies) == 0:
-                uid = email_thread.initial_email.imap_id
+                logger.debug(f"No replies in thread for email {message_id}")
                 message_id = email_thread.initial_email.message_id
+                msg_id = email_thread.initial_email.imap_id
                 references_ids = email_thread.initial_email.references
-            elif len(email_thread.replies) > 0:
-                uid = email_thread.replies[-1].imap_id
+            elif len(email_thread.replies) > 0 and email_thread.replies[-1].sender != bot_email:
+                logger.debug(f"Last email in thread for email {message_id} is from {email_thread.replies[-1].sender}")
                 message_id = email_thread.replies[-1].message_id
+                msg_id = email_thread.replies[-1].imap_id
                 references_ids = email_thread.replies[-1].references
-                logger.debug(
-                    f"Most recent email in thread: {email_thread.replies[-1]} | Sent at {email_thread.replies[-1].timestamp}"
-                )
-                if email_thread.replies[-1].sender == bot_email:
-                    logger.debug(
-                        f"Most recent email in thread for email {message_id} is from the bot. Skipping..."
-                    )
-                    continue
-
-            if is_newer_reference(client, message_id):
-                logger.debug(f"Email {message_id} has newer references. Skipping...")
+            elif len(email_thread.replies) > 0 and email_thread.replies[-1].sender == bot_email:
+                logger.debug(f"Last email in thread for email {message_id} is from the bot")
                 continue
+            else:
+                ValueError("Invalid email thread")
+            send_reply(
+                thread=get_thread_history(client, email_thread),
+                client=client,
+                msg_id=msg_id,
+                message_id=message_id,
+                references_ids=references_ids,
+                openai=openai,
+                model=args.openai_model,
+            )
 
-            # If only INBOX is fetched, the bot's replies may not be in EmailThread
-            # Thus, we can't just do if email_thread.replies[-1].sender != bot_email
-            thread = get_thread_history(client, msg_id)
-            send_reply(thread, client, uid, message_id, references_ids, openai)
-
-        ic([thread for thread in email_threads.values()])
         logger.debug(f"Keys in email_threads: {len(email_threads.keys())}")
 
 
 # Function to check if an email has been read
 def is_new_email(client, msg_id):
     flags = client.get_flags([msg_id])
     return b"\\Seen" not in flags.get(msg_id, [])
@@ -230,20 +248,16 @@
     return sender != bot_email
 
 
 def get_thread_history(
     client: IMAPClient, message_identifier: str | int | EmailThread
 ) -> list[dict]:
     """Fetch the entire thread history for the specified message ID."""
-
+    # Might be better to use "is"
     if isinstance(message_identifier, EmailThread):
-        # TODO: At this point, EmaiLThread should be the default due to it only needing to search all folders once.
-        logger.warning(
-            "Getting thread history from EmailThread object. If EmailThread does not include sent emails (not just INBOX fetched) this will exclude the bot's replies."
-        )  # noqa E501
         thread_history = []
         thread_history.append(
             {
                 "sender": message_identifier.initial_email.sender,
                 "content": message_identifier.initial_email.body,
             }
         )
@@ -289,15 +303,15 @@
             prev_message_id = message.get("In-Reply-To")
             prev_msg_id = get_uid_from_message_id(client, prev_message_id)
             prev_msg_data = client.fetch([prev_msg_id], ["RFC822"])
             prev_raw_message = prev_msg_data[prev_msg_id][b"RFC822"]
             prev_message = message_from_bytes(prev_raw_message)
             thread_history.append(
                 {
-                    "sender": get_sender(message),
+                    "sender": get_sender(message)["email"],
                     "content": get_plain_email_content(message),
                     "timestamp": make_tz_aware(parsedate_to_datetime(message.get("Date"))),
                 }
             )
             message = prev_message
         # Sort the thread history by timestamp
         thread_history = sorted(thread_history, key=lambda x: x["timestamp"])
@@ -384,44 +398,48 @@
 def send_reply(
     thread: list[dict],
     client: IMAPClient,
     msg_id: int,
     message_id: str,
     references_ids: list[str],
     openai: OpenAI,
-    model="mistralai/mistral-7b-instruct:free",
+    model: str,
 ):
     """Send a reply to the email with the specified message ID."""
-    # smtp = yagmail.SMTP(user=args.smtp_username, password=args.smtp_password, host=args.smtp_host, port=args.smtp_port)
-    logger.info(f"Sending reply to email {message_id}")
-    thread = get_thread_history(client, msg_id)
     # Set roles deletes the sender key so we need to store the sender before calling it
     sender = thread[-1]["sender"]
     thread = set_roles(thread)
     references_ids.append(message_id)
-    logger.debug(f"Thread history (message_identifier): {thread}")
-    logger.debug(f"Thread history length (message_identifier): {len(thread)}")
+    # thread_from_msg_id = get_thread_history(client, msg_id)
+    # logger.debug(f"Thread history (message_identifier): {thread_from_msg_id}")
+    # logger.debug(f"Thread history length (message_identifier): {len(thread_from_msg_id)}")
+    # thread_from_object = get_thread_history(client, email_threads[list(email_threads.keys())[-1]])
+    # logger.debug(f"Thread history (EmailThread object): {thread_from_object}")
+    # logger.debug(f"Thread history length (EmailThread object): {len(thread_from_object)}")
+    logger.info(f"Sending reply to email {message_id} to {sender}")
+    logger.debug(f"Thread history: {thread}")
+    logger.debug(f"Thread history length: {len(thread)}")
     generated_response = openai.chat.completions.create(
         model=model,
         messages=thread,
     )
     generated_response = generated_response.choices[0].message.content
-    logger.info(f"Generated response: {generated_response}")
+    logger.debug(f"Generated response: {generated_response}")
     yag = yagmail.SMTP(
         user=args.smtp_username,
         password=args.smtp_password,
         host=args.smtp_host,
         port=int(args.smtp_port),
     )
-    logger.debug(f"Sending email to {sender}")
     yag.send(
-        to=sender["email"],
+        to=sender,
         subject=f"Re: {SUBJECT}",
         headers={"In-Reply-To": message_id, "References": " ".join(references_ids)},
         contents=generated_response,
+        message_id=make_msgid(domain=args.message_id_domain if args.message_id_domain else "llmail"),
     )
 
 
 def get_plain_email_content(message: Message | str) -> str:
     """Get the content of the email message. If a  message object is provided, it will be parsed
     Otherwise, it is assumed that the content is already a string and will be converted to markdown.
     """
```

### Comparing `llmail-0.1.0/llmail/utils/cli_args.py` & `llmail-0.1.1/llmail/utils/cli_args.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 For reference, Gmail's IMAP settings are:
 - Hostname: imap.gmail.com
 - Port: 993
 - Username: Your full Gmail address
 - Password: App token (when using 2FA) or perhaps your regular password (if not using 2FA ?)
 """
 
-# TODO: Add argument for specific IMAP folder. Default to INBOX
 
 
 def set_argparse():
     global argparser
 
     if Path(".env").is_file():
         dotenv.load_dotenv()
@@ -28,41 +27,61 @@
 
     # Set up argparse
     argparser = argparse.ArgumentParser(
         prog="LLMail",
         description="Interact with an LLM through email.",
         epilog=":)",
     )
-
+    # Subcommands
+    subparsers = argparser.add_subparsers(
+        # Dest means that the current subcommand can be accessed via args.subcommand
+        dest="subcommand",
+        title="Subcommands",
+        )
+    # Subcommand: list-folders
+    _ = subparsers.add_parser("list-folders", help="List all folders in the IMAP account and exit")
     # General arguments
     argparser.add_argument(
         "--log-level",
         "-l",
         help="Log level",
         default=os.getenv("LOG_LEVEL") if os.getenv("LOG_LEVEL") else "INFO",
     )
     argparser.add_argument(
         "--watch-interval",
         "-w",
         help="Interval in seconds to check for new emails. If not set, will only check once.",
         type=int,
-        default=None,
+        default=int(os.getenv("WATCH_INTERVAL")) if os.getenv("WATCH_INTERVAL") else None,
     )
     # OpenAI-compatible API arguments
     ai_api = argparser.add_argument_group("OpenAI-compatible API")
     ai_api.add_argument(
         "--openai-api-key", help="OpenAI API key", default=os.getenv("OPENAI_API_KEY")
     )
     ai_api.add_argument(
         "--openai-base-url",
         help="OpenAI API endpoint",
         default=os.getenv("OPENAI_BASE_URL"),
     )
+    ai_api.add_argument(
+        "--openai-model",
+        help="Model to use for the LLM",
+        default=os.getenv("OPENAI_MODEL") if os.getenv("OPENAI_MODEL") else "mistralai/mistral-7b-instruct:free",
+    )
     # Email arguments
     email = argparser.add_argument_group("Email")
+    email.add_argument(
+        "--folder",
+        "-f",
+        help="IMAP folder(s) to watch for new emails",
+        # Argparse should append to a list if None is the default
+        default=os.getenv("FOLDER").split(",") if os.getenv("FOLDER") else None,
+        action="append",
+    )
     imap = email.add_argument_group("IMAP")
     imap.add_argument("--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST"))
     imap.add_argument("--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT"))
     imap.add_argument(
         "--imap-username",
         help="IMAP server username",
         default=os.getenv("IMAP_USERNAME"),
@@ -81,14 +100,19 @@
         default=os.getenv("SMTP_USERNAME"),
     )
     smtp.add_argument(
         "--smtp-password",
         help="SMTP server password",
         default=os.getenv("SMTP_PASSWORD"),
     )
+    smtp.add_argument(
+        "--message-id-domain",
+        help="Domain to use for Message-ID header",
+        default=os.getenv("MESSAGE_ID_DOMAIN") if os.getenv("MESSAGE_ID_DOMAIN") else None,
+    )
 
     check_required_args(
         [
             "imap_host",
             "imap_port",
             "imap_username",
             "imap_password",
```

### Comparing `llmail-0.1.0/pyproject.toml` & `llmail-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "llmail"
-version = "0.1.0"
+version = "0.1.1"
 description = "Interact with LLMs via email"
 authors = ["slashtechno <77907286+slashtechno@users.noreply.github.com>"]
+repository = "https://github.com/slashtechno/llmail"
+keywords = ["llm", "email", "ai", "openai"]
 license = "GNU AGPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 loguru = "^0.7.2"
 python-dotenv = "^1.0.1"
```

### Comparing `llmail-0.1.0/PKG-INFO` & `llmail-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 Metadata-Version: 2.1
 Name: llmail
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interact with LLMs via email
+Home-page: https://github.com/slashtechno/llmail
 License: GNU AGPLv3
+Keywords: llm,email,ai,openai
 Author: slashtechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
 Requires-Dist: imapclient (>=3.0.1,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.25.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: yagmail[all] (>=0.15.293,<0.16.0)
+Project-URL: Repository, https://github.com/slashtechno/llmail
 Description-Content-Type: text/markdown
 
 # LLMail  
 Interact with Large Language Models (LLMs) via email.
 
 ### Features  
 - Utilize any OpenAI-compatible API
+    - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) offers free access to specific models with an OpenAI-compatible API
 - Check every _n_ seconds 
 - No need for a local database - uses IMAP
 
 ## Prerequisites  
 ### Python  
-- Python ^3.11
-- Poetry <!-- (optional)  -->
-- An API key from an OpenAI-compatible API
-    - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) provides free access to select models
-        - Right now, they are the only provider that will work due to the model being hard-coded (for now)
+- Python ^3.11  
+- Poetry (optional)  
+- An API key from an OpenAI-compatible API  
+### Docker
+- Docker  
 
 ## Usage  
-### Installation  
+### Installing from PyPi with `pip` (recommended)  
+This assumes you have the correct version of Python installed
+1. `pip install llmail`  
+    a. You may need to use `pip3` instead of `pip`  
+2. `llmail`  
+
+### Installation from source or with Docker
 Cloning the repository is not required when installing from PyPi but is required when installing from source  
 1. Clone this repo with `git clone https://github.com/slashtechno/llmail`  
 2. `cd` into the cloned repository  
-3. Install with [Poetry](https://python-poetry.org/) <!-- or [Docker](https://www.docker.com/) -->
+3. Install and run with one of the following methods:
 
-<!-- 
-#### Installing from PyPi with pip (recommended)  
-This assumes you have the correct version of Python installed
-1. `pip install llmail`  
-    a. You may need to use `pip3` instead of `pip`  
-2. `llmail`   -->
 
-#### Poetry  
+
+#### Poetry
 1. `poetry install`  
 2. `poetry run -- llmail`  
 
-<!-- #### Docker  -->
+#### Docker
+1. Configure with the steps below  
+2. `docker compose up -d`
+
 ### Configuration  
-To configure the program, either use CLI flags (`--help` for more information) or environment variables.  
-It is recommended to just copy .env.example to .env and fill in the necessary information.
+To configure the program, either use CLI flags (`--help` for more information) or environment variables.
+It is recommended to just copy `.env.example` to `.env` and fill in the necessary information.
 
 ### How to uninstall  
 - If you used Poetry, just delete the virtual environment and then the cloned repository
```

