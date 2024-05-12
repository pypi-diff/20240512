# Comparing `tmp/pygramcore-1.0.4.tar.gz` & `tmp/pygramcore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygramcore-1.0.4.tar", last modified: Fri May 10 15:03:35 2024, max compression
+gzip compressed data, was "pygramcore-1.1.0.tar", last modified: Sun May 12 16:44:08 2024, max compression
```

## Comparing `pygramcore-1.0.4.tar` & `pygramcore-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.788496 pygramcore-1.0.4/
--rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4405 2024-05-10 15:03:35.787497 pygramcore-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3684 2024-05-09 20:03:27.000000 pygramcore-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.761495 pygramcore-1.0.4/pygramcore/
--rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.778995 pygramcore-1.0.4/pygramcore/elements/
--rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/elements/__init__.py
--rw-rw-rw-   0        0        0     9598 2024-05-10 14:46:19.000000 pygramcore-1.0.4/pygramcore/elements/post.py
--rw-rw-rw-   0        0        0    14556 2024-05-10 14:46:25.000000 pygramcore-1.0.4/pygramcore/elements/user.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.783495 pygramcore-1.0.4/pygramcore/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.4/pygramcore/exceptions/__init__.py
--rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.4/pygramcore/exceptions/auth.py
--rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.4/pygramcore/exceptions/format.py
--rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/exceptions/post.py
--rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/exceptions/user.py
--rw-rw-rw-   0        0        0     9078 2024-05-10 14:58:26.000000 pygramcore-1.0.4/pygramcore/pygram.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.785498 pygramcore-1.0.4/pygramcore/utils/
--rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/utils/__init__.py
--rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.4/pygramcore/utils/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:03:35.786995 pygramcore-1.0.4/pygramcore.egg-info/
--rw-rw-rw-   0        0        0     4405 2024-05-10 15:03:35.000000 pygramcore-1.0.4/pygramcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2024-05-10 15:03:35.000000 pygramcore-1.0.4/pygramcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:03:35.000000 pygramcore-1.0.4/pygramcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-10 15:03:35.000000 pygramcore-1.0.4/pygramcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 15:03:35.000000 pygramcore-1.0.4/pygramcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:03:35.788999 pygramcore-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-05-10 15:03:22.000000 pygramcore-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:08.001672 pygramcore-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4405 2024-05-12 16:44:08.000674 pygramcore-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3684 2024-05-09 20:03:27.000000 pygramcore-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.957674 pygramcore-1.1.0/pygramcore/
+-rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.1.0/pygramcore/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-05-11 16:56:00.000000 pygramcore-1.1.0/pygramcore/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.988674 pygramcore-1.1.0/pygramcore/elements/
+-rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.1.0/pygramcore/elements/__init__.py
+-rw-rw-rw-   0        0        0    10317 2024-05-11 16:50:36.000000 pygramcore-1.1.0/pygramcore/elements/post.py
+-rw-rw-rw-   0        0        0    15476 2024-05-12 16:35:55.000000 pygramcore-1.1.0/pygramcore/elements/user.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.994174 pygramcore-1.1.0/pygramcore/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.1.0/pygramcore/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.1.0/pygramcore/exceptions/auth.py
+-rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.1.0/pygramcore/exceptions/format.py
+-rw-rw-rw-   0        0        0      116 2024-05-10 16:05:33.000000 pygramcore-1.1.0/pygramcore/exceptions/navigation.py
+-rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.1.0/pygramcore/exceptions/post.py
+-rw-rw-rw-   0        0        0      876 2024-05-10 15:42:22.000000 pygramcore-1.1.0/pygramcore/exceptions/user.py
+-rw-rw-rw-   0        0        0    10369 2024-05-11 17:00:18.000000 pygramcore-1.1.0/pygramcore/pygram.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.997175 pygramcore-1.1.0/pygramcore/utils/
+-rw-rw-rw-   0        0        0       46 2024-05-10 15:59:56.000000 pygramcore-1.1.0/pygramcore/utils/__init__.py
+-rw-rw-rw-   0        0        0      134 2024-05-10 15:58:32.000000 pygramcore-1.1.0/pygramcore/utils/misc.py
+-rw-rw-rw-   0        0        0      843 2024-05-10 15:59:24.000000 pygramcore-1.1.0/pygramcore/utils/navigation.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.999675 pygramcore-1.1.0/pygramcore.egg-info/
+-rw-rw-rw-   0        0        0     4405 2024-05-12 16:44:07.000000 pygramcore-1.1.0/pygramcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-05-12 16:44:07.000000 pygramcore-1.1.0/pygramcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:44:07.000000 pygramcore-1.1.0/pygramcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-12 16:44:07.000000 pygramcore-1.1.0/pygramcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 16:44:07.000000 pygramcore-1.1.0/pygramcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:44:08.001672 pygramcore-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-05-10 15:10:17.000000 pygramcore-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:44:07.998174 pygramcore-1.1.0/tests/
+-rw-rw-rw-   0        0        0     2365 2024-05-12 16:20:48.000000 pygramcore-1.1.0/tests/test_user.py
```

### Comparing `pygramcore-1.0.4/LICENSE` & `pygramcore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.4/PKG-INFO` & `pygramcore-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.4
+Version: 1.1.0
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.4 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.1.0 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.4/README.md` & `pygramcore-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.4/pygramcore/elements/post.py` & `pygramcore-1.1.0/pygramcore/elements/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from dataclasses import dataclass
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.common.exceptions import StaleElementReferenceException
 from datetime import datetime
