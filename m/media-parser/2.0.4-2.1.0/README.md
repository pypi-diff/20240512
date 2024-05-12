# Comparing `tmp/media_parser-2.0.4.tar.gz` & `tmp/media_parser-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-2.0.4.tar", max compression
+gzip compressed data, was "media_parser-2.1.0.tar", max compression
```

## Comparing `media_parser-2.0.4.tar` & `media_parser-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-05-08 10:49:50.277922 media_parser-2.0.4/LICENSE
--rw-r--r--   0        0        0      891 2024-05-08 10:49:50.277922 media_parser-2.0.4/README.md
--rw-r--r--   0        0        0      239 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/__init__.py
--rw-r--r--   0        0        0      258 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/context.py
--rw-r--r--   0        0        0       42 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/database/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/database/base.py
--rw-r--r--   0        0        0      451 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/database/models.py
--rw-r--r--   0        0        0      127 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/models/__init__.py
--rw-r--r--   0        0        0     4859 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/models/medias.py
--rw-r--r--   0        0        0      171 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/__init__.py
--rw-r--r--   0        0        0     5208 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/base.py
--rw-r--r--   0        0        0     5824 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/instagram.py
--rw-r--r--   0        0        0     4195 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/reddit.py
--rw-r--r--   0        0        0     9815 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/tiktok.py
--rw-r--r--   0        0        0     3169 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/twitter.py
--rw-r--r--   0        0        0     3348 2024-05-08 10:49:50.277922 media_parser-2.0.4/media_parser/parsers/youtube.py
--rw-r--r--   0        0        0      862 2024-05-08 10:49:50.281922 media_parser-2.0.4/media_parser/utils.py
--rw-r--r--   0        0        0     2763 2024-05-08 10:49:50.281922 media_parser-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 media_parser-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-12 17:06:26.841215 media_parser-2.1.0/LICENSE
+-rw-r--r--   0        0        0      891 2024-05-12 17:06:26.841215 media_parser-2.1.0/README.md
+-rw-r--r--   0        0        0      239 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/context.py
+-rw-r--r--   0        0        0       42 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/database/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/database/base.py
+-rw-r--r--   0        0        0      451 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/database/models.py
+-rw-r--r--   0        0        0      127 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4859 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/models/medias.py
+-rw-r--r--   0        0        0      171 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/base.py
+-rw-r--r--   0        0        0     5790 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/instagram.py
+-rw-r--r--   0        0        0     4510 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/reddit.py
+-rw-r--r--   0        0        0     9905 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/tiktok.py
+-rw-r--r--   0        0        0     3135 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/twitter.py
+-rw-r--r--   0        0        0     3294 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/parsers/youtube.py
+-rw-r--r--   0        0        0      862 2024-05-12 17:06:26.845215 media_parser-2.1.0/media_parser/utils.py
+-rw-r--r--   0        0        0     2763 2024-05-12 17:06:26.845215 media_parser-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 media_parser-2.1.0/PKG-INFO
```

### Comparing `media_parser-2.0.4/LICENSE` & `media_parser-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.4/README.md` & `media_parser-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.4/media_parser/database/base.py` & `media_parser-2.1.0/media_parser/database/base.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.4/media_parser/models/medias.py` & `media_parser-2.1.0/media_parser/models/medias.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.4/media_parser/parsers/base.py` & `media_parser-2.1.0/media_parser/parsers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from abc import ABC, abstractmethod
 from re import Match, Pattern
 from typing import Any, ClassVar, Required, Self, TypedDict
 
 import aiohttp
 from motor.motor_asyncio import AsyncIOMotorCollection
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 
 from media_parser.database import GroupedMediaModel, MongoModelController
 from media_parser.models import Media, ParserType
 from media_parser.utils import generate_timer
 
 logger = logging.getLogger(__name__)
 time_it = generate_timer(logger)
@@ -53,27 +53,31 @@
         return medias
 
 
 class BaseParserConfig(TypedDict):
     type: Required[ParserType]
 
 
-class BaseParser(ABC):
+class BaseParser(ABC, BaseModel):
     TYPE: ClassVar[ParserType]
