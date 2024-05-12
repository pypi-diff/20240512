# Comparing `tmp/accesser-0.9.2.tar.gz` & `tmp/accesser-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accesser-0.9.2.tar", last modified: Sun Mar 10 05:05:59 2024, max compression
+gzip compressed data, was "accesser-0.9.3.tar", last modified: Sun May 12 09:02:37 2024, max compression
```

## Comparing `accesser-0.9.2.tar` & `accesser-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 05:05:59.310205 accesser-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-10 05:05:55.000000 accesser-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-10 05:05:59.310205 accesser-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-10 05:05:55.000000 accesser-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 05:05:59.306205 accesser-0.9.2/accesser/
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/pac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 05:05:59.306205 accesser-0.9.2/accesser/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/cert_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/certmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/importca.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-10 05:05:55.000000 accesser-0.9.2/accesser/utils/sysproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 05:05:59.310205 accesser-0.9.2/accesser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-10 05:05:59.000000 accesser-0.9.2/accesser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-10 05:05:55.000000 accesser-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 05:05:59.310205 accesser-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:02:37.168451 accesser-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-12 09:02:28.000000 accesser-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-12 09:02:37.168451 accesser-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-12 09:02:28.000000 accesser-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:02:37.164451 accesser-0.9.3/accesser/
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/pac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:02:37.168451 accesser-0.9.3/accesser/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/cert_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/certmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/importca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-12 09:02:28.000000 accesser-0.9.3/accesser/utils/sysproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:02:37.168451 accesser-0.9.3/accesser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 09:02:37.000000 accesser-0.9.3/accesser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-12 09:02:28.000000 accesser-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:02:37.168451 accesser-0.9.3/setup.cfg
```

### Comparing `accesser-0.9.2/LICENSE` & `accesser-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/PKG-INFO` & `accesser-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.9.2
+Version: 0.9.3
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.2/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.3/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U "accesser[doh,doq]"
 ```
 如果你不需要 DNS-over-HTTPS 和 DNS-over-QUIC，则可以不用带`[doh,doq]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.9.2/README.md` & `accesser-0.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.2/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.3/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U "accesser[doh,doq]"
 ```
 如果你不需要 DNS-over-HTTPS 和 DNS-over-QUIC，则可以不用带`[doh,doq]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.9.2/accesser/__init__.py` & `accesser-0.9.3/accesser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 import os, sys
 import json
 import fnmatch
 import random
 import ssl
 import asyncio
@@ -140,20 +140,17 @@
             cert_policy = False if cert_verify_list is False else True
         elif server_hostname_key is not None:
             cert_verify_list = [setting.config['alter_hostname'][server_hostname_key]]
             cert_policy = setting.config['check_hostname']
         else:
             cert_verify_list = [host]
             cert_policy = setting.config['check_hostname']
-        if not cert_policy is False:
-            try:
-                next(filter(lambda h:match_hostname(cert, h, cert_policy), cert_verify_list))
-            except StopIteration:
-                logger.warning(f"[{i_port:5}] {cert_verify_list} don't march either of {cert_message}.")
-                return
+        if  cert_policy is not False and not any(match_hostname(cert, h, cert_policy) for h in cert_verify_list):
+            logger.warning(f"[{i_port:5}] {cert_verify_list} don't march either of {cert_message}.")
+            return
         await asyncio.gather(
             forward_stream(reader, remote_writer),
             forward_stream(remote_reader, writer)
         )
     writer.close()
     remote_writer.close()
     await remote_writer.wait_closed()
```

### Comparing `accesser-0.9.2/accesser/config.toml` & `accesser-0.9.3/accesser/config.toml`

 * *Files 7% similar despite different names*

```diff
@@ -94,31 +94,34 @@
 "steamcommunity.com" = "www.valvesoftware.com"
 "docs.github.com" = "api.github.com"
 "pubsub-edge.twitch.tv" = "external-2.us-west-2.prod.twitchpubsubedge.twitch.a2z.com"
 "irc-ws.chat.twitch.tv" = "websocket-7.us-west-2.prod.twitchircedge.twitch.a2z.com"
 "vod-secure.twitch.tv" = "ds0h3roq6wcgc.cloudfront.net"
 "extension-files.twitch.tv" = "d36mepituis1gg.cloudfront.net"
 "panels.twitch.tv" = "d1ut6fykkt3imt.cloudfront.net"
