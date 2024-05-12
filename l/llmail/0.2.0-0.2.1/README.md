# Comparing `tmp/llmail-0.2.0.tar.gz` & `tmp/llmail-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmail-0.2.0.tar", max compression
+gzip compressed data, was "llmail-0.2.1.tar", max compression
```

## Comparing `llmail-0.2.0.tar` & `llmail-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-29 23:31:53.519788 llmail-0.2.0/llmail/__init__.py
--rw-r--r--   0        0        0    22080 2024-05-12 03:02:00.564879 llmail-0.2.0/llmail/__main__.py
--rw-r--r--   0        0        0        0 2024-04-29 23:49:56.280104 llmail-0.2.0/llmail/utils/__init__.py
--rw-r--r--   0        0        0     4681 2024-05-12 02:54:37.168425 llmail-0.2.0/llmail/utils/cli_args.py
--rw-r--r--   0        0        0      846 2024-05-12 03:15:41.530487 llmail-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1532 2024-05-12 03:11:36.325088 llmail-0.2.0/README.md
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 llmail-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34516 2024-05-12 19:52:49.524992 llmail-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1532 2024-05-12 19:52:49.524992 llmail-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 19:52:49.524992 llmail-0.2.1/llmail/__init__.py
+-rw-r--r--   0        0        0    22752 2024-05-12 19:52:49.524992 llmail-0.2.1/llmail/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-12 19:52:49.524992 llmail-0.2.1/llmail/utils/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-12 19:52:49.524992 llmail-0.2.1/llmail/utils/cli_args.py
+-rw-r--r--   0        0        0      846 2024-05-12 19:52:49.528992 llmail-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 llmail-0.2.1/PKG-INFO
```

### Comparing `llmail-0.2.0/LICENSE` & `llmail-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmail-0.2.0/llmail/__main__.py` & `llmail-0.2.1/llmail/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
 
 args = None
 bot_email = None
 
 email_threads = {}
 
-SUBJECT = "autoreply password"
 
 
 def main():
     """Main entry point for the script."""
     global args
     global bot_email
     global email_threads
@@ -93,23 +92,34 @@
 
             # Set up logging
             set_primary_logger(args.log_level)
             ic(args)
             if args.watch_interval:
                 logger.info(f"Watching for new emails every {args.watch_interval} seconds")
                 while True:
-                    fetch_and_process_emails()
+                    fetch_and_process_emails(
+                        subject=args.subject_key,
+                        alias=args.alias,
+                        system_prompt=args.system_prompt,
+                    )
                     time.sleep(args.watch_interval)
                     # **EMPTY THREADS**
                     email_threads = {}
             else:
-                fetch_and_process_emails()
-
-
-def fetch_and_process_emails():
+                fetch_and_process_emails(
+                    subject=args.subject_key,
+                    alias=args.alias,
+                    system_prompt=args.system_prompt,
+                )
+
+def fetch_and_process_emails(
+        subject: str,
+        alias: str = None,
+        system_prompt: str = None,
+):
     """Fetch and process emails from the IMAP server."""
     global email_threads
     openai = OpenAI(api_key=args.openai_api_key, base_url=args.openai_base_url)
     with IMAPClient(args.imap_host) as client:
         client.login(args.imap_username, args.imap_password)
 
         email_threads = {}
@@ -120,16 +130,16 @@
         for folder in folders:
             try:
                 client.select_folder(folder)
             # If the error is imaplib.IMAP4.error: select failed:...
             except imaplib.IMAP4.error:
                 logger.debug(f"Failed to select folder {folder[2]}. Skipping...")
                 continue
-            # messages = client.search([f"(OR SUBJECT \"{SUBJECT}\" SUBJECT \"Re: {SUBJECT}\")"])
-            messages = client.search(["OR", "SUBJECT", SUBJECT, "SUBJECT", f"Re: {SUBJECT}"])
+            # Might be smart to also search for forwarded emails
+            messages = client.search(["OR", "SUBJECT", subject, "SUBJECT", f"Re: {subject}"])
             for msg_id in messages:
                 # TODO: It seems this will throw a KeyError if an email is sent while this for loop is running. May have been fixed by emptying email_threads at the end of the while loop? This should be tested again to confirm
                 msg_data = client.fetch([msg_id], ["ENVELOPE", "BODY[]", "RFC822.HEADER"])
                 envelope = msg_data[msg_id][b"ENVELOPE"]
                 subject = envelope.subject.decode()
                 timestamp = envelope.date
                 # Parse the headers from the email data
@@ -215,19 +225,22 @@
             elif len(email_thread.replies) > 0 and email_thread.replies[-1].sender == bot_email:
                 logger.debug(f"Last email in thread for email {message_id} is from the bot")
                 continue
             else:
                 ValueError("Invalid email thread")
             send_reply(
                 thread=get_thread_history(client, email_thread),
+                subject=subject,
+                alias=args.alias,
                 client=client,
                 msg_id=msg_id,
                 message_id=message_id,
                 references_ids=references_ids,
                 openai=openai,
+                system_prompt=system_prompt,
                 model=args.openai_model,
             )
 
         logger.debug(f"Keys in email_threads: {len(email_threads.keys())}")
 
 
 # Function to check if an email has been read