+    _parsers: list["BaseParser"] = PrivateAttr(default_factory=list)
 
     def __init__(self, *args, config: dict[str, dict[str, Any]] | None = None, **kwargs):
         super().__init__(*args, **kwargs)
         if config is None:
             config = {}
+
         if type(self) is BaseParser:
             self._parsers: list[BaseParser] = [
                 parser(**conf)
                 for parser in BaseParser.__subclasses__()
                 if (conf := config.get(parser.TYPE.value.lower(), None)) is not None
             ]
+        else:
+            self._parsers = [self]
 
     def supported(self) -> dict[ParserType, bool]:
         return {parser.TYPE: parser._is_supported() for parser in self._parsers}
 
     @abstractmethod
     def reg_exps(self) -> list[Pattern[str]]:
         raise NotImplementedError
```

### Comparing `media_parser-2.0.4/media_parser/parsers/instagram.py` & `media_parser-2.1.0/media_parser/parsers/instagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import asyncio
 import json
 import logging
 import re
 from re import Match, Pattern
 
 import aiohttp
-from pydantic import BaseModel, Field
+from pydantic import Field
 
 from media_parser.models import Media, ParserType, Video
-
-from .base import BaseParser as BaseParser
-from .base import MediaCache
+from media_parser.parsers.base import BaseParser, MediaCache
 
 logger = logging.getLogger(__name__)
 
 USER_AGENT = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36"
 
 
-class InstagramParser(BaseParser, BaseModel, type=ParserType.INSTAGRAM):
+class InstagramParser(BaseParser, type=ParserType.INSTAGRAM):
     instagram_saas_token: str | None = Field(default=None, description="Set this for enable instagram proxy")
     instagram_saas_api: str = Field(
         default="https://api.lamadava.com", description="Set this to change instagram saas api"
     )
     user_agent: str = Field(default=USER_AGENT, description="Set this to change user agent")
 
     def reg_exps(self) -> list[Pattern[str]]:
```

### Comparing `media_parser-2.0.4/media_parser/parsers/reddit.py` & `media_parser-2.1.0/media_parser/parsers/reddit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+import asyncio
 import logging
 import re
 from re import Match, Pattern
 from urllib.parse import urlparse
 
 import aiohttp
 from aiohttp import InvalidURL
-from pydantic import BaseModel, Field
+from pydantic import Field
 
 from media_parser.models import Media, ParserType, Video
-
-from .base import BaseParser as BaseParser
-from .base import MediaCache
+from media_parser.parsers.base import BaseParser, MediaCache
 
 logger = logging.getLogger(__name__)
 
 