+from urllib.parse import urljoin
 
 from ..pygram import Navigator, check_authorization
 from ..exceptions.post import *
 from ..utils import *
 from ..constants import *
 
 
 @dataclass
 class Post(metaclass=Navigator):
     id: str
 
     def __post_init__(self):
         self._driver: webdriver.Chrome
-        self.url = f"{INSTAGRAM_URL}/p/{self.id}"
+
+    @property
+    def url(self):
+        url = urljoin(INSTAGRAM_URL, f"/p/{self.id}")
+        return url
 
     @check_authorization
     def like(self) -> None:
         """
         Likes the post.
 
         Raises:
@@ -265,14 +270,36 @@
         # Check for form elements
         found_elements = self._driver.find_elements(By.TAG_NAME, "form")
 
         self._driver.implicitly_wait(IMPLICIT_WAIT)
         return bool(found_elements)
 
     @check_authorization
+    def get_author(self):
+        """
+        Finds the user who created the post.
+
+        Returns:
+            User: Author's user object.
+
+        Raises:
+            NotAuthenticated: Raises when the current account is not logged in.
+        """
+        # To prevent from circular import
+        from .user import User
+
+        username = self._driver.find_element(
+            By.XPATH,
+            '//div[@class="xyinxu5 x1pi30zi x1g2khh7 x1swvt13"]//span[@class="_ap3a _aaco _aacw _aacx _aad7 _aade"]',
+        ).text
+
+        user = User(username)
+        return user
+
+    @check_authorization
     def get_date_posted(self) -> datetime:
         """
         Gets the date the the post was published.
 
         Returns:
             datetime: Publish date.
         """
```

### Comparing `pygramcore-1.0.4/pygramcore/elements/user.py` & `pygramcore-1.1.0/pygramcore/elements/user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import dataclass
 from typing import Literal
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from urllib.parse import urlparse
+from selenium.common.exceptions import ElementClickInterceptedException
+from urllib.parse import urlparse, urljoin
 import time
 
 from ..pygram import *
 from ..exceptions.user import *
 from ..utils import *
 from ..constants import *
 
@@ -19,90 +20,146 @@
     Decorator function that opens and closes the user dialog. The user dialog is where you can take actions on a user, such as: unfollowing, adding or removing from close friends, etc...
     """
 
     def wrapper(user: "User", *args, **kwargs):
         if not user.is_following():
             raise UserNotFollowed(user.name)
 
-        # Check if it's not already open
-        if user.user_dialog_open():
-            return
-
-        # Open the dialog
-        dialog_btn = user._driver.find_element(By.XPATH, '//div[text()="Following"]')
-        dialog_btn.click()
+        # Raises a click interception error if the dialog was open already
+        try:
+            user.open_user_dialog()
+        except ElementClickInterceptedException:
+            pass
 
         # Perform function being decorated
         value = func(user, *args, **kwargs)
 
         # Attempt to close the user dialog, some actions
         # close the dialog automatically (e.g. unfollowing)
         try:
-            close_btn = user._driver.find_element(
-                By.CSS_SELECTOR,
-                "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div > div.x78zum5.xds687c.x1iorvi4.x1sxyh0.xjkvuk6.xurb0ha.x10l6tqk.x1vjfegm > div > div > svg",
-            )
-            close_btn.click()
+            user._driver.implicitly_wait(0)
+            user.close_user_dialog()
         except:
             pass
         finally:
             user._driver.implicitly_wait(IMPLICIT_WAIT)
 
         return value
 
     return wrapper
 
 
+def check_private(func):
+    """
+    Decorator that checks if a user is private.
+
+    Raises:
+        UserIsPrivate: Raises whent the user is private
+    """
+
+    def wrapper(user: "User", *args, **kwargs):
+        if user.is_private():
+            raise UserIsPrivate(user.name)
+
+        value = func(user, *args, **kwargs)
+        return value
+
+    return wrapper
+
+
+def check_following(func):
+    """
+    Decorator that checks if the logged in account follows the user.
+
+    Raises:
+        UserNotFollowed: Raises when the user is not followed.
+    """
+
+    def wrapper(user: "User", *args, **kwargs):
+        if not user.is_following():
+            raise UserNotFollowed(user.name)
+
+        value = func(user, *args, **kwargs)
+        return value
+
+    return wrapper
+
+
 @dataclass
 class User(metaclass=Navigator):
     """
     Represents an Instagram user.
 
     Args:
         name (str): Username of the user.
     """
 
     name: str
 
     def __post_init__(self):
         self._driver: webdriver.Chrome
-        self.url = f"{INSTAGRAM_URL}/{self.name}/"
+
+    @property
+    def url(self):
+        url = urljoin(INSTAGRAM_URL, self.name)
+        return url
 
     @check_authorization
     def is_private(self) -> bool:
-        pass
+        """
+        Checks if the user has a private account.
+
+        Returns:
+            bool: Whether the account is private.
+
+        Raises:
+            NotAuthenticated: Raises when the current account is not logged in.
+        """
+        self._driver.implicitly_wait(2)
+
+        # Attempt to find the div that contains "This account is private"
+        elements_found = self._driver.find_elements(
+            By.XPATH,
+            '//div[@class="x9f619 xjbqb8w x78zum5 x168nmei x13lgxp2 x5pf9jr xo71vjh x1uhb9sk x1plvlek xryxfnj x1c4vz4f x2lah0s x1q0g3np xqjyukv x6s0dn4 x1oa3qoh x1nhvcw1"]',
+        )
+
+        self._driver.implicitly_wait(IMPLICIT_WAIT)
+
+        return bool(elements_found)
 
     @check_authorization
     def follow(self) -> None:
         """
         Follows the user with the current account logged in.
 
         Raises:
             UserAlreadyFollowed: Raises when the user is already followed. Use `.is_followed()` to check if followed.
             NotAuthenticated: Raises when the current account is not logged in.
         """
         if self.is_following():
             raise UserAlreadyFollowed(self.name)
 
-        follow_btn = self._driver.find_element(By.XPATH, '//div[text()="Follow"]')
+        follow_btn = self._driver.find_element(
+            By.XPATH, '//button[@class=" _acan _acap _acas _aj1- _ap30"]'
+        )
         follow_btn.click()
 
     @check_authorization
+    @check_private
+    @check_following
     @user_dialog_action
-    def unfollow(self) -> None:
+    def unfollow(self):
         """
         Unfollows the user with the current account logged in.
 
         Raises:
             UserNotFollowed: Raises when the user is not followed. Use `.is_followed()` to check if followed.
             NotAuthenticated: Raises when the current account is not logged in.
+            UserIsPrivate: Raises when the user is private.
         """
-        if not self.is_following():
-            raise UserNotFollowed(self.name)
-
         unfollow_btn = self._driver.find_element(
             By.CSS_SELECTOR,
             "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div > div:nth-child(8)",
         )
         unfollow_btn.click()
 
     @check_authorization
