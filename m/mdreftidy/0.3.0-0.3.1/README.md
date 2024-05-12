# Comparing `tmp/mdreftidy-0.3.0.tar.gz` & `tmp/mdreftidy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/mdreftidy/dist/.tmp-mej6pa3h/mdreftidy-0.3.0.tar", last modified: Sat May  4 21:45:18 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/mdreftidy/dist/.tmp-9gybj2al/mdreftidy-0.3.1.tar", last modified: Sun May 12 03:10:22 2024, max compression
```

## Comparing `mdreftidy-0.3.0.tar` & `mdreftidy-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.753028 mdreftidy-0.3.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdreftidy-0.3.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-04 21:45:18.743990 mdreftidy-0.3.0/PKG-INFO
--r-xr-xr-x   0 realz     (1000) realz     (1000)    15415 2024-05-04 18:48:12.000000 mdreftidy-0.3.0/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.529585 mdreftidy-0.3.0/mdreftidy/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      393 2024-05-02 12:48:46.000000 mdreftidy-0.3.0/mdreftidy/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6904 2024-05-03 10:26:36.000000 mdreftidy-0.3.0/mdreftidy/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    19184 2024-05-03 13:21:53.000000 mdreftidy-0.3.0/mdreftidy/mdreftidy.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.717476 mdreftidy-0.3.0/mdreftidy.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      297 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       49 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1566 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       10 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/top_level.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3746 2024-05-03 14:05:54.000000 mdreftidy-0.3.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-04 21:45:18.754119 mdreftidy-0.3.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-12 03:10:22.426248 mdreftidy-0.3.1/
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-12 03:10:22.179921 mdreftidy-0.3.1/.github/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    13808 2024-05-11 18:43:37.000000 mdreftidy-0.3.1/.github/README.remotified.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdreftidy-0.3.1/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    20357 2024-05-12 03:10:22.412488 mdreftidy-0.3.1/PKG-INFO
+-r-xr-xr-x   0 realz     (1000) realz     (1000)    12906 2024-05-11 18:43:36.000000 mdreftidy-0.3.1/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-12 03:10:22.262003 mdreftidy-0.3.1/mdreftidy/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      393 2024-05-02 12:48:46.000000 mdreftidy-0.3.1/mdreftidy/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     6904 2024-05-03 10:26:36.000000 mdreftidy-0.3.1/mdreftidy/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    19184 2024-05-03 13:21:53.000000 mdreftidy-0.3.1/mdreftidy/mdreftidy.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-12 03:10:22.389489 mdreftidy-0.3.1/mdreftidy.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    20357 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      326 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       49 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1705 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       10 2024-05-12 03:10:22.000000 mdreftidy-0.3.1/mdreftidy.egg-info/top_level.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     3934 2024-05-10 06:09:00.000000 mdreftidy-0.3.1/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-12 03:10:22.427248 mdreftidy-0.3.1/setup.cfg
```

### Comparing `mdreftidy-0.3.0/LICENSE.md` & `mdreftidy-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.3.0/PKG-INFO` & `mdreftidy-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreftidy
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -57,14 +57,16 @@
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.11.0; extra == "prod"
 Requires-Dist: pyyaml==6.0.1; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.3.0; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
 Requires-Dist: backports-tarfile==1.1.1; extra == "dev"
+Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
+Requires-Dist: bs4==0.0.2; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
@@ -81,14 +83,15 @@
 Requires-Dist: jaraco-context==5.3.0; extra == "dev"
 Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
 Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
+Requires-Dist: mdremotifier==0.3.1; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
@@ -107,19 +110,22 @@
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: snipinator==1.4.0; extra == "dev"
+Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
+Requires-Dist: types-beautifulsoup4==4.12.0.20240504; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.26.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
@@ -137,26 +143,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdreftidy][22]</div>
+# <div align="center">![mdreftidy][1]</div>
 
 <div align="center">
 
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -170,40 +176,40 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
 **CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references
 for markdown**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdreftidy does:
 
