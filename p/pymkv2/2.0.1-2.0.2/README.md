# Comparing `tmp/pymkv2-2.0.1.tar.gz` & `tmp/pymkv2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymkv2-2.0.1.tar", max compression
+gzip compressed data, was "pymkv2-2.0.2.tar", max compression
```

## Comparing `pymkv2-2.0.1.tar` & `pymkv2-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-10 13:52:03.198863 pymkv2-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2543 2024-05-10 13:54:05.543434 pymkv2-2.0.1/README.md
--rw-r--r--   0        0        0      521 2023-10-19 00:13:50.056583 pymkv2-2.0.1/pymkv/BCP47.py
--rw-r--r--   0        0        0      597 2024-05-11 20:31:37.952374 pymkv2-2.0.1/pymkv/ISO639_2.py
--rw-r--r--   0        0        0     3115 2024-05-11 20:31:37.952429 pymkv2-2.0.1/pymkv/MKVAttachment.py
--rw-r--r--   0        0        0    40210 2024-05-11 20:31:37.952490 pymkv2-2.0.1/pymkv/MKVFile.py
--rw-r--r--   0        0        0    14612 2024-05-11 20:31:37.952623 pymkv2-2.0.1/pymkv/MKVTrack.py
--rw-r--r--   0        0        0     8735 2024-05-11 20:31:37.952723 pymkv2-2.0.1/pymkv/Timestamp.py
--rw-r--r--   0        0        0     1761 2024-05-11 20:31:37.952776 pymkv2-2.0.1/pymkv/TypeTrack.py
--rw-r--r--   0        0        0     3941 2024-05-11 20:31:37.952832 pymkv2-2.0.1/pymkv/Verifications.py
--rw-r--r--   0        0        0      738 2024-05-11 20:31:37.952883 pymkv2-2.0.1/pymkv/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-11 20:31:14.640288 pymkv2-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 pymkv2-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-12 01:21:08.052855 pymkv2-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2543 2024-05-12 01:21:08.052855 pymkv2-2.0.2/README.md
+-rw-r--r--   0        0        0      521 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/BCP47.py
+-rw-r--r--   0        0        0      550 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/ISO639_2.py
+-rw-r--r--   0        0        0     2904 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/MKVAttachment.py
+-rw-r--r--   0        0        0    39513 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/MKVFile.py
+-rw-r--r--   0        0        0    14332 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/MKVTrack.py
+-rw-r--r--   0        0        0     8592 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/Timestamp.py
+-rw-r--r--   0        0        0     1685 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/TypeTrack.py
+-rw-r--r--   0        0        0     3653 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/Verifications.py
+-rw-r--r--   0        0        0      560 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 pymkv2-2.0.2/PKG-INFO
```

### Comparing `pymkv2-2.0.1/LICENSE.txt` & `pymkv2-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.1/README.md` & `pymkv2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.1/pymkv/BCP47.py` & `pymkv2-2.0.2/pymkv/BCP47.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.1/pymkv/ISO639_2.py` & `pymkv2-2.0.2/pymkv/ISO639_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # sheldon woodward
 # 3/18/18
 
 """ISO639-2 Three Character Language Codes"""
 
-from typing import Optional
-
 from iso639 import languages
 
 
-def is_iso639_2(language) -> Optional[bool]:
+def is_iso639_2(language):
     """The `is_iso639_2` function checks if a given language code is a valid ISO 639-2 language code.
 
     Args:
         language: The language code to be checked.
 
     Returns:
         bool: True if the language code is a valid ISO 639-2 language code, False otherwise.
```

### Comparing `pymkv2-2.0.1/pymkv/MKVAttachment.py` & `pymkv2-2.0.2/pymkv/MKVAttachment.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,16 @@
 
 Now, the MKV can be muxed with both attachments.
 
 >>> mkv.add_attachment(attachment)
 >>> mkv.mux('path/to/output.mkv')
 """
 
-from __future__ import annotations
-
+from os.path import expanduser, isfile
 from mimetypes import guess_type
-from pathlib import Path
 
 
 class MKVAttachment:
     """A class that represents an MKV attachment for an :class:`~pymkv.MKVFile` object.
 
     Parameters
     ----------
@@ -53,44 +51,37 @@
     description : str
         The description that will be given to the attachment when muxed into a file.
     attach_once : bool
         Determines if the attachment should be added to all split files or only the first. Default is False,
         which will attach to all files.
     """
 
-    def __init__(
-            self,
-            file_path: str,
-            name: str | None = None,
-            description: str | None = None,
-            attach_once: bool | None = False,
-    ) -> None:
+    def __init__(self, file_path, name=None, description=None, attach_once=False):
         self.mime_type = None
         self._file_path = None
         self.file_path = file_path
         self.name = name
         self.description = description
         self.attach_once = attach_once
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return repr(self.__dict__)
 
     @property
-    def file_path(self) -> str:
+    def file_path(self):
         """str: The path to the attachment file.
 
         Raises
         ------
         FileNotFoundError
             Raised if `file_path` does not exist.
         """
         return self._file_path
 
     @file_path.setter
-    def file_path(self, file_path: str) -> None:
-        file_path = Path.expanduser(Path(file_path))
-        if not Path.is_file(file_path):
-            msg = f'"{file_path}" does not exist'
-            raise FileNotFoundError(msg)
+    def file_path(self, file_path):
+        file_path = expanduser(file_path)
+        if not isfile(file_path):
+            raise FileNotFoundError(f'"{file_path}" does not exist')
         self.mime_type = guess_type(file_path)[0]
         self.name = None
         self._file_path = file_path
```

### Comparing `pymkv2-2.0.1/pymkv/MKVFile.py` & `pymkv2-2.0.2/pymkv/MKVFile.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,27 +30,26 @@
 Combine two MKVs. This example takes two existing MKVs and combines their tracks into a single MKV file.
 
 >>> mkv1 = MKVFile('/path/to/file1.mkv')
 >>> mkv2 = MKVFile('/path/to/file2.mkv')
 >>> mkv1.add_file(mkv2)
 >>> mkv1.mux('/path/to/output.mkv')
 """
-from __future__ import annotations
 
 import json
 import logging
-import subprocess as sp
 from os.path import expanduser, isfile
+import subprocess as sp
 
 import bitmath
 
-from pymkv.ISO639_2 import is_iso639_2
-from pymkv.MKVAttachment import MKVAttachment
 from pymkv.MKVTrack import MKVTrack
+from pymkv.MKVAttachment import MKVAttachment
 from pymkv.Timestamp import Timestamp
+from pymkv.ISO639_2 import is_iso639_2
 from pymkv.Verifications import verify_matroska, verify_mkvmerge
 
 
 class MKVFile:
     """A class that represents an MKV file.
 
     The :class:`~pymkv.MKVFile` class can either import a pre-existing MKV file or create a new one. After an
