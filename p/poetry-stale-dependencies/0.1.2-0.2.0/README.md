# Comparing `tmp/poetry_stale_dependencies-0.1.2.tar.gz` & `tmp/poetry_stale_dependencies-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_stale_dependencies-0.1.2.tar", max compression
+gzip compressed data, was "poetry_stale_dependencies-0.2.0.tar", max compression
```

## Comparing `poetry_stale_dependencies-0.1.2.tar` & `poetry_stale_dependencies-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     2049 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/LICENSE
--rw-r--r--   0        0        0       86 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/__init__.py
--rw-r--r--   0        0        0       22 2024-05-09 12:08:40.765956 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/_version.py
--rw-r--r--   0        0        0     3494 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/config.py
--rw-r--r--   0        0        0     3807 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/inspections.py
--rw-r--r--   0        0        0     2494 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/lock_spec.py
--rw-r--r--   0        0        0     3537 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/plugin.py
--rw-r--r--   0        0        0     6555 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/remote.py
--rw-r--r--   0        0        0      315 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/util.py
--rw-r--r--   0        0        0     3403 2024-05-09 12:08:21.733996 poetry_stale_dependencies-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 poetry_stale_dependencies-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2049 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1265 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/README.md
+-rw-r--r--   0        0        0       86 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-12 08:50:19.774423 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/_version.py
+-rw-r--r--   0        0        0     3952 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/config.py
+-rw-r--r--   0        0        0     6977 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/inspections.py
+-rw-r--r--   0        0        0     4468 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/lock_spec.py
+-rw-r--r--   0        0        0     5424 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/plugin.py
+-rw-r--r--   0        0        0     2806 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/project_spec.py
+-rw-r--r--   0        0        0     7386 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/remote.py
+-rw-r--r--   0        0        0      315 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/util.py
+-rw-r--r--   0        0        0     3424 2024-05-12 08:50:02.130450 poetry_stale_dependencies-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 poetry_stale_dependencies-0.2.0/PKG-INFO
```

### Comparing `poetry_stale_dependencies-0.1.2/LICENSE` & `poetry_stale_dependencies-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/config.py` & `poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from poetry_stale_dependencies.inspections import PackageInspectSpecs
 from poetry_stale_dependencies.lock_spec import LegacyPackageSource, PackageSpec
 
 
 def parse_timedelta(v: Any) -> timedelta:
     if not isinstance(v, str):
         raise ValueError("Timedelta must be a string (examples: 1d, 2w, 3mo, 4y)")
+    if v == "0":
+        return timedelta(0)
     if v.endswith("d"):
         return timedelta(days=int(v[:-1]))
     if v.endswith("w"):
         return timedelta(weeks=int(v[:-1]))
     if v.endswith("mo"):
         return timedelta(days=int(v[:-2]) * 30)
     if v.endswith("y"):
@@ -25,54 +27,64 @@
 
 
 @dataclass
 class PackageConfig:
     ignore: bool = False
     ignore_versions: Sequence[str] = ()
     time_to_stale: timedelta | None = None
-    include_remote_prepreleases: bool = False
+    time_to_ripe: timedelta | None = None
+    include_prereleases: bool = False
 
     @classmethod
     def from_raw(cls, raw: dict[str, Any]) -> PackageConfig:
         tts = raw.get("time_to_stale")
         if tts is not None:
             time_to_stale = parse_timedelta(tts)
         else:
             time_to_stale = None
+
+        ttr = raw.get("time_to_ripe")
+        if ttr is not None:
+            time_to_ripe = parse_timedelta(ttr)
+        else:
+            time_to_ripe = None
         return cls(
             ignore=raw.get("ignore", False),
             ignore_versions=raw.get("ignore_versions", []),
             time_to_stale=time_to_stale,
-            include_remote_prepreleases=raw.get("include_remote_prepreleases", False),
+            time_to_ripe=time_to_ripe,
+            include_prereleases=raw.get("include_prereleases", False),
         )
 
     Default: ClassVar[PackageConfig]
 
 
 PackageConfig.Default = PackageConfig()
 
 
 @dataclass
 class Config:
     lockfile: str
     sources: Sequence[str]
     packages: Mapping[str, PackageConfig]
     time_to_stale: timedelta