-Turn this ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Turn this ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -217,15 +223,15 @@
 [3]: ./reference-link-out-of-order-3
 [1]: ./unused-reference-link-1
 
 ```
 <!---->
 
 Into this
-([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
+([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -254,20 +260,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.1
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Example README: ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -303,24 +309,24 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdreftidy.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdreftidy.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - Example:
-  - Original: [./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md).
+  - Original: [./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md).
   - Tidied:
-    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
-  - Generation script: [./mdreftidy/examples/example.sh](./mdreftidy/examples/example.sh).
+    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
+  - Generation script: [./mdreftidy/examples/example.sh](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdreftidy
 - Projects using mdreftidy:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -343,25 +349,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](./LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdreftidy are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -369,75 +375,74 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ----------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐               |
+| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
     git: scripts, tests.
     xxhash: scripts (changeguard).
     rsync: out-of-directory test.
     expect: for `unbuffer`, useful to grab and compare ansi color symbols.
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
-    
+
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](.python-version) (which is currently
-    `3.8.0
-`).
+    [.python-version](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.python-version) (which is currently
+    `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](./README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](./pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](./README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdreftidy-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -449,101 +454,33 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
-[3]:
-  https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
-[4]:
-  https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdreftidy/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
-[12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[14]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
-[15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[17]: https://github.com/realazthat/mdreftidy/tree/master
-[18]: https://github.com/realazthat/mdreftidy/tree/develop
-
 <!-- Logo from https://lucide.dev/icons/users -->
 
-[19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
 <!-- Logo from https://lucide.dev/icons/laptop-minimal -->
 
-[20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
-[23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]:
-  https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper
-  "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]:
-  https://github.com/ravgeetdhillon/markdown-imgur-upload
-  "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]:
-  https://github.com/chocoluffy/lazy-markdown
-  "Uploads to LeanCloud, readme is a bit unclear"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
-[99]: https://github.com/dce/mdrenum
+[1]: https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdreftidy/
+[9]: https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdreftidy/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/master?style=plastic
+[14]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
+[16]: https://github.com/realazthat/mdreftidy/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[19]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[21]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
```

### Comparing `mdreftidy-0.3.0/README.md` & `mdreftidy-0.3.1/.github/README.remotified.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdreftidy][22]</div>
+# <div align="center">![mdreftidy][1]</div>
 
 <div align="center">
 
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -43,40 +43,40 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
 **CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references
 for markdown**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdreftidy does:
 
-Turn this ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Turn this ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -90,15 +90,15 @@
 [3]: ./reference-link-out-of-order-3
 [1]: ./unused-reference-link-1
 
 ```
 <!---->
 
 Into this
-([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
+([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -127,20 +127,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.1
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Example README: ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -176,24 +176,24 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdreftidy.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdreftidy.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - Example:
-  - Original: [./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md).
+  - Original: [./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md).
   - Tidied:
-    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
-  - Generation script: [./mdreftidy/examples/example.sh](./mdreftidy/examples/example.sh).
+    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
+  - Generation script: [./mdreftidy/examples/example.sh](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdreftidy
 - Projects using mdreftidy:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -216,25 +216,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](./LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdreftidy are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -242,75 +242,74 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ----------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐               |
+| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
     git: scripts, tests.
     xxhash: scripts (changeguard).
     rsync: out-of-directory test.
     expect: for `unbuffer`, useful to grab and compare ansi color symbols.
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
-    
+
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](.python-version) (which is currently
-    `3.8.0
-`).
+    [.python-version](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.python-version) (which is currently
+    `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](./README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](./pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](./README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdreftidy-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -322,101 +321,33 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
-[3]:
-  https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
-[4]:
-  https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdreftidy/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
-[12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[14]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
-[15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[17]: https://github.com/realazthat/mdreftidy/tree/master
-[18]: https://github.com/realazthat/mdreftidy/tree/develop
-
 <!-- Logo from https://lucide.dev/icons/users -->
 
-[19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
 <!-- Logo from https://lucide.dev/icons/laptop-minimal -->
 
-[20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
-[23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]:
-  https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper
-  "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]:
-  https://github.com/ravgeetdhillon/markdown-imgur-upload
-  "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]:
-  https://github.com/chocoluffy/lazy-markdown
-  "Uploads to LeanCloud, readme is a bit unclear"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
-[99]: https://github.com/dce/mdrenum
+[1]: https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdreftidy/
+[9]: https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdreftidy/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/master?style=plastic
+[14]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
+[16]: https://github.com/realazthat/mdreftidy/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[19]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[21]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
```

#### html2text {}

```diff
@@ -1,162 +1,140 @@
 #
-                               ![mdreftidy][22]
-          ![**Audience:** Developers][19] ![**Platform:** Linux][20]
+                                ![mdreftidy][1]
+           ![**Audience:** Developers][2] ![**Platform:** Linux][3]
  _?ð_?_?_?_FF_ee_aa_tt_uu_rr_ee_ss ? ?•?  _?ð_?_?_? _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ? ?•?  _?ð_?_?_?_UU_ss_aa_gg_ee ? ?•?  _?ð_?_?_?»_CC_LL_II ? ?•?  _?ð_?_?_?¡_EE_xx_aa_mm_pp_ll_ee_ss
                               ? ?•?  _?â_?_?_RR_ee_qq_uu_ii_rr_ee_mm_ee_nn_tt_ss
-  ![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5] [!
-[Python Version][8]][5] **CLI to tidy ({renumber,move-to-bottom,sort,clean}) up
+   ![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8] [!
+[Python Version][9]][8] **CLI to tidy ({renumber,move-to-bottom,sort,clean}) up
                     {image,link} references for markdown**
 ---
 | | Status | Stable | Unstable | | | ----------------- | ----------------------
----- | ------------------------- | ------------------------- | ----------------
--- | | **[Master][17]** | [![Build and Test][1]][2] | [![since tagged][6]][10]
- | | ![last commit][7] | | **[Develop][18]** | [![Build and Test][11]][2] | [!
-  [since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+----- | ------------------------- | ------------------------- | ---------------
+--- | | **[Master][10]** | [![Build and Test][11]][12] | [![since tagged][13]]
+[14] | | ![last commit][15] | | **[Develop][16]** | [![Build and Test][17]][12]
+| [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 [Demo]## â What What mdreftidy does: Turn this ([./mdreftidy/examples/
-EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)): ```md # Example markdown file ##
-Reference link: Out of order [Reference link: Out of order 1][3], [Reference
-link: Out of order 2][2]. [2]: ./reference-link-out-of-order-2 ## Footnotes
-[6]: ./unused-reference-link-6 [3]: ./reference-link-out-of-order-3 [1]: ./
-unused-reference-link-1 ``` Into this ([./mdreftidy/examples/EXAMPLE.all-
-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md)): ```md #
-Example markdown file ## Reference link: Out of order [Reference link: Out of
-order 1][1], [Reference link: Out of order 2][2]. ## Footnotes [1]: ./
-reference-link-out-of-order-3 [2]: ./reference-link-out-of-order-2 ``` This is
-useful for uploading `README.md` files to third-party sites, like the npmjs.com
-registry, or pypi.org registry, because these registries will break the local
-images in your README when displayed on their sites. ## ð Features -
-Renumbers references by order used. - Optionally removes unused references. -
-Optionally moves references to the bottom. - Optionally sorts reference blocks.
-## ð  Installation ```bash # Install from pypi (https://pypi.org/project/
-mdreftidy/) pip install mdreftidy # Install from git (https://github.com/
-realazthat/mdreftidy) pip install git+https://github.com/realazthat/
-mdreftidy.git@v0.3.0 ``` ## ð Usage Example README: ([./mdreftidy/examples/
-EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)): ```md # Example markdown file ##
+EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/
+examples/EXAMPLE.md)): ```md # Example markdown file ## Reference link: Out of
+order [Reference link: Out of order 1][3], [Reference link: Out of order 2][2].
+[2]: ./reference-link-out-of-order-2 ## Footnotes [6]: ./unused-reference-link-
+6 [3]: ./reference-link-out-of-order-3 [1]: ./unused-reference-link-1 ``` Into
+this ([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/
+realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-
+opts.tidied.md)): ```md # Example markdown file ## Reference link: Out of order
+[Reference link: Out of order 1][1], [Reference link: Out of order 2][2]. ##
+Footnotes [1]: ./reference-link-out-of-order-3 [2]: ./reference-link-out-of-
+order-2 ``` This is useful for uploading `README.md` files to third-party
+sites, like the npmjs.com registry, or pypi.org registry, because these
+registries will break the local images in your README when displayed on their
+sites. ## ð Features - Renumbers references by order used. - Optionally
+removes unused references. - Optionally moves references to the bottom. -
+Optionally sorts reference blocks. ## ð  Installation ```bash # Install from
+pypi (https://pypi.org/project/mdreftidy/) pip install mdreftidy # Install from
+git (https://github.com/realazthat/mdreftidy) pip install git+https://
+github.com/realazthat/mdreftidy.git@v0.3.1 ``` ## ð Usage Example README: (
+[./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/
+v0.3.1/mdreftidy/examples/EXAMPLE.md)): ```md # Example markdown file ##
 Reference link: Out of order [Reference link: Out of order 1][3], [Reference
 link: Out of order 2][2]. [2]: ./reference-link-out-of-order-2 ## Footnotes
 [6]: ./unused-reference-link-6 [3]: ./reference-link-out-of-order-3 [1]: ./
 unused-reference-link-1 ``` Generating the README: ```bash $ python -
 m mdreftidy.cli ./mdreftidy/examples/EXAMPLE.md --move-to-bottom --remove-
 unused --sort-ref-blocks --renumber -o - 2>/dev/null # Example markdown file ##
 Reference link: Out of order [Reference link: Out of order 1][1], [Reference
 link: Out of order 2][2]. ## Footnotes [1]: ./reference-link-out-of-order-3
 [2]: ./reference-link-out-of-order-2 ``` ## ð» Command Line Options [Output
 of `python -m mdreftidy.cli --help`]## ð¡ Examples - Example: - Original: [./
-mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md). - Tidied: [./
-mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/
-EXAMPLE.all-opts.tidied.md). - Generation script: [./mdreftidy/examples/
-example.sh](./mdreftidy/examples/example.sh). ## â Requirements - Linux-like
+mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/
+v0.3.1/mdreftidy/examples/EXAMPLE.md). - Tidied: [./mdreftidy/examples/
+EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/
+v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md). - Generation script: [./
+mdreftidy/examples/example.sh](https://github.com/realazthat/mdreftidy/blob/
+v0.3.1/mdreftidy/examples/example.sh). ## â Requirements - Linux-like
 environment - Why: Uses pexpect.spawn(). - Python 3.8+ - Why: Some dev
 dependencies require Python 3.8+. ### Tested Platforms - WSL2 Ubuntu 20.04,
 Python `3.8.0`. - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`,
-tested in GitHub Actions workflow ([build-and-test.yml](./.github/workflows/
-build-and-test.yml)). ## ð¤ Versioning We use SemVer for versioning. For the
-versions available, see the tags on this repository. ## ð License This
-project is licensed under the MIT License - see the [./LICENSE.md](./
-LICENSE.md) file for details. ## ð Thanks Main libraries used in mdreftidy
-are: - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe). -
-Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
-## ð¤ Related Projects Not complete, and not necessarily up to date. Make a
-PR ([contributions](#-contributions)) to insert/modify. | Project | Stars |
-Last Update | Language | Platform | Similarity X Obviousness | | --------------
---- | ----- | ------------ | -------- | -------- | ------------------------ | |
-[dce/mdrenum][60] | 2 | `2023/11/16` | JS | CLI | â­â­â­â­â­ | ## ð«¡
-Contributions ### Development environment: Linux-like - For running `pre.sh`
-(Linux-like environment). - From [./.github/dependencies.yml](./.github/
+tested in GitHub Actions workflow ([build-and-test.yml](https://github.com/
+realazthat/mdreftidy/blob/v0.3.1/.github/workflows/build-and-test.yml)). ##
+ð¤ Versioning We use SemVer for versioning. For the versions available, see
+the tags on this repository. ## ð License This project is licensed under the
+MIT License - see the [./LICENSE.md](https://github.com/realazthat/mdreftidy/
+blob/v0.3.1/LICENSE.md) file for details. ## ð Thanks Main libraries used in
+mdreftidy are: - Markdown AST: [mistletoe](https://github.com/miyuchina/
+mistletoe). - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/
+rich-argparse). ## ð¤ Related Projects Not complete, and not necessarily up
+to date. Make a PR ([contributions](#-contributions)) to insert/modify. |
+Project | Stars | Last Update | Language | Platform | Similarity X Obviousness
+| | ----------------- | ----- | ------------ | -------- | -------- | ----------
+-------------- | | [dce/mdrenum][60] | 2 | `2023/11/16` | JS | CLI |
+â­â­â­â­â­ | ## ð«¡ Contributions ### Development environment: Linux-like
+- For running `pre.sh` (Linux-like environment). - From [./.github/
+dependencies.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/
 dependencies.yml), which is used for the GH Action to do a fresh install of
 everything: ```yaml bash: scripts. findutils: scripts. grep: tests. xxd: tests.
 git: scripts, tests. xxhash: scripts (changeguard). rsync: out-of-directory
 test. expect: for `unbuffer`, useful to grab and compare ansi color symbols.
 jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to
 generate the README; the README generator needs to use `tomlq` (which is a part
 of `yq`) to query `pyproject.toml`. ``` - Requires `pyenv`, or an exact
-matching version of python as in [.python-version](.python-version) (which is
-currently `3.8.0 `). - `jq`, ([installation](https://jqlang.github.io/jq/))
-required for [yq](https://github.com/kislyuk/yq), which is itself required for
-our [./README.md](./README.md) generation, which uses `tomlq` (from the [yq]
-(https://github.com/kislyuk/yq) package) to include version strings from [./
-pyproject.toml](./pyproject.toml). - act (to run the GH Action locally): -
+matching version of python as in [.python-version](https://github.com/
+realazthat/mdreftidy/blob/v0.3.1/.python-version) (which is currently `3.8.0
+`). - `jq`, ([installation](https://jqlang.github.io/jq/)) required for [yq]
+(https://github.com/kislyuk/yq), which is itself required for our [./README.md]
+(https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) generation,
+which uses `tomlq` (from the [yq](https://github.com/kislyuk/yq) package) to
+include version strings from [./pyproject.toml](https://github.com/realazthat/
+mdreftidy/blob/v0.3.1/pyproject.toml). - act (to run the GH Action locally): -
 Requires nodejs. - Requires Go. - docker. - Generate animation: - docker ###
 Commit Process 1. (Optionally) Fork the `develop` branch. 2. Stage your files:
 `git add path/to/file.py`. 3. `bash ./scripts/pre.sh`, this will format, lint,
 and test the code. 4. `git status` check if anything changed (generated [./
-README.md](./README.md) for example), if so, `git add` the changes, and go back
-to the previous step. 5. `git commit -m "..."`. 6. Make a PR to `develop` (or
-push to develop if you have the rights). ## ðð Release Process These
-instructions are for maintainers of the project. 1. In the `develop` branch,
-run `bash ./scripts/pre.sh` to ensure everything is in order. 2. In the
-`develop` branch, bump the version in [./pyproject.toml](./pyproject.toml),
-following semantic versioning principles. Also modify the
-`last_unstable_release` and `last_stable_release` in the `[tool.mdreftidy-
+README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) for
+example), if so, `git add` the changes, and go back to the previous step. 5.
+`git commit -m "..."`. 6. Make a PR to `develop` (or push to develop if you
+have the rights). ## ðð Release Process These instructions are for
+maintainers of the project. 1. In the `develop` branch, run `bash ./scripts/
+pre.sh` to ensure everything is in order. 2. In the `develop` branch, bump the
+version in [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/
+v0.3.1/pyproject.toml), following semantic versioning principles. Also modify
+the `last_unstable_release` and `last_stable_release` in the `[tool.mdreftidy-
 project-metadata]` table as appropriate. Run `bash ./scripts/pre.sh` to ensure
 everything is in order. 3. In the `develop` branch, commit these changes with a
 message like `"Prepare release X.Y.Z"`. (See the contributions section [above]
 (#commit-process)). 4. Merge the `develop` branch into the `master` branch:
 `git checkout master && git merge develop --no-ff`. 5. `master` branch: Tag the
 release: Create a git tag for the release with `git tag -a vX.Y.Z -m "Version
 X.Y.Z"`. 6. Publish to PyPI: Publish the release to PyPI with `bash ./scripts/
 deploy-to-pypi.sh`. 7. Push to GitHub: Push the commit and tags to GitHub with
 `git push && git push --tags`. 8. The `--no-ff` option adds a commit to the
 master branch for the merge, so refork the develop branch from the master
 branch: `git checkout develop && git merge master`. 9. Push the develop branch
-to GitHub: `git push origin develop`. [1]: https://img.shields.io/github/
-actions/workflow/status/realazthat/mdreftidy/build-and-
-test.yml?branch=master&style=plastic [2]: https://github.com/realazthat/
-mdreftidy/actions/workflows/build-and-test.yml [3]: https://img.shields.io/
-github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E [4]: https://
-img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E [5]: https://
-pypi.org/project/mdreftidy/ [6]: https://img.shields.io/github/commits-since/
-realazthat/mdreftidy/v0.3.0/master?style=plastic [7]: https://img.shields.io/
-github/last-commit/realazthat/mdreftidy/master?style=plastic [8]: https://
-img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E [9]: https:
-//img.shields.io/github/languages/top/realazthat/
-mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [10]: https://
-github.com/realazthat/mdreftidy/compare/v0.3.0...master [11]: https://
-img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-
-test.yml?branch=develop&style=plastic [12]: https://img.shields.io/github/
-commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic [13]: https://
-github.com/realazthat/mdreftidy/compare/v0.3.0...develop [14]: https://
-img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/
-develop?style=plastic [16]: https://github.com/realazthat/mdreftidy/compare/
-v0.3.0...develop [17]: https://github.com/realazthat/mdreftidy/tree/master
-[18]: https://github.com/realazthat/mdreftidy/tree/develop [19]: https://
+to GitHub: `git push origin develop`. [1]: https://raw.githubusercontent.com/
+realazthat/mdreftidy/v0.3.1/.github/logo-exported.svg [2]: https://
 img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-[20]: https://img.shields.io/badge/Platform-Linux-
+[3]: https://img.shields.io/badge/Platform-Linux-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md [22]: ./.github/logo-exported.svg [23]: https://
-docs.github.com/en/get-started/writing-on-github/working-with-advanced-
-formatting/creating-a-permanent-link-to-a-code-snippet [24]: https://
-github.com/zakhenry/embedme [25]: https://github.com/electrovir/markdown-code-
-example-inserter [26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme [28]: https://github.com/drewavis/
-markdowninclude [29]: https://github.com/tokusumi/markdown-embed-code [30]:
-https://github.com/ARMmbed/snippet [31]: https://github.com/SimonCropp/
-MarkdownSnippets [32]: https://github.com/shiftkey/scribble [33]: https://
-github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md [34]:
-https://github.com/JulianCataldo/remark-embed [35]: https://github.com/
-calebpeterson/jest-transformer-test-md [36]: https://github.com/ildar-
-shaimordanov/git-markdown-snippet [37]: https://github.com/sammndhr/gridsome-
-remark-embed-snippet [38]: https://gridsome.org/ [39]: https://github.com/
-gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet [40]: https://
-github.com/gatsbyjs/gatsby [41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises [43]: https://
-github.com/devincornell/pymddoc [44]: https://github.com/NativeScript/markdown-
-snippet-injector [45]: https://github.com/polywrap/doc-snippets [46]: https://
-github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets [47]:
-https://github.com/xrd/oreilly-snippets [48]: https://github.com/DamonOehlman/
-injectcode [49]: https://github.com/fuxingloh/remark-code-import-replace [50]:
-https://github.com/teyc/markdown-snippet [51]: https://github.com/marc-bouvier-
-graveyard/baldir_markdown [52]: https://github.com/tjstankus/commitate [53]:
-https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI." [54]:
-https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud." [55]: https:/
-/github.com/crh19970307/mdul "Uploads to sm.ms" [56]: https://github.com/
-SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud" [57]:
-https://github.com/jen6/imgo "Upload to Google Drive" [58]: https://github.com/
-ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because
-it requires you to put the images into a particular directory" [59]: https://
-github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
-unclear" [61]: https://github.com/loheagn/gopic "Upload to cloud, not clear
-which cloud" [99]: https://github.com/dce/mdrenum
+[4]: https://img.shields.io/github/languages/top/realazthat/
+mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [5]: https://
+img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md [7]: https:
+//img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E [8]: https://
+pypi.org/project/mdreftidy/ [9]: https://img.shields.io/pypi/pyversions/
+mdreftidy?style=plastic&color=0A1E1E [10]: https://github.com/realazthat/
+mdreftidy/tree/master [11]: https://img.shields.io/github/actions/workflow/
+status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdreftidy/actions/workflows/build-and-
+test.yml [13]: https://img.shields.io/github/commits-since/realazthat/
+mdreftidy/v0.3.1/master?style=plastic [14]: https://github.com/realazthat/
+mdreftidy/compare/v0.3.1...master [15]: https://img.shields.io/github/last-
+commit/realazthat/mdreftidy/master?style=plastic [16]: https://github.com/
+realazthat/mdreftidy/tree/develop [17]: https://img.shields.io/github/actions/
+workflow/status/realazthat/mdreftidy/build-and-
+test.yml?branch=develop&style=plastic [18]: https://img.shields.io/github/
+commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic [19]: https://
+github.com/realazthat/mdreftidy/compare/v0.3.1...develop [20]: https://
+img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/
+develop?style=plastic [21]: https://github.com/realazthat/mdreftidy/compare/
+v0.3.1...develop [22]: https://img.shields.io/github/last-commit/realazthat/
+mdreftidy/develop?style=plastic
```

### Comparing `mdreftidy-0.3.0/mdreftidy/cli.py` & `mdreftidy-0.3.1/mdreftidy/cli.py`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.3.0/mdreftidy/mdreftidy.py` & `mdreftidy-0.3.1/mdreftidy/mdreftidy.py`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.3.0/mdreftidy.egg-info/PKG-INFO` & `mdreftidy-0.3.1/mdreftidy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreftidy
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -57,14 +57,16 @@
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.11.0; extra == "prod"
 Requires-Dist: pyyaml==6.0.1; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.3.0; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
 Requires-Dist: backports-tarfile==1.1.1; extra == "dev"
+Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
+Requires-Dist: bs4==0.0.2; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
@@ -81,14 +83,15 @@
 Requires-Dist: jaraco-context==5.3.0; extra == "dev"
 Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
 Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
+Requires-Dist: mdremotifier==0.3.1; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
@@ -107,19 +110,22 @@
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: snipinator==1.4.0; extra == "dev"
+Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
+Requires-Dist: types-beautifulsoup4==4.12.0.20240504; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.26.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
@@ -137,26 +143,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdreftidy][22]</div>
+# <div align="center">![mdreftidy][1]</div>
 
 <div align="center">
 
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -170,40 +176,40 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
 **CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references
 for markdown**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdreftidy does:
 
-Turn this ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Turn this ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -217,15 +223,15 @@
 [3]: ./reference-link-out-of-order-3
 [1]: ./unused-reference-link-1
 
 ```
 <!---->
 
 Into this
-([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
+([./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -254,20 +260,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.1
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
+Example README: ([./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 ## Reference link: Out of order
 
@@ -303,24 +309,24 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdreftidy.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdreftidy.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - Example:
-  - Original: [./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md).
+  - Original: [./mdreftidy/examples/EXAMPLE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.md).
   - Tidied:
-    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](./mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
-  - Generation script: [./mdreftidy/examples/example.sh](./mdreftidy/examples/example.sh).
+    [./mdreftidy/examples/EXAMPLE.all-opts.tidied.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/EXAMPLE.all-opts.tidied.md).
+  - Generation script: [./mdreftidy/examples/example.sh](https://github.com/realazthat/mdreftidy/blob/v0.3.1/mdreftidy/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdreftidy
 - Projects using mdreftidy:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -343,25 +349,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](./LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdreftidy are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -369,75 +375,74 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ----------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐               |
+| [dce/mdrenum][60] | 2     | `2023/11/16` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
     git: scripts, tests.
     xxhash: scripts (changeguard).
     rsync: out-of-directory test.
     expect: for `unbuffer`, useful to grab and compare ansi color symbols.
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
-    
+
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](.python-version) (which is currently
-    `3.8.0
-`).
+    [.python-version](https://github.com/realazthat/mdreftidy/blob/v0.3.1/.python-version) (which is currently
+    `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](./README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](./pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](./README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdreftidy/blob/v0.3.1/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdreftidy/blob/v0.3.1/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdreftidy-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -449,101 +454,33 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
-[3]:
-  https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
-[4]:
-  https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdreftidy/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
-[12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[14]:
-  https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
-[15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
-[17]: https://github.com/realazthat/mdreftidy/tree/master
-[18]: https://github.com/realazthat/mdreftidy/tree/develop
-
 <!-- Logo from https://lucide.dev/icons/users -->
 
-[19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
 <!-- Logo from https://lucide.dev/icons/laptop-minimal -->
 
-[20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
-[23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]:
-  https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper
-  "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]:
-  https://github.com/ravgeetdhillon/markdown-imgur-upload
-  "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]:
-  https://github.com/chocoluffy/lazy-markdown
-  "Uploads to LeanCloud, readme is a bit unclear"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
-[99]: https://github.com/dce/mdrenum
+[1]: https://raw.githubusercontent.com/realazthat/mdreftidy/v0.3.1/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdreftidy/blob/v0.3.1/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdreftidy/
+[9]: https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdreftidy/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/master?style=plastic
+[14]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
+[16]: https://github.com/realazthat/mdreftidy/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[19]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.1/develop?style=plastic
+[21]: https://github.com/realazthat/mdreftidy/compare/v0.3.1...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
```

### Comparing `mdreftidy-0.3.0/mdreftidy.egg-info/requires.txt` & `mdreftidy-0.3.1/mdreftidy.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 [:python_version < "3.8"]
 importlib-metadata
 
 [dev]
 argcomplete==3.3.0
 autoflake==2.3.1
 backports-tarfile==1.1.1
+beautifulsoup4==4.12.3
+bs4==0.0.2
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 changeguard==0.3.1
 charset-normalizer==3.3.2
 colorama==0.4.6
 cryptography==42.0.5
@@ -33,14 +35,15 @@
 jaraco-context==5.3.0
 jaraco-functools==4.0.1
 jeepney==0.8.0
 jinja2==3.1.3
 keyring==25.2.0
 markdown-it-py==3.0.0
 markupsafe==2.1.5
+mdremotifier==0.3.1
 mdurl==0.1.2
 mistletoe==1.3.0
 more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.17
 nodeenv==1.8.0
@@ -59,19 +62,22 @@
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 rich-argparse==1.4.0
 secretstorage==3.3.3
 snipinator==1.4.0
+soupsieve==2.5
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
 twine==5.0.0
+types-beautifulsoup4==4.12.0.20240504
 types-colorama==0.4.15.20240311
+types-html5lib==1.1.11.20240228
 types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
 urllib3==2.2.1
 virtualenv==20.26.0
 xmltodict==0.13.0
 yapf==0.40.2
 yq==3.2.3
```

### Comparing `mdreftidy-0.3.0/pyproject.toml` & `mdreftidy-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdreftidy"
-version = "0.3.0"
+version = "0.3.1"
 description = "CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
-readme = "README.md"
+readme = ".github/README.remotified.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
@@ -59,14 +59,16 @@
 # Set of dev dependencies, all pinned, so that they are known to work. To add a
 # new dependency here, add the unpinned package name here, and then run
 # `EXTRA=dev bash scripts/pin-extra-reqs.sh`.
 dev = [
   "argcomplete==3.3.0",
   "autoflake==2.3.1",
   "backports-tarfile==1.1.1",
+  "beautifulsoup4==4.12.3",
+  "bs4==0.0.2",
   "certifi==2024.2.2",
   "cffi==1.16.0",
   "cfgv==3.4.0",
   "changeguard==0.3.1",
   "charset-normalizer==3.3.2",
   "colorama==0.4.6",
   "cryptography==42.0.5",
@@ -83,14 +85,15 @@
   "jaraco-context==5.3.0",
   "jaraco-functools==4.0.1",
   "jeepney==0.8.0",
   "jinja2==3.1.3",
   "keyring==25.2.0",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.5",
+  "mdremotifier==0.3.1",
   "mdurl==0.1.2",
   "mistletoe==1.3.0",
   "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
   "nh3==0.2.17",
   "nodeenv==1.8.0",
@@ -109,19 +112,22 @@
   "requests==2.31.0",
   "requests-toolbelt==1.0.0",
   "rfc3986==2.0.0",
   "rich==13.7.1",
   "rich-argparse==1.4.0",
   "secretstorage==3.3.3",
   "snipinator==1.4.0",
+  "soupsieve==2.5",
   "toml-sort==0.23.1",
   "tomli==2.0.1",
   "tomlkit==0.12.4",
   "twine==5.0.0",
+  "types-beautifulsoup4==4.12.0.20240504",
   "types-colorama==0.4.15.20240311",
+  "types-html5lib==1.1.11.20240228",
   "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
   "urllib3==2.2.1",
   "virtualenv==20.26.0",
   "xmltodict==0.13.0",
   "yapf==0.40.2",
   "yq==3.2.3",
@@ -133,14 +139,14 @@
 
 [project.urls]
 Homepage = "https://github.com/realazthat/mdreftidy"
 Documentation = "https://github.com/realazthat/mdreftidy"
 Repository = "https://github.com/realazthat/mdreftidy"
 
 [tool.mdreftidy-project-metadata]
-last_unstable_release = "0.3.0"
-last_stable_release = "0.3.0"
+last_unstable_release = "0.3.1"
+last_stable_release = "0.3.1"
 
 [tool.setuptools]
 packages = ["mdreftidy"]
 
 [tool.tomlsort]
```