@@ -80,93 +79,84 @@
 
     Raises
     ------
     FileNotFoundError
         Raised if the path to mkvmerge could not be verified.
     """
 
-    def __init__(
-            self,
-            file_path: str | None = None,
-            title: str | None = None,
-            mkvmerge_path: str | None = "mkvmerge",
-    ) -> None:
+    def __init__(self, file_path=None, title=None, mkvmerge_path='mkvmerge'):
         self.mkvmerge_path = mkvmerge_path
         self.title = title
         self._chapters_file = None
         self._chapter_language = None
         self._global_tags_file = None
         self._link_to_previous_file = None
         self._link_to_next_file = None
         self.tracks: list[MKVTrack] = []
         self.attachments = []
         self._number_file = 0
 
         if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
-            msg = (
-                "mkvmerge is not at the specified path, add it there or change"
-                                    "the mkvmerge_path property"
-            )
-            raise FileNotFoundError(msg)
+            raise FileNotFoundError('mkvmerge is not at the specified path, add it there or change'
+                                    'the mkvmerge_path property')
 
         if file_path is not None:
             # add file title
             file_path = expanduser(file_path)
-            info_json = json.loads(sp.check_output([self.mkvmerge_path, "-J", file_path]).decode())
-            if self.title is None and "title" in info_json["container"]["properties"]:
-                self.title = info_json["container"]["properties"]["title"]
+            info_json = json.loads(sp.check_output([self.mkvmerge_path, '-J', file_path]).decode())
+            if self.title is None and 'title' in info_json['container']['properties']:
+                self.title = info_json['container']['properties']['title']
 
             # add tracks with info
-            for track in info_json["tracks"]:
-                new_track = MKVTrack(file_path, track_id=track["id"], mkvmerge_path=self.mkvmerge_path)
-                if "track_name" in track["properties"]:
-                    new_track.track_name = track["properties"]["track_name"]
-                if "language" in track["properties"]:
-                    new_track.language = track["properties"]["language"]
-                if "language_ietf" in track["properties"]:
-                    new_track.language_ietf = track["properties"]["language_ietf"]
-                if "default_track" in track["properties"]:
-                    new_track.default_track = track["properties"]["default_track"]
-                if "forced_track" in track["properties"]:
-                    new_track.forced_track = track["properties"]["forced_track"]
-                if "flag_commentary" in track["properties"]:
-                    new_track.flag_commentary = track["properties"]["flag_commentary"]
-                if "flag_hearing_impaired" in track["properties"]:
-                    new_track.flag_hearing_impaired = track["properties"]["flag_hearing_impaired"]
-                if "flag_visual_impaired" in track["properties"]:
-                    new_track.flag_visual_impaired = track["properties"]["flag_visual_impaired"]
-                if "flag_original" in track["properties"]:
-                    new_track.flag_original = track["properties"]["flag_original"]
+            for track in info_json['tracks']:
+                new_track = MKVTrack(file_path, track_id=track['id'], mkvmerge_path=self.mkvmerge_path)
+                if 'track_name' in track['properties']:
+                    new_track.track_name = track['properties']['track_name']
+                if 'language' in track['properties']:
+                    new_track.language = track['properties']['language']
+                if 'language_ietf' in track['properties']:
+                    new_track.language_ietf = track['properties']['language_ietf']
+                if 'default_track' in track['properties']:
+                    new_track.default_track = track['properties']['default_track']
+                if 'forced_track' in track['properties']:
+                    new_track.forced_track = track['properties']['forced_track']
+                if 'flag_commentary' in track['properties']:
+                    new_track.flag_commentary = track['properties']['flag_commentary']
+                if 'flag_hearing_impaired' in track['properties']:
+                    new_track.flag_hearing_impaired = track['properties']['flag_hearing_impaired']
+                if 'flag_visual_impaired' in track['properties']:
+                    new_track.flag_visual_impaired = track['properties']['flag_visual_impaired']
+                if 'flag_original' in track['properties']:
+                    new_track.flag_original = track['properties']['flag_original']
                 self.add_track(new_track, new_file=False)
 
         # split options
         self._split_options = []
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return repr(self.__dict__)
 
     @property
     def chapter_language(self):
         """str: The language code of the chapters in the :class:`~pymkv.MKVFile` object.
 
         Raises
         ------
         ValueError
             Raised if not a valid ISO 639-2 language code.
         """
         return self._chapter_language
 
     @chapter_language.setter
-    def chapter_language(self, language: str) -> None:
+    def chapter_language(self, language):
         if language is not None and not is_iso639_2(language):
-            msg = "not an ISO639-2 language code"
-            raise ValueError(msg)
+            raise ValueError('not an ISO639-2 language code')
         self._chapter_language = language
 
-    def command(self, output_path: str, subprocess: bool = False) -> str | list:
+    def command(self, output_path, subprocess=False):
         """Generates an mkvmerge command based on the configured :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         output_path : str
             The path to be used as the output file in the mkvmerge command.
         subprocess : bool
@@ -174,97 +164,132 @@
 
         Returns
         -------
         str, list of str
             The full command to mux the :class:`~pymkv.MKVFile` as a string containing spaces. Will be returned as a
             list of strings with no spaces if `subprocess` is True.
         """
-        output_path = expanduser(output_path)
-        command = [
-            self.mkvmerge_path,
-            "-o",
-            output_path,
-            *(["--title", self.title] if self.title else []),
-        ]
 
+        output_path = expanduser(output_path)
+        command = [self.mkvmerge_path, '-o', output_path]
+        if self.title is not None:
+            command.extend(['--title', self.title])
         track_order = []
         for track in self.tracks:
-            track_order.append(f"{track.file_id}:{track.track_id}")
-
-            command.extend(["--track-name", f"{track.track_id!s}:{track.track_name}"] if track.track_name else [])
-            command.extend(["--language", f"{track.track_id!s}:{track.language_ietf}"] if track.language_ietf else
-                           ["--language", f"{track.track_id!s}:{track.language}"] if track.language else [])
-            command.extend(["--sync", f"{track.track_id!s}:{track.sync}"] if track.sync else [])
-            command.extend(["--tags", f"{track.track_id!s}:{track.tags}"] if track.tags else [])
-
-            command.extend(
-                [
-                    "--default-track",
-                    f"{track.track_id!s}:{'1' if track.default_track else '0'}",
-                    "--forced-track",
-                    f"{track.track_id!s}:{'1' if track.forced_track else '0'}",
-                    "--hearing-impaired-flag",
-                    f"{track.track_id!s}:{'1' if track.flag_hearing_impaired else '0'}",
-                    "--visual-impaired-flag",
-                    f"{track.track_id!s}:{'1' if track.flag_visual_impaired else '0'}",
-                    "--original-flag",
-                    f"{track.track_id!s}:{'1' if track.flag_original else '0'}",
-                    "--commentary-flag",
-                    f"{track.track_id!s}:{'1' if track.flag_commentary else '0'}",
-                ],
-            )
-            if track.track_type == "audio":
-                command.extend(["-D", "-a", str(track.track_id), "-S"])
-            elif track.track_type == "subtitles":
-                command.extend(["-D", "-A", "-s", str(track.track_id)])
-            elif track.track_type == "video":
-                command.extend(["-d", str(track.track_id), "-A", "-S"])
+            # for track_order
+            track_order.append(f'{track.file_id}:{track.track_id}')
+            # flags
+            if track.track_name is not None:
+                command.extend(['--track-name', f'{str(track.track_id)}:{track.track_name}'])
+            if track.language_ietf is not None:
+                command.extend(['--language', f'{str(track.track_id)}:{track.language_ietf}'])
+            elif track.language is not None:
+                command.extend(['--language', f'{str(track.track_id)}:{track.language}'])
+            if track.sync is not None:
+                command.extend(['--sync', f'{str(track.track_id)}:{track.sync}'])
+            if track.tags is not None:
+                command.extend(['--tags', f'{str(track.track_id)}:{track.tags}'])
+            if track.default_track:
+                command.extend(['--default-track', f'{str(track.track_id)}:1'])
+            else:
+                command.extend(['--default-track', f'{str(track.track_id)}:0'])
+            if track.forced_track:
+                command.extend(['--forced-track', f'{str(track.track_id)}:1'])
+            else:
+                command.extend(['--forced-track', f'{str(track.track_id)}:0'])
+            if track.flag_hearing_impaired:
+                command.extend(['--hearing-impaired-flag', f'{str(track.track_id)}:1'])
+            else:
+                command.extend(['--hearing-impaired-flag', f'{str(track.track_id)}:0'])
+            if track.flag_visual_impaired:
+                command.extend(['--visual-impaired-flag', f'{str(track.track_id)}:1'])
             else:
-                command.extend(["-D", "-A", "-S"])
+                command.extend(['--visual-impaired-flag', f'{str(track.track_id)}:0'])
+            if track.flag_original:
+                command.extend(['--original-flag', f'{str(track.track_id)}:1'])
+            else:
+                command.extend(['--original-flag', f'{str(track.track_id)}:0'])
+            if track.flag_commentary:
+                command.extend(['--commentary-flag', f'{str(track.track_id)}:1'])
+            else:
+                command.extend(['--commentary-flag', f'{str(track.track_id)}:0'])
 
-            command.extend(["--no-chapters"] if track.no_chapters else [])
-            command.extend(["--no-global-tags"] if track.no_global_tags else [])
-            command.extend(["--no-track-tags"] if track.no_track_tags else [])
-            command.extend(["--no-attachments"] if track.no_attachments else [])
+            # remove extra tracks
+            if track.track_type == 'audio':
+                command.append('-D')
+                command.extend(['-a', str(track.track_id), '-S'])
+            elif track.track_type == 'subtitles':
+                command.extend(('-D', '-A', '-s', str(track.track_id)))
+            elif track.track_type == 'video':
+                command.extend(['-d', str(track.track_id), '-A', '-S'])
+            else:
+                command.extend(('-D', '-A', '-S'))
+            # exclusions
+            if track.no_chapters:
+                command.append('--no-chapters')
+            if track.no_global_tags:
+                command.append('--no-global-tags')
+            if track.no_track_tags:
+                command.append('--no-track-tags')
+            if track.no_attachments:
+                command.append('--no-attachments')
 
+            # add path
             command.append(track.file_path)
 
+        # add attachments
         for attachment in self.attachments:
-            command.extend(["--attachment-name", attachment.name] if attachment.name else [])
-            command.extend(["--attachment-description", attachment.description] if attachment.description else [])
-            command.extend(["--attachment-mime-type", attachment.mime_type] if attachment.mime_type else [])
-
-            command.extend(
-                ["--attach-file-once" if attachment.attach_once else "--attach-file", attachment.file_path],
-            )
-
-        command.extend(["--chapter-language", self._chapter_language] if self._chapter_language else [])
-        command.extend(["--chapters", self._chapters_file] if self._chapters_file else [])
-        command.extend(["--global-tags", self._global_tags_file] if self._global_tags_file else [])
-        command.extend(["--link-to-previous", f"={self._link_to_previous_file}"] if self._link_to_previous_file else [])
-        command.extend(["--link-to-next", f"={self._link_to_next_file}"] if self._link_to_next_file else [])
+            # info
+            if attachment.name is not None:
+                command.extend(['--attachment-name', attachment.name])
+            if attachment.description is not None:
+                command.extend(['--attachment-description', attachment.description])
+            if attachment.mime_type is not None:
+                command.extend(['--attachment-mime-type', attachment.mime_type])
+
+            # add path
+            if not attachment.attach_once:
+                command.extend(['--attach-file', attachment.file_path])
+            else:
+                command.extend(['--attach-file-once', attachment.file_path])
+
+        # chapters
+        if self._chapter_language is not None:
+            command.extend(['--chapter-language', self._chapter_language])
+        if self._chapters_file is not None:
+            command.extend(['--chapters', self._chapters_file])
+
+        # global tags
+        if self._global_tags_file is not None:
+            command.extend(['--global-tags', self._global_tags_file])
+
+        # linking
+        if self._link_to_previous_file is not None:
+            command.extend(['--link-to-previous', f'={self._link_to_previous_file}'])
+        if self._link_to_next_file is not None:
+            command.extend(['--link-to-next', f'={self._link_to_next_file}'])
+
+        # tracks order
+        if track_order:
+            command.extend(['--track-order', ','.join(track_order)])
 
-        command.extend(["--track-order", ",".join(track_order)] if track_order else [])
+        # split options
         command.extend(self._split_options)
 
         return command if subprocess else " ".join(command)
 
-    def mux(self, output_path: str, silent: bool = False) -> int:
+    def mux(self, output_path, silent=False):
         """Mixes the specified :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         output_path : str
             The path to be used as the output file in the mkvmerge command.
         silent : bool, optional
             By default the mkvmerge output will be shown unless silent is True.
