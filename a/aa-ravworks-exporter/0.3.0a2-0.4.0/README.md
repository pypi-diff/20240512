# Comparing `tmp/aa_ravworks_exporter-0.3.0a2.tar.gz` & `tmp/aa_ravworks_exporter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_ravworks_exporter-0.3.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_ravworks_exporter-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_ravworks_exporter-0.3.0a2.tar` & `aa_ravworks_exporter-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/LICENSE
--rw-r--r--   0        0        0     1472 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/README.md
--rwxr-xr-x   0        0        0     1572 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/pyproject.toml
--rw-r--r--   0        0        0      138 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/__init__.py
--rw-r--r--   0        0        0      531 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/__init__.py
--rw-r--r--   0        0        0      726 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/corptools.py
--rw-r--r--   0        0        0      753 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/memberaudit.py
--rw-r--r--   0        0        0      344 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/skill_settings.py
--rw-r--r--   0        0        0        0 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/structures/__init__.py
--rw-r--r--   0        0        0     1850 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/structures/structures.py
--rw-r--r--   0        0        0     1868 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/structures/structures_settings.py
--rw-r--r--   0        0        0     1424 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/forms.py
--rw-r--r--   0        0        0        0 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/migrations/__init__.py
--rw-r--r--   0        0        0       29 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/models.py
--rw-r--r--   0        0        0      620 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/templates/ravworks_exporter/index.html
--rw-r--r--   0        0        0      142 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/urls.py
--rw-r--r--   0        0        0     2348 2024-01-04 16:00:44.772330 aa_ravworks_exporter-0.3.0a2/ravworks_exporter/views.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 aa_ravworks_exporter-0.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1472 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/README.md
+-rwxr-xr-x   0        0        0     1567 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/corptools.py
+-rw-r--r--   0        0        0      753 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/memberaudit.py
+-rw-r--r--   0        0        0      344 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/skill_settings.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/__init__.py
+-rw-r--r--   0        0        0     1850 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures.py
+-rw-r--r--   0        0        0    10791 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures_settings.py
+-rw-r--r--   0        0        0     2378 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/forms.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/migrations/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/models.py
+-rw-r--r--   0        0        0      620 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/templates/ravworks_exporter/index.html
+-rw-r--r--   0        0        0      142 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/urls.py
+-rw-r--r--   0        0        0     2593 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/views.py
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 aa_ravworks_exporter-0.4.0/PKG-INFO
```

### Comparing `aa_ravworks_exporter-0.3.0a2/LICENSE` & `aa_ravworks_exporter-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/README.md` & `aa_ravworks_exporter-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/pyproject.toml` & `aa_ravworks_exporter-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 classifiers = [
     "Environment :: Web Environment",
 	"Framework :: Django",
 	"Framework :: Django :: 4",
 	"Framework :: Django :: 4.2",
 	"Operating System :: POSIX :: Linux",
-	"Development Status :: 3 - Alpha",
+	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Natural Language :: English",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
@@ -36,15 +36,15 @@
 	"allianceauth_ravworks",
 	"ravworks_exporter",
 	"ravworks_config",
 	"eveonline",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "allianceauth==4.0.0a5",
+    "allianceauth~=4.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Maestro-Zacht/aa-ravworks-exporter"
 Source = "https://github.com/Maestro-Zacht/aa-ravworks-exporter"
 Tracker = "https://github.com/Maestro-Zacht/aa-ravworks-exporter/issues"
 Changelog = "https://github.com/Maestro-Zacht/aa-ravworks-exporter/releases"
```

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/auth_hooks.py` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/corptools.py` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/corptools.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/skills/memberaudit.py` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/exporters/structures/structures.py` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/templates/ravworks_exporter/index.html` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/templates/ravworks_exporter/index.html`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.3.0a2/ravworks_exporter/views.py` & `aa_ravworks_exporter-0.4.0/ravworks_exporter/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import json
+import re
 
-from django.shortcuts import render
+from django.shortcuts import render, get_object_or_404
 from django.http import FileResponse
 from django.contrib.auth.decorators import login_required
 from django.contrib import messages
 from django.core.files.base import ContentFile
 
 from allianceauth.services.hooks import get_extension_logger
+from allianceauth.eveonline.models import EveCharacter
 
 from .forms import ExportForm
 
 logger = get_extension_logger(__name__)
 
+skills_re = re.compile(r'^(?P<app>memberaudit|corptools)-(?P<character_id>\d+)$')
+
 
 @login_required
 def index(request):
     if request.method == 'POST':
         form = ExportForm(request.user, request.POST, request.FILES)
         if form.is_valid():
             error = False
             config = json.load(form.cleaned_data['config'])
-            ownership = (
-                request.user.character_ownerships
-                .select_related('character')
-                .get(character__character_id=form.cleaned_data['character'])
-            )
-
-            if form.cleaned_data['skills'] == 'memberaudit':
-                from .exporters.skills.memberaudit import import_skills, is_character_added
-
-                if not is_character_added(ownership.character):
-                    messages.error(request, f"Character {ownership.character.character_name} is not added to MemberAudit")
-                    error = True
-                else:
-                    config.update(import_skills(ownership.character))
-            elif form.cleaned_data['skills'] == 'corptools':
-                from .exporters.skills.corptools import import_skills, is_character_added
-
-                if not is_character_added(ownership.character):
-                    messages.error(request, f"Character {ownership.character.character_name} is not added to CorpTools")
-                    error = True
-                else:
-                    config.update(import_skills(ownership.character))
+
+            if form.cleaned_data['skills']:
+                m = skills_re.match(form.cleaned_data['skills'])
+                app = m.group('app')
+                character = get_object_or_404(EveCharacter, character_id=int(m.group('character_id')), character_ownership__user=request.user)
+
+                if app == 'memberaudit':
+                    from .exporters.skills.memberaudit import import_skills, is_character_added
+
+                    if not is_character_added(character):
+                        messages.error(request, f"Character {character.character_name} is not added to MemberAudit")
+                        error = True
+                    else:
+                        config.update(import_skills(character))
+                elif app == 'corptools':
+                    from .exporters.skills.corptools import import_skills, is_character_added
+
+                    if not is_character_added(character):
+                        messages.error(request, f"Character {character.character_name} is not added to CorpTools")
+                        error = True
+                    else:
+                        config.update(import_skills(character))
 
             if form.cleaned_data['structures']:
                 from .exporters.structures.structures import export_structures
 
-                config['hidden_my_structures'] = export_structures(ownership.user)
+                config['hidden_my_structures'] = export_structures(request.user)
+                config['hidden_allocation_dict'] = {}
 
             if not error:
                 updated_config = ContentFile(json.dumps(config, indent=4).encode())
                 return FileResponse(updated_config, as_attachment=True, filename='config.json')
 
     else:
         form = ExportForm(request.user)
```

### Comparing `aa_ravworks_exporter-0.3.0a2/PKG-INFO` & `aa_ravworks_exporter-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.3.0a2
+Version: 0.4.0
 Summary: Ravworks config exporter for AllianceAuth
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: allianceauth==4.0.0a5
+Requires-Dist: allianceauth~=4.0
 Project-URL: Changelog, https://github.com/Maestro-Zacht/aa-ravworks-exporter/releases
 Project-URL: Homepage, https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Project-URL: Source, https://github.com/Maestro-Zacht/aa-ravworks-exporter
 Project-URL: Tracker, https://github.com/Maestro-Zacht/aa-ravworks-exporter/issues
 
 # AllianceAuth Ravworks Exporter
```

