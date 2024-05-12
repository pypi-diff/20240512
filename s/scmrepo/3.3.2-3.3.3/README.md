# Comparing `tmp/scmrepo-3.3.2.tar.gz` & `tmp/scmrepo-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-3.3.2.tar", last modified: Wed Apr 24 16:18:41 2024, max compression
+gzip compressed data, was "scmrepo-3.3.3.tar", last modified: Sun May 12 20:13:35 2024, max compression
```

## Comparing `scmrepo-3.3.2.tar` & `scmrepo-3.3.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.733954 scmrepo-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-24 16:18:22.000000 scmrepo-3.3.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 16:18:22.000000 scmrepo-3.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-24 16:18:22.000000 scmrepo-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 16:18:41.733954 scmrepo-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-24 16:18:22.000000 scmrepo-3.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-24 16:18:22.000000 scmrepo-3.3.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-24 16:18:22.000000 scmrepo-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:18:41.733954 scmrepo-3.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.717954 scmrepo-3.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (127)    34820 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (127)    37035 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/src/scmrepo/git/lfs/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/smudge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.733954 scmrepo-3.3.2/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_lfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/user.key.pub
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/vendor/test_paramiko_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.581308 scmrepo-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-12 20:13:21.000000 scmrepo-3.3.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-12 20:13:21.000000 scmrepo-3.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-12 20:13:21.000000 scmrepo-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-12 20:13:35.581308 scmrepo-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-12 20:13:21.000000 scmrepo-3.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-12 20:13:21.000000 scmrepo-3.3.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-12 20:13:21.000000 scmrepo-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:13:35.581308 scmrepo-3.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.565307 scmrepo-3.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (127)    34740 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (127)    37035 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/lfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/smudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_lfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/vendor/test_paramiko_vendor.py
```

### Comparing `scmrepo-3.3.2/.cruft.json` & `scmrepo-3.3.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/.github/workflows/release.yaml` & `scmrepo-3.3.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/.github/workflows/tests.yaml` & `scmrepo-3.3.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/.gitignore` & `scmrepo-3.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/.pre-commit-config.yaml` & `scmrepo-3.3.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-json
       - id: check-merge-conflict
@@ -16,15 +16,15 @@
       - id: check-yaml
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.5'
+    rev: 'v0.4.3'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
```

### Comparing `scmrepo-3.3.2/CODE_OF_CONDUCT.rst` & `scmrepo-3.3.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/CONTRIBUTING.rst` & `scmrepo-3.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/LICENSE` & `scmrepo-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/PKG-INFO` & `scmrepo-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.2
+Version: 3.3.3
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,15 @@
 Requires-Dist: pytest-asyncio<1,>=0.23.2; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-docker<4,>=1; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-sugar; extra == "tests"
 Requires-Dist: pytest-test-utils<0.2,>=0.1.0; extra == "tests"
 Provides-Extra: dev
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: scmrepo[tests]; extra == "dev"
 Requires-Dist: types-certifi; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-paramiko; extra == "dev"
 Requires-Dist: types-tqdm; extra == "dev"
 
 scmrepo
```

### Comparing `scmrepo-3.3.2/README.rst` & `scmrepo-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/noxfile.py` & `scmrepo-3.3.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/pyproject.toml` & `scmrepo-3.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "pytest-cov>=4.1.0",
     "pytest-docker>=1,<4",
     "pytest-mock",
     "pytest-sugar",
     "pytest-test-utils>=0.1.0,<0.2",
 ]
 dev = [
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     "scmrepo[tests]",
     "types-certifi",
     "types-mock",
     "types-paramiko",
     "types-tqdm",
 ]
```

### Comparing `scmrepo-3.3.2/src/scmrepo/asyn.py` & `scmrepo-3.3.3/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/base.py` & `scmrepo-3.3.3/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/exceptions.py` & `scmrepo-3.3.3/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/fs.py` & `scmrepo-3.3.3/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/__init__.py` & `scmrepo-3.3.3/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/base.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                 repo = clone_from()
 
             with closing(repo):
                 if mirror:
                     cls._set_mirror(repo, progress=progress)
                 else:
                     cls._set_default_tracking_branch(repo)