-        Returns
-        -------
-        int of Any
-            return code
 
         Raises
         ------
         ValueError
             Raised if the external mkvmerge command fails with a non-zero exit status.
             This includes scenarios such as invalid command arguments, errors in
             processing the :class:`~pymkv.MKVFile`, or issues with output file writing. The error
@@ -286,15 +311,15 @@
                 error_message += f"\nError Output:\n{error_details}"
                 logging.error(error_details)
             logging.error("Non-zero exit status when running %s (%s)", args, proc.returncode)
             raise ValueError(error_message)
 
         return proc.returncode
 
-    def add_file(self, file: MKVFile) -> None:
+    def add_file(self, file):
         """Add an MKV file into the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         file : str, :class:`~pymkv.MKVFile`
             The file to be combined with the :class:`~pymkv.MKVFile` object.
 
@@ -311,19 +336,18 @@
             self.tracks = self.tracks + new_tracks
         elif isinstance(file, MKVFile):
             self._number_file += 1
             for track in file.tracks:
                 track.file_id = self._number_file
             self.tracks = self.tracks + file.tracks
         else:
-            msg = "track is not str or MKVFile"
-            raise TypeError(msg)
+            raise TypeError('track is not str or MKVFile')
         self.order_tracks_by_file_id()
 
-    def add_track(self, track: str | MKVTrack, new_file: bool = True) -> None:
+    def add_track(self, track, new_file: bool = True):
         """Add a track to the :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         track : str, :class:`~pymkv.MKVTrack`
             The track to be added to the :class:`~pymkv.MKVFile` object.
         new_file : bool, optional
@@ -337,25 +361,24 @@
         """
         if isinstance(track, str):
             new_track = MKVTrack(track, mkvmerge_path=self.mkvmerge_path)
             self._extracted_from_add_track(new_track, new_file)
         elif isinstance(track, MKVTrack):
             self._extracted_from_add_track(track, new_file)
         else:
-            msg = "track is not str or MKVTrack"
-            raise TypeError(msg)
+            raise TypeError('track is not str or MKVTrack')
         self.order_tracks_by_file_id()
 
-    def _extracted_from_add_track(self, track: MKVTrack, new_file: bool = False) -> None:
+    def _extracted_from_add_track(self, track: MKVTrack, new_file: bool = False):
         if new_file:
             self._number_file += 1
         track.file_id = self._number_file
         self.tracks.append(track)
 
-    def add_attachment(self, attachment: str | MKVAttachment) -> None:
+    def add_attachment(self, attachment):
         """Add an attachment to the :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         attachment : str, :class:`~pymkv.MKVAttachment`
             The attachment to be added to the :class:`~pymkv.MKVFile` object.
 
@@ -365,18 +388,17 @@
             Raised if if `attachment` is not a string-like path to an attachment file or an :class:`~pymkv.MKVAttachment`.
         """
         if isinstance(attachment, str):
             self.attachments.append(MKVAttachment(attachment))
         elif isinstance(attachment, MKVAttachment):
             self.attachments.append(attachment)
         else:
-            msg = "Attachment is not str of MKVAttachment"
-            raise TypeError(msg)
+            raise TypeError('attachment is not str of MKVAttachment')
 
-    def get_track(self, track_num: int | None = None) -> MKVTrack:
+    def get_track(self, track_num=None):
         """Get a :class:`~pymkv.MKVTrack` from the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int, optional
             Index of track to retrieve. Will return list of :class:`~pymkv.MKVTrack` objects if argument is not
             provided.
@@ -385,15 +407,15 @@
         -------
         :class:`~pymkv.MKVTrack`, list of :class:`~pymkv.MKVTrack`
             A list of all :class:`~pymkv.MKVTrack` objects in an :class:`~pymkv.MKVFile`. Returns a specific
             :class:`~pymkv.MKVTrack` if `track_num` is specified.
         """
         return self.tracks if track_num is None else self.tracks[track_num]
 
-    def move_track_front(self, track_num: int) -> None:
+    def move_track_front(self, track_num):
         """Set a track as the first in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move to the front.
 
@@ -402,18 +424,17 @@
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
         if 0 <= track_num < len(self.tracks):
             self.tracks.insert(0, self.tracks.pop(track_num))
             self.order_tracks_by_file_id()
         else:
-            msg = "track index out of range"
-            raise IndexError(msg)
+            raise IndexError('track index out of range')
 
-    def move_track_end(self, track_num: int) -> None:
+    def move_track_end(self, track_num):
         """Set as track as the last in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move to the back.
 
@@ -422,79 +443,76 @@
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
         if 0 <= track_num < len(self.tracks):
             self.tracks.append(self.tracks.pop(track_num))
             self.order_tracks_by_file_id()
         else:
-            msg = "track index out of range"
-            raise IndexError(msg)
+            raise IndexError('track index out of range')
 
-    def move_track_forward(self, track_num: int) -> None:
+    def move_track_forward(self, track_num):
         """Move a track forward in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move forward.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if not 0 <= track_num < len(self.tracks) - 1:
-            msg = "Track index out of range"
-            raise IndexError(msg)
-        self.tracks[track_num], self.tracks[track_num + 1] = self.tracks[track_num + 1], self.tracks[track_num]
-        self.order_tracks_by_file_id()
+        if 0 <= track_num < len(self.tracks) - 1:
+            self.tracks[track_num], self.tracks[track_num + 1] = self.tracks[track_num + 1], self.tracks[track_num]
+            self.order_tracks_by_file_id()
+        else:
+            raise IndexError('track index out of range')
 
