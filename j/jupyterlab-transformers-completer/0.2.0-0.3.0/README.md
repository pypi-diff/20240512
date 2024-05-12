# Comparing `tmp/jupyterlab_transformers_completer-0.2.0.tar.gz` & `tmp/jupyterlab_transformers_completer-0.3.0.tar.gz`

## Comparing `jupyterlab_transformers_completer-0.2.0.tar` & `jupyterlab_transformers_completer-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/.copier-answers.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/.gitmodules
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/install.json
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   258983 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/yarn.lock
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyter-config/server-config/jupyterlab_transformers_completer.json
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/_version.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/package.json
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/213.a1ad7d216eb96a92ae43.js
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/468.f0db1903cded82371272.js
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/747.82e78a8edf88647d214c.js
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/remoteEntry.803ed28d69af610a8e80.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/src/index.ts
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/src/models.ts
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/src/types.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/src/utils.ts
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/src/worker.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/style/index.js
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/LICENSE
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/README.md
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/.copier-answers.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/.gitmodules
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/install.json
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0   259295 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/yarn.lock
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyter-config/server-config/jupyterlab_transformers_completer.json
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/_version.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/package.json
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/213.e59dfc8de12e64063153.js
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/468.cb1c62bdaf01b682273e.js
+-rw-r--r--   0        0        0   894660 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/488.593a8bdbb534307f9db2.js
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/488.593a8bdbb534307f9db2.js.LICENSE.txt
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/747.82e78a8edf88647d214c.js
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/remoteEntry.c35f93a8e4c705cb30c5.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/style.js
+-rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15021 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/src/index.ts
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/src/models.ts
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/src/types.ts
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/src/utils.ts
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/src/worker.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/style/index.js
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/README.md
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 jupyterlab_transformers_completer-0.3.0/PKG-INFO
```

### Comparing `jupyterlab_transformers_completer-0.2.0/.copier-answers.yml` & `jupyterlab_transformers_completer-0.3.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/RELEASE.md` & `jupyterlab_transformers_completer-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/package.json` & `jupyterlab_transformers_completer-0.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444443%*

 * *Differences: {"'dependencies'": "{'@xenova/transformers': '~2.17.1'}", "'version'": "'0.3.0'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "bugs": {
         "url": "https://github.com/krassowski/jupyterlab-transformers-completer/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.1.0",
         "@jupyterlab/completer": "^4.1.0",
-        "@xenova/transformers": "~2.6.2"
+        "@xenova/transformers": "~2.17.1"
     },
     "description": "Inline completion provider using tranformers.js for JupyterLab.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
@@ -179,9 +179,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_transformers_completer-0.2.0/tsconfig.json` & `jupyterlab_transformers_completer-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/yarn.lock` & `jupyterlab_transformers_completer-0.3.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,21 @@
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
+"@huggingface/jinja@npm:^0.2.2":
+  version: 0.2.2
+  resolution: "@huggingface/jinja@npm:0.2.2"
+  checksum: 8a6e3e287863d437920990afa2ca25d83c51997bd5ba0325ea90633e52469c2d901178cbd758cc362b45ad1c9521fccf372884fd59e58d2916d6b2e5bb15f776
+  languageName: node
+  linkType: hard
+
 "@humanwhocodes/config-array@npm:^0.11.11":
   version: 0.11.11
   resolution: "@humanwhocodes/config-array@npm:0.11.11"
   dependencies:
     "@humanwhocodes/object-schema": ^1.2.1
     debug: ^4.1.1
     minimatch: ^3.0.5
@@ -898,15 +905,15 @@
     "@jupyterlab/application": ^4.1.0
     "@jupyterlab/builder": ^4.1.0
     "@jupyterlab/completer": ^4.1.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@typescript-eslint/eslint-plugin": ^6.1.0
     "@typescript-eslint/parser": ^6.1.0
-    "@xenova/transformers": ~2.6.2
+    "@xenova/transformers": ~2.17.1
     css-loader: ^6.7.1
     eslint: ^8.36.0
     eslint-config-prettier: ^8.8.0
     eslint-plugin-prettier: ^5.0.0
     npm-run-all: ^4.1.5
     prettier: ^3.0.0
     rimraf: ^5.0.1
@@ -1891,25 +1898,26 @@
   peerDependenciesMeta:
     webpack-dev-server:
       optional: true
   checksum: 75f0e54681796d567a71ac3e2781d2901a8d8cf1cdfc82f261034dddac59a8343e8c3bc5e32b4bb9d6766759ba49fb29a5cd86ef1701d79c506fe886bb63ac75
   languageName: node
   linkType: hard
 
-"@xenova/transformers@npm:~2.6.2":
-  version: 2.6.2
-  resolution: "@xenova/transformers@npm:2.6.2"
+"@xenova/transformers@npm:~2.17.1":
+  version: 2.17.1
+  resolution: "@xenova/transformers@npm:2.17.1"
   dependencies:
+    "@huggingface/jinja": ^0.2.2
     onnxruntime-node: 1.14.0
     onnxruntime-web: 1.14.0
     sharp: ^0.32.0
   dependenciesMeta:
     onnxruntime-node:
       optional: true
