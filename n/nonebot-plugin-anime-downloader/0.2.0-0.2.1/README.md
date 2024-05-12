# Comparing `tmp/nonebot_plugin_anime_downloader-0.2.0.tar.gz` & `tmp/nonebot_plugin_anime_downloader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_anime_downloader-0.2.0.tar", last modified: Sun May  5 05:28:51 2024, max compression
+gzip compressed data, was "nonebot_plugin_anime_downloader-0.2.1.tar", last modified: Sun May 12 03:35:37 2024, max compression
```

## Comparing `nonebot_plugin_anime_downloader-0.2.0.tar` & `nonebot_plugin_anime_downloader-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/LICENSE
--rw-r--r--   0        0        0     4232 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/README.md
--rw-r--r--   0        0        0    15250 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/acgrip/__init__.py
--rw-r--r--   0        0        0      654 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/config.py
--rw-r--r--   0        0        0      698 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/data_source.py
--rw-r--r--   0        0        0     1609 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/models.py
--rw-r--r--   0        0        0      175 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/models.py
--rw-r--r--   0        0        0     2860 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/routes.py
--rw-r--r--   0        0        0      761 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/tasks.py
--rw-r--r--   0        0        0      481 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/templates/index.html
--rw-r--r--   0        0        0     3928 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/utils.py
--rw-r--r--   0        0        0      730 2024-05-05 05:28:51.884538 nonebot_plugin_anime_downloader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4232 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/README.md
+-rw-r--r--   0        0        0    14721 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/acgrip/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/config.py
+-rw-r--r--   0        0        0      698 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/data_source.py
+-rw-r--r--   0        0        0     2109 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/downloader/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/downloader/exceptions.py
+-rw-r--r--   0        0        0     1214 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/downloader/models.py
+-rw-r--r--   0        0        0      191 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/models.py
+-rw-r--r--   0        0        0     3067 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/routes.py
+-rw-r--r--   0        0        0      631 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/tasks.py
+-rw-r--r--   0        0        0      481 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/templates/index.html
+-rw-r--r--   0        0        0     3928 2024-05-12 03:35:06.294956 nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/utils.py
+-rw-r--r--   0        0        0      730 2024-05-12 03:35:37.779116 nonebot_plugin_anime_downloader-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/LICENSE` & `nonebot_plugin_anime_downloader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/README.md` & `nonebot_plugin_anime_downloader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_alconna import UniMessage, Target
 
 from .config import Config
 from .tasks import TaskManager
 from .routes import VideoManager
 from .downloader import TorrentDownloader
