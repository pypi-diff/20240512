# Comparing `tmp/dekcli-0.1.8.tar.gz` & `tmp/dekcli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekcli-0.1.8.tar", last modified: Thu Mar  7 10:47:18 2024, max compression
+gzip compressed data, was "dekcli-0.1.9.tar", last modified: Fri Mar  8 19:06:30 2024, max compression
```

## Comparing `dekcli-0.1.8.tar` & `dekcli-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      321 2024-03-07 10:47:16.502333 dekcli-0.1.8/README.md
--rw-r--r--   0        0        0      732 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/__init__.py
--rw-r--r--   0        0        0      118 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/click/__entry__.py
--rw-r--r--   0        0        0       54 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/click/__init__.py
--rw-r--r--   0        0        0     3407 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/click/gitea.py
--rw-r--r--   0        0        0        0 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/core/git/__init__.py
--rw-r--r--   0        0        0     3891 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/core/git/giteaapi.py
--rw-r--r--   0        0        0      209 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/core/git/ref.py
--rw-r--r--   0        0        0     1513 2024-03-07 10:47:16.502333 dekcli-0.1.8/dekcli/core/git/repo.py
--rw-r--r--   0        0        0      488 2024-03-07 10:47:18.210343 dekcli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 dekcli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      321 2024-03-08 19:06:28.758065 dekcli-0.1.9/README.md
+-rw-r--r--   0        0        0      732 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/__init__.py
+-rw-r--r--   0        0        0      118 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/click/__entry__.py
+-rw-r--r--   0        0        0       54 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/click/__init__.py
+-rw-r--r--   0        0        0     3440 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/click/gitea.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/core/git/__init__.py
+-rw-r--r--   0        0        0     3891 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/core/git/giteaapi.py
+-rw-r--r--   0        0        0      209 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/core/git/ref.py
+-rw-r--r--   0        0        0     1513 2024-03-08 19:06:28.758065 dekcli-0.1.9/dekcli/core/git/repo.py
+-rw-r--r--   0        0        0      488 2024-03-08 19:06:30.822149 dekcli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 dekcli-0.1.9/PKG-INFO
```

### Comparing `dekcli-0.1.8/dekcli/__init__.py` & `dekcli-0.1.9/dekcli/__init__.py`

 * *Files identical despite different names*

### Comparing `dekcli-0.1.8/dekcli/click/gitea.py` & `dekcli-0.1.9/dekcli/click/gitea.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,13 +85,14 @@
                 repo = ors.get_or_create(org_name, repo_name, repo_data['branches'][0])
                 git_repo = git.Repo(repo_data['path'])
                 origin = git_repo.create_remote('origin', repo.ssh_url)
                 print(f"pushing: {repo.ssh_url}", flush=True)
                 for name in repo_data['branches']:
                     origin.push(refspec=f"{name}:{name}")
                 tags = repo_data['tags']
-                for tag in tags[:-1]:
+                for tag in tags[:-2]:
                     origin.push(tag)
                 if tags:
-                    time.sleep(1)
                     giteaapi.patch_repo(ins, org_name, repo_name, dict(has_actions=True))
-                    origin.push(tags[-1])
+                    time.sleep(1)
+                for tag in tags[-2:]:
+                    origin.push(tag)
```

### Comparing `dekcli-0.1.8/dekcli/core/git/giteaapi.py` & `dekcli-0.1.9/dekcli/core/git/giteaapi.py`

 * *Files identical despite different names*

### Comparing `dekcli-0.1.8/dekcli/core/git/repo.py` & `dekcli-0.1.9/dekcli/core/git/repo.py`

 * *Files identical despite different names*

### Comparing `dekcli-0.1.8/PKG-INFO` & `dekcli-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dekcli
-Version: 0.1.8
+Version: 0.1.9
 Author-Email: sanzenwin <sanzenwin@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: py-gitea<=0.2.8
 Requires-Dist: dektools<1.0.0
 Requires-Dist: GitPython<=3.1.41
 Description-Content-Type: text/markdown
```