+"extensions-discovery-images.twitch.tv" = "d3m1uefep57n8q.cloudfront.net"
 "downloads.scratch.mit.edu" = "d2as4384mnnkdz.cloudfront.net"
 "gn-web-assets.api.bbc.com" = "static-web-assets.gnl-common.bbcverticals.com"
 "onedrive.live.com" = "0.azureedge.net"
+"euronews.com" = "euronews.news"
 
 
 [cert_verify]
 
 # 为域名分别设置证书校验策略，其值可以是一个包含用于校验的域名的列表（有一个匹配就通过），也可以是 false 表示不校验
 # 这比 [alter_hostname] 和全局的 check_hostname 的优先级高，但不会在 Client Hello 中作为 server_name 发送。
 # Set the certificate validation policy for domains individually. The values can be a array contain strings which represent the domain name used to verify the certificate (pass if there is a match), or false which means disabling the verification.
 # It has as a higher priority than [alter_hostname] and the global check_hostname, but will not be sent as server_name in Client Hello.
 
 "singlelogin.se" = ["1lib.fr", "singlelogin.se", "singlelogin.re"]
+"*.singlelogin.se" = ["1lib.fr", "singlelogin.se", "singlelogin.re"]
 "singlelogin.re" = ["1lib.fr", "singlelogin.se", "singlelogin.re"]
+"*.singlelogin.re" = ["1lib.fr", "singlelogin.se", "singlelogin.re"]
 "scratch.mit.edu" = ["scratchfoundation.map.fastly.net"]
 "*.scratch.mit.edu" = ["scratchfoundation.map.fastly.net"]
-"euronews.com" = ["fastly.com"]
 "*.euronews.com" = ["fastly.com"]
 "mega.io" = ["static.mega.co.nz"]
 "bandcamp.com" = ["fastly.com"]
 "*.bandcamp.com" = ["fastly.com"]
 "nytimes.com" = ["fastly.com"]
 "*.nytimes.com" = ["fastly.com"]
 "reddit.com" = ["fastly.com"]
@@ -172,30 +175,46 @@
 "reddit.com" = "fastly.com"
 ".reddit.com" = "fastly.com"
 "redd.it" = "fastly.com"
 ".redd.it" = "fastly.com"
 ".redditstatic.com" = "fastly.com"
 "redditmedia.com" = "fastly.com"
 ".redditmedia.com" = "fastly.com"
+".euronews.com" = "fastly.com"
 "www.bbc.com" = "151.101.128.81"
 "disqus.com" = "151.101.64.134"
 "i.imgur.com" = "151.101.196.193"
 "i.stack.imgur.com" = "151.101.196.193"
 ".theepochtimes.com" = "151.139.128.13"
 "donate.epochtimes.com" = "151.139.128.13"
 "i.epochtimes.com" = "151.139.128.13"
+"mediawiki.org" = "text-lb.esams.wikimedia.org"
 ".mediawiki.org" = "text-lb.esams.wikimedia.org"
+"wikipedia.org" = "text-lb.esams.wikimedia.org"
 ".wikipedia.org" = "text-lb.esams.wikimedia.org"
+"wikiquote.org" = "text-lb.esams.wikimedia.org"
 ".wikiquote.org" = "text-lb.esams.wikimedia.org"
+"wikinews.org" = "text-lb.esams.wikimedia.org"
 ".wikinews.org" = "text-lb.esams.wikimedia.org"
+"wikiversity.org" = "text-lb.esams.wikimedia.org"
 ".wikiversity.org" = "text-lb.esams.wikimedia.org"
+"wiktionary.org" = "text-lb.esams.wikimedia.org"
 ".wiktionary.org" = "text-lb.esams.wikimedia.org"
+"wikibooks.org" = "text-lb.esams.wikimedia.org"
 ".wikibooks.org" = "text-lb.esams.wikimedia.org"
+"wikivoyage.org" = "text-lb.esams.wikimedia.org"
 ".wikivoyage.org" = "text-lb.esams.wikimedia.org"