-        except Exception as exc:  # noqa: BLE001
+        except Exception as exc:
             raise CloneError(url, os.fsdecode(to_path)) from exc
 
     @staticmethod
     def _set_default_tracking_branch(repo: "Repo"):
         from dulwich.refs import LOCAL_BRANCH_PREFIX, parse_symref_value
 
         try:
@@ -576,15 +576,15 @@
         from dulwich.client import HTTPUnauthorized, get_transport_and_path
         from dulwich.errors import NotGitRepository
         from dulwich.porcelain import get_remote_repo
 
         try:
             _remote, location = get_remote_repo(self.repo, url)
             client, path = get_transport_and_path(location, **kwargs)
-        except Exception as exc:  # noqa: BLE001
+        except Exception as exc:
             raise InvalidRemote(url) from exc
 
         try:
             if base:
                 yield from (
                     os.fsdecode(ref)
                     for ref in client.get_refs(path)
@@ -613,15 +613,15 @@
         from dulwich.errors import NotGitRepository, SendPackError
         from dulwich.objectspec import parse_reftuples
         from dulwich.porcelain import DivergedBranches, check_diverged, get_remote_repo
 
         try:
             _remote, location = get_remote_repo(self.repo, url)
             client, path = get_transport_and_path(location, **kwargs)
-        except Exception as exc:  # noqa: BLE001
+        except Exception as exc:
             raise SCMError(f"'{url}' is not a valid Git remote or URL") from exc
 
         change_result = {}
         selected_refs = []
 
         def update_refs(refs):
             from dulwich.objects import ZERO_SHA
@@ -906,15 +906,15 @@
     def validate_git_remote(self, url: str, **kwargs):
         from dulwich.client import LocalGitClient, get_transport_and_path
         from dulwich.porcelain import get_remote_repo
 
         try:
             _, location = get_remote_repo(self.repo, url)
             client, path = get_transport_and_path(location, **kwargs)
-        except Exception as exc:  # noqa: BLE001
+        except Exception as exc:
             raise InvalidRemote(url) from exc
         if isinstance(client, LocalGitClient) and not os.path.exists(
             os.path.join("", path)
         ):
             raise InvalidRemote(url)
 
     def get_remote_url(self, remote: str) -> str:
@@ -985,9 +985,9 @@
     from dulwich.client import HTTPUnauthorized
 
     try:
         refs = porcelain.ls_remote(url)
         return {os.fsdecode(ref): sha.decode("ascii") for ref, sha in refs.items()}
     except HTTPUnauthorized as exc:
         raise AuthError(url) from exc
-    except Exception as exc:  # noqa: BLE001
+    except Exception as exc:
         raise InvalidRemote(url) from exc
```

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/gitpython.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/filter.py` & `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/filter.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/config.py` & `scmrepo-3.3.3/src/scmrepo/git/config.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/credentials.py` & `scmrepo-3.3.3/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/client.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/fetch.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/fetch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import fnmatch
 import io
 import os
+import re
 from collections.abc import Iterable, Iterator
 from typing import TYPE_CHECKING, Callable, Optional
 
 from scmrepo.exceptions import InvalidRemote, SCMError
 
 from .pointer import HEADERS, Pointer
 
@@ -94,22 +95,43 @@
         except KeyError:
             pass
 
     # return default Git fetch URL for this remote
     return scm.get_remote_url(remote)
 
 
+_ROOT_PATH_PREFIX_REGEX = re.compile(r"^(?P<prefix>[^*?\[]*(?:/|$))")
+
+
 def _collect_objects(
     scm: "Git",
     rev: str,
     include: Optional[list[str]],
     exclude: Optional[list[str]],
 ) -> Iterator[Pointer]:
     fs = scm.get_fs(rev)
-    for path in _filter_paths(fs.find("/"), include, exclude):
+    # Optimize path filtering if the `include` list contains exactly one path.
+    # First, determine the root directory wherein to initiate the file search.
+    # If the `include` path is a Unix filename pattern, determine the static
+    # path prefix and set it as the root directory. Second, if the path and the
+    # root are identical or the Unix filename pattern matches *any* (i.e., `**`)
+    # file under the root directory, unset `include` to avoid unnecessary
+    # filtering work.
+    if (
+        include
+        and len(include) == 1
+        and (result := _ROOT_PATH_PREFIX_REGEX.match(path := include[0]))
+    ):
+        root = result.group("prefix")
+        if path in {root, f'{root.rstrip("/")}/**'}:
+            include = []
+    else:
+        root = "/"
+
+    for path in _filter_paths(fs.find(root), include, exclude):
         check_path = path.lstrip("/")
         if scm.check_attr(check_path, "filter", source=rev) == "lfs":
             try:
                 with fs.open(path, "rb", raw=True) as fobj:
                     with io.BufferedReader(fobj) as reader:
                         data = reader.peek(100)
                         if any(data.startswith(header) for header in HEADERS):
```

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/pointer.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/pointer.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/progress.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/smudge.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/smudge.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/lfs/storage.py` & `scmrepo-3.3.3/src/scmrepo/git/lfs/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         try:
             return open(path, **kwargs)  # noqa: SIM115
         except FileNotFoundError:
             if not fetch_url or not isinstance(obj, Pointer):
                 raise
         try:
             self.fetch(fetch_url, [obj], batch_size=batch_size)
-        except BaseException as exc:  # noqa: BLE001
+        except BaseException as exc:
             raise FileNotFoundError(
                 errno.ENOENT, os.strerror(errno.ENOENT), path
             ) from exc
         return open(path, **kwargs)  # noqa: SIM115
 
     def close(self):
         pass
```

### Comparing `scmrepo-3.3.2/src/scmrepo/git/objects.py` & `scmrepo-3.3.3/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/git/stash.py` & `scmrepo-3.3.3/src/scmrepo/git/stash.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Supports the same keyword arguments as apply().
         """
         logger.debug("Popping from stash '%s'", self.ref)
         ref = f"{self.ref}@{{0}}"
         rev = self.scm.resolve_rev(ref)
         try:
             self.apply(rev, **kwargs)
-        except Exception as exc:  # noqa: BLE001
+        except Exception as exc:
             raise SCMError("Could not apply stash commit") from exc
         self.drop()
         return rev
 
     def apply(
         self,
         rev: str,
```

### Comparing `scmrepo-3.3.2/src/scmrepo/progress.py` & `scmrepo-3.3.3/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/urls.py` & `scmrepo-3.3.3/src/scmrepo/urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo/utils.py` & `scmrepo-3.3.3/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-3.3.3/src/scmrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.2
+Version: 3.3.3
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,15 @@
 Requires-Dist: pytest-asyncio<1,>=0.23.2; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-docker<4,>=1; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-sugar; extra == "tests"
 Requires-Dist: pytest-test-utils<0.2,>=0.1.0; extra == "tests"
 Provides-Extra: dev
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: scmrepo[tests]; extra == "dev"
 Requires-Dist: types-certifi; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-paramiko; extra == "dev"
 Requires-Dist: types-tqdm; extra == "dev"
 
 scmrepo
```

### Comparing `scmrepo-3.3.2/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-3.3.3/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/conftest.py` & `scmrepo-3.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_credentials.py` & `scmrepo-3.3.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_dulwich.py` & `scmrepo-3.3.3/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_fs.py` & `scmrepo-3.3.3/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_git.py` & `scmrepo-3.3.3/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_lfs.py` & `scmrepo-3.3.3/tests/test_lfs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_noscm.py` & `scmrepo-3.3.3/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_pygit2.py` & `scmrepo-3.3.3/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_scmrepo.py` & `scmrepo-3.3.3/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_stash.py` & `scmrepo-3.3.3/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/test_urls.py` & `scmrepo-3.3.3/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/user.key` & `scmrepo-3.3.3/tests/user.key`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.2/tests/vendor/test_paramiko_vendor.py` & `scmrepo-3.3.3/tests/vendor/test_paramiko_vendor.py`

 * *Files identical despite different names*