@@ -393,25 +406,30 @@
     # ^10 is a formatting directive to center with a padding of 10
     logger_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</green> |<level>{level: ^10}</level>| <level>{message}</level>"
     logger.add(stderr, format=logger_format, colorize=True, level=log_level)
 
 
 def send_reply(
     thread: list[dict],
+    subject: str,
+    alias: str,
     client: IMAPClient,
     msg_id: int,
     message_id: str,
     references_ids: list[str],
     openai: OpenAI,
+    system_prompt: str,
     model: str,
 ):
     """Send a reply to the email with the specified message ID."""
     # Set roles deletes the sender key so we need to store the sender before calling it
     sender = thread[-1]["sender"]
     thread = set_roles(thread)
+    if system_prompt:   
+        thread.insert(0, {"role": "system", "content": system_prompt})
     references_ids.append(message_id)
     # thread_from_msg_id = get_thread_history(client, msg_id)
     # logger.debug(f"Thread history (message_identifier): {thread_from_msg_id}")
     # logger.debug(f"Thread history length (message_identifier): {len(thread_from_msg_id)}")
     # thread_from_object = get_thread_history(client, email_threads[list(email_threads.keys())[-1]])
     # logger.debug(f"Thread history (EmailThread object): {thread_from_object}")
     # logger.debug(f"Thread history length (EmailThread object): {len(thread_from_object)}")
@@ -421,22 +439,22 @@
     generated_response = openai.chat.completions.create(
         model=model,
         messages=thread,
     )
     generated_response = generated_response.choices[0].message.content
     logger.debug(f"Generated response: {generated_response}")
     yag = yagmail.SMTP(
-        user=args.smtp_username,
+        user={args.smtp_username: alias} if alias else args.smtp_username,
         password=args.smtp_password,
         host=args.smtp_host,
         port=int(args.smtp_port),
     )
     yag.send(
         to=sender,
-        subject=f"Re: {SUBJECT}",
+        subject=f"Re: {subject}",
         headers={"In-Reply-To": message_id, "References": " ".join(references_ids)},
         contents=generated_response,
         message_id=make_msgid(domain=args.message_id_domain if args.message_id_domain else "llmail"),
     )
 
 
 def get_plain_email_content(message: Message | str) -> str:
```

### Comparing `llmail-0.2.0/llmail/utils/cli_args.py` & `llmail-0.2.1/llmail/utils/cli_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,40 @@
         default=os.getenv("OPENAI_BASE_URL"),
     )
     ai_api.add_argument(
         "--openai-model",
         help="Model to use for the LLM",
         default=os.getenv("OPENAI_MODEL") if os.getenv("OPENAI_MODEL") else "mistralai/mistral-7b-instruct:free",
     )
+    ai_api.add_argument(
+        "--system-prompt",
+        help="Prepend this to the message history sent to the LLM as a message from the system role",
+        default=os.getenv("SYSTEM_PROMPT") if os.getenv("SYSTEM_PROMPT") else None,
+    )
     # Email arguments
     email = argparser.add_argument_group("Email")
     email.add_argument(
         "--folder",
         "-f",
         help="IMAP folder(s) to watch for new emails",
         # Argparse should append to a list if None is the default
         default=os.getenv("FOLDER").split(",") if os.getenv("FOLDER") else None,
         action="append",
     )
+    email.add_argument(
+        "--subject-key",
+        "-s",
+        help="Emails with this subject will be replied to",
+        default=os.getenv("SUBJECT_KEY") if os.getenv("SUBJECT_KEY") else "llmail autoreply",
+    )
+    email.add_argument(
+        "--alias",
+        help="Name to use in the 'From' in addition to the email address",
+        default=os.getenv("ALIAS") if os.getenv("ALIAS") else "LLMail",
+    )
     imap = email.add_argument_group("IMAP")
     imap.add_argument("--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST"))
     imap.add_argument("--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT"))
     imap.add_argument(
         "--imap-username",
         help="IMAP server username",
         default=os.getenv("IMAP_USERNAME"),
```

### Comparing `llmail-0.2.0/pyproject.toml` & `llmail-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmail"
-version = "0.2.0"
+version = "0.2.1"
 description = "Interact with LLMs via email"
 authors = ["slashtechno <77907286+slashtechno@users.noreply.github.com>"]
 repository = "https://github.com/slashtechno/llmail"
 keywords = ["llm", "email", "ai", "openai"]
 license = "GNU AGPLv3"
 readme = "README.md"
```

### Comparing `llmail-0.2.0/README.md` & `llmail-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llmail-0.2.0/PKG-INFO` & `llmail-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmail
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interact with LLMs via email
 Home-page: https://github.com/slashtechno/llmail
 License: GNU AGPLv3
 Keywords: llm,email,ai,openai
 Author: slashtechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

