# Comparing `tmp/mandown-1.7.0.tar.gz` & `tmp/mandown-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.7.0.tar", max compression
+gzip compressed data, was "mandown-1.8.0.tar", max compression
```

## Comparing `mandown-1.7.0.tar` & `mandown-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.7.0/LICENSE
--rw-r--r--   0        0        0     3932 2024-01-08 00:13:59.089190 mandown-1.7.0/README.md
--rw-r--r--   0        0        0      523 2024-01-08 00:13:53.844256 mandown-1.7.0/mandown/__init__.py
--rw-r--r--   0        0        0    11931 2024-01-08 00:12:51.143045 mandown-1.7.0/mandown/api.py
--rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.7.0/mandown/base.py
--rw-r--r--   0        0        0    17292 2023-06-22 01:19:59.487322 mandown-1.7.0/mandown/cli.py
--rw-r--r--   0        0        0     2576 2023-07-14 02:30:34.879860 mandown-1.7.0/mandown/comic.py
--rw-r--r--   0        0        0      700 2023-06-22 00:52:39.390941 mandown-1.7.0/mandown/convert_utils.py
--rw-r--r--   0        0        0     5549 2023-04-28 17:41:44.918635 mandown-1.7.0/mandown/io.py
--rw-r--r--   0        0        0     5102 2023-04-28 17:41:44.926635 mandown-1.7.0/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4109 2023-04-28 17:41:44.926635 mandown-1.7.0/mandown/processor/ops.py
--rw-r--r--   0        0        0     1603 2023-04-28 17:41:44.926635 mandown-1.7.0/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1502 2024-01-07 22:35:45.164287 mandown-1.7.0/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2017 2023-04-28 17:41:44.919635 mandown-1.7.0/mandown/sources/base_source.py
--rw-r--r--   0        0        0     3371 2024-01-07 22:29:55.113688 mandown-1.7.0/mandown/sources/source_blogtruyenmoi.py
--rw-r--r--   0        0        0     5108 2023-12-31 05:46:30.059505 mandown-1.7.0/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2569 2023-06-21 02:59:09.077067 mandown-1.7.0/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2697 2023-04-28 17:41:44.920635 mandown-1.7.0/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3744 2023-04-28 17:41:44.920635 mandown-1.7.0/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3056 2023-12-31 05:04:57.262844 mandown-1.7.0/mandown/sources/source_manhuaes.py
--rw-r--r--   0        0        0     3567 2023-07-14 02:43:47.054901 mandown-1.7.0/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     5222 2024-01-08 00:11:23.300149 mandown-1.7.0/mandown/sources/source_thecomicseries.py
--rw-r--r--   0        0        0     4128 2023-12-31 05:46:20.951620 mandown-1.7.0/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.7.0/mandown/ui/form.ui
--rw-r--r--   0        0        0     7214 2023-04-28 17:41:44.928635 mandown-1.7.0/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.7.0/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     7049 2023-04-28 17:41:44.928635 mandown-1.7.0/mandown/ui/ui.py
--rw-r--r--   0        0        0     1403 2024-01-08 00:14:04.746119 mandown-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3885 2024-05-12 17:51:49.558004 mandown-1.8.0/README.md
+-rw-r--r--   0        0        0      542 2024-05-12 17:53:03.014544 mandown-1.8.0/mandown/__init__.py
+-rw-r--r--   0        0        0    11901 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/api.py
+-rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.8.0/mandown/base.py
+-rw-r--r--   0        0        0    17068 2024-05-12 16:28:10.003897 mandown-1.8.0/mandown/cli.py
+-rw-r--r--   0        0        0     2562 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/comic.py
+-rw-r--r--   0        0        0      700 2023-06-22 00:52:39.390941 mandown-1.8.0/mandown/convert_utils.py
+-rw-r--r--   0        0        0     5543 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/io.py
+-rw-r--r--   0        0        0     5095 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4064 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1597 2024-03-08 17:11:50.448985 mandown-1.8.0/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1505 2024-05-12 17:51:49.558004 mandown-1.8.0/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2016 2024-03-08 17:11:50.448985 mandown-1.8.0/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     3301 2024-05-12 16:09:43.070512 mandown-1.8.0/mandown/sources/source_blogtruyenmoi.py
+-rw-r--r--   0        0        0     4476 2024-05-12 17:51:49.558004 mandown-1.8.0/mandown/sources/source_kuaikanmanhua.py
+-rw-r--r--   0        0        0     5045 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2535 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2641 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3658 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3044 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/sources/source_manhuaes.py
+-rw-r--r--   0        0        0     3567 2023-07-14 02:43:47.054901 mandown-1.8.0/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     5154 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/sources/source_thecomicseries.py
+-rw-r--r--   0        0        0     4059 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.8.0/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7060 2024-03-08 17:14:31.384962 mandown-1.8.0/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.8.0/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     6954 2024-03-08 17:14:31.383962 mandown-1.8.0/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1603 2024-05-12 17:52:55.373592 mandown-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.8.0/PKG-INFO
```

### Comparing `mandown-1.7.0/LICENSE` & `mandown-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.7.0/README.md` & `mandown-1.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # mandown
 
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/mandown)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Download from PyPI](https://img.shields.io/pypi/v/mandown)](https://pypi.org/project/mandown)
 [![Download from the AUR](https://img.shields.io/aur/version/mandown-git)](https://aur.archlinux.org/packages/mandown-git)
 [![Latest release](https://img.shields.io/github/v/release/potatoeggy/mandown?display_name=tag)](https://github.com/potatoeggy/mandown/releases/latest)
 [![License](https://img.shields.io/github/license/potatoeggy/mandown)](/LICENSE)
 
 Mandown is a comic downloader and a CBZ, EPUB, MOBI, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
@@ -90,21 +89,23 @@
 
 ## Supported sites
 
 To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
 
 - <https://blogtruyenmoi.com>
 - <https://comicfury.com>
+- https://\*.thecomicseries.com
 - <https://mangasee123.com>
 - <https://manganato.com>
 - <https://webtoons.com>
 - <https://mangadex.org>
 - <https://mangakakalot.com>
-- <https://manhuaes.com>
+- <https://manhuaaz.com>
 - <https://readcomiconline.li>
+- <https://www.kuaikanmanhua.com>
 
 ## Basic library usage
 
 See the [docs](/docs/) for more information and examples.
 
 To just download the images:
```

### Comparing `mandown-1.7.0/mandown/__init__.py` & `mandown-1.8.0/mandown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     convert_progress,
     download,
     download_progress,
     load,
     process,
     process_progress,
     query,
+    save_metadata,
 )
 from .base import BaseChapter, BaseMetadata
 from .comic import BaseComic
 from .io import MD_METADATA_FILE
 from .processor import (
     ProcessConfig,
     ProcessOps,
     ProcessOptionMismatchError,
     Processor,
 )
 from .processor.profiles import SupportedProfiles, all_profiles
 
-__version__ = (1, 7, 0)
+__version__ = (1, 8, 0)
 __version_str__ = ".".join(map(str, __version__))
```

### Comparing `mandown-1.7.0/mandown/api.py` & `mandown-1.8.0/mandown/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,17 +134,15 @@
                     ),
                     [comicon.Chapter(chap.title, chap.slug)],
                 )
                 for chap in comic.chapters
             ]
 
             yield len(comicon_comics)
-            existing_filenames = {
-                file.name for file in dest_folder.iterdir() if file.is_file()
-            }
+            existing_filenames = {file.name for file in dest_folder.iterdir() if file.is_file()}
             for comicomic in comicon_comics:
                 yield comicomic.metadata.title
 
                 # do not overwrite existing cache
                 if f"{comicomic.metadata.title}.{to.value}" in existing_filenames:
                     continue
                 for _ in convert_one(comicomic, comic_path, to, dest_folder):
```

### Comparing `mandown-1.7.0/mandown/base.py` & `mandown-1.8.0/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.7.0/mandown/cli.py` & `mandown-1.8.0/mandown/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,15 @@
     sources,
 )
 
 app = typer.Typer()
 
 
 def cli_init_metadata_interactive() -> None:
-    path: Path = (
-        typer.prompt("Folder path", default=Path.cwd(), type=Path)
-        .expanduser()
-        .resolve()
-    )
+    path: Path = typer.prompt("Folder path", default=Path.cwd(), type=Path).expanduser().resolve()
 
     try:
         comic = api.load(path)
     except FileNotFoundError:
         # expected if no metadata exists
         ...
     except IOError as err:
@@ -78,17 +74,15 @@
             default=", ".join(metadata.genres) or None,
         ).split(",")
     ]
     metadata.cover_art = typer.prompt(
         "Cover art URL (enter 'EXISTS' if cover.png/jpg already exists)",
         default=metadata.cover_art or None,
     ).strip()