-  checksum: 025cd9b7fb6d281c9c58d08e0228236005d7733dc1b4855088178a9903124ace5aed92c2979d01325141f76bd9d267de519d3149dd67c824de300cf4366350c6
+  checksum: ff99a95268555d69bb67eb9ea494aced915c2de75973967f74bcc5fe0c7bd490bd3bb40a2906cd34007dcb4f5cb847ed3cde63beef25069f6af0e328fe3b23b6
   languageName: node
   linkType: hard
 
 "@xtuc/ieee754@npm:^1.2.0":
   version: 1.2.0
   resolution: "@xtuc/ieee754@npm:1.2.0"
   checksum: ac56d4ca6e17790f1b1677f978c0c6808b1900a5b138885d3da21732f62e30e8f0d9120fcf8f6edfff5100ca902b46f8dd7c1e3f903728634523981e80e2885a
@@ -6760,24 +6768,24 @@
     fast-fifo: ^1.2.0
     streamx: ^2.15.0
   checksum: f3627f918581976e954ff03cb8d370551053796b82564f8c7ca8fac84c48e4d042026d0854fc222171a34ff9c682b72fae91be9c9b0a112d4c54f9e4f443e9c5
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.2.0
-  resolution: "tar@npm:6.2.0"
+  version: 6.2.1
+  resolution: "tar@npm:6.2.1"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^5.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
-  checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
+  checksum: f1322768c9741a25356c11373bce918483f40fa9a25c69c59410c8a1247632487edef5fe76c5f12ac51a6356d2f1829e96d2bc34098668a2fc34d76050ac2b6c
   languageName: node
   linkType: hard
 
 "terser-webpack-plugin@npm:^5.3.7":
   version: 5.3.9
   resolution: "terser-webpack-plugin@npm:5.3.9"
   dependencies:
```

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/__init__.py` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/package.json` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9751157407407406%*

 * *Differences: {"'dependencies'": "{'@xenova/transformers': '~2.17.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c35f93a8e4c705cb30c5.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "bugs": {
         "url": "https://github.com/krassowski/jupyterlab-transformers-completer/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.1.0",
         "@jupyterlab/completer": "^4.1.0",
-        "@xenova/transformers": "~2.6.2"
+        "@xenova/transformers": "~2.17.1"
     },
     "description": "Inline completion provider using tranformers.js for JupyterLab.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
@@ -100,15 +100,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/krassowski/jupyterlab-transformers-completer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.803ed28d69af610a8e80.js",
+            "load": "static/remoteEntry.c35f93a8e4c705cb30c5.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_transformers_completer/labextension"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/213.a1ad7d216eb96a92ae43.js` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/213.e59dfc8de12e64063153.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 (() => {
     "use strict";
-    var e, t, s, r, o = {
-            213: (e, t, s) => {
-                s.a(e, (async (e, t) => {
+    var e, t, r, o, s, n, a = {
+            213: (e, t, r) => {
+                r.a(e, (async (e, t) => {
                     try {
-                        const e = await import("https://cdn.jsdelivr.net/npm/@xenova/transformers@2.6.2");
-                        class s {
+                        const e = await r(488);
+                        class o {
                             constructor() {
                                 this._sharedArray = null, this._completionModels = new Map
                             }
                             async handleMessage(e) {
                                 const t = e.data;
                                 switch (t.action) {
                                     case "generate":
@@ -25,183 +25,241 @@
                                     default:
                                         console.error("Unhandled message", e)
                                 }
                             }
                             async _generate(e) {
                                 const {
                                     model: t,
-                                    text: s,
-                                    idTokens: r,
-                                    counter: o
+                                    text: r,
+                                    idTokens: o,
+                                    counter: s
                                 } = e, n = this._sharedArray;
                                 if (null === n) throw Error("Cannot generate before `initializeBuffer` message got processed");
                                 const a = this._initializeModel({
                                         model: t
                                     }),
                                     i = await a.instance;
-                                if (n[0] !== o) return void console.log("Skipping generation because new request was sent since");
+                                if (n[0] !== s) return void console.log("Skipping generation because new request was sent since");
                                 let l = [];
                                 try {
-                                    l = await i(s, {
+                                    l = await i(r, {
                                         max_new_tokens: e.maxNewTokens,
                                         temperature: e.temperature,
                                         top_k: e.topK,
                                         do_sample: e.doSample,
                                         num_beams: e.generateN,
                                         num_return_sequences: e.generateN,
                                         repetition_penalty: e.repetitionPenalty,
                                         diversity_penalty: e.diversityPenalty,
                                         num_beam_groups: e.generateN,
                                         callback_function: e => {
-                                            if (n[0] !== o) throw Error("Execution interrupted");
+                                            if (n[0] !== s) throw Error("Execution interrupted");
                                             for (let t = 0; t < e.length; t++) {
-                                                const o = i.tokenizer.decode(e[t].output_token_ids, {
+                                                const s = i.tokenizer.decode(e[t].output_token_ids, {
                                                     skip_special_tokens: !0
                                                 });
                                                 self.postMessage({
                                                     status: "update",
-                                                    output: o.substring(s.length),
-                                                    idToken: r[t]
+                                                    output: s.substring(r.length),
+                                                    idToken: o[t]
                                                 })
                                             }
                                         }
                                     })
                                 } catch (e) {
                                     const t = {
                                         error: {
                                             message: e.message
                                         },
-                                        idTokens: r
+                                        idTokens: o
                                     };
                                     "Execution interrupted" === e.message ? self.postMessage({
                                         status: "interrupted",
                                         ...t
                                     }) : self.postMessage({
                                         status: "exception",
                                         ...t
                                     })
                                 }
                                 for (let e = 0; e < l.length; e++) self.postMessage({
                                     status: "complete",
-                                    output: l[e].generated_text.substring(s.length),
-                                    idToken: r[e]
+                                    output: l[e].generated_text.substring(r.length),
+                                    idToken: o[e]
                                 })
                             }
                             _initializeModel(e) {
                                 let t = this._completionModels.get(e.model);
-                                return t || (t = new r({
+                                return t || (t = new s({
                                     model: e.model,
                                     onLoadingProgress: t => {
                                         self.postMessage({
                                             ...t,
                                             model: e.model
                                         })
                                     }
                                 }), this._completionModels.set(e.model, t), t)
                             }
                             _configure(t) {
-                                e.env.allowLocalModels = t.allowLocalModels
+                                e.env.allowLocalModels = t.allowLocalModels, e.env.allowRemoteModels = t.allowRemoteModels, e.env.localModelPath = t.localModelPath, e.env.remoteHost = t.remoteHost
                             }
                             _initializeBuffer(e) {
                                 this._sharedArray = new Int32Array(e.buffer)
                             }
                             _disposeModel(e) {
                                 const t = this._completionModels.get(e.model);
                                 if (t) return this._completionModels.delete(e.model), t.dispose()
                             }
                         }
-                        class r {
+                        class s {
                             constructor(t) {
                                 this._task = "text-generation", this._model = t.model, this._instance = e.pipeline(this._task, this._model, {
                                     progress_callback: e => {
                                         t.onLoadingProgress(e)
                                     }
                                 })
                             }
                             get instance() {
                                 return this._instance
                             }
                             async dispose() {
                                 (await this._instance).dispose()
                             }
                         }
-                        const o = new s;
-                        self.addEventListener("message", o.handleMessage.bind(o)), self.postMessage({
+                        const n = new o;
+                        self.addEventListener("message", n.handleMessage.bind(n)), self.postMessage({
                             status: "worker-started"
                         }), t()
                     } catch (e) {
                         t(e)
                     }
                 }), 1)
             }
         },
-        n = {};
+        i = {};
 
-    function a(e) {
-        var t = n[e];
+    function l(e) {
+        var t = i[e];
         if (void 0 !== t) return t.exports;
-        var s = n[e] = {
+        var r = i[e] = {
             exports: {}
         };
-        return o[e](s, s.exports, a), s.exports
+        return a[e](r, r.exports, l), r.exports
     }
-    a.m = o, a.c = n, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", t = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", s = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", r = e => {
+    l.m = a, l.c = i, l.x = () => {
+        var e = l.O(void 0, [488], (() => l(213)));
+        return l.O(e)
+    }, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", t = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", r = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", o = e => {
         e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
-    }, a.a = (o, n, a) => {
+    }, l.a = (s, n, a) => {
         var i;
         a && ((i = []).d = -1);
-        var l, c, d, p = new Set,
-            u = o.exports,
-            _ = new Promise(((e, t) => {
-                d = t, c = e
+        var l, c, p, u = new Set,
+            d = s.exports,
+            f = new Promise(((e, t) => {
+                p = t, c = e
             }));
-        _[t] = u, _[e] = e => (i && e(i), p.forEach(e), _.catch((e => {}))), o.exports = _, n((o => {
+        f[t] = d, f[e] = e => (i && e(i), u.forEach(e), f.catch((e => {}))), s.exports = f, n((s => {
             var n;
-            l = (o => o.map((o => {
-                if (null !== o && "object" == typeof o) {
-                    if (o[e]) return o;
-                    if (o.then) {
+            l = (s => s.map((s => {
+                if (null !== s && "object" == typeof s) {
+                    if (s[e]) return s;
+                    if (s.then) {
                         var n = [];
-                        n.d = 0, o.then((e => {
-                            a[t] = e, r(n)
+                        n.d = 0, s.then((e => {
+                            a[t] = e, o(n)
                         }), (e => {
-                            a[s] = e, r(n)
+                            a[r] = e, o(n)
                         }));
                         var a = {};
                         return a[e] = e => e(n), a
                     }
                 }
                 var i = {};
-                return i[e] = e => {}, i[t] = o, i
-            })))(o);
+                return i[e] = e => {}, i[t] = s, i
+            })))(s);
             var a = () => l.map((e => {
-                    if (e[s]) throw e[s];
+                    if (e[r]) throw e[r];
                     return e[t]
                 })),
                 c = new Promise((t => {
                     (n = () => t(a)).r = 0;
-                    var s = e => e !== i && !p.has(e) && (p.add(e), e && !e.d && (n.r++, e.push(n)));
-                    l.map((t => t[e](s)))
+                    var r = e => e !== i && !u.has(e) && (u.add(e), e && !e.d && (n.r++, e.push(n)));
+                    l.map((t => t[e](r)))
                 }));
             return n.r ? c : a()
-        }), (e => (e ? d(_[s] = e) : c(u), r(i)))), i && i.d < 0 && (i.d = 0)
-    }, a.d = (e, t) => {
-        for (var s in t) a.o(t, s) && !a.o(e, s) && Object.defineProperty(e, s, {
+        }), (e => (e ? p(f[r] = e) : c(d), o(i)))), i && i.d < 0 && (i.d = 0)
+    }, s = [], l.O = (e, t, r, o) => {
+        if (!t) {
+            var n = 1 / 0;
+            for (p = 0; p < s.length; p++) {
+                for (var [t, r, o] = s[p], a = !0, i = 0; i < t.length; i++)(!1 & o || n >= o) && Object.keys(l.O).every((e => l.O[e](t[i]))) ? t.splice(i--, 1) : (a = !1, o < n && (n = o));
+                if (a) {
+                    s.splice(p--, 1);
+                    var c = r();
+                    void 0 !== c && (e = c)
+                }
+            }
+            return e
+        }
+        o = o || 0;
+        for (var p = s.length; p > 0 && s[p - 1][2] > o; p--) s[p] = s[p - 1];
+        s[p] = [t, r, o]
+    }, l.d = (e, t) => {
+        for (var r in t) l.o(t, r) && !l.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
-            get: t[s]
+            get: t[r]
         })
-    }, a.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), (() => {
-        a.S = {};
+    }, l.f = {}, l.e = e => Promise.all(Object.keys(l.f).reduce(((t, r) => (l.f[r](e, t), t)), [])), l.u = e => e + ".593a8bdbb534307f9db2.js?v=593a8bdbb534307f9db2", l.g = function() {
+        if ("object" == typeof globalThis) return globalThis;
+        try {
+            return this || new Function("return this")()
+        } catch (e) {
+            if ("object" == typeof window) return window
+        }
+    }(), l.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), l.r = e => {
+        "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
+            value: "Module"
+        }), Object.defineProperty(e, "__esModule", {
+            value: !0
+        })
+    }, (() => {
+        l.S = {};
         var e = {},
             t = {};
-        a.I = (s, r) => {
-            r || (r = []);
-            var o = t[s];
-            if (o || (o = t[s] = {}), !(r.indexOf(o) >= 0)) {
-                if (r.push(o), e[s]) return e[s];
-                a.o(a.S, s) || (a.S[s] = {}), a.S[s];
+        l.I = (r, o) => {
+            o || (o = []);
+            var s = t[r];
+            if (s || (s = t[r] = {}), !(o.indexOf(s) >= 0)) {
+                if (o.push(s), e[r]) return e[r];
+                l.o(l.S, r) || (l.S[r] = {}), l.S[r];
                 var n = [];
-                return e[s] = n.length ? Promise.all(n).then((() => e[s] = 1)) : 1
+                return e[r] = n.length ? Promise.all(n).then((() => e[r] = 1)) : 1
             }
         }
-    })(), a(213)
+    })(), (() => {
+        var e;
+        l.g.importScripts && (e = l.g.location + "");
+        var t = l.g.document;
+        if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
+            var r = t.getElementsByTagName("script");
+            if (r.length)
+                for (var o = r.length - 1; o > -1 && !e;) e = r[o--].src
+        }
+        if (!e) throw new Error("Automatic publicPath is not supported in this browser");
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), l.p = e
+    })(), (() => {
+        var e = {
+            213: 1
+        };
+        l.f.i = (t, r) => {
+            e[t] || importScripts(l.p + l.u(t))
+        };
+        var t = self.webpackChunk_jupyterlab_transformers_completer = self.webpackChunk_jupyterlab_transformers_completer || [],
+            r = t.push.bind(t);
+        t.push = t => {
+            var [o, s, n] = t;
+            for (var a in s) l.o(s, a) && (l.m[a] = s[a]);
+            for (n && n(l); o.length;) e[o.pop()] = 1;
+            r(t)
+        }
+    })(), n = l.x, l.x = () => l.e(488).then(n), l.x()
 })();
```

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/468.f0db1903cded82371272.js` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/468.cb1c62bdaf01b682273e.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_jupyterlab_transformers_completer = self.webpackChunk_jupyterlab_transformers_completer || []).push([
     [468], {
         468: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => m
             });
-            var s = o(501),
-                i = o(870),
+            var s = o(138),
+                i = o(712),
                 r = o(930);
 
             function n(e, t = 2, o = 1024) {
                 if (0 === e) return "0 B";
                 const s = t,
                     i = ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"],
                     r = Math.floor(Math.log(e) / Math.log(o));
@@ -34,15 +34,15 @@
                     repo: "Xenova/WizardCoder-1B-V1.0",
                     licence: "bigcode-openrail-m",
                     humanEval: 23.8
                 }, {
                     repo: "Xenova/J-350M",
                     licence: "bsd-3-clause"
                 }],
-                c = [{
+                l = [{
                     repo: "Xenova/gpt2",
                     licence: "mit"
                 }, {
                     repo: "Xenova/TinyLLama-v0",
                     licence: "apache-2.0"
                 }, {
                     repo: "Xenova/dlite-v2-774m",
@@ -67,30 +67,40 @@
                     licence: "apache-2.0"
                 }, {
                     repo: "Xenova/distilgpt2",
                     licence: "apache-2.0"
                 }, {
                     repo: "Xenova/llama-160m",
                     licence: "other"
+                }, {
+                    repo: "Xenova/Qwen1.5-0.5B-Chat",
+                    licence: "tongyi-qianwen-research"
+                }, {
+                    repo: "Xenova/bloom-560m",
+                    licence: "bigscience-bloom-rail-1.0"
                 }],
-                l = {
+                d = {
                     codeModel: "Xenova/tiny_starcoder_py",
                     textModel: "Xenova/gpt2",
                     temperature: .5,
                     doSample: !1,
                     topK: 5,
                     maxNewTokens: 50,
                     generateN: 2,
                     maxContextWindow: 512,
                     diversityPenalty: 1,
-                    repetitionPenalty: 1
+                    repetitionPenalty: 1,
+                    allowLocalModels: !1,
+                    allowRemoteModels: !0,
+                    remoteHost: "https://huggingface.co/",
+                    localModelPath: "/models/"
                 };
-            class d {
+            class c {
                 constructor(e) {
-                    this.options = e, this.identifier = "@krassowski/inline-completer", this.name = "Transformers powered completions", this._currentGeneration = 0, this._currentModels = {}, this._loadingNotifications = {}, this._ready = {}, this._settings = l, this._streamPromises = new Map, this._tokenCounter = 0, this._workerStarted = new r.PromiseDelegate;
+                    this.options = e, this.identifier = "@krassowski/inline-completer", this.name = "Transformers powered completions", this._currentGeneration = 0, this._currentModels = {}, this._loadingNotifications = {}, this._ready = {}, this._settings = d, this._streamPromises = new Map, this._tokenCounter = 0, this._workerStarted = new r.PromiseDelegate;
                     try {
                         SharedArrayBuffer
                     } catch (e) {
                         (0, i.showErrorMessage)("SharedArrayBuffer not available", "Server extension enabling `same-origin` and `require-corp` headers is required for jupyterlab-transformers-completer to access `SharedArrayBuffer` which is used to synchronously communicate with the language model WebWorker.")
                     }
                     const t = new SharedArrayBuffer(1024);
                     this._sharedArray = new Int32Array(t), e.worker.addEventListener("message", this._onMessageReceived.bind(this)), this._workerStarted.promise.then((() => {
@@ -114,15 +124,15 @@
                             },
                             textModel: {
                                 title: "Text model",
                                 description: "Model used in Markdown (cells and files) and plain text files.",
                                 oneOf: [{
                                     const: "none",
                                     title: "No model"
-                                }, ...c.map(this._formatModelOptions)],
+                                }, ...l.map(this._formatModelOptions)],
                                 type: "string"
                             },
                             temperature: {
                                 minimum: 0,
                                 maximum: 1,
                                 type: "number",
                                 title: "Temperature",
@@ -163,21 +173,50 @@
                                 description: "1.0 means not penalty."
                             },
                             maxContextWindow: {
                                 title: "Context window",
                                 minimum: 1,
                                 type: "number",
                                 description: "At most how many characters should be provided to the model. Smaller context results in faster generation at a cost of less accurate suggestions."
+                            },
+                            allowLocalModels: {
+                                type: "boolean",
+                                title: "Check Local Model Database",
+                                default: !1,
+                                description: "Whether to allow downloading models from local database of models. If set to false (default) the models will be downloaded from remote host."
+                            },
+                            allowRemoteModels: {
+                                type: "boolean",
+                                title: "Check Remote Model Database",
+                                default: !0,
+                                description: "Whether to allow downloading models from remote database of models."
+                            },
+                            localModelPath: {
+                                type: "string",
+                                title: "Local Model Database Path",
+                                default: "/models/"
+                            },
+                            remoteHost: {
+                                type: "string",
+                                title: "Remote Host",
+                                description: "The remote host from which to download the models.",
+                                default: "https://huggingface.co/"
                             }
                         },
-                        default: l
+                        default: d
                     }
                 }
                 async configure(e) {
-                    this._settings = e, await this._workerStarted.promise, this._switchModel(this._settings.codeModel, "code"), this._switchModel(this._settings.textModel, "text")
+                    this._settings = e, await this._workerStarted.promise, this._postMessage({
+                        action: "configure",
+                        allowLocalModels: this._settings.allowLocalModels,
+                        allowRemoteModels: this._settings.allowRemoteModels,
+                        localModelPath: this._settings.localModelPath,
+                        remoteHost: this._settings.remoteHost
+                    }), this._switchModel(this._settings.codeModel, "code"), this._switchModel(this._settings.textModel, "text")
                 }
                 async fetch(e, t) {
                     const o = ["text/x-ipythongfm", "text/x-markdown", "text/plain", "text/x-rst", "text/x-latex", "text/x-rsrc"].includes(e.mimeType) ? this._settings.textModel : this._settings.codeModel;
                     await this._ready[o].promise, this._abortPrevious(), this._streamPromises = new Map;
                     const s = this._prefixFromRequest(e),
                         i = [],
                         r = [];
@@ -345,15 +384,15 @@
             const m = {
                 id: "@jupyterlab/transformers-completer:plugin",
                 description: "An in-browser AI completion provider for JupyterLab.",
                 requires: [s.ICompletionProviderManager],
                 autoStart: !0,
                 activate: (e, t) => {
                     const s = new Worker(new URL(o.p + o.u(213), o.b)),
-                        i = new d({
+                        i = new c({
                             worker: s
                         });
                     t.registerInlineProvider(i)
                 }
             }
         }
     }
```

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/747.82e78a8edf88647d214c.js` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/747.82e78a8edf88647d214c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/jupyterlab_transformers_completer/labextension/static/remoteEntry.803ed28d69af610a8e80.js` & `jupyterlab_transformers_completer-0.3.0/jupyterlab_transformers_completer/labextension/static/remoteEntry.c35f93a8e4c705cb30c5.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, p, d, c, h, v, m = {
+    var e, r, t, n, o, a, i, u, l, f, s, p, c, d, h, v, m = {
             93: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(468).then((() => () => t(468))),
                         "./extension": () => t.e(468).then((() => () => t(468))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,47 +43,47 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        213: "a1ad7d216eb96a92ae43",
-        468: "f0db1903cded82371272",
+        213: "e59dfc8de12e64063153",
+        468: "cb1c62bdaf01b682273e",
         747: "82e78a8edf88647d214c"
     } [e] + ".js?v=" + {
-        213: "a1ad7d216eb96a92ae43",
-        468: "f0db1903cded82371272",
+        213: "e59dfc8de12e64063153",
+        468: "cb1c62bdaf01b682273e",
         747: "82e78a8edf88647d214c"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/transformers-completer:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                c = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -108,15 +108,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(468).then((() => () => g(468))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab/transformers-completer", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@jupyterlab/transformers-completer", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,79 +166,79 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, p = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !o : "" == p != o);
-                if ("u" == f) {
+                var f, s, p = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == p ? u > n && !o : "" == p != o);
+                if ("u" == s) {
                     if (!l || "u" != p) return !1
                 } else if (l)
-                    if (p == f)
+                    if (p == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != p && "n" != p) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < p != o) return !1;
+                    if (u <= n || s < p != o) return !1;
                     l = !1
                 } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var c = [],
+            d = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
         }
-        return !!c()
+        return !!d()
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), p(e[t][o])
-    }, f = e => {
+        return a(n, o) || s(l(e, t, o, n)), p(e[t][o])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), c = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
-        501: () => d("default", "@jupyterlab/completer", [1, 4, 1, 4]),
-        870: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 4]),
-        930: () => d("default", "@lumino/coreutils", [1, 2, 0, 0])
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), d = {}, h = {
+        138: () => c("default", "@jupyterlab/completer", [1, 4, 2, 0]),
+        712: () => c("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        930: () => c("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, v = {
-        468: [501, 870, 930]
+        468: [138, 712, 930]
     }, g.f.consumes = (e, r) => {
         g.o(v, e) && v[e].forEach((e => {
-            if (g.o(c, e)) return r.push(c[e]);
+            if (g.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    c[e] = 0, g.m[e] = t => {
+                    d[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], g.m[e] = t => {
+                    delete d[e], g.m[e] = t => {
                         throw delete g.c[e], r
                     }
                 };
             try {
                 var o = h[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         g.b = document.baseURI || self.location.href;
         var e = {
```

### Comparing `jupyterlab_transformers_completer-0.2.0/src/index.ts` & `jupyterlab_transformers_completer-0.3.0/src/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,24 @@
   CompletionHandler,
   IInlineCompletionList,
   IInlineCompletionItem
 } from '@jupyterlab/completer';
 import type { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { Notification, showErrorMessage } from '@jupyterlab/apputils';
 import { JSONValue, PromiseDelegate } from '@lumino/coreutils';
-import type { ClientMessage, WorkerMessage, IModelSettings } from './types';
+import type {
+  ClientMessage,
+  WorkerMessage,
+  IModelSettings,
+  ITransformersSettings
+} from './types';
 import { formatFileSize } from './utils';
 import { IModelInfo, codeModels, textModels } from './models';
 
-interface ISettings extends IModelSettings {
+interface ISettings extends IModelSettings, ITransformersSettings {
   codeModel: string;
   textModel: string;
   maxContextWindow: number;
 }
 
 const DEFAULT_SETTINGS: ISettings = {
   codeModel: 'Xenova/tiny_starcoder_py',
@@ -29,15 +34,19 @@
   temperature: 0.5,
   doSample: false,
   topK: 5,
   maxNewTokens: 50,
   generateN: 2,
   maxContextWindow: 512,
   diversityPenalty: 1,
-  repetitionPenalty: 1
+  repetitionPenalty: 1,
+  allowLocalModels: false,
+  allowRemoteModels: true,
+  remoteHost: 'https://huggingface.co/',
+  localModelPath: '/models/'
 };
 
 class TransformersInlineProvider implements IInlineCompletionProvider {
   readonly identifier = '@krassowski/inline-completer';
   readonly name = 'Transformers powered completions';
 
   constructor(protected options: TransformersInlineProvider.IOptions) {
@@ -132,23 +141,55 @@
         // Words could be better but can be over-optimistic - one word can be several tokens).
         maxContextWindow: {
           title: 'Context window',
           minimum: 1,
           type: 'number',
           description:
             'At most how many characters should be provided to the model. Smaller context results in faster generation at a cost of less accurate suggestions.'
+        },
+        allowLocalModels: {
+          type: 'boolean',
+          title: 'Check Local Model Database',
+          default: false,
+          description:
+            'Whether to allow downloading models from local database of models. If set to false (default) the models will be downloaded from remote host.'
+        },
+        allowRemoteModels: {
+          type: 'boolean',
+          title: 'Check Remote Model Database',
+          default: true,
+          description:
+            'Whether to allow downloading models from remote database of models.'
+        },
+        localModelPath: {
+          type: 'string',
+          title: 'Local Model Database Path',
+          default: '/models/'
+        },
+        remoteHost: {
+          type: 'string',
+          title: 'Remote Host',
+          description: 'The remote host from which to download the models.',
+          default: 'https://huggingface.co/'
         }
       },
       default: DEFAULT_SETTINGS as any
     };
   }
 
   async configure(settings: { [property: string]: JSONValue }): Promise<void> {
     this._settings = settings as any as ISettings;
     await this._workerStarted.promise;
+    this._postMessage({
+      action: 'configure',
+      allowLocalModels: this._settings.allowLocalModels,
+      allowRemoteModels: this._settings.allowRemoteModels,
+      localModelPath: this._settings.localModelPath,
+      remoteHost: this._settings.remoteHost
+    });
     this._switchModel(this._settings.codeModel, 'code');
     this._switchModel(this._settings.textModel, 'text');
   }
 
   async fetch(
     request: CompletionHandler.IRequest,
     context: IInlineCompletionContext
```

### Comparing `jupyterlab_transformers_completer-0.2.0/src/models.ts` & `jupyterlab_transformers_completer-0.3.0/src/models.ts`

 * *Files 12% similar despite different names*

```diff
@@ -78,9 +78,17 @@
   {
     repo: 'Xenova/distilgpt2',
     licence: 'apache-2.0'
   },
   {
     repo: 'Xenova/llama-160m',
     licence: 'other'
+  },
+  {
+    repo: 'Xenova/Qwen1.5-0.5B-Chat',
+    licence: 'tongyi-qianwen-research'
+  },
+  {
+    repo: 'Xenova/bloom-560m',
+    licence: 'bigscience-bloom-rail-1.0'
   }
 ];
```

### Comparing `jupyterlab_transformers_completer-0.2.0/src/types.ts` & `jupyterlab_transformers_completer-0.3.0/src/types.ts`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,24 @@
   doSample: boolean;
   repetitionPenalty: number;
   diversityPenalty: number;
   // this a default for `num_return_sequences`, `num_beams` and `num_beam_groups`.
   generateN: number;
 }
 
+export interface ITransformersSettings {
+  allowLocalModels: (typeof env)['allowLocalModels'];
+  allowRemoteModels: (typeof env)['allowRemoteModels'];
+  remoteHost: (typeof env)['remoteHost'];
+  localModelPath: (typeof env)['localModelPath'];
+}
+
 export namespace ClientMessage {
-  export interface IConfigure {
+  export interface IConfigure extends ITransformersSettings {
     action: 'configure';
-    allowLocalModels: (typeof env)['allowLocalModels'];
-    allowRemoteModels: (typeof env)['allowRemoteModels'];
-    remoteHost: (typeof env)['remoteHost'];
-    localModelPath: (typeof env)['localModelPath'];
   }
   export interface IInitializeBuffer {
     action: 'initializeBuffer';
     buffer: SharedArrayBuffer;
   }
   export interface IInitializeModel {
     action: 'initializeModel';
```

### Comparing `jupyterlab_transformers_completer-0.2.0/src/utils.ts` & `jupyterlab_transformers_completer-0.3.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/src/worker.ts` & `jupyterlab_transformers_completer-0.3.0/src/worker.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 import type { Pipeline } from '@xenova/transformers';
 import type {
   transformersModule,
   ClientMessage as Message,
   WorkerMessage
 } from './types';
 
-// Note: neither importScripts nor module import worked, see:
-// https://github.com/webpack/webpack/issues/16633
-// https://github.com/webpack/webpack/issues/16173
-// https://github.com/jupyterlab/jupyterlab/issues/10197
-const transformers = (await import(
-  /* webpackIgnore: true */
-  // eslint-disable-next-line @typescript-eslint/ban-ts-comment
-  // @ts-ignore
-  'https://cdn.jsdelivr.net/npm/@xenova/transformers@2.6.2'
-)) as transformersModule;
+const transformers = await require('@xenova/transformers/dist/transformers');
 
 class Worker {
   async handleMessage(event: MessageEvent) {
     const data = event.data;
     switch (data.action) {
       case 'generate':
         return this._generate(data as Message.IGenerate);
@@ -133,15 +124,21 @@
     });
     this._completionModels.set(data.model, model);
     return model;
   }
 
   private _configure(data: Message.IConfigure) {
     // Allow to download the model from the hub.
-    transformers.env.allowLocalModels = data.allowLocalModels;
+    (transformers as transformersModule).env.allowLocalModels =
+      data.allowLocalModels;
+    (transformers as transformersModule).env.allowRemoteModels =
+      data.allowRemoteModels;
+    (transformers as transformersModule).env.localModelPath =
+      data.localModelPath;
+    (transformers as transformersModule).env.remoteHost = data.remoteHost;
   }
 
   private _initializeBuffer(data: Message.IInitializeBuffer) {
     this._sharedArray = new Int32Array(data.buffer);
   }
 
   private _disposeModel(data: Message.IDisposeModel) {
```

### Comparing `jupyterlab_transformers_completer-0.2.0/.gitignore` & `jupyterlab_transformers_completer-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/LICENSE` & `jupyterlab_transformers_completer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_transformers_completer-0.2.0/README.md` & `jupyterlab_transformers_completer-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 # jupyterlab-transformers-completer
 
 [![Extension status](https://img.shields.io/badge/status-experimental-red 'not ready to be used')](https://jupyterlab-contrib.github.io/)
-[![Github Actions Status](https://github.com/krassowski/jupyterlab-transformers-completer/workflows/Build/badge.svg)](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml)
+[![Build](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml/badge.svg)](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/krassowski/jupyterlab-transformers-completer/main?urlpath=lab)
 
 Inline completion provider using `transformers.js` for JupyterLab
 
-This extension is currently aimed for developers of JupyterLab extensions (and advanced JupyterLab users) to explore the proof of concept integration of the new inline completions API added in JupyterLab 4.1.
+This extension is aimed for developers of JupyterLab extensions (and advanced JupyterLab users) to explore the integration of the inline completions API added in JupyterLab 4.1.
 
 All models linked from this demonstration run exclusively **in your browser**, and are:
 
 - order of magnitudes smaller than the state-of-the-art models,
 - producing correspondingly lower accuracy of suggestions/answers.
 
 These models are not vetted for accuracy nor propriety and should not be deployed without further validation.
 
 ![demo-transformers](https://github.com/krassowski/jupyterlab-transformers-completer/assets/5832902/c81ca9c1-925d-498d-8650-520f8a570f99)
 
+### Usage
+
+1. Go to Settings → Inline Completer → choose the models for code (in code cells and scripts) and text (in markdown cells and plain files) generation.
+2. The models will be downloaded, compiled, and cached in your browser as indicated by pop-up notifications in bottom right corner.
+3. Start typing a few words in the code cell or Markdown cell and observe the suggestions; hover over to see shortcuts.
+4. Adjust model configuration in settings as needed; in particular increasing the repetition penalty, adjusting temperature and top _k_ is recommended.
+
+### Known issues
+
+- Sometimes it is required to go to settings after installation and modify settings to trigger model download and compilation
+- Sometimes the browser will cache a faulty (e.g not fully downloaded) file resulting in Syntax Error when parsing; you can try in an incognito/private mode to confirm that this is transient and clear browser cache to remove such file.
+
 ## Requirements
 
 - JupyterLab >= 4.1.0 or Jupyter Notebook >= 7.1.0
 - A browser supporting:
   - [`SharedArrayBuffer`](https://caniuse.com/sharedarraybuffer)
   - [Web Workers](https://caniuse.com/webworkers)
   - Dynamic import for workers (behind `dom.workers.modules.enabled` in Firefox)
@@ -39,15 +51,15 @@
 ```
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install -U 'jupyterlab>=4.1.0a3' jupyterlab-transformers-completer
+pip install -U 'jupyterlab>=4.1.0' jupyterlab-transformers-completer
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jupyterlab_transformers_completer-0.2.0/pyproject.toml` & `jupyterlab_transformers_completer-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=4.1.0,<5", "hatch-nodejs-version>=0.3.2"]
+requires = [
+    "hatchling>=1.5.0",
+    "jupyterlab>=4.1.0,<5",
+    "hatch-nodejs-version>=0.3.2"
+]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab-transformers-completer"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `jupyterlab_transformers_completer-0.2.0/PKG-INFO` & `jupyterlab_transformers_completer-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab-transformers-completer
-Version: 0.2.0
+Version: 0.3.0
+Dynamic: Keywords
 Summary: Inline completion provider using tranformers.js for JupyterLab.
 Project-URL: Homepage, https://github.com/krassowski/jupyterlab-transformers-completer
 Project-URL: Bug Tracker, https://github.com/krassowski/jupyterlab-transformers-completer/issues
 Project-URL: Repository, https://github.com/krassowski/jupyterlab-transformers-completer.git
 Author-email: Michał Krassowski <mkrassowski@quansight.com>
 License: BSD 3-Clause License
         
@@ -52,30 +53,42 @@
 Requires-Dist: jupyterlab-server>=2.25.2
 Requires-Dist: jupyterlab<5,>=4.1.0
 Description-Content-Type: text/markdown
 
 # jupyterlab-transformers-completer
 
 [![Extension status](https://img.shields.io/badge/status-experimental-red 'not ready to be used')](https://jupyterlab-contrib.github.io/)
-[![Github Actions Status](https://github.com/krassowski/jupyterlab-transformers-completer/workflows/Build/badge.svg)](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml)
+[![Build](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml/badge.svg)](https://github.com/krassowski/jupyterlab-transformers-completer/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/krassowski/jupyterlab-transformers-completer/main?urlpath=lab)
 
 Inline completion provider using `transformers.js` for JupyterLab
 
-This extension is currently aimed for developers of JupyterLab extensions (and advanced JupyterLab users) to explore the proof of concept integration of the new inline completions API added in JupyterLab 4.1.
+This extension is aimed for developers of JupyterLab extensions (and advanced JupyterLab users) to explore the integration of the inline completions API added in JupyterLab 4.1.
 
 All models linked from this demonstration run exclusively **in your browser**, and are:
 
 - order of magnitudes smaller than the state-of-the-art models,
 - producing correspondingly lower accuracy of suggestions/answers.
 
 These models are not vetted for accuracy nor propriety and should not be deployed without further validation.
 
 ![demo-transformers](https://github.com/krassowski/jupyterlab-transformers-completer/assets/5832902/c81ca9c1-925d-498d-8650-520f8a570f99)
 
+### Usage
+
+1. Go to Settings → Inline Completer → choose the models for code (in code cells and scripts) and text (in markdown cells and plain files) generation.
+2. The models will be downloaded, compiled, and cached in your browser as indicated by pop-up notifications in bottom right corner.
+3. Start typing a few words in the code cell or Markdown cell and observe the suggestions; hover over to see shortcuts.
+4. Adjust model configuration in settings as needed; in particular increasing the repetition penalty, adjusting temperature and top _k_ is recommended.
+
+### Known issues
+
+- Sometimes it is required to go to settings after installation and modify settings to trigger model download and compilation
+- Sometimes the browser will cache a faulty (e.g not fully downloaded) file resulting in Syntax Error when parsing; you can try in an incognito/private mode to confirm that this is transient and clear browser cache to remove such file.
+
 ## Requirements
 
 - JupyterLab >= 4.1.0 or Jupyter Notebook >= 7.1.0
 - A browser supporting:
   - [`SharedArrayBuffer`](https://caniuse.com/sharedarraybuffer)
   - [Web Workers](https://caniuse.com/webworkers)
   - Dynamic import for workers (behind `dom.workers.modules.enabled` in Firefox)
@@ -94,15 +107,15 @@
 ```
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install -U 'jupyterlab>=4.1.0a3' jupyterlab-transformers-completer
+pip install -U 'jupyterlab>=4.1.0' jupyterlab-transformers-completer
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
```