@@ -112,54 +169,60 @@
 
         Returns:
             bool: whether the account logged in follows the user.
 
         Raises:
             NotAuthenticated: Raises when the current account is not logged in.
         """
+        follow_btn = self._driver.find_element(
+            By.CSS_SELECTOR, "button._acan._acap._aj1-._ap30"
+        )
+        classes = follow_btn.get_attribute("class")
 
-        self._driver.implicitly_wait(1)
-
-        if self._driver.find_elements(By.XPATH, '//div[text()="Follow"]'):
-            self._driver.implicitly_wait(10)
-            return False
-        elif self._driver.find_elements(By.XPATH, '//div[text()="Following"]'):
-            self._driver.implicitly_wait(10)
-            return True
+        # "_acat" when following
+        # "_acas" when not
+        return "_acat" in classes
 
     @check_authorization
+    @check_private
+    @check_following
     @user_dialog_action
     def add_close_friend(self):
         """
         Adds the user to the current account's close friends.
 
         Raises:
             UserCloseFriend: Raises when the user is already a close friend.
             NotAuthenticated: Raises when the current account is not logged in.
+            UserNotFollowed: Raises when the user is not followed.
         """
         if self.is_close_friend():
             raise UserCloseFriend(self.name)
+        self.open_user_dialog()
 
         close_friend_btn = self._driver.find_element(
-            By.CSS_SELECTOR, "svg[aria-label='Close friend']"
+            By.CSS_SELECTOR, 'svg[aria-label="Close friend"]'
         )
         close_friend_btn.click()
 
     @check_authorization
+    @check_following
     @user_dialog_action
     def remove_close_friend(self):
         """
         Removes the user from the current account's close friends.
 
         Raises:
             UserNotCloseFriend: Raises when the user is not close friends already.
             NotAuthenticated: Raises when the current account is not logged in.
+            UserNotFollowed: Raises when the user is not followed.
         """
         if not self.is_close_friend():
             raise UserNotCloseFriend(self.name)
+        self.open_user_dialog()
 
         close_friend_btn = self._driver.find_element(
             By.CSS_SELECTOR, "svg[aria-label='Close friend']"
         )
         close_friend_btn.click()
 
     @check_authorization
@@ -170,36 +233,29 @@
 
         Returns:
             bool: Whether the user is a close friend
 
         Raises:
             NotAuthenticated: Raises when the current account is not logged in.
         """
-        self._driver.implicitly_wait(2)
-
-        # Check if not close friend
-        elements = self._driver.find_elements(
-            By.XPATH, '//svg[contains(@class,"x5n08af")][@width="16"]'
-        )
-
-        if elements:
-            self._driver.implicitly_wait(IMPLICIT_WAIT)
+        # A user isn't a close friend if not followed in the first place
+        if not self.is_following():
             return False
 
         # Check if already close friend