-    metadata.description = typer.prompt(
-        "Description", default=metadata.description or None
-    ).strip()
+    metadata.description = typer.prompt("Description", default=metadata.description or None).strip()
     metadata.url = metadata.url
 
     typer.secho("Metadata collected, now adding chapters...", fg=typer.colors.GREEN)
 
     folders_in_cd = sorted(f for f in path.iterdir() if f.is_dir())
     delta = len(folders_in_cd)  # #folders - #chapters
     if chapters:
@@ -130,17 +124,15 @@
     if not res:
         raise typer.Abort()
 
     typer.secho(
         f"All done! Saving metadata to {path / MD_METADATA_FILE}...",
         fg=typer.colors.GREEN,
     )
-    api.init_parse_comic(
-        path, BaseComic(metadata, chapters), metadata.cover_art != "EXISTS"
-    )
+    api.init_parse_comic(path, BaseComic(metadata, chapters), metadata.cover_art != "EXISTS")
 
 
 def cli_query(url: str) -> BaseComic:
     typer.echo(f"Searching sources for {url}")
 
     try:
         comic = api.query(url)
@@ -169,17 +161,15 @@
         # handle kindlegen errors
         typer.secho(str(err), fg=typer.colors.RED)
         raise typer.Abort() from None
 
     len_second_conv = -1
 
     first_convert_message = (
-        f"Packing {target_format.value}(s)"
-        if is_single_conversion
-        else "Pre-converting comic"
+        f"Packing {target_format.value}(s)" if is_single_conversion else "Pre-converting comic"
     )
 
     try:
         with typer.progressbar(
             iterator,
             length=len_first_conv,
             label=first_convert_message,
@@ -213,32 +203,28 @@
     if not split_by_chapters:
         dest_file = dest_folder / f"{comic_path.stem}.{target_format.value}"
         typer.secho(f"Successfully converted to {dest_file}", fg=typer.colors.GREEN)
     else:
         typer.secho(f"Successfully converted to {dest_folder}", fg=typer.colors.GREEN)
 
 
-def cli_process(
-    comic_path: Path, options: list[ProcessOps], config: ProcessConfig
-) -> None:
+def cli_process(comic_path: Path, options: list[ProcessOps], config: ProcessConfig) -> None:
     if ProcessOps.NO_POSTPROCESSING in options:
         return
 
     try:
         comic = api.load(comic_path)
     except FileNotFoundError as err:
         typer.secho(
             f"Comic not found at {comic_path}, is md-metadata.json missing?",
             fg=typer.colors.RED,
         )
         raise typer.Exit(1) from err
 
-    typer.secho(
-        f"Applying processing options: {', '.join(options)}", fg=typer.colors.GREEN
-    )
+    typer.secho(f"Applying processing options: {', '.join(options)}", fg=typer.colors.GREEN)
     try:
         with typer.progressbar(
             api.process_progress(comic_path, options, config),
             length=len(comic.chapters),
             label="Processing",
         ) as progress:
             for _ in progress:
@@ -331,17 +317,15 @@
         raise typer.Exit(1) from err
     cli_process(folder_path, options, config)
 
 
 @app.command(no_args_is_help=True)
 def get(
     url: str,
-    dest: Path = typer.Argument(
-        Path.cwd(), help="The destination folder to download to."
-    ),
+    dest: Path = typer.Argument(Path.cwd(), help="The destination folder to download to."),
     convert_to: ConvertFormats = typer.Option(
         "none", "--convert", "-c", help="The format to download the comic as"
     ),
     start: Optional[int] = typer.Option(
         None,
         "--start",
         "-s",
@@ -452,17 +436,15 @@
     if processing_options:
         try:
             config = ProcessConfig(
                 target_size=target_size,
                 output_profile=size_profile,
             )
         except Exception as err:
-            typer.secho(
-                f"Could not apply processing options: {err}", fg=typer.colors.RED
-            )
+            typer.secho(f"Could not apply processing options: {err}", fg=typer.colors.RED)
             raise typer.Exit(1) from err
 
         cli_process(dest / comic.metadata.title, processing_options, config)
 
     # convert
     if convert_to != ConvertFormats.NONE:
         cli_convert(
@@ -473,17 +455,15 @@
             split_by_chapters,
         )
 
 
 @app.command(name="init-metadata")
 def init_metadata(
     path: Optional[Path] = typer.Argument(None, help="The folder to initialise"),
-    source_url: Optional[str] = typer.Argument(
-        None, help="The url to get metadata from"
-    ),
+    source_url: Optional[str] = typer.Argument(None, help="The url to get metadata from"),
     download_cover: bool = typer.Option(
         False,
         "--download-cover",
         "-d",
         help="If --source-url is passed: Download the cover image from the source.",
     ),
 ) -> None:
@@ -496,17 +476,15 @@
     """
 
     if path is None:
         # interactive session
         return cli_init_metadata_interactive()
 
     if (path / MD_METADATA_FILE).is_file():
-        return typer.echo(
-            "Metadata already found. Please remove it to create new metadata."
-        )
+        return typer.echo("Metadata already found. Please remove it to create new metadata.")
 
     try:
         if source_url is not None:
             donor = api.query(source_url)
             comic = api.init_parse_comic(path, donor, download_cover)
         else:
             comic = api.init_parse_comic(path)
@@ -552,18 +530,15 @@
         for source in sources.get_all_classes():
             typer.echo(f"{source.name}: {', '.join(source.domains)}")
         raise typer.Exit()
 
     if list_profiles:
         typer.echo("Available profiles:")
         typer.echo(
-            "\n".join(
-                f" - {profile.name}: {profile.id!r}"
-                for profile in all_profiles.values()
-            )
+            "\n".join(f" - {profile.name}: {profile.id!r}" for profile in all_profiles.values())
         )
         raise typer.Exit()
 
 
 def main() -> None:
     app()
```

### Comparing `mandown-1.7.0/mandown/comic.py` & `mandown-1.8.0/mandown/comic.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,15 @@
         current source.
 
         :param `chapter`: The chapter to fetch
         :return: A list of image URLs
         """
         return self.source.fetch_chapter_image_list(chapter)
 
-    def set_chapter_range(
-        self, *, start: int | None = None, end: int | None = None
-    ) -> None:
+    def set_chapter_range(self, *, start: int | None = None, end: int | None = None) -> None:
         """
         `start` and `end` are zero-indexed.
 
         :param `start`: The index of the first chapter to keep
         :param `end`: The index of the last chapter to keep (exclusive)
         """
         self.chapters = self.chapters[start:end]
```

### Comparing `mandown-1.7.0/mandown/convert_utils.py` & `mandown-1.8.0/mandown/convert_utils.py`

 * *Files identical despite different names*

### Comparing `mandown-1.7.0/mandown/io.py` & `mandown-1.8.0/mandown/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 from .comic import BaseComic
 
 NUM_LEFT_PAD_DIGITS = 5
 FILE_PADDING = f"0{NUM_LEFT_PAD_DIGITS}"
 MD_METADATA_FILE = "md-metadata.json"
 
 
-def async_download_image(
-    data: tuple[str, Path | str, str | None, dict[str, str] | None]
-) -> None:
+def async_download_image(data: tuple[str, Path | str, str | None, dict[str, str] | None]) -> None:
     """
     Download an image from a URL to a destination folder, fixing the file extension if necessary.
 
     :param `data`: A tuple of the url, destination folder, filename, and headers.
     """
     url, dest_folder, filename, headers = data
     dest_folder = Path(dest_folder)
```

### Comparing `mandown-1.7.0/mandown/processor/__init__.py` & `mandown-1.8.0/mandown/processor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,21 +46,17 @@
 
     :param `image_path`: The path to the image to process
     :raises `ImportError`: If Pillow is not installed
     :raises `ProcessOptionMismatchError`: If an option is not valid for
     a given operation or there are missing options
     """
 
-    def __init__(
-        self, image_path: Path | str, config: ProcessConfig | None = None
-    ) -> None:
+    def __init__(self, image_path: Path | str, config: ProcessConfig | None = None) -> None:
         if not HAS_PILLOW:
-            raise ImportError(
-                "Pillow was not found and is needed for processing. Is it installed?"
-            )
+            raise ImportError("Pillow was not found and is needed for processing. Is it installed?")
 
         super().__init__(config)
         self.image_path = Path(image_path)
         self._image = Image.open(self.image_path)
         self.is_modified = False
 
         # WARN: dangerous if there are multiple types of operations
@@ -88,17 +84,15 @@
         self.image.save(filename)
 
         for image in self.new_images:
             # increment by one "a" each time
             filename = filename.with_stem(filename.stem + "a")
             image.save(filename)
 
-    def process(
-        self, operations: list[ProcessOps], filename: Path | str | None = None
-    ) -> None:
+    def process(self, operations: list[ProcessOps], filename: Path | str | None = None) -> None:
         """
         Perform the operations in `operations` on the image in sequence
         and save it to disk. If `filename` is not None, it will be saved
         with that filename instead. If "none" is in `operations`, no
         post-processing will be done.
 
         :param operations: A list of operations to perform on the image
@@ -109,31 +103,30 @@
         given operation or there are missing options
         """
         if ProcessOps.NO_POSTPROCESSING in operations:
             return
 
         # TODO: move all the checks together
         # there are some in ProcessConfig rn
-        resize_op_valid = bool(
-            self.config.output_profile or self.config.target_size
-        ) ^ bool(ProcessOps.RESIZE in operations)
+        resize_op_valid = bool(self.config.output_profile or self.config.target_size) ^ bool(
+            ProcessOps.RESIZE in operations
+        )
         if resize_op_valid:
             # if any of the following is true:
             # - target_size is set and resize is not
             # - profile is set and resize is not
             # - resize is set and neither target_size nor profile is set
-            raise ProcessOptionMismatchError(
-                "resize must be used with target_size or profile"
-            )
+            # testing if only one of them is set is done in the resize op itself
+            raise ProcessOptionMismatchError("resize must be used with target_size or profile")
 
         for func in operations:
             try:
-                images: tuple[Image.Image, ...] | Image.Image | None = getattr(
-                    self, func
-                )(self.image)
+                images: tuple[Image.Image, ...] | Image.Image | None = getattr(self, func)(
+                    self.image
+                )
 
                 if images is None:
                     continue
 
                 if isinstance(images, Image.Image):
                     images = (images,)
```

### Comparing `mandown-1.7.0/mandown/processor/ops.py` & `mandown-1.8.0/mandown/processor/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 try:
     from PIL import Image, ImageChops
 
     if not hasattr(Image, "Resampling"):  # Pillow<9.0
         Image.Resampling = Image
 except ImportError:
-
     if not TYPE_CHECKING:
 
         class Image:
             class Image:
                 pass
 
         class ImageChops:
@@ -43,17 +42,15 @@
     """
     The output size profile to use for the image. Only
     used if `resize` is enabled. Mutually exclusive with `target_size`.
     """
 
     def __post_init__(self) -> None:
         if self.target_size is not None and self.output_profile is not None:
-            raise ValueError(
-                "Only one of `target_size` or `output_profile` can be specified."
-            )
+            raise ValueError("Only one of `target_size` or `output_profile` can be specified.")
 
         if self.output_profile is not None:
             if self.output_profile not in all_profiles:
                 raise KeyError(
                     f"Invalid output profile: {self.output_profile}. See mandown."
                     "all_profiles or mandown --list-profiles for a list of valid profiles."
                 )
@@ -83,17 +80,15 @@
         Rotate the image 90 degrees if it is a double page so it fits on the screen.
         """
         width, height = image.size
         if width > height:
             return image.rotate(90, expand=1)
         return None
 
-    def split_double_pages(
-        self, image: Image.Image
-    ) -> tuple[Image.Image, Image.Image] | None:
+    def split_double_pages(self, image: Image.Image) -> tuple[Image.Image, Image.Image] | None:
         """
         Split the image into two separate images if it is a double page.
         """
         width, height = image.size
         if not width > height:
             return None
```

### Comparing `mandown-1.7.0/mandown/processor/profiles.py` & `mandown-1.8.0/mandown/processor/profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,10 +52,8 @@
     "librah2o": ("Kobo Libra H2O", (1264, 1680)),
     "nia": ("Kobo Nia", (758, 1024)),
     "clara2e": ("Kobo Clara 2E", (1072, 1448)),
     "libra2": ("Kobo Libra 2", (1264, 1680)),
     "sage": ("Kobo Sage", (1440, 1920)),
 }
 
-all_profiles = {
-    id: OutputProfile(id, *profile) for id, profile in __all_profiles_data.items()
-}
+all_profiles = {id: OutputProfile(id, *profile) for id, profile in __all_profiles_data.items()}
```

### Comparing `mandown-1.7.0/mandown/sources/__init__.py` & `mandown-1.8.0/mandown/sources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 This module contains all the source modules.
 
 The source modules are dynamically imported and added to the __class_list
 variable. This variable is used by the get_class_for() function to return
 the correct source class for a given URL.
 """
 
-
 import sys
 import types
 
 from . import (
     source_blogtruyenmoi,
+    source_kuaikanmanhua,
     source_mangadex,
     source_mangakakalot,
     source_manganato,
     source_mangasee,
     source_manhuaes,
     source_readcomiconline,
     source_thecomicseries,
@@ -30,17 +30,15 @@
 
 def _get_all_source_modules() -> list[str]:
     """
     Return a list of all source modules.
     """
     out = []
     for _, val in globals().items():
-        if isinstance(val, types.ModuleType) and val.__name__.startswith(
-            "mandown.sources.source_"
-        ):
+        if isinstance(val, types.ModuleType) and val.__name__.startswith("mandown.sources.source_"):
             out.append(val.__name__)
     return out
 
 
 for i in _get_all_source_modules():
     __class_list.append(sys.modules[i].get_class())
```

### Comparing `mandown-1.7.0/mandown/sources/base_source.py` & `mandown-1.8.0/mandown/sources/base_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     domains = ["Source domains goes here"]
     headers: dict[str, str] = {}
 
     _metadata: BaseMetadata | None = None
     _chapters: list[BaseChapter] = []
 
     def __init__(self, url: str):
-
         self.url = url
 
     @property
     def metadata(self) -> BaseMetadata:
         """
         Return the metadata of the comic, fetching and caching it if necessary.
         """
```

### Comparing `mandown-1.7.0/mandown/sources/source_blogtruyenmoi.py` & `mandown-1.8.0/mandown/sources/source_blogtruyenmoi.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,18 @@
         self.url = f"https://blogtruyenmoi.com/{self.id}"
         self._scripts: str | None = None
 
     def fetch_metadata(self) -> BaseMetadata:
         soup = BeautifulSoup(self._get_scripts(), "lxml")
 
         title: str = (
-            soup.select_one("div#breadcrumbs > span:nth-child(2)")
-            .text.split(" > ")[-1]
-            .strip()
+            soup.select_one("div#breadcrumbs > span:nth-child(2)").text.split(" > ")[-1].strip()
         )
-        authors: list[str] = [
-            soup.select_one('div.description > p > a[href^="/tac-gia"]').text
-        ]
-        genres: list[str] = [
-            string.text.strip() for string in soup.select("span.category > a")
-        ]
+        authors: list[str] = [soup.select_one('div.description > p > a[href^="/tac-gia"]').text]
+        genres: list[str] = [string.text.strip() for string in soup.select("span.category > a")]
         cover_art: str = soup.select_one(".thumbnail > img")["src"]
 
         description_list: list[str] = []
         for child in soup.select_one("div.detail > div.content").children:
             if child.name and child.name.lower() == "br":
                 # br tags usually indicate the end of the description
                 break
```

### Comparing `mandown-1.7.0/mandown/sources/source_mangadex.py` & `mandown-1.8.0/mandown/sources/source_mangadex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Source file for mangadex.org
 """
 # pylint: disable=invalid-name
 
-
 import re
 import time
 
 import requests
 from bs4 import BeautifulSoup
 from slugify import slugify
 
@@ -23,17 +22,17 @@
         super().__init__(url)
         self._soup: BeautifulSoup | None = None
         self.lang_code = ""
 
         # https://api.mangadex.org/manga/de4b3c43-5243-4399-9fc3-68a3c0747138
         self.id = self.url.split("/")[4]
         if self.url.startswith("https://mangadex.org/chapter"):
-            r: dict = self._get(f"https://api.mangadex.org/chapter/{self.id}").json()[
-                "data"
-            ]["relationships"]
+            r: dict = self._get(f"https://api.mangadex.org/chapter/{self.id}").json()["data"][
+                "relationships"
+            ]
             self.id: str = next(filter(lambda i: i["type"] == "manga", r))["id"]  # type: ignore
 
     def fetch_metadata(self) -> BaseMetadata:
         # TODO: support non-English downloads
         r = self._get(
             f"https://api.mangadex.org/manga/{self.id}"
             "?includes[]=author&includes[]=cover_art&includes[]=artist"
@@ -90,17 +89,15 @@
             f"https://api.mangadex.org/manga/{self.id}/"
             f"feed?limit=500&translatedLanguage[]={self.lang_code}"
             "&order[volume]=asc&order[chapter]=asc"
         ).json()
 
         chapters: list[BaseChapter] = []
         for i, c in enumerate(r["data"]):
-            chapter_title: str = (
-                c["attributes"]["title"] or f"Chapter {c['attributes']['chapter']}"
-            )
+            chapter_title: str = c["attributes"]["title"] or f"Chapter {c['attributes']['chapter']}"
             chapter_slug: str = f"{i}-{slugify(chapter_title)}"
             chapters.append(
                 BaseChapter(
                     chapter_title,
                     f"https://mangadex.org/chapter/{c['id']}",
                     chapter_slug,
                 )
@@ -138,15 +135,13 @@
             elif r.status_code == 404:
                 raise RuntimeError(
                     "This chapter is not downloadable from MangaDex. If you "
                     "believe this to be an error, please open a GitHub issue."
                 )
             time.sleep(1)
         else:
-            raise RuntimeError(
-                "MangaDex is probably rate-limiting us, try again later?"
-            )
+            raise RuntimeError("MangaDex is probably rate-limiting us, try again later?")
         return r
 
 
 def get_class() -> type[BaseSource]:
     return MangaDexSource
```

### Comparing `mandown-1.7.0/mandown/sources/source_mangakakalot.py` & `mandown-1.8.0/mandown/sources/source_mangakakalot.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,15 @@
         description_html.find("p").replace_with("")  # remove p block
         description = description_html.get_text().strip()
 
         return BaseMetadata(title, authors, self.url, genres, description, cover_art)
 
     def fetch_chapter_list(self) -> list[BaseChapter]:
         soup = BeautifulSoup(self._get_scripts(), "lxml")
-        chapters = [
-            BaseChapter(c.next_element, c["href"])
-            for c in soup.select(".row > span > a")
-        ]
+        chapters = [BaseChapter(c.next_element, c["href"]) for c in soup.select(".row > span > a")]
         chapters.reverse()
         return chapters
 
     def fetch_chapter_image_list(self, chapter: BaseChapter) -> list[str]:
         soup = BeautifulSoup(requests.get(chapter.url).text, "lxml")
         images = []
         for i in soup.select(".container-chapter-reader > img"):
```

### Comparing `mandown-1.7.0/mandown/sources/source_manganato.py` & `mandown-1.8.0/mandown/sources/source_manganato.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,21 @@
                 authors.append(el.next_element)
             elif el["href"].startswith("https://manganato.com/genre"):
                 genres.append(el.next_element)
 
         cover_img = next(iter(soup.select("span.info-image > img.img-loading")))
         cover_art: str = cover_img["src"]
 
-        description = soup.select_one(
-            "#panel-story-info-description > h3"
-        ).nextSibling.text.strip()
+        description = soup.select_one("#panel-story-info-description > h3").nextSibling.text.strip()
 
         return BaseMetadata(title, authors, self.url, genres, description, cover_art)
 
     def fetch_chapter_list(self) -> list[BaseChapter]:
         soup = BeautifulSoup(self._get_scripts(), "lxml")
-        chapters = [
-            BaseChapter(c.next_element, c["href"])
-            for c in soup.select("a.chapter-name")
-        ]
+        chapters = [BaseChapter(c.next_element, c["href"]) for c in soup.select("a.chapter-name")]
         chapters.reverse()
         return chapters
 
     def fetch_chapter_image_list(self, chapter: BaseChapter) -> list[str]:
         soup = BeautifulSoup(requests.get(chapter.url).text, "lxml")
         images = []
         for i in soup.find_all("img"):
```

### Comparing `mandown-1.7.0/mandown/sources/source_mangasee.py` & `mandown-1.8.0/mandown/sources/source_mangasee.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 from ..base import BaseChapter, BaseMetadata
 from .base_source import BaseSource
 
 
 class MangaSeeSource(BaseSource):
     name = "MangaSee"
     domains = ["https://mangasee123.com"]
-    USER_AGENT = (
-        "Mozilla/5.0 (Windows NT 10.0; WOW64; rv:77.0) Gecko/20100101 Firefox/77.0"
-    )
+    USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; WOW64; rv:77.0) Gecko/20100101 Firefox/77.0"
 
     def __init__(self, url: str) -> None:
         super().__init__(url)
         self.id = self.url_to_id(url)
         self._scripts: str | None = None
 
     def fetch_metadata(self) -> BaseMetadata:
@@ -40,39 +38,33 @@
         authors: list[str] = [a.next_element for a in authors_html]
 
         genres: list[str] = metadata_json["genre"]
 
         description_html = soup.select_one("div.top-5.Content")
         description = str(description_html.next_element).strip()
 
-        cover_art = soup.select_one('div[style="padding-right:0px;"] img.bottom-5')[
-            "src"
-        ]
+        cover_art = soup.select_one('div[style="padding-right:0px;"] img.bottom-5')["src"]
 
         return BaseMetadata(title, authors, self.url, genres, description, cover_art)
 
     def fetch_chapter_list(self) -> list[BaseChapter]:
-        feed = feedparser.parse(
-            f"https://mangasee123.com/rss/{self.id}.xml", agent=self.USER_AGENT
-        )
+        feed = feedparser.parse(f"https://mangasee123.com/rss/{self.id}.xml", agent=self.USER_AGENT)
 
         chapters = []
         for c in feed["entries"]:
             chapter_title = str(c["title"]).lstrip(self.metadata.title).strip()
             chapters.append(BaseChapter(chapter_title, c["link"]))
 
         chapters.reverse()
         return chapters
 
     def fetch_chapter_image_list(self, chapter: BaseChapter) -> list[str]:
         soup = BeautifulSoup(requests.get(chapter.url).text, "lxml")
         full_js = str(
-            soup.find("script", type="application/ld+json")
-            .find_next("script")
-            .next_element
+            soup.find("script", type="application/ld+json").find_next("script").next_element
         )
 
         index_start = full_js.index("vm.CurChapter =") + len("vm.CurChapter =")
         index_end = full_js.index(";", index_start)
         chapter_details: dict = json.loads(full_js[index_start:index_end])
 
         index_start = full_js.index("vm.CurPathName =") + len("vm.CurPathName =")
```

### Comparing `mandown-1.7.0/mandown/sources/source_manhuaes.py` & `mandown-1.8.0/mandown/sources/source_manhuaes.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,15 @@
             requests.post(
                 "https://manhuaaz.com/wp-admin/admin-ajax.php",
                 data={"action": "manga_get_chapters", "manga": self.numerical_id},
             ).text,
             "lxml",
         )
         chapters = [
-            BaseChapter(c.text.strip(), c["href"])
-            for c in soup.select(".wp-manga-chapter a")
+            BaseChapter(c.text.strip(), c["href"]) for c in soup.select(".wp-manga-chapter a")
         ]
         chapters.reverse()
         return chapters
 
     def fetch_chapter_image_list(self, chapter: BaseChapter) -> list[str]:
         soup = BeautifulSoup(requests.get(chapter.url).text, "lxml")
         return [el["data-src"] for el in soup.select("img.wp-manga-chapter-img")]
```

### Comparing `mandown-1.7.0/mandown/sources/source_readcomiconline.py` & `mandown-1.8.0/mandown/sources/source_readcomiconline.py`

 * *Files identical despite different names*

### Comparing `mandown-1.7.0/mandown/sources/source_thecomicseries.py` & `mandown-1.8.0/mandown/sources/source_thecomicseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,19 @@
                     index = i - 1
                     break
 
         if index is None:
             num_pages = len(pages)
         else:
             soup3 = BeautifulSoup(
-                requests.get(
-                    f"https://comicfury.com{page_list_urls[index]['href']}"
-                ).text,
+                requests.get(f"https://comicfury.com{page_list_urls[index]['href']}").text,
                 "lxml",
             )
             # index is zero-indexed
-            num_pages = len(pages) * (index + 1) + len(
-                soup3.select(".archive-comics > a")
-            )
+            num_pages = len(pages) * (index + 1) + len(soup3.select(".archive-comics > a"))
 
         # their api only returns images after the first page
         # so we have to fetch it ourselves
         soup4 = BeautifulSoup(
             requests.get(f"https://comicfury.com{pages[0]['href']}").text,
             "lxml",
         )
```

### Comparing `mandown-1.7.0/mandown/sources/source_webtoons.py` & `mandown-1.8.0/mandown/sources/source_webtoons.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Source file for webtoons.com
 """
 # pylint: disable=invalid-name
 
-
 import re
 
 import requests
 from bs4 import BeautifulSoup
 
 from ..base import BaseChapter, BaseMetadata
 from .base_source import BaseSource
@@ -71,17 +70,15 @@
             genres,
             description,
             cover_art,
         )
 
     def fetch_chapter_list(self) -> list[BaseChapter]:
         soup = self._get_soup()
-        titles = [
-            str(e.next_element) for e in soup.select("p.sub_title > span.ellipsis")
-        ]
+        titles = [str(e.next_element) for e in soup.select("p.sub_title > span.ellipsis")]
 
         links: list[str] = [e["href"] for e in soup.select('a[class^="NPI=a:list"]')]
 
         chapters = [BaseChapter(t, u) for t, u in zip(titles, links)]
         chapters.reverse()
         return chapters
 
@@ -93,29 +90,25 @@
         return images
 
     def _get_soup(self) -> BeautifulSoup:
         if self._soup:
             return self._soup
 
         # mobile serves all chapters in one page
-        mobile_url = (
-            f"https://m.webtoons.com/{self._title_path}/list?title_no={self._title_no}"
-        )
+        mobile_url = f"https://m.webtoons.com/{self._title_path}/list?title_no={self._title_no}"
 
         self._soup = BeautifulSoup(
             requests.get(mobile_url, headers=self.headers).text,
             "lxml",
         )
         return self._soup
 
     def _get_desktop_soup(self) -> BeautifulSoup:
         desktop_url = f"https://www.webtoons.com/{self._title_path}/list?title_no={self._title_no}"
-        return BeautifulSoup(
-            requests.get(desktop_url, headers=self.headers).text, "lxml"
-        )
+        return BeautifulSoup(requests.get(desktop_url, headers=self.headers).text, "lxml")
 
     @staticmethod
     def check_url(url: str) -> bool:
         return bool(
             re.match(r"https://www.webtoons.com/.*/list\?title_no=.*", url)
             or re.match(r"https://m.webtoons.com/.*/list\?title_no=.*", url)
             or re.match(r"https://www.webtoons.com/.*/viewer\?title_no=.*", url)
```

### Comparing `mandown-1.7.0/mandown/ui/form.ui` & `mandown-1.8.0/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.7.0/mandown/ui/mainwin.py` & `mandown-1.8.0/mandown/ui/mainwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,37 +158,23 @@
 
         QMetaObject.connectSlotsByName(Widget)
 
     # setupUi
 
     def retranslateUi(self, Widget):
         Widget.setWindowTitle(QCoreApplication.translate("Widget", "Widget", None))
-        self.label_4.setText(
-            QCoreApplication.translate("Widget", "Source Folder / URL:", None)
-        )
-        self.button_from_url.setText(
-            QCoreApplication.translate("Widget", "Search URL", None)
-        )
-        self.button_from_folder.setText(
-            QCoreApplication.translate("Widget", "Open Folder", None)
-        )
+        self.label_4.setText(QCoreApplication.translate("Widget", "Source Folder / URL:", None))
+        self.button_from_url.setText(QCoreApplication.translate("Widget", "Search URL", None))
+        self.button_from_folder.setText(QCoreApplication.translate("Widget", "Open Folder", None))
         self.label_5.setText(QCoreApplication.translate("Widget", "Save to:", None))
         self.pushButton_3.setText(QCoreApplication.translate("Widget", "Browse", None))
         self.label_2.setText(QCoreApplication.translate("Widget", "Metadata", None))
         self.label.setText(QCoreApplication.translate("Widget", "Chapters", None))
         self.label_3.setText(QCoreApplication.translate("Widget", "Convert?", None))
         self.radio_no_convert.setText(QCoreApplication.translate("Widget", "No", None))
-        self.radio_convert_epub.setText(
-            QCoreApplication.translate("Widget", "EPUB", None)
-        )
-        self.radio_convert_pdf.setText(
-            QCoreApplication.translate("Widget", "PDF", None)
-        )
-        self.radio_convert_cbz.setText(
-            QCoreApplication.translate("Widget", "CBZ", None)
-        )
-        self.label_progress.setText(
-            QCoreApplication.translate("Widget", "Downloading...", None)
-        )
+        self.radio_convert_epub.setText(QCoreApplication.translate("Widget", "EPUB", None))
+        self.radio_convert_pdf.setText(QCoreApplication.translate("Widget", "PDF", None))
+        self.radio_convert_cbz.setText(QCoreApplication.translate("Widget", "CBZ", None))
+        self.label_progress.setText(QCoreApplication.translate("Widget", "Downloading...", None))
         self.button_start.setText(QCoreApplication.translate("Widget", "Start!", None))
 
     # retranslateUi
```

### Comparing `mandown-1.7.0/mandown/ui/ui.py` & `mandown-1.8.0/mandown/ui/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=no-member,invalid-name,pointless-string-statement
 """
 Generate mainwin.py while in mandown/ui/ with
 `uic -g python -o mainwin.py form.ui`
 """
+
 import sys
 from pathlib import Path
 
 import requests
 from PySide6.QtGui import QImage, QPixmap
 
 import mandown
@@ -91,32 +92,28 @@
         for i, chap in enumerate(self.comic.chapters):
             self.ui.chapter_table.setItem(i, 0, QTableWidgetItem(""))
             self.ui.chapter_table.setItem(i, 1, QTableWidgetItem(chap.title))
 
         # refresh screen w/metadata et al here
         if comic.metadata.cover_art:
             r = requests.get(comic.metadata.cover_art)
-            self.img_cover = QPixmap(
-                QImage.fromData(r.content).scaledToHeight(COVER_IMG_HEIGHT)
-            )
+            self.img_cover = QPixmap(QImage.fromData(r.content).scaledToHeight(COVER_IMG_HEIGHT))
             self.ui.label_image.setPixmap(self.img_cover)
 
     @property
     def text_dest_full(self) -> str:
         return str(Path(self.ui.text_dest.text()) / self.comic.metadata.title)
 
     """
     Hooks go here!
     """
 
     def hook_from_folder(self) -> None:
         # TODO: directly look for md-metadata.json instead
-        self.source_path = QFileDialog.getExistingDirectory(
-            self, "Open Comic Folder", "~"
-        )
+        self.source_path = QFileDialog.getExistingDirectory(self, "Open Comic Folder", "~")
         self.ui.text_source.setText(self.source_path)
         self.ui.text_dest.setText(str(Path(self.source_path).parent))
 
         # load metadata
         try:
             self.comic = mandown.load(self.source_path)
         except FileNotFoundError:
@@ -137,17 +134,15 @@
                 "Unknown Comic",
                 "Could not find comic: URL did not match any sources.",
                 QMessageBox.Ok,
             )
         self.comic = comic
 
     def hook_set_dest(self) -> None:
-        self.dest_path = QFileDialog.getExistingDirectory(
-            self, "Set Destination Folder", "~"
-        )
+        self.dest_path = QFileDialog.getExistingDirectory(self, "Set Destination Folder", "~")
         self.ui.text_dest.setText(self.dest_path)
 
     def hook_go(self) -> None:
         if not self.ui.text_source.text():
             # if empty
             res = QMessageBox.critical(
                 self,
@@ -209,17 +204,15 @@
                     self.text_dest_full,
                 ),
                 start=1,
             ):
                 self.ui.label_progress.setText(text)
                 self.ui.progress_bar.setValue(int(i / max_size * 100))
 
-        res = QMessageBox.information(
-            self, "Done", "All operations complete.", QMessageBox.Ok
-        )
+        res = QMessageBox.information(self, "Done", "All operations complete.", QMessageBox.Ok)
 
         self.ui.progress_bar.setDisabled(True)
 
 
 def main() -> None:
     app = QApplication([])
     wid = MandownQtUi()
```

### Comparing `mandown-1.7.0/pyproject.toml` & `mandown-1.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 [tool.poetry]
 name = "mandown"
-version = "1.7.0"
+version = "1.8.0"
 description = "Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter"
-authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
+authors = ["potatoeggy <eggyrules@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
 
 [tool.poetry.scripts]
 mandown = "mandown.cli:main"
 mandown-gui = "mandown.ui.ui:main"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<3.13"
 typer = "^0.7.0"
-feedparser = "^6.0.10"
+feedparser = "^6.0.11"
 beautifulsoup4 = "^4.12.2"
 requests = "^2.31.0"
-lxml = "^4.9.2"
-Pillow = "^9.5.0"
+lxml = "^5.1.0"
+pillow = "^10.2.0"
 python-slugify = "^8.0.1"
-PySide6 = {version = "^6.4.0", optional = true}
-natsort = "^8.1.0"
+PySide6 = { version = "^6.6.1", optional = true }
+natsort = "^8.4.0"
 filetype = "^1.2.0"
-comicon = "^1.0.0"
+comicon = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
-types-requests = "^2.31.0.1"
-types-lxml = "^2023.3.28"
+types-requests = "^2.31.0.20240106"
+types-lxml = "^2023.10.21"
+pytest-xdist = "^3.5.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.2"
+pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 gui = ["PySide6"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-select = ["B", "C", "E", "F", "W"]
-ignore = ["B905"]
-exclude = ["mandown/ui/*", "build/*"]
 target-version = "py310"
 line-length = 100
 
-[tool.ruff.mccabe]
-max-complexity = 18
+[tool.ruff.lint]
+mccabe.max-complexity = 18
+select = ["B", "C", "E", "F", "I", "W"]
+ignore = ["B905"]
+exclude = ["mandown/ui/*", "build/*"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "mandown/cli.py" = ["B008"]
 "tests/*" = ["E501"]
+
+[tool.coverage.run]
+concurrency = ["multiprocessing"]
+parallel = true
+sigterm = true
+
+[tool.pylint.MASTER]
+extension-pkg-allow-list = ["lxml", "PySide6"]
```

### Comparing `mandown-1.7.0/PKG-INFO` & `mandown-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.7.0
+Version: 1.8.0
 Summary: Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
-Author: Daniel Chen
-Author-email: danielchen04@hotmail.ca
-Requires-Python: >=3.10,<3.12
+Author: potatoeggy
+Author-email: eggyrules@gmail.com
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: gui
-Requires-Dist: Pillow (>=9.5.0,<10.0.0)
-Requires-Dist: PySide6 (>=6.4.0,<7.0.0) ; extra == "gui"
+Requires-Dist: PySide6 (>=6.6.1,<7.0.0) ; extra == "gui"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: comicon (>=1.0.0,<2.0.0)
-Requires-Dist: feedparser (>=6.0.10,<7.0.0)
+Requires-Dist: comicon (>=1.0.1,<2.0.0)
+Requires-Dist: feedparser (>=6.0.11,<7.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: natsort (>=8.1.0,<9.0.0)
+Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: natsort (>=8.4.0,<9.0.0)
+Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://github.com/potatoeggy/mandown
 Project-URL: Repository, https://github.com/potatoeggy/mandown
 Description-Content-Type: text/markdown
 
 # mandown
 
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/mandown)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Download from PyPI](https://img.shields.io/pypi/v/mandown)](https://pypi.org/project/mandown)
 [![Download from the AUR](https://img.shields.io/aur/version/mandown-git)](https://aur.archlinux.org/packages/mandown-git)
 [![Latest release](https://img.shields.io/github/v/release/potatoeggy/mandown?display_name=tag)](https://github.com/potatoeggy/mandown/releases/latest)
 [![License](https://img.shields.io/github/license/potatoeggy/mandown)](/LICENSE)
 
 Mandown is a comic downloader and a CBZ, EPUB, MOBI, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
@@ -120,21 +120,23 @@
 
 ## Supported sites
 
 To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
 
 - <https://blogtruyenmoi.com>
 - <https://comicfury.com>
+- https://\*.thecomicseries.com
 - <https://mangasee123.com>
 - <https://manganato.com>
 - <https://webtoons.com>
 - <https://mangadex.org>
 - <https://mangakakalot.com>
-- <https://manhuaes.com>
+- <https://manhuaaz.com>
 - <https://readcomiconline.li>
+- <https://www.kuaikanmanhua.com>
 
 ## Basic library usage
 
 See the [docs](/docs/) for more information and examples.
 
 To just download the images:
```