+    time_to_ripe: timedelta
 
     @classmethod
     def from_raw(cls, raw: dict[str, Any]) -> Config:
         packages = {}
         for package, package_config in raw.get("packages", {}).items():
             packages[package] = PackageConfig.from_raw(package_config)
 
         return cls(
             lockfile=raw.get("lockfile", "poetry.lock"),
             sources=raw.get("sources", ("pypi",)),
             packages=packages,
             time_to_stale=parse_timedelta(raw.get("time_to_stale", "2w")),
+            time_to_ripe=parse_timedelta(raw.get("time_to_ripe", "3d")),
         )
 
     def lockfile_path(self) -> Path:
         return Path(self.lockfile)
 
     def inspect_specs(self, package: str, specs: Sequence[PackageSpec]) -> Iterator[PackageInspectSpecs]:
         package_config = self.packages.get(package) or PackageConfig.Default
@@ -83,17 +95,19 @@
             specs = [spec for spec in specs if spec.version not in package_config.ignore_versions]
         if not specs:
             return
         by_source: dict[LegacyPackageSource | None, list[str]] = {}
         for spec in specs:
             by_source.setdefault(spec.source, []).append(spec.version)
         time_to_stale = package_config.time_to_stale or self.time_to_stale
+        time_to_ripe = package_config.time_to_ripe or self.time_to_ripe
         ignore_versions = frozenset(package_config.ignore_versions)
         for source, versions in by_source.items():
             yield PackageInspectSpecs(
                 package,
                 source,
                 time_to_stale,
+                time_to_ripe,
                 versions,
                 ignore_versions,
-                not package_config.include_remote_prepreleases,
+                not package_config.include_prereleases,
             )
```

### Comparing `poetry_stale_dependencies-0.1.2/poetry_stale_dependencies/remote.py` & `poetry_stale_dependencies-0.2.0/poetry_stale_dependencies/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import re
 from collections.abc import Container, Iterator, Sequence
 from dataclasses import dataclass
-from datetime import datetime
+from datetime import date, datetime
 from re import Pattern
 from sys import version_info
 from typing import TYPE_CHECKING, Any
 
 from cleo.commands.command import Command
 from cleo.io.outputs.output import Verbosity
 from httpx import Client
 
 from poetry_stale_dependencies.lock_spec import LegacyPackageSource
+from poetry_stale_dependencies.util import render_timedelta
 
 if TYPE_CHECKING:
     from poetry_stale_dependencies.config import PackageInspectSpecs
 
 
 @dataclass
 class RemoteReleaseSpec:
@@ -94,16 +95,31 @@
                     verbosity=Verbosity.VERY_VERBOSE,
                 )
                 continue
 
             releases.append(RemoteReleaseSpec(version, files))
         return cls(source, releases)
 
-    def applicable_releases(self) -> Iterator[RemoteReleaseSpec]:
-        return (release for release in reversed(self.releases) if any(not file.yanked for file in release.files))
+    def applicable_releases(self, package_name: str, ripe_time: date, com: Command) -> Iterator[RemoteReleaseSpec]:
+        for release in reversed(self.releases):
+            if all(file.yanked for file in release.files):
+                com.line(
+                    f"{package_name}[{self.source.reference}]: Ignoring release {release.version} because all files are yanked",
+                    verbosity=Verbosity.VERY_VERBOSE,
+                )
+                continue
+            release_time = release.upload_time().date()
+            if release_time > ripe_time:
+                age = date.today() - release_time
+                com.line(
+                    f"{package_name}[{self.source.reference}]: Ignoring release {release.version} because it was uploaded after ripe time (release age: {render_timedelta(age)})",
+                    verbosity=Verbosity.VERBOSE,
+                )
+                continue
+            yield release
 
 
 prerelease_pattern = re.compile(r".*(rc|a|b|dev)\d*$")
 
 
 def is_prerelease(version: str) -> bool:
     return bool(prerelease_pattern.fullmatch(version))
```

### Comparing `poetry_stale_dependencies-0.1.2/pyproject.toml` & `poetry_stale_dependencies-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "poetry-stale-dependencies"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
+readme = "README.md"
 authors = ["Biocatch LTD <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 poetry = "^1.7.1"
 cleo = "^2.1.0"
 tomli = "^2.0.1"
```