+from .downloader.exceptions import TorrentExistsError
 from .data_source import ACGRIPBase, UserBase, VideoBase, ACGRIPData, User, Video
 from .utils import is_tag_match_title, generate_folder_name, extract_tags_from_title
 from .acgrip import (
     make_request,
     extract_data,
     get_anime_data,
     fetch_torrent_data,
@@ -89,37 +90,29 @@
 VideoBase.metadata.create_all(video_engine)
 
 acgrip_session = sessionmaker(bind=acg_rip_engine)()
 user_session = sessionmaker(bind=user_engine)()
 video_session = sessionmaker(bind=video_engine)()
 
 
-async def check_video_downloaded(title: str, torrent_id: int, user_id: str):
-    logger.info(f"Checking whether {title} is downloaded for {user_id}...")
-    if torrent_id in video_manager.ids:
-        logger.info(f"{title} is downloaded for {user_id}! Sending message...")
-        # send message to user
-        msg = (
-            f"{title} 现在可以观看了！\n"
-            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
-        )
-        chat_type = str(user_id).split("_")[0]
-        id_ = str(user_id).split("_")[-1]
-        target = Target(
-            id=id_,
-            parent_id=id_ if chat_type == "group" else "",
-            channel=chat_type == "group",
-            private=chat_type == "private",
-        )
-        await UniMessage(msg).send(target)
-        logger.info(f"Message sent to {user_id}!")
-
-        scheduler.remove_job(f"{title}_{user_id}")
-    else:
-        logger.info(f"{title} is not downloaded yet for {user_id}.")
+async def send_notification(title: str, torrent_id: int, user_id: str):
+    msg = (
+        f"{title} 现在可以观看了！\n"
+        + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
+    )
+    chat_type = str(user_id).split("_")[0]
+    id_ = str(user_id).split("_")[-1]
+    target = Target(
+        id=id_,
+        parent_id=id_ if chat_type == "group" else "",
+        channel=chat_type == "group",
+        private=chat_type == "private",
+    )
+    await UniMessage(msg).send(target)
+    logger.info(f"Message sent to {user_id}!")
 
 
 @scheduler.scheduled_job("interval", seconds=plugin_config.acgrip_interval)
 @nonebot.get_driver().on_startup
 async def fetch_acgrip_data():
     html_content = await make_request(base_url=plugin_config.acgrip_url)
     data = extract_data(replace_html_entities(html_content))
@@ -130,15 +123,15 @@
         if acgrip_session.query(ACGRIPData).filter_by(id=entry["id"]).first() is None:
             new_data.append(entry)
 
     if new_data == []:
         logger.debug("No new data found.")
         return None
 
-    logger.info(f"ACG.RIP updated with {len(new_data)} new entries.\n{new_data}")
+    logger.info(f"ACG.RIP updated with {len(new_data)} new entries.")
 
     # store new data
     for entry in new_data:
         acgrip_session.add(ACGRIPData(**entry))
     acgrip_session.commit()
 
     # check if any user is interested in the new data
@@ -147,28 +140,15 @@
         tags_str = user.tags
         tags_list: List[List[str]] = json.loads(tags_str)
         for tags in tags_list:
             for entry in new_data:
                 if is_tag_match_title(tags, entry["title"]):
                     # check if the video is already downloaded
                     if entry["id"] in video_manager.ids:
-                        # send message to user
-                        msg = (
-                            f"{entry['title']} 现在可以观看了！\n"
-                            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{entry['id']}"
-                        )
-                        chat_type = str(user.id).split("_")[0]
-                        id_ = str(user.id).split("_")[-1]
-                        target = Target(
-                            id=id_,
-                            parent_id=id_ if chat_type == "group" else "",
-                            channel=chat_type == "group",
-                            private=chat_type == "private",
-                        )
-                        await UniMessage(msg).send(target)
+                        await send_notification(entry["title"], entry["id"], user.id)
                         continue
 
                     # start download torrent
                     logger.info(f"Downloading {entry['title']} for {user.id}...")
 
                     if str(entry["url"]).startswith("http"):
                         url = f"{entry['url']}.torrent"
@@ -176,76 +156,93 @@
                         url = f"{plugin_config.acgrip_url}{entry['url']}.torrent"
 
                     torrent_data = await fetch_torrent_data(url)
                     try:
                         torrent_info = await torrent_downloader.download_torrent(
                             torrent_data, generate_folder_name(tags)
                         )
+                    except TorrentExistsError:
+                        logger.warning(
+                            f"Torrent {entry['title']} already exists in the download queue."
+                        )
+                        continue
                     except Exception:
                         logger.warning(
                             f"Failed to download {entry['title']} for {user.id}! Probably due to the same torrent."
                         )
                     task_manager.add(
                         {
                             "id": user.id,
                             "content": torrent_info,
                             "torrent_id": int(entry["id"]),
+                            "status": "downloading",
                         }
                     )
 
-                    # set a scheduler to check if the video is downloaded
-                    scheduler.add_job(
-                        check_video_downloaded,
-                        "interval",
-                        seconds=10,
-                        args=(entry["title"], int(entry["id"]), user.id),
-                        id=f"{entry['title']}_{user.id}",
-                    )
-
 
 @scheduler.scheduled_job("interval", seconds=60)
 async def check_for_tasks():
-    tasks = task_manager.get()
-
-    for task in tasks:
+    for task in task_manager.content:
         hash_str = task["content"]["hash"]
 
         torrent_info = await torrent_downloader.get_torrent_info(hash_str)
 
-        if torrent_info["progress"] != 1:
-            logger.info(f"Torrent {task['content']['name']} is not downloaded yet.")
-            task_manager.add(
-                {
-                    "id": task["id"],
-                    "content": torrent_info,
-                    "torrent_id": task["torrent_id"],
-                }
+        if torrent_info["progress"] == 1:
+            logger.info(f"Torrent {task['content']['name']} downloaded.")
+            task["status"] = "downloaded"
+            task_manager.save()
+
+        if task["status"] == "downloaded":
+            existing_video = (
+                video_session.query(Video).filter_by(id=task["torrent_id"]).first()
             )
-            return None
+            if existing_video is None:
+                video_session.add(
+                    Video(
+                        id=task["torrent_id"],
+                        title=torrent_info["name"],
+                        path=f"{torrent_info['save_path']}\\{torrent_info['name']}",
+                    )
+                )
 
-        logger.success(
-            f"Torrent {task['content']['name']} is downloaded, waiting to be added to the route..."
-        )
+            video_session.commit()
 
-        existing_video = (
-            video_session.query(Video).filter_by(id=task["torrent_id"]).first()
-        )
-        if existing_video is None:
-            video_session.add(
-                Video(
-                    id=task["torrent_id"],
-                    title=torrent_info["name"],
-                    path=f"{torrent_info['save_path']}\\{torrent_info['name']}",
-                )
+            if not Path(
+                f"{torrent_info['save_path']}\\{torrent_info['name']}"
+            ).exists():
+                continue
+
+            video_manager.add_route(
+                Path(f"{torrent_info['save_path']}\\{torrent_info['name']}"),
+                task["torrent_id"],
+            )
+
+            logger.success(f"Added route for video {torrent_info['name']}.")
+
+            task["status"] = "wait_for_send"
+
+        if task["status"] == "wait_for_send":
+            await send_notification(
+                torrent_info["name"], task["torrent_id"], task["id"]
             )
 
-        video_session.commit()
+            task["status"] = "sent"
+            task_manager.save()
+
+            logger.info(
+                f"Notification of {torrent_info['name']} sent for {task['id']}."
+            )
+
+    # remove sent tasks
+    task_manager.content = [
+        task for task in task_manager.content if task["status"] != "sent"
+    ]
+    task_manager.save()
 
 
-@scheduler.scheduled_job("interval", seconds=30)
 @nonebot.get_driver().on_startup
 async def check_for_new_videos():
     videos = video_session.query(Video).all()
 
     for video in videos:
         if not Path(video.path).exists():
             continue
@@ -408,27 +405,22 @@
     torrent_data = await fetch_torrent_data(
         f"{plugin_config.acgrip_url}/t/{torrent_id}.torrent"
     )
     try:
         torrent_info = await torrent_downloader.download_torrent(
             torrent_data, generate_folder_name(tags)
         )
-    except Exception:
-        await download.finish("下载失败！请稍后重试。")
+    except TorrentExistsError:
+        await download.finish("任务已处于下载队列中")
+    except Exception as e:
+        await download.finish(f"下载失败！请稍后重试。\n{type(e).__name__}: {e}")
 
     task_manager.add(
         {
             "id": id_,
             "content": torrent_info,
             "torrent_id": int(torrent_id),
+            "status": "downloading",
         }
     )
 
     await download.send(f"开始下载 {anime_entry.title}...")
-
-    scheduler.add_job(
-        check_video_downloaded,
-        "interval",
-        seconds=10,
-        args=(anime_entry.title, int(torrent_id), id_),
-        id=f"{anime_entry.title}_{id_}",
-    )
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/acgrip/__init__.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/acgrip/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/config.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/data_source.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/downloader/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import binascii
 import torrent_parser
 from pathlib import Path
 from qbittorrentapi import Client
 from nonebot.utils import run_sync
 
 from .models import TorrentInfo
+from .exceptions import TorrentExistsError, TorrentUnexistsError
 
 
 class TorrentDownloader:
     def __init__(self, host: str, username: str, password: str, download_path: Path):
         self.client = Client(host=host, username=username, password=password)
         self.download_path = download_path
 
@@ -20,26 +21,36 @@
         info_bytes = torrent_parser.encode(torrent["info"])
         info_hash = binascii.hexlify(hashlib.sha1(info_bytes).digest()).decode()
         return info_hash
 
     async def download_torrent(
         self, torrent_file: bytes, folder_name: str
     ) -> TorrentInfo:
+        hash_str = self._get_torrent_hash(torrent_file)
+
+        if (await self.is_torrent_exists(hash_str)):
+            raise TorrentExistsError(f"Torrent with hash {hash_str} already exists.")
+
         text = await run_sync(self.client.torrents_add)(
             torrent_files=torrent_file, save_path=self.download_path / folder_name
         )
 
         if text == "Fails.":
             raise Exception("Failed to download torrent.")
 
-        hash_str = self._get_torrent_hash(torrent_file)
         await run_sync(self.client.torrents_reannounce)(torrent_hashes=hash_str)
 
         torrent_info = (
             await run_sync(self.client.torrents_info)(torrent_hashes=hash_str)
         )[0]
 
         return torrent_info
 
+    async def is_torrent_exists(self, hash_str: str) -> bool:
+        torrents = await run_sync(self.client.torrents_info)(torrent_hashes=hash_str)
+        return torrents != []
+
     async def get_torrent_info(self, hash_str: str) -> TorrentInfo:
         torrents = await run_sync(self.client.torrents_info)(torrent_hashes=hash_str)
+        if torrents == []:
+            raise TorrentUnexistsError(f"Torrent with hash {hash_str} does not exist.")
         return torrents[0]
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/models.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/downloader/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/routes.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,8 +71,12 @@
             return StreamingResponse(
                 iterfile(),
                 status_code=status_code,
                 headers=headers,
                 media_type=f"video/{video_path.suffix[1:]}",
             )
 
-        logger.success(f"Added route for video {video_path.name}.")
+    def add_routes(self, video_paths: List[Path], torrent_ids: List[int]) -> None:
+        for video_path, torrent_id in zip(video_paths, torrent_ids):
+            self.add_route(video_path, torrent_id)
+
+        logger.success(f"Added routes for {len(video_paths)} videos.")
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/tasks.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,13 +18,7 @@
     def save(self) -> None:
         with open(self._file_path, "w", encoding="utf-8") as f:
             json.dump(self.content, f, indent=4, ensure_ascii=False)
 
     def add(self, content: Task) -> None:
         self.content.append(content)
         self.save()
-
-    def get(self) -> List[Task]:
-        tasks = self.content
-        self.content = []
-        self.save()
-        return tasks
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/utils.py` & `nonebot_plugin_anime_downloader-0.2.1/nonebot_plugin_anime_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.2.0/pyproject.toml` & `nonebot_plugin_anime_downloader-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-anime-downloader"
-version = "0.2.0"
+version = "0.2.1"
 description = "✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "aiohttp>=3.9.5",
```

### Comparing `nonebot_plugin_anime_downloader-0.2.0/PKG-INFO` & `nonebot_plugin_anime_downloader-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-anime-downloader
-Version: 0.2.0
+Version: 0.2.1
 Summary: ✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: aiohttp>=3.9.5
 Requires-Dist: qbittorrent-api>=2024.3.60
```