-        elements = self._driver.find_elements(
-            By.XPATH,
-            '//svg[contains(@class,"x1g9anri")]',
+        close_friends_icon = self._driver.find_element(
+            By.CSS_SELECTOR,
+            'svg[aria-label="Close friend"]',
         )
 
-        if elements:
-            self._driver.implicitly_wait(IMPLICIT_WAIT)
-            return True
+        classes = close_friends_icon.get_attribute("class")
+        return "x1g9anri" in classes
 
     @check_authorization
+    @check_following
     @user_dialog_action
     def mute(
         self,
         *modes: Literal["posts", "stories"],
     ):
         """
         Mutes the user's posts and/or stories. It is important to note that this function only enables the option, and can't disable it.
@@ -212,14 +268,15 @@
         user = User("username")
         user.mute("stories", "posts")
         ```
 
         Raises:
             ValueError: if a mode in the arguments does not exist.
             NotAuthenticated: Raises when the current account is not logged in.
+            UserNotFollowed: Raises when the user is not followed.
         """
         if isinstance(modes[0], str):
             modes = list(modes)
 
         if not all(mode in ["posts", "stories"] for mode in modes):
             raise ValueError("This mute mode does not exist!")
 
@@ -248,30 +305,14 @@
         # Submit options
         submit_btn = self._driver.find_element(
             By.CSS_SELECTOR,
             "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div > div.x9f619.xjbqb8w.x78zum5.x168nmei.x13lgxp2.x5pf9jr.xo71vjh.x1uhb9sk.x1plvlek.xryxfnj.x1c4vz4f.x2lah0s.xdt5ytf.xqjyukv.x1qjc9v5.x1oa3qoh.x1nhvcw1 > div.x9f619.xjbqb8w.x78zum5.x168nmei.x13lgxp2.x5pf9jr.xo71vjh.x1y1aw1k.x1sxyh0.xwib8y2.xurb0ha.x1uhb9sk.x1plvlek.xryxfnj.x1c4vz4f.x2lah0s.xdt5ytf.xqjyukv.x1qjc9v5.x1oa3qoh.x1nhvcw1 > div",
         )
         submit_btn.click()
 
-    def user_dialog_open(self) -> bool:
-        """
-        Checks if the user dialog is open. The user dialog refers to the menu that opens when clicking the 'Following' button in the user page.
-
-        Returns:
-            bool: Whether the dialog is open
-        """
-        elements = self._driver.find_elements(
-            By.CSS_SELECTOR,
-            "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div > div.x9f619.xjbqb8w.x78zum5.x168nmei.x13lgxp2.x5pf9jr.xo71vjh.xyamay9.x1pi30zi.x1l90r2v.x1swvt13.x1uhb9sk.x1plvlek.xryxfnj.x1c4vz4f.x2lah0s.xdt5ytf.xqjyukv.x6s0dn4.x1oa3qoh.x1nhvcw1 > span",
-        )
-
-        # Return whether any elements are in the list (found or not)
-        is_open = bool(elements)
-        return is_open
-
     def get_total_posts(self) -> int:
         """
         Get the user's total amount of posts.
 
         Returns:
             int: total posts
         """
@@ -307,20 +348,26 @@
         _, _, following_span = self._driver.find_elements(By.CSS_SELECTOR, "span._ac2a")
         following_str = following_span.find_element(By.CSS_SELECTOR, "span").text
 
         # Remove the commas and convert to integer
         followers = int(following_str.replace(",", ""))
         return followers
 
+    @check_authorization
+    @check_private
     def send_dm(self, message: str) -> None:
         """
         Send a DM (direct message) to the user.
 
         Args:
             message (str): Message to send the user.
+
+        Raises:
+            NotAuthenticated: Raises when the current account is not logged in.
+            UserIsPrivate: Raises when the user is private.
         """
         # Enter the DMs
         message_btn = self._driver.find_element(By.XPATH, '//div[text()="Message"]')
         message_btn.click()
 
         # Write the the message
         message_input = self._driver.find_element(
@@ -331,14 +378,15 @@
 
         # Send message
         message_input = message_input.send_keys(Keys.ENTER)
 
         # Wait for message to send, moving on immediately after doesn't send the message
         time.sleep(0.5)
 
+    @check_private
     def get_posts(self, reels=True, limit=25) -> list:
         """
         Get a list of posts from the user's account.
 
         Args:
             reels (bool, optional): Whether to include reels or not. Defaults to True.
             limit (int, optional): Limits the amount of posts to retrieve. Defaults to 25 and can't be above 100.
@@ -352,14 +400,17 @@
         user = User("username")
         posts = user.get_posts()
 
         # Like his first three posts
         for post in posts[:3]:
             post.like()
         ```
+
+        Raises:
+            UserIsPrivate: Raises when the user is private.
         """
         from .post import Post
 
         css_selector = "a[href^='/p/']"
         if reels:
             css_selector += ",a[href^='/reel/']"
 
@@ -388,7 +439,18 @@
                 posts.append(post)
 
             # If no new posts loaded, break the loop
             if len(post_elements) == 0:
                 break
 
         return posts[:limit]
+
+    def open_user_dialog(self):
+        dialog_btn = self._driver.find_element(By.XPATH, '//div[text()="Following"]')
+        dialog_btn.click()
+
+    def close_user_dialog(self):
+        close_btn = self._driver.find_element(
+            By.CSS_SELECTOR,
+            'svg[aria-label="Close"]',
+        )
+        close_btn.click()
```

### Comparing `pygramcore-1.0.4/pygramcore/pygram.py` & `pygramcore-1.1.0/pygramcore/pygram.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 import pickle, os, time, random
 
 from .constants import *
 from .exceptions.auth import *
 from .exceptions.format import *
-from .utils.misc import write, navigate
+from .exceptions.navigation import *
+from .utils.navigation import *
 
 
 def check_authorization(func):
     """
     Decorator that checks if the current account is logged in.
 
     Raises:
@@ -46,26 +47,27 @@
 
     return driver
 
 
 class Navigator(type):
     def __new__(cls, name, bases, dct):
         """
-        Wraps all relevant functions with _default_initialize_website to initialize the object's url and provide the current instance of the driver.
+        Wraps all relevant functions with necessary wrapper functions.
         """
         fn_black_list = [
             "get_instance",
             "_initialize_website",
             "is_logged_in",
             "save_cookies",
         ]
 
         _initialize_website = dct.get(
             "_initialize_website", cls._default_initialize_website
         )
+
         for key, value in dct.items():
             if not key.startswith("__") and key not in fn_black_list:
                 # Support for class methods that aren't the get_instance function.
                 # This is done to prevent a recursion error, because the get_instance
                 # function is the function used in _initialize_website (causing the error)
                 if isinstance(value, classmethod):
                     wrapped_method = classmethod(
@@ -93,14 +95,54 @@
         """
         if not hasattr(self, "_driver"):
             self._driver = Account.get_instance()
 
         if hasattr(self, "url"):
             navigate(self._driver, self.url)
 
+            # Check if the URL has been found.
+            self._driver.implicitly_wait(1)
+            found_not_found_text = bool(
+                self._driver.find_elements(
+                    By.XPATH, '//span[text()="Sorry, this page isn\'t available."]'
+                )
+            )
+            self._driver.implicitly_wait(IMPLICIT_WAIT)
+
+            # Check if the text has not been found. If so, it should raise the
+            # PageNotFound exception.
+            if found_not_found_text:
+                raise PageNotFound(self._driver.current_url)
+
+    @classmethod
+    def _check_page_found(self):
+        """
+        Check if the current page has been found.
+
+        Raises:
+            PageNotFound: Raises when page wasn't found.
+        """
+        driver = Account.get_instance()
+
+        driver.implicitly_wait(2)
+
+        print("checking shit")
+        found_not_found_text = bool(
+            driver.find_elements(
+                By.XPATH, '//span[text()="Sorry, this page isn\'t available."]'
+            )
+        )
+
+        driver.implicitly_wait(IMPLICIT_WAIT)
+
+        # Check if the text has not been found. If so, it should raise the
+        # PageNotFound exception.
+        if not found_not_found_text:
+            raise PageNotFound(driver.current_url)
+
 
 class Account(metaclass=Navigator):
     _driver: webdriver.Chrome
     _logged_in: bool = False
 
     url: str = INSTAGRAM_URL
 
@@ -220,15 +262,15 @@
         """
         Removes all cookies and adds a list of new ones.
 
         Args:
             cookies (list[dict]): List of cookies from `.get_cookies()`.
         """
         cls._driver.delete_all_cookies()
-        cls._driver.get(INSTAGRAM_URL)
+        navigate(cls._driver, INSTAGRAM_URL)
 
         for cookie in cookies:
             cls._driver.add_cookie(cookie)
 
     @classmethod
     def load_cookies(cls, path: str):
         """
```

### Comparing `pygramcore-1.0.4/pygramcore/utils/misc.py` & `pygramcore-1.1.0/pygramcore/utils/navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime
 from selenium import webdriver
 import time, random
 
 
 def navigate(driver: webdriver.Chrome, url: str):
     """
     Navigates to a URL only if the URL is different to the current.
@@ -22,11 +21,7 @@
         input (WebElement): The input to write in.
         text (str): Text to be written.
         speed (int): Divides the random float (from 0 to 1). The higher the number the faster it writes. Defaults to 5.
     """
     for letter in text:
         input.send_keys(letter)
         time.sleep(random.random() / speed)
-
-
-def parse_instagram_date(time: str):
-    return datetime.strptime(time, "%Y-%m-%dT%H:%M:%S.%fZ")
```

### Comparing `pygramcore-1.0.4/pygramcore.egg-info/PKG-INFO` & `pygramcore-1.1.0/pygramcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.4
+Version: 1.1.0
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.4 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.1.0 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.4/pygramcore.egg-info/SOURCES.txt` & `pygramcore-1.1.0/pygramcore.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 pygramcore.egg-info/top_level.txt
 pygramcore/elements/__init__.py
 pygramcore/elements/post.py
 pygramcore/elements/user.py
 pygramcore/exceptions/__init__.py
 pygramcore/exceptions/auth.py
 pygramcore/exceptions/format.py
+pygramcore/exceptions/navigation.py
 pygramcore/exceptions/post.py
 pygramcore/exceptions/user.py
 pygramcore/utils/__init__.py
-pygramcore/utils/misc.py
+pygramcore/utils/misc.py
+pygramcore/utils/navigation.py
+tests/test_user.py
```

### Comparing `pygramcore-1.0.4/setup.py` & `pygramcore-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.4"
+VERSION = "1.1.0"
 DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