-    def move_track_backward(self, track_num: int) -> None:
+    def move_track_backward(self, track_num):
         """Move a track backward in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move backward.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if not 0 < track_num < len(self.tracks):
-            msg = "Track index out of range"
-            raise IndexError(msg)
-        self.tracks[track_num], self.tracks[track_num - 1] = self.tracks[track_num - 1], self.tracks[track_num]
-        self.order_tracks_by_file_id()
+        if 0 < track_num < len(self.tracks):
+            self.tracks[track_num], self.tracks[track_num - 1] = self.tracks[track_num - 1], self.tracks[track_num]
+            self.order_tracks_by_file_id()
+        else:
+            raise IndexError('track index out of range')
 
-    def swap_tracks(self, track_num_1: int, track_num_2: int) -> None:
+    def swap_tracks(self, track_num_1, track_num_2):
         """Swap the position of two tracks in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num_1 : int
             The track number of one track to swap.
         track_num_2 : int
             The track number of the other track to swap
 
         Raises
         ------
         IndexError
             Raised if `track_num_1` or `track_num_2` are out of range of the track list.
         """
-        if not 0 <= track_num_1 < len(self.tracks) or not 0 <= track_num_2 < len(
-            self.tracks,
-        ):
-            msg = "Track index out of range"
-            raise IndexError(msg)
-        self.tracks[track_num_1], self.tracks[track_num_2] = self.tracks[track_num_2], self.tracks[track_num_1]
-        self.order_tracks_by_file_id()
+        if 0 <= track_num_1 < len(self.tracks) and 0 <= track_num_2 < len(self.tracks):
+            self.tracks[track_num_1], self.tracks[track_num_2] = self.tracks[track_num_2], self.tracks[track_num_1]
+            self.order_tracks_by_file_id()
+        else:
+            raise IndexError('track index out of range')
 
-    def replace_track(self, track_num: int, track: MKVTrack) -> None:
+    def replace_track(self, track_num, track):
         """Replace a track with another track in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to replace.
         track : :class:`~pymkv.MKVTrack`
@@ -505,18 +523,17 @@
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
         if 0 <= track_num < len(self.tracks):
             self.tracks[track_num] = track
             self.order_tracks_by_file_id()
         else:
-            msg = "track index out of range"
-            raise IndexError(msg)
+            raise IndexError('track index out of range')
 
-    def remove_track(self, track_num: int) -> None:
+    def remove_track(self, track_num):
         """Remove a track from the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to remove.
 
@@ -525,22 +542,21 @@
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
         if 0 <= track_num < len(self.tracks):
             del self.tracks[track_num]
             self.order_tracks_by_file_id()
         else:
-            msg = "track index out of range"
-            raise IndexError(msg)
+            raise IndexError('track index out of range')
 
-    def split_none(self) -> None:
+    def split_none(self):
         """Remove all splitting options."""
         self._split_options = []
 
-    def split_size(self, size: bitmath.Bitmath | int, link: bool | None = False) -> None:
+    def split_size(self, size, link=False):
         """Split the output file into parts by size.
 
         Parameters
         ----------
         size : :obj:`bitmath`, int
             The size of each split file. Takes either a :obj:`bitmath` size object or an integer representing the
             number of bytes.
@@ -548,39 +564,38 @@
             Determines if the split files should be linked together after splitting.
 
         Raises
         ------
         TypeError
             Raised if if `size` is not a bitmath object or an integer.
         """
-        if getattr(size, "__module__", None) == bitmath.__name__:
+        if getattr(size, '__module__', None) == bitmath.__name__:
             size = size.bytes
         elif not isinstance(size, int):
-            msg = "size is not a bitmath object or integer"
-            raise TypeError(msg)
-        self._split_options = ["--split", f"size:{size}"]
+            raise TypeError('size is not a bitmath object or integer')
+        self._split_options = ['--split', f'size:{size}']
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_duration(self, duration: str | int, link: bool | None = False) -> None:
+    def split_duration(self, duration, link=False):
         """Split the output file into parts by duration.
 
         Parameters
         ----------
         duration : str, int
             The duration of each split file. Takes either a str formatted to HH:MM:SS.nnnnnnnnn or an integer
             representing the number of seconds. The duration string requires formatting of at least M:S.
         link : bool, optional
             Determines if the split files should be linked together after splitting.
         """
-        self._split_options = ["--split", f"duration:{Timestamp(duration)!s}"]
+        self._split_options = ['--split', f'duration:{str(Timestamp(duration))}']
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_timestamps(self, *timestamps: str | int | list | tuple, link: bool | None = False) -> None:
+    def split_timestamps(self, *timestamps, link=False):
         """Split the output file into parts by timestamps.
 
         Parameters
         ----------
         *timestamps : str, int, list, tuple
             The timestamps to split the file by. Can be passed as any combination of strs and ints, inside or outside
             an :obj:`Iterable` object. Any lists will be flattened. Timestamps must be ints, representing seconds,
@@ -592,33 +607,30 @@
         ------
         ValueError
             Raised if invalid or improperly formatted timestamps are passed in for `*timestamps`.
         """
         # check if in timestamps form
         ts_flat = MKVFile.flatten(timestamps)
         if len(ts_flat) == 0:
-            msg = f'"{timestamps}" are not properly formatted timestamps'
-            raise ValueError(msg)
+            raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
         if None in ts_flat:
-            msg = f'"{timestamps}" are not properly formatted timestamps'
-            raise ValueError(msg)
-        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:], strict=False):
+            raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
+        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:]):
             if Timestamp(ts_1) >= Timestamp(ts_2):
-                msg = f'"{timestamps}" are not properly formatted timestamps'
-                raise ValueError(msg)
+                raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
 
         # build ts_string from timestamps
-        ts_string = "timestamps:"
+        ts_string = 'timestamps:'
         for ts in ts_flat:
-            ts_string += f"{Timestamp(ts)!s},"
-        self._split_options = ["--split", ts_string[:-1]]
+            ts_string += f'{str(Timestamp(ts))},'
+        self._split_options = ['--split', ts_string[:-1]]
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_frames(self, *frames, link=False) -> None:
+    def split_frames(self, *frames, link=False):
         """Split the output file into parts by frames.
 
         Parameters
         ----------
         *frames : int, list, tuple
             The frames to split the file by. Can be passed as any combination of ints, inside or outside an
             :obj:`Iterable` object. Any lists will be flattened. Frames must be ints.
@@ -631,34 +643,31 @@
             Raised if non-int frames are passed in for `*frames` or within the `*frames` iterable.
         ValueError
             Raised if improperly formatted frames are passed in for `*frames`.
         """
         # check if in frames form
         f_flat = MKVFile.flatten(frames)
         if len(f_flat) == 0:
-            msg = f'"{frames}" are not properly formatted frames'
-            raise ValueError(msg)
+            raise ValueError(f'"{frames}" are not properly formatted frames')
         for f in f_flat:
             if not isinstance(f, int):
-                msg = f'frame "{f}" not an int'
-                raise TypeError(msg)
-        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:], strict=False):
+                raise TypeError(f'frame "{f}" not an int')
+        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:]):
             if f_1 >= f_2:
-                msg = f'"{frames}" are not properly formatted frames'
-                raise ValueError(msg)
+                raise ValueError(f'"{frames}" are not properly formatted frames')
 
         # build f_string from frames
-        f_string = "frames:"
+        f_string = 'frames:'
         for f in f_flat:
-            f_string += f"{f!s},"
-        self._split_options = ["--split", f_string[:-1]]
+            f_string += f'{str(f)},'
+        self._split_options = ['--split', f_string[:-1]]
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_timestamp_parts(self, timestamp_parts, link=False) -> None:
+    def split_timestamp_parts(self, timestamp_parts, link=False):
         """Split the output in parts by time parts.
 
         Parameters
         ----------
         timestamp_parts : list, tuple
             An Iterable of timestamp sets. Each timestamp set should be an Iterable of an even number of timestamps
             or any number of timestamp pairs. The very first and last timestamps are permitted to be None. Timestamp
@@ -671,46 +680,41 @@
         TypeError
             Raised if any of the timestamp sets are not a list or tuple.
         ValueError
             Raised if `timestamp_parts` contains improperly formatted parts.
         """
         ts_flat = MKVFile.flatten(timestamp_parts)
         if len(timestamp_parts) == 0:
-            msg = f'"{timestamp_parts}" are not properly formatted parts'
-            raise ValueError(msg)
+            raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
 
         if None in ts_flat[1:-1]:
-            msg = f'"{timestamp_parts}" are not properly formatted parts'
-            raise ValueError(msg)
+            raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
 
-        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:], strict=False):
+        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:]):
             if None not in (ts_1, ts_2) and Timestamp(ts_1) >= Timestamp(ts_2):
-                msg = f'"{timestamp_parts}" are not properly formatted parts'
-                raise ValueError(msg)
+                raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
 
-        ts_string = "parts:"
+        ts_string = 'parts:'
         for ts_set in timestamp_parts:
             ts_set = MKVFile.flatten(ts_set)
             if not isinstance(ts_set, (list, tuple)):
-                msg = "set is not of type list or tuple"
-                raise TypeError(msg)
+                raise TypeError('set is not of type list or tuple')
             if len(ts_set) < 2 or len(ts_set) % 2 != 0:
-                msg = f'"{ts_set}" is not a properly formatted set'
-                raise ValueError(msg)
+                raise ValueError(f'"{ts_set}" is not a properly formatted set')
             for index, ts in enumerate(ts_set):
                 if index % 2 == 0 and index > 0:
-                    ts_string += "+"
+                    ts_string += '+'
                 if ts is not None:
                     ts_string += str(Timestamp(ts))
-                ts_string += "-" if index % 2 == 0 else ","
-        self._split_options = ["--split", ts_string[:-1]]
+                ts_string += '-' if index % 2 == 0 else ','
+        self._split_options = ['--split', ts_string[:-1]]
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_parts_frames(self, frame_parts, link=False) -> None:
+    def split_parts_frames(self, frame_parts, link=False):
         """Split the output in parts by frames.
 
         Parameters
         ----------
         frame_parts : list, tuple
             An Iterable of frame sets. Each frame set should be an :obj:`Iterable` object of an even number of frames
             or any