-class RedditParser(BaseParser, BaseModel, type=ParserType.REDDIT):
+class RedditParser(BaseParser, type=ParserType.REDDIT):
     user_agent: str | None = Field("video downloader (by u/Jag_k)", description="User agent for Reddit API")
     client_id: str = Field(..., description="Client ID for Reddit API")
     client_secret: str = Field(..., description="Client secret for Reddit API")
 
     def reg_exps(self) -> list[Pattern[str]]:
         return [
             # redd.it/2gmzqe
@@ -125,7 +124,21 @@
 
     else:
         submission_id = parts[parts.index("comments") + 1]
 
     if not submission_id.isalnum():
         raise InvalidURL(url)
     return submission_id
+
+
+if __name__ == "__main__":
+
+    async def main():
+        async with aiohttp.ClientSession() as session:
+            print(
+                await RedditParser().parse(
+                    session,
+                    "www.reddit.com/r/redditdev/comments/2gmzqe/praw_https/",
+                )
+            )
+
+    asyncio.run(main())
```

### Comparing `media_parser-2.0.4/media_parser/parsers/tiktok.py` & `media_parser-2.1.0/media_parser/parsers/tiktok.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 import logging
 import re
 from re import Match
 from typing import Literal
 
 import aiohttp
 from aiohttp import ClientSession
-from pydantic import BaseModel, Field
+from pydantic import Field
 
-from media_parser.context import MAX_SIZE
+from media_parser.context import get_max_size
 from media_parser.models import Image, Media, ParserType, Video
+from media_parser.parsers.base import BaseParser, MediaCache
 from media_parser.utils import generate_timer
 
-from .base import BaseParser as BaseParser
-from .base import MediaCache
-
 logger = logging.getLogger(__name__)
 
 TT_USER_AGENT = (
     "com.ss.android.ugc.trill/494+Mozilla/5.0+(Linux;+Android+12;+2112123G+Build/SKQ1.211006.001;+wv)"
     "+AppleWebKit/537.36+(KHTML,+like+Gecko)+Version/4.0+Chrome/107.0.5304.105+Mobile+Safari/537.36"
 )
 
 time_it = generate_timer(logger)
 
 
-class TiktokParser(BaseParser, BaseModel, type=ParserType.TIKTOK):
+class TiktokParser(BaseParser, type=ParserType.TIKTOK):
     user_agent: str = Field(default=TT_USER_AGENT)
 
     def reg_exps(self):
         return [
             # https://www.tiktok.com/t/ZS8s7cPmd/
             re.compile(r"(?:https?://)?(?:www\.)?tiktok\.com/(?P<short_suffix>\w+)/(?P<id>\w+)/?"),
             # https://vt.tiktok.com/ZSRq1jcrg/
             # https://vm.tiktok.com/ZSRq1jcrg/
             re.compile(r"(?:https?://)?(?:(?P<domain>[a-z]{2})\.)?tiktok\.com/(?P<id>\w+)/?"),
             # https://www.tiktok.com/@thejoyegg/video/7136001098841591041
-            re.compile(r"(?:https?://)?(?:www\.)?tiktok\.com/@(?P<author>\w+)/video/(?P<video_id>\d+)/?"),
+            re.compile(
+                r"(?:https?://)?(?:www\.)?tiktok\.com/@(?P<author>\w+)/(?P<type_of>video|photo)/(?P<video_id>\d+)/?"
+            ),
         ]
 
     def _is_supported(self) -> bool:
         return True
 
     async def _parse(
         self,
@@ -81,15 +81,15 @@
             "Getting video link from: %s (video_id=%d)",
             original_url,
             video_id,
         )
 
         try:
             with time_it("tiktok_get_video_data"):
-                data: dict = await self._get_video_data(video_id)
+                data: dict = await self._get_media_data(session, video_id)
 
         except Exception as e:
             logger.exception(
                 "Error while getting video data: %s",
                 original_url,
                 exc_info=e,
             )
@@ -114,18 +114,15 @@
             elif media_type == "image":
                 return await cache.save_group(self._process_image(data, original_url))
         return []
 
     def _process_video(self, data: dict, original_url: str) -> list[Video]:
         max_quality_url = data.get("video_data", {}).get("nwm_video_url_HQ")
 
-        try:
-            max_size = float(MAX_SIZE.get("inf"))
-        except ValueError:
-            max_size = float("inf")
+        max_size = get_max_size()
 
         try:
             url: str | None = max(
                 filter(
                     lambda x: x.get("data_size", 0) <= max_size,
                     (x.get("play_addr", {}) for x in data.get("video", {}).get("bit_rate", [])),
                 ),
@@ -194,34 +191,37 @@
         base = url.rsplit("/", 1)[-1]
         author = url.split("@", 1)[-1].split("/", 1)[0]
         if not base or not base.isdigit():
             return None
         return author, int(base)
 
     @staticmethod
-    async def _get_video_data(video_id: int) -> dict:
-        async with ClientSession(
-            headers={
-                "Accept": "application/json",
-                "User-Agent": TT_USER_AGENT,
-            }
-        ) as session:
-            async with session.get(
-                "https://api16-normal-c-useast1a.tiktokv.com/aweme/v1/feed/",
-                params={
-                    "aweme_id": video_id,
-                },
-            ) as resp:
-                raw_data: dict = await resp.json()
-            if not raw_data:
-                logger.error("Empty response with %r", resp.url)
-                return {}
+    async def _get_media_data(session: ClientSession, video_id: int) -> dict:
+        async with session.get(
+            "https://api16-normal-c-useast1a.tiktokv.com/aweme/v1/feed/",
+            params={
+                "iid": "7318518857994389254",
+                "device_id": "7318517321748022790",
+                "channel": "googleplay",
+                "app_name": "musical_ly",
+                "version_code": "300904",
+                "device_platform": "android",
+                "device_type": "ASUS_Z01QD",
+                "os_version": "9",
+                "aweme_id": video_id,
+            },
+        ) as resp:
+            raw_data: dict = await resp.json()
+        if not raw_data:
+            logger.error("Empty response with %r", resp.url)
+            return {}
         if not raw_data.get("aweme_list", []):
             logger.info("No aweme_list in response")
             return {}
+
         data = raw_data["aweme_list"][0]
         url_type_code = data["aweme_type"]
         url_type_code_dict = {
             0: "video",
             51: "video",
             55: "video",
             58: "video",
@@ -265,17 +265,16 @@
             }
         return data | api_data
 
 
 if __name__ == "__main__":
 
     async def main():
-        parser = TiktokParser()
         async with ClientSession() as session:
             print(
-                await parser.parse(
+                await TiktokParser().parse(
                     session,
-                    "https://vm.tiktok.com/ZMYQFQBQ9/",
+                    "https://www.tiktok.com/@kastella_/photo/7364744013653527814",
                 )
             )
 
     asyncio.run(main())
```

### Comparing `media_parser-2.0.4/media_parser/parsers/twitter.py` & `media_parser-2.1.0/media_parser/parsers/twitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import logging
 import re
 from re import Match
 
 import aiohttp
-from pydantic import BaseModel, Field
+from pydantic import Field
 
 from media_parser.models import Media, ParserType, Video
-
-from .base import BaseParser as BaseParser
-from .base import MediaCache
+from media_parser.parsers.base import BaseParser, MediaCache
 
 logger = logging.getLogger(__name__)
 
 # https://twitter.com/Yoda4ever/status/1580609309217628160
 TWITTER_RE = re.compile(r"(?:https?://)?(?:www\.)?twitter\.com/(?P<user>\w+)/status/(?P<id>\d+)")
 # https://x.com/Yoda4ever/status/1580609309217628160
 X_RE = re.compile(r"(?:https?://)?(?:www\.)?x\.com/(?P<user>\w+)/status/(?P<id>\d+)")
 
 
-class TwitterParser(BaseParser, BaseModel, type=ParserType.TWITTER):
+class TwitterParser(BaseParser, type=ParserType.TWITTER):
     twitter_bearer_token: str = Field(..., description="Bearer token for Twitter API")
 
     def reg_exps(self):
         return [
             TWITTER_RE,
             X_RE,
             # https://t.co/sOHvySZwUo
```

### Comparing `media_parser-2.0.4/media_parser/parsers/youtube.py` & `media_parser-2.1.0/media_parser/parsers/youtube.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 import logging
 import re
 from re import Match
 
 import aiohttp
 import httpx
 import pytube
-from pydantic import BaseModel
 from pytube import StreamQuery
 from pytube.exceptions import PytubeError
 
 from media_parser.context import get_max_size
 from media_parser.models import Media, ParserType, Video
-
-from .base import BaseParser as BaseParser
-from .base import MediaCache
+from media_parser.parsers.base import BaseParser, MediaCache
 
 logger = logging.getLogger(__name__)
 
 
-class YoutubeParser(BaseParser, BaseModel, type=ParserType.YOUTUBE):
+class YoutubeParser(BaseParser, type=ParserType.YOUTUBE):
     def reg_exps(self):
         return [
             # https://www.youtube.com/watch?v=TCrP1SE2DkY
             # https://youtu.be/TCrP1SE2DkY
             re.compile(r"(?:https?://)?" r"(?:" r"(?:www\.)?youtube\.com/watch\?v=" r"|youtu.be/" r")(?P<id>[\w-]+)"),
             # https://youtube.com/shorts/hBOLCcvbGHM
             # https://youtube.com/watch?v=hBOLCcvbGHM
```

### Comparing `media_parser-2.0.4/media_parser/utils.py` & `media_parser-2.1.0/media_parser/utils.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.4/pyproject.toml` & `media_parser-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "2.0.4"
+version = "2.1.0"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
```

### Comparing `media_parser-2.0.4/PKG-INFO` & `media_parser-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 2.0.4
+Version: 2.1.0
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
```

