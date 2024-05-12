# Comparing `tmp/tghtml-1.1.4.tar.gz` & `tmp/tghtml-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tghtml-1.1.4.tar", max compression
+gzip compressed data, was "tghtml-1.1.5.tar", max compression
```

## Comparing `tghtml-1.1.4.tar` & `tghtml-1.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-12-31 10:33:23.146381 tghtml-1.1.4/LICENSE
--rw-r--r--   0        0        0      424 2023-12-31 13:51:51.923667 tghtml-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       91 2023-12-31 13:51:56.130667 tghtml-1.1.4/tghtml/__init__.py
--rw-r--r--   0        0        0     5228 2023-12-31 13:44:52.977692 tghtml-1.1.4/tghtml/core.py
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 tghtml-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 21:01:53.124555 tghtml-1.1.5/LICENSE
+-rw-r--r--   0        0        0      424 2024-05-12 21:46:47.537436 tghtml-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-12 21:01:53.124555 tghtml-1.1.5/tghtml/__init__.py
+-rw-r--r--   0        0        0     5306 2024-05-12 21:46:29.272374 tghtml-1.1.5/tghtml/core.py
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 tghtml-1.1.5/PKG-INFO
```

### Comparing `tghtml-1.1.4/LICENSE` & `tghtml-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tghtml-1.1.4/tghtml/core.py` & `tghtml-1.1.5/tghtml/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from dataclasses import dataclass, field
 from readability import Document
 
 from bs4 import BeautifulSoup, Tag
 
 
 def get_tag_content(tag: Tag) -> str:
@@ -15,15 +17,15 @@
     "em",
     "code",
     "s",
     "strike",
     "del",
     "u",
     "pre",
-    "blockquote"
+    "blockquote",
 ]
 
 
 @dataclass
 class TgHTML:
     html: str
     blocklist: list | tuple = ()
@@ -43,18 +45,22 @@
         return self.parsed
 
     def __str__(self) -> str:
         return self.parsed
 
     @property
     def parsed(self):
-        print(self.soup)
         self._filter()
         self._clean()
-        return self.html.strip().replace("\n", "\n\n")
+
+        return (
+            re.sub("\n{2,}", "\n", self.html.strip().replace("\ufeff", "\n"))
+            .replace("JDAN_EXTRA_SPACE", "\n")
+            .replace("\n", "\n\n")
+        )
 
     def _filter(self):
         for p in self.soup.findAll("p"):
             if "Это статья о" in p.text or "Vide etiam paginam discretivam:" in p.text:
                 p.replace_with("")
 
             elif p.text.replace("\n", "") == "":
@@ -103,16 +109,15 @@
                     tag.replace_with("")
             except Exception:
                 pass
 
             for tag in self.soup.find_all("span"):
                 if (
                     getattr(tag, "attrs", {})
-                    or {}
-                    .get("style", "")
+                    or {}.get("style", "")
                     .strip()
                     .replace(" ", "")
                     .find("font-style:italic")
                     != -1
                 ):
                     tag.name = "i"
 
@@ -129,23 +134,22 @@
                 BeautifulSoup(
                     "<p><b>" + get_tag_content(tag) + "</b></p>", "html.parser"
                 )
             )
 
         for tag in self.soup.find_all(["cite"]):
             tag.replace_with(
-                BeautifulSoup(
-                    " <i>" + get_tag_content(tag) + "</i>", "html.parser"
-                )
+                BeautifulSoup(" <i>" + get_tag_content(tag) + "</i>", "html.parser")
             )
 
         for tag in self.soup.find_all("div", {"class": "ts-Цитата"}):
             child = tag.find("blockquote")
             new_tag = BeautifulSoup(
-                TgHTML(get_tag_content(child), allowed_tags=["b", "i"]).parsed, "html.parser"
+                TgHTML(get_tag_content(child), allowed_tags=["b", "i"]).parsed,
+                "html.parser",
             )
 
             tag.replace_with(new_tag)
 
         for tag in self.soup.find_all("blockquote"):
             tag.wrap(Tag(name="p"))
```