@@ -724,46 +728,40 @@
         TypeError
             Raised if any of the frame sets are not a list or tuple.
         ValueError
             Raised if `frame_parts` contains improperly formatted parts.
         """
         f_flat = MKVFile.flatten(frame_parts)
         if len(frame_parts) == 0:
-            msg = f'"{frame_parts}" are not properly formatted parts'
-            raise ValueError(msg)
+            raise ValueError(f'"{frame_parts}" are not properly formatted parts')
         if None in f_flat[1:-1]:
-            msg = f'"{frame_parts}" are not properly formatted parts'
-            raise ValueError(msg)
-        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:], strict=False):
+            raise ValueError(f'"{frame_parts}" are not properly formatted parts')
+        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:]):
             if None not in (f_1, f_2) and f_1 >= f_2:
-                msg = f'"{frame_parts}" are not properly formatted parts'
-                raise ValueError(msg)
-        f_string = "parts:"
+                raise ValueError(f'"{frame_parts}" are not properly formatted parts')
+        f_string = 'parts:'
         for f_set in frame_parts:
             f_set = MKVFile.flatten(f_set)
             if not isinstance(f_set, (list, tuple)):
-                msg = "set is not of type list or tuple"
-                raise TypeError(msg)
+                raise TypeError('set is not of type list or tuple')
             if len(f_set) < 2 or len(f_set) % 2 != 0:
-                msg = f'"{f_set}" is not a properly formatted set'
-                raise ValueError(msg)
+                raise ValueError(f'"{f_set}" is not a properly formatted set')
             for index, f in enumerate(f_set):
                 if not isinstance(f, int) and f is not None:
-                    msg = f'frame "{f}" not an int'
-                    raise TypeError(msg)
+                    raise TypeError(f'frame "{f}" not an int')
                 if index % 2 == 0 and index > 0:
-                    f_string += "+"
+                    f_string += '+'
                 if f is not None:
                     f_string += str(f)
-                f_string += "-" if index % 2 == 0 else ","
-        self._split_options = ["--split", f_string[:-1]]
+                f_string += '-' if index % 2 == 0 else ','
+        self._split_options = ['--split', f_string[:-1]]
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def split_chapters(self, *chapters, link=False) -> None:
+    def split_chapters(self, *chapters, link=False):
         """Split the output file into parts by chapters.
 
         Parameters
         ----------
         *chapters : int, list, tuple
            The chapters to split the file by. Can be passed as any combination of ints, inside or outside an
            :obj:`Iterable` object. Any lists will be flattened. Chapters must be ints.
@@ -775,35 +773,32 @@
         TypeError
             Raised if any chapters in `*chapters` are not of type int.
         ValueError
             Raised if `*chapters` contains improperly formatted chapters.
        """
         c_flat = MKVFile.flatten(chapters)
         if not chapters:
-            self._split_options = ["--split", "chapters:all"]
+            self._split_options = ['--split', 'chapters:all']
             return
         for c in c_flat:
             if not isinstance(c, int):
-                msg = f'chapter "{c}" not an int'
-                raise TypeError(msg)
+                raise TypeError(f'chapter "{c}" not an int')
             if c < 1:
-                msg = f'"{chapters}" are not properly formatted chapters'
-                raise ValueError(msg)
-        for c_1, c_2 in zip(c_flat[:-1], c_flat[1:], strict=False):
+                raise ValueError(f'"{chapters}" are not properly formatted chapters')
+        for c_1, c_2 in zip(c_flat[:-1], c_flat[1:]):
             if c_1 >= c_2:
-                msg = f'"{chapters}" are not properly formatted chapters'
-                raise ValueError(msg)
-        c_string = "chapters:"
+                raise ValueError(f'"{chapters}" are not properly formatted chapters')
+        c_string = 'chapters:'
         for c in c_flat:
-            c_string += f"{c!s},"
-        self._split_options = ["--split", c_string[:-1]]
+            c_string += f'{str(c)},'
+        self._split_options = ['--split', c_string[:-1]]
         if link:
-            self._split_options += "--link"
+            self._split_options += '--link'
 
-    def link_to_previous(self, file_path) -> None:
+    def link_to_previous(self, file_path):
         """Link the output file as the predecessor of the `file_path` file.
 
         Parameters
         ----------
         file_path : str
             Path of the file to be linked to.
 
@@ -811,23 +806,21 @@
         ------
         TypeError
             Raised if `file_path` is not of type str.
         ValueError
             Raised if file at `file_path` cannot be verified as an MKV.
         """
         if not isinstance(str, file_path):
-            msg = f'"{file_path}" is not of type str'
-            raise TypeError(msg)
+            raise TypeError(f'"{file_path}" is not of type str')
         file_path = expanduser(file_path)
         if not verify_matroska(file_path):
-            msg = f'"{file_path}" is not a matroska file'
-            raise ValueError(msg)
+            raise ValueError(f'"{file_path}" is not a matroska file')
         self._link_to_previous_file = file_path
 
-    def link_to_next(self, file_path) -> None:
+    def link_to_next(self, file_path):
         """Link the output file as the successor of the `file_path` file.
 
         Parameters
         ----------
         file_path : str
             Path of the file to be linked to.
 
@@ -835,28 +828,26 @@
         ------
         TypeError
             Raised if `file_path` is not of type str.
         ValueError
             Raised if file at `file_path` cannot be verified as an MKV.
         """
         if not isinstance(file_path, str):
-            msg = f'"{file_path}" is not of type str'
-            raise TypeError(msg)
+            raise TypeError(f'"{file_path}" is not of type str')
         file_path = expanduser(file_path)
         if not verify_matroska(file_path):
-            msg = f'"{file_path}" is not a matroska file'
-            raise ValueError(msg)
+            raise ValueError(f'"{file_path}" is not a matroska file')
         self._link_to_next_file = file_path
 
-    def link_to_none(self) -> None:
+    def link_to_none(self):
         """Remove all linking to previous and next options."""
         self._link_to_previous_file = None
         self._link_to_next_file = None
 
-    def chapters(self, file_path, language=None) -> None:
+    def chapters(self, file_path, language=None):
         """Add a chapters file to the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         file_path : str
             The chapters file to be added to the :class:`~pymkv.MKVFile` object.
         language : str, optional
@@ -866,24 +857,22 @@
         ------
         FileNotFoundError
             Raised if the file at `file_path` does not exist.
         TypeError
             Raised if `file_path` is not of type str.
         """
         if not isinstance(file_path, str):
-            msg = f'"{file_path}" is not of type str'
-            raise TypeError(msg)
+            raise TypeError(f'"{file_path}" is not of type str')
         file_path = expanduser(file_path)
         if not isfile(file_path):
-            msg = f'"{file_path}" does not exist'
-            raise FileNotFoundError(msg)
+            raise FileNotFoundError(f'"{file_path}" does not exist')
         self._chapters_file = file_path
         self.chapter_language = language
 
-    def global_tags(self, file_path) -> None:
+    def global_tags(self, file_path):
         """Add global tags to the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         file_path : str
             The tags file to be added to the :class:`~pymkv.MKVFile` object.
 
@@ -891,23 +880,21 @@
         ------
         FileNotFoundError
             Raised if the file at `file_path` does not exist.
         TypeError
             Raised if `file_path` is not of type str.
         """
         if not isinstance(file_path, str):
-            msg = f'"{file_path}" is not of type str'
-            raise TypeError(msg)
+            raise TypeError(f'"{file_path}" is not of type str')
         file_path = expanduser(file_path)
         if not isfile(file_path):
-            msg = f'"{file_path}" does not exist'
-            raise FileNotFoundError(msg)
+            raise FileNotFoundError(f'"{file_path}" does not exist')
         self._global_tags_file = file_path
 
-    def track_tags(self, *track_ids, exclusive: bool | None = False) -> None:
+    def track_tags(self, *track_ids, exclusive=False):
         """Include or exclude tags from specific tracks.
 
         Parameters
         ----------
         *track_ids : int, list, tuple
             Track ids to have tags included or excluded from.
         exclusive : bool, optional