+"wikisource.org" = "text-lb.esams.wikimedia.org"
 ".wikisource.org" = "text-lb.esams.wikimedia.org"
+"wikidata.org" = "text-lb.esams.wikimedia.org"
 ".wikidata.org" = "text-lb.esams.wikimedia.org"
+"wikimedia.org" = "text-lb.esams.wikimedia.org"
+"upload.wikimedia.org" = "upload-lb.esams.wikimedia.org"
+".wikimedia.org" = "text-lb.esams.wikimedia.org"
 "exhentai.org" = "178.175.128.252"
 "scratch.mit.edu" = "scratchfoundation.map.fastly.net"
 ".scratch.mit.edu" = "scratchfoundation.map.fastly.net"
 "archive.org" = "207.241.224.27"
 "mastodon.social" = "fastly.com"
-"*.mastodon.social" = "fastly.com"
+"*.mastodon.social" = "fastly.com"
+"singlelogin.se" = "195.66.210.33"
+".singlelogin.se" = "195.66.210.33"
```

### Comparing `accesser-0.9.2/accesser/pac` & `accesser-0.9.3/accesser/pac`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,23 @@
   "thetvdb.com": 1,
   "tumblr.com": 1,
   "tumblr.co": 1,
   "uptodown.com": 1,
   "vimeo.com": 1,
   "wenxuecity.com": 1,
   "wikipedia.org": 1,
+  "mediawiki.org": 1,
+  "wikiquote.org": 1,
+  "wikinews.org": 1,
+  "wikiversity.org": 1,
+  "wiktionary.org": 1,
+  "wikibooks.org": 1,
+  "wikivoyage.org": 1,
+  "wikisource.org": 1,
+  "wikidata.org": 1,
   "singlelogin.re": 1,
   "singlelogin.se": 1,
   "archive.org": 1,
   "amazon.co.jp": 1,
   "discord.com": 1,
   "discordapp.com": 1,
   "discord.gg": 1,
```

### Comparing `accesser-0.9.2/accesser/utils/cert_verify.py` & `accesser-0.9.3/accesser/utils/cert_verify.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser/utils/certmanager.py` & `accesser-0.9.3/accesser/utils/certmanager.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser/utils/importca.py` & `accesser-0.9.3/accesser/utils/importca.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser/utils/log.py` & `accesser-0.9.3/accesser/utils/log.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser/utils/setting.py` & `accesser-0.9.3/accesser/utils/setting.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser/utils/sysproxy.py` & `accesser-0.9.3/accesser/utils/sysproxy.py`

 * *Files identical despite different names*

### Comparing `accesser-0.9.2/accesser.egg-info/PKG-INFO` & `accesser-0.9.3/accesser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accesser
-Version: 0.9.2
+Version: 0.9.3
 Summary: 🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST
 Author: URenko
 Project-URL: Homepage, https://github.com/URenko/Accesser
 Project-URL: Bug Tracker, https://github.com/URenko/Accesser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 [![](https://img.shields.io/github/release/URenko/Accesser.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/pypi/v/accesser)](https://pypi.org/project/accesser/)
 [![](https://img.shields.io/github/downloads/URenko/Accesser/total.svg)](https://github.com/URenko/Accesser/releases/latest)
 [![](https://img.shields.io/github/license/URenko/Accesser.svg)](https://github.com/URenko/Accesser/blob/master/LICENSE)
 
 ## 使用
 ### 如果不知道什么是Python
-从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.2/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
+从[这里](https://github.com/URenko/Accesser/releases/download/v0.9.3/accesser.exe)下载Windows一键程序，运行既可（建议关闭其他代理软件），首次使用会要求安装证书，选是即可。
 ### 如果已经安装了Python 3.10*或更高版本
 ```
 pip3 install -U "accesser[doh,doq]"
 ```
 如果你不需要 DNS-over-HTTPS 和 DNS-over-QUIC，则可以不用带`[doh,doq]`。
 
 然后通过如下命令启动：
```

### Comparing `accesser-0.9.2/pyproject.toml` & `accesser-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "accesser"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="URenko" },
 ]
 description = "🌏一个解决SNI RST导致维基百科、Pixiv等站点无法访问的工具 | A tool for solving SNI RST"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