@@ -921,48 +908,45 @@
         TypeError
             Raised if an ids from `*track_ids` are not of type int.
         ValueError
             Raised if `*track_ids` are improperly formatted.
         """
         ids_flat = MKVFile.flatten(track_ids)
         if not track_ids:
-            msg = f'"{track_ids}" are not properly formatted track ids'
-            raise ValueError(msg)
+            raise ValueError(f'"{track_ids}" are not properly formatted track ids')
         for tid in ids_flat:
             if not isinstance(tid, int):
-                msg = f'track id "{tid}" not an int'
-                raise TypeError(msg)
+                raise TypeError(f'track id "{tid}" not an int')
             if tid < 0 or tid >= len(self.tracks):
-                msg = "track id out of range"
-                raise IndexError(msg)
+                raise IndexError('track id out of range')
         for tid in ids_flat if exclusive else list(set(range(len(self.tracks))) - set(ids_flat)):
             self.tracks[tid].no_track_tags = True
 
-    def no_chapters(self) -> None:
+    def no_chapters(self):
         """Ignore the existing chapters of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_chapters = True
 
-    def no_global_tags(self) -> None:
+    def no_global_tags(self):
         """Ignore the existing global tags of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_global_tags = True
 
-    def no_track_tags(self) -> None:
+    def no_track_tags(self):
         """Ignore the existing track tags of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_track_tags = True
 
-    def no_attachments(self) -> None:
+    def no_attachments(self):
         """Ignore the existing attachments of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_attachments = True
 
     @staticmethod
-    def flatten(item: list | tuple) -> list:
+    def flatten(item):
         """Flatten a list or a tuple.
 
         Takes a list or a tuple that contains other lists or tuples and flattens into a non-nested list.
 
         Examples
         --------
         >>> tup = ((1, 2), (3, (4, 5)))
@@ -982,15 +966,15 @@
         if not isinstance(item, (list, tuple)):
             return [item]
         flat_list = []
         for item in item:
             flat_list.extend(MKVFile.flatten(item))
         return flat_list
 
-    def order_tracks_by_file_id(self) -> None:
+    def order_tracks_by_file_id(self):
         """
         Orders tracks based on their file ID. Tracks from the same file will have the same file ID.
 
         This method first generates a list of unique file paths from the existing tracks.
         Then, it assigns each track a file ID, which is the index of its file path in the unique list.
         As a result, tracks from the same file will have the same file ID.
         """
```

### Comparing `pymkv2-2.0.1/pymkv/MKVTrack.py` & `pymkv2-2.0.2/pymkv/MKVTrack.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,25 +33,23 @@
 >>> file.add_track(track2)
 >>> file.add_track(track3)
 >>> file.mux('path/to/output.mkv')
 """
 
 import json
 import os.path
-import subprocess as sp
 from os import devnull
 from os.path import expanduser, isfile
+import subprocess as sp
 from pathlib import Path
-from typing import Optional
-from __future__ import annotations
 
-from pymkv.BCP47 import is_bcp47
-from pymkv.ISO639_2 import is_iso639_2
 from pymkv.TypeTrack import get_track_extension
 from pymkv.Verifications import verify_supported
+from pymkv.ISO639_2 import is_iso639_2
+from pymkv.BCP47 import is_bcp47
 
 
 class MKVTrack:
     """A class that represents a track for an :class:`~pymkv.MKVFile` object.
 
     :class:`~pymkv.MKVTrack` objects are video, audio, or subtitles. Tracks can be standalone files or a single track
     within an MKV file, both can be handled by pymkv. An :class:`~pymkv.MKVTrack` object can be added to an
@@ -107,15 +105,15 @@
         If attachments exist in the track file, don't include them when this :class:`~pymkv.MKVTrack` object is a track
         in an :class:`~pymkv.MKVFile` mux operation. This option has no effect on standalone track files, only tracks
         that are already part of an MKV file.
     """
 
     def __init__(self, file_path, track_id=0, track_name=None, language=None, language_ietf=None, default_track=False,
                  forced_track=False, flag_commentary=False, flag_hearing_impaired=False, flag_visual_impaired=False,
-                 flag_original=False, mkvmerge_path="mkvmerge", mkvextract_path="mkvextract", sync=None) -> None:
+                 flag_original=False, mkvmerge_path='mkvmerge', mkvextract_path='mkvextract', sync=None):
         # track info
         self._track_codec = None
         self._track_type = None
 
         # base
         self.mkvmerge_path = mkvmerge_path
         self._file_path = None
@@ -147,15 +145,15 @@
         self.no_track_tags = False
         self.no_attachments = False
 
         # mkvextract
         self.mkvextract_path = mkvextract_path
         self.extension = get_track_extension(self)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return repr(self.__dict__)
 
     @property
     def file_path(self):
         """str: The path to the track or MKV file containing the desired track.
 
         Setting this property will verify the passed in file is supported by mkvmerge and set the track_id to 0. It
@@ -165,19 +163,18 @@
         ------
         ValueError
             Raised if `file_path` is not a supported file type.
         """
         return self._file_path
 
     @file_path.setter
-    def file_path(self, file_path) -> None:
+    def file_path(self, file_path):
         file_path = expanduser(file_path)
         if not verify_supported(file_path, mkvmerge_path=self.mkvmerge_path):
-            msg = '"{}" is not a supported file'
-            raise ValueError(msg)
+            raise ValueError('"{}" is not a supported file')
         self._file_path = file_path
         self.track_id = 0
 
     @property
     def file_id(self):
         """int: The ID of the file the track belongs to.
 
@@ -188,81 +185,78 @@
         ------
         IndexError
             Raised if the passed in index is out of range of the file's tracks.
         """
         return self._file_id
 
     @file_id.setter
-    def file_id(self, file_id: int) -> None:
+    def file_id(self, file_id: int):
         if isinstance(file_id, int):
             self._file_id = file_id
         else:
-            msg = "file_id must be an integer"
-            raise ValueError(msg)
+            raise ValueError('file_id must be an integer')
 
     @property
-    def track_id(self) -> int:
+    def track_id(self):
         """int: The ID of the track within the file.
 
         Setting *track_id* will check that the ID passed in exists in the file. It will then look at the new track
         and set the codec and track type. Should be left at 0 unless extracting a specific track from an MKV.
 
         Raises
         ------
         IndexError
             Raised if the passed in index is out of range of the file's tracks.
         """
         return self._track_id
 
     @track_id.setter
-    def track_id(self, track_id: int) -> None:
-        info_json = json.loads(sp.check_output([self.mkvmerge_path, "-J", self.file_path]).decode())
-        if not 0 <= track_id < len(info_json["tracks"]):
-            msg = "track index out of range"
-            raise IndexError(msg)
+    def track_id(self, track_id):
+        info_json = json.loads(sp.check_output([self.mkvmerge_path, '-J', self.file_path]).decode())
+        if not 0 <= track_id < len(info_json['tracks']):
+            raise IndexError('track index out of range')
         self._track_id = track_id
         try:
-            self._pts = info_json["tracks"][track_id]["start_pts"]
+            self._pts = info_json['tracks'][track_id]["start_pts"]
         except KeyError:
             self._pts = 0
-        self._track_codec = info_json["tracks"][track_id]["codec"]
-        self._track_type = info_json["tracks"][track_id]["type"]
+        self._track_codec = info_json['tracks'][track_id]['codec']
+        self._track_type = info_json['tracks'][track_id]['type']
 
     @property
-    def language(self) -> str:
+    def language(self):
         """str: The language of the track.
 
         Setting this property will verify that the passed in language is an ISO-639 language code and use it as the
         language for the track.
 
         Raises
         ------
         ValueError
             Raised if the passed in language is not an ISO 639-2 language code.
         """
         return self._language
 
     @language.setter
-    def language(self, language: str) -> None:
+    def language(self, language):
         """Sets the language of the MKVTrack.
 
         Args:
             language: The language to be set for the MKVTrack.
 
         Returns:
             None
 
         Raises:
             ValueError: If the provided language is not a valid ISO639-2 language code.
         """
         if language is None or is_iso639_2(language):
             self._language = language
         else:
-            msg = "not an ISO639-2 language code"
-            raise ValueError(msg)
+            raise ValueError('not an ISO639-2 language code')
 
     @property
     def pts(self):
         """Returns the value of the `pts` property.
         The Presentation Timestamp (PTS) in multimedia files indicates the exact time when a frame or audio sample
         should be presented to the user, ensuring accurate synchronization between audio and video streams.
 
@@ -279,15 +273,15 @@
         """int: track delay.
 
         Setting this property allows you to wiggle the track negatively/positively.
         """
         return self._sync
 
     @sync.setter
-    def sync(self, sync) -> None:
+    def sync(self, sync):
         """Sets the value of the `sync` property.
 
         Args:
             sync: The value to be set for the `sync` property.
 
         Returns:
             None
@@ -306,20 +300,19 @@
         ------
         ValueError
             Raised if the passed in language is not a BCP47 language code.
         """
         return self._language_ietf
 
     @language_ietf.setter
-    def language_ietf(self, language_ietf) -> None:
+    def language_ietf(self, language_ietf):
         if language_ietf is None or is_bcp47(language_ietf):
             self._language_ietf = language_ietf
         else:
-            msg = "not a BCP47 language code"
-            raise ValueError(msg)
+            raise ValueError('not a BCP47 language code')
 
     @property
     def tags(self):
         """str: The tags file to include with the track.
 
         Setting this property will check that the file path passed in exists and set it as the tags file.
 
@@ -329,35 +322,33 @@
             Raised if the passed in file does not exist or is not a file.
         TypeError
             Raises if the passed in file is not of type str.
         """
         return self._tags
 
     @tags.setter
-    def tags(self, file_path: str) -> None:
+    def tags(self, file_path):
         if not isinstance(file_path, str):
-            msg = f'"{file_path}" is not of type str'
-            raise TypeError(msg)
-        file_path = Path(file_path).expanduser()
-        if not file_path.is_file():
-            msg = f'"{file_path}" does not exist'
-            raise FileNotFoundError(msg)
-        self._tags = str(file_path)
+            raise TypeError(f'"{file_path}" is not of type str')
+        file_path = expanduser(file_path)
+        if not isfile(file_path):
+            raise FileNotFoundError(f'"{file_path}" does not exist')
+        self._tags = file_path
 
     @property
-    def track_codec(self) -> str:
+    def track_codec(self):
         """str: The codec of the track such as h264 or AAC."""
         return self._track_codec
 
     @property
-    def track_type(self) -> str:
+    def track_type(self):
         """str: The type of track such as video or audio."""
         return self._track_type
 
-    def extract(self, output_path: str | None = None, silent: bool = False) -> str:
+    def extract(self, output_path: str = None, silent: bool = False) -> str:
         """Extract the track as a file.
 
         Parameters
         ----------
         output_path : str
             The path to be used as the output file in the mkvextract command.
         silent : bool, optional
@@ -372,13 +363,14 @@
             extract_info_file += f"_{self.track_name}"
         if output_path is None:
             output_path = f"{self.file_path}{extract_info_file}"
         else:
             file = Path(self.file_path)
             output_path = os.path.join(output_path, f"{file.name}{extract_info_file}")
         output_path = expanduser(output_path)
-        command = [self.mkvextract_path, "tracks", f"{self.file_path}", f"{self.track_id}:{output_path}"]
+        command = [self.mkvextract_path, 'tracks', f"{self.file_path}", f"{self.track_id}:{output_path}"]
         if silent:
-            sp.run(command, stdout=open(devnull, "wb"), check=True)
+            sp.run(command, stdout=open(devnull, 'wb'), check=True)
         else:
+            print('Running with command:\n"' + " ".join(command) + '"')
             sp.run(command, check=True, capture_output=True)
         return output_path
```

### Comparing `pymkv2-2.0.1/pymkv/Timestamp.py` & `pymkv2-2.0.2/pymkv/Timestamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Timestamp Class"""
 
 from re import match
 
 
 class Timestamp:
-    def __init__(self, timestamp=None, hh=None, mm=None, ss=None, nn=None, form="MM:SS") -> None:
+    def __init__(self, timestamp=None, hh=None, mm=None, ss=None, nn=None, form='MM:SS'):
         """A class that represents a timestamp used in MKVFiles.
 
         The Timestamp class represents a timestamp used in mkvmerge. These are commonly used for splitting MKVFiles.
         Specific time values can overridden in the timestamp using 'hh', 'mm', 'ss', and 'nn'. Any override value
         that is greater than its maximum (ex. 61 minutes) will be set to 0.
 
         timestamp (str, int, Timestamp):
@@ -93,132 +93,128 @@
             return self.mm >= other.mm
         elif self.ss != other.ss:
             return self.ss >= other.ss
         elif self.nn != other.nn:
             return self.nn >= other.nn
         return True
 
-    def __str__(self) -> str:
+    def __str__(self):
         return self.ts
 
     def __getitem__(self, index):
         return (self.hh, self.mm, self.ss, self.ss)[index]
 
     @property
     def ts(self):
         """Generates the timestamp specified in the object."""
         # parse timestamp format
-        format_groups = match(r"^(([Hh]{1,2}):)?([Mm]{1,2}):([Ss]{1,2})(\.([Nn]{1,9}))?$", self.form).groups()
+        format_groups = match('^(([Hh]{1,2}):)?([Mm]{1,2}):([Ss]{1,2})(\.([Nn]{1,9}))?$', self.form).groups()
         timestamp_format = [format_groups[i] is not None for i in (1, 2, 3, 5)]
 
         # create timestamp string
-        timestamp_string = ""
+        timestamp_string = ''
         if timestamp_format[0] or self._hh:
-            timestamp_string += f"{self.hh:0=2d}:"
+            timestamp_string += '{0:0=2d}:'.format(self.hh)
         if timestamp_format[1] or self._mm:
-            timestamp_string += f"{self.mm:0=2d}:"
+            timestamp_string += '{0:0=2d}:'.format(self.mm)
         if timestamp_format[2] or self._ss:
-            timestamp_string += f"{self.ss:0=2d}"
+            timestamp_string += '{0:0=2d}'.format(self.ss)
         if timestamp_format[3] or self._nn:
-            timestamp_string += f"{self.nn / 1000000000:.9f}".rstrip("0")[1:] if self.nn else ".0"
+            timestamp_string += '{:.9f}'.format(self.nn / 1000000000).rstrip('0')[1:] if self.nn else '.0'
         return timestamp_string
 
     @ts.setter
-    def ts(self, timestamp) -> None:
+    def ts(self, timestamp):
         """Set a new timestamp.
 
         timestamp (str, int):
             A str of a timestamp acceptable to mkvmerge or an int representing seconds. This value will be
             the basis of the timestamp.
         """
         if not isinstance(timestamp, (int, str)):
-            msg = f'"{type(timestamp)}" is not str or int type'
-            raise TypeError(msg)
+            raise TypeError(f'"{type(timestamp)}" is not str or int type')
         self._hh = None
         self._mm = None
         self._ss = None
         self._nn = None
         self.extract(timestamp)
 
     @property
     def hh(self):
         return self._hh
 
     @hh.setter
-    def hh(self, value) -> None:
+    def hh(self, value):
         self._hh = value
 
     @property
     def mm(self):
         return self._mm
 
     @mm.setter
-    def mm(self, value) -> None:
+    def mm(self, value):
         self._mm = value if value < 60 else 0
 
     @property
     def ss(self):
         return self._ss
 
     @ss.setter
-    def ss(self, value) -> None:
+    def ss(self, value):
         self._ss = value if value < 60 else 0
 
     @property
     def nn(self):
         return self._nn
 
     @nn.setter
-    def nn(self, value) -> None:
+    def nn(self, value):
         self._nn = value if value < 1000000000 else 0
 
     @property
     def form(self):
         return self._form
 
     @form.setter
-    def form(self, form) -> None:
+    def form(self, form):
         self._form = form
 
     @staticmethod
-    def verify(timestamp) -> bool:
+    def verify(timestamp):
         """Verify a timestamp has the proper form to be used in mkvmerge.
 
         timestamp (str, int):
             The timestamp to be verified.
         """
         if not isinstance(timestamp, str):
-            msg = f'"{type(timestamp)}" is not str type'
-            raise TypeError(msg)
-        elif match(r"^[0-9]{1,2}(:[0-9]{1,2}){1,2}(\.[0-9]{1,9})?$", timestamp):
+            raise TypeError(f'"{type(timestamp)}" is not str type')
+        elif match('^[0-9]{1,2}(:[0-9]{1,2}){1,2}(\.[0-9]{1,9})?$', timestamp):
             return True
         return False
 
-    def extract(self, timestamp) -> None:
+    def extract(self, timestamp):
         """Extracts time info from a timestamp.
 
         timestamp (str, int):
             A str of a timestamp acceptable to mkvmerge or an int representing seconds. The timing info will be
             extracted from this parameter.
         """
         if not isinstance(timestamp, (str, int)):
-            msg = f'"{type(timestamp)}" is not str or int type'
-            raise TypeError(msg)
+            raise TypeError(f'"{type(timestamp)}" is not str or int type')
         elif isinstance(timestamp, str) and not Timestamp.verify(timestamp):
-            msg = f'"{timestamp}" is not a valid timestamp'
-            raise ValueError(msg)
+            raise ValueError(f'"{timestamp}" is not a valid timestamp')
         elif isinstance(timestamp, str):
             self.splitting_timestamp(timestamp)
         elif isinstance(timestamp, int):
             self._hh = int(timestamp / 3600)
             self._mm = int(timestamp % 3600 / 60)
             self._ss = int(timestamp % 3600 % 60)
             self._nn = 0
 
-    def splitting_timestamp(self, timestamp) -> None:
+    def splitting_timestamp(self, timestamp):
         """
         The `splitting_timestamp` function splits a timestamp into its individual components and assigns them to instance variables.
 
         Args:
         self: The instance of the class.
 
         Returns:
@@ -239,15 +235,15 @@
             ----------
             timestamp
 
             Returns
             -------
         '''
         """
-        timestamp_groups = match(r"^(([0-9]{1,2}):)?([0-9]{1,2}):([0-9]{1,2})(\.([0-9]{1,9}))?$", timestamp).groups()
+        timestamp_groups = match('^(([0-9]{1,2}):)?([0-9]{1,2}):([0-9]{1,2})(\.([0-9]{1,9}))?$', timestamp).groups()
 
         timestamp = [timestamp_groups[i] for i in (1, 2, 3, 4)]
         timestamp_clean = []
         for ts in timestamp:
             if ts is None:
                 timestamp_clean.append(0)
             else:
```

### Comparing `pymkv2-2.0.1/pymkv/TypeTrack.py` & `pymkv2-2.0.2/pymkv/TypeTrack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from __future__ import annotations
+from typing import Optional
 
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from pymkv import MKVTrack
+from pymkv import MKVTrack
 
 type_files = {
     "video": {
         "V_MPEG1": "mpg",
         "V_MPEG2": "mpg",
         "V_MPEG4/ISO/AVC": "264",
         "MPEG-4p10": "h264",
@@ -48,15 +45,15 @@
         "VOBSUB": "sub",
         "USF": "usf",
         "WEBVTT": "vtt",
     },
 }
 
 
-def get_track_extension(track: MKVTrack) -> str | None:
+def get_track_extension(track: MKVTrack) -> Optional[str]:
     """str: Extension of a track.
 
     Parameters
     ----------
     track : :class:`~pymkv.MKVTrack`
         The :class:`~pymkv.MKVTrack` from which the file extension by track type will be obtained.
 
@@ -65,8 +62,7 @@
     str
         Return the extension of a track. If the track is a video, audio or subtitle track, an extension is returned.
     """
     track_type = track.track_type
     track_codec = track.track_codec
     if track_type in type_files and track_codec in type_files[track_type]:
         return type_files[track_type][track_codec]
-    return None
```

### Comparing `pymkv2-2.0.1/pymkv/Verifications.py` & `pymkv2-2.0.2/pymkv/Verifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,100 @@
 # sheldon woodward
 # 3/24/18
 
 """Verification functions for mkvmerge and associated files."""
 
 import json
 import os
-import subprocess as sp
 from os.path import expanduser, isfile
 from re import match
+import subprocess as sp
 
 
-def verify_mkvmerge(mkvmerge_path="mkvmerge"):
+def verify_mkvmerge(mkvmerge_path='mkvmerge'):
     """Verify mkvmerge is working.
 
     mkvmerge_path (str):
         Alternate path to mkvmerge if it is not already in the $PATH variable.
     """
     try:
-        output = sp.check_output([mkvmerge_path, "-V"]).decode()
+        output = sp.check_output([mkvmerge_path, '-V']).decode()
     except (sp.CalledProcessError, FileNotFoundError):
         return False
-    return bool(match("mkvmerge.*", output))
+    return bool(match('mkvmerge.*', output))
 
 
-def verify_matroska(file_path, mkvmerge_path="mkvmerge"):
+def verify_matroska(file_path, mkvmerge_path='mkvmerge'):
     """Verify if a file is a Matroska file.
 
     file_path (str):
         Path of the file to be verified.
     mkvmerge_path (str):
         Alternate path to mkvmerge if it is not already in the $PATH variable.
     """
     if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
-        msg = (
-            "mkvmerge is not at the specified path, add it there or change the mkvmerge_path "
-                                "property"
-        )
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError('mkvmerge is not at the specified path, add it there or change the mkvmerge_path '
+                                'property')
 
     if isinstance(file_path, os.PathLike):
         file_path = str(file_path)
     elif not isinstance(file_path, str):
-        msg = f'"{file_path}" is not of type str'
-        raise TypeError(msg)
+        raise TypeError(f'"{file_path}" is not of type str')
     file_path = expanduser(file_path)
     if not isfile(file_path):
-        msg = f'"{file_path}" does not exist'
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError(f'"{file_path}" does not exist')
     try:
-        info_json = json.loads(sp.check_output([mkvmerge_path, "-J", expanduser(file_path)]).decode())
+        info_json = json.loads(sp.check_output([mkvmerge_path, '-J', expanduser(file_path)]).decode())
 
     except sp.CalledProcessError as e:
-        msg = f'"{file_path}" could not be opened'
-        raise ValueError(msg) from e
-    return info_json["container"]["type"] == "Matroska"
+        raise ValueError(f'"{file_path}" could not be opened') from e
+    return info_json['container']['type'] == 'Matroska'
 
 
-def verify_recognized(file_path, mkvmerge_path="mkvmerge"):
+def verify_recognized(file_path, mkvmerge_path='mkvmerge'):
     """Verify a file is recognized by mkvmerge.
 
     file_path (str):
         Path to the file to be verified.
     mkvmerge_path (str):
         Alternate path to mkvmerge if it is not already in the $PATH variable.
     """
     if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
-        msg = (
-            "mkvmerge is not at the specified path, add it there or change the mkvmerge_path "
-                                "property"
-        )
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError('mkvmerge is not at the specified path, add it there or change the mkvmerge_path '
+                                'property')
 
     if not isinstance(file_path, str):
-        msg = f'"{file_path}" is not of type str'
-        raise TypeError(msg)
+        raise TypeError(f'"{file_path}" is not of type str')
     file_path = expanduser(file_path)
     if not isfile(file_path):
-        msg = f'"{file_path}" does not exist'
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError(f'"{file_path}" does not exist')
     try:
-        info_json = json.loads(sp.check_output([mkvmerge_path, "-J", file_path]).decode())
+        info_json = json.loads(sp.check_output([mkvmerge_path, '-J', file_path]).decode())
 
     except sp.CalledProcessError as e:
-        msg = f'"{file_path}" could not be opened'
-        raise ValueError(msg) from e
-    return info_json["container"]["recognized"]
+        raise ValueError(f'"{file_path}" could not be opened') from e
+    return info_json['container']['recognized']
 
 
-def verify_supported(file_path, mkvmerge_path="mkvmerge"):
+def verify_supported(file_path, mkvmerge_path='mkvmerge'):
     """Verify a file is supported by mkvmerge.
 
     file_path (str):
         Path to the file to be verified.
     mkvmerge_path (str):
         Alternate path to mkvmerge if it is not already in the $PATH variable.
     """
     if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
-        msg = (
-            "mkvmerge is not at the specified path, add it there or change the mkvmerge_path "
-                                "property"
-        )
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError('mkvmerge is not at the specified path, add it there or change the mkvmerge_path '
+                                'property')
 
     if not isinstance(file_path, str):
-        msg = f'"{file_path}" is not of type str'
-        raise TypeError(msg)
+        raise TypeError(f'"{file_path}" is not of type str')
     file_path = expanduser(file_path)
     if not isfile(file_path):
-        msg = f'"{file_path}" does not exist'
-        raise FileNotFoundError(msg)
+        raise FileNotFoundError(f'"{file_path}" does not exist')
     try:
-        info_json = json.loads(sp.check_output([mkvmerge_path, "-J", file_path]).decode())
+        info_json = json.loads(sp.check_output([mkvmerge_path, '-J', file_path]).decode())
 
     except sp.CalledProcessError as e:
-        msg = '"{}" could not be opened'
-        raise ValueError(msg) from e
-    return info_json["container"]["supported"]
+        raise ValueError('"{}" could not be opened') from e
+    return info_json['container']['supported']
```

### Comparing `pymkv2-2.0.1/pyproject.toml` & `pymkv2-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymkv2"
-version = "2.0.1"
+version = "2.0.2"
 description = "A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge."
 authors = [
     "Sheldon Woodward <me@sheldonw.com>",
     "GitBib"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `pymkv2-2.0.1/PKG-INFO` & `pymkv2-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkv2
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge.
 License: MIT
 Keywords: wrapper
 Author: Sheldon Woodward
 Author-email: me@sheldonw.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

