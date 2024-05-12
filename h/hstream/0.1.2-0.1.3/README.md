# Comparing `tmp/hstream-0.1.2.tar.gz` & `tmp/hstream-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.2.tar", max compression
+gzip compressed data, was "hstream-0.1.3.tar", max compression
```

## Comparing `hstream-0.1.2.tar` & `hstream-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4318 2024-05-11 12:21:43.141596 hstream-0.1.2/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.2/hstream/__init__.py
--rw-r--r--   0        0        0      142 2024-05-09 13:05:58.281937 hstream-0.1.2/hstream/__main__.py
--rw-r--r--   0        0        0     2377 2024-05-11 13:19:26.505499 hstream-0.1.2/hstream/cli.py
--rw-r--r--   0        0        0    16829 2024-05-11 11:38:42.857136 hstream-0.1.2/hstream/components/components.py
--rw-r--r--   0        0        0     4633 2024-05-09 13:05:58.283127 hstream-0.1.2/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-11 01:21:34.641755 hstream-0.1.2/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-11 01:21:34.644340 hstream-0.1.2/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      757 2024-05-11 03:52:48.159049 hstream-0.1.2/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      368 2024-05-11 04:02:12.326494 hstream-0.1.2/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7232 2024-05-11 12:14:46.432202 hstream-0.1.2/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      660 2024-05-11 01:21:34.646023 hstream-0.1.2/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-11 01:21:34.646562 hstream-0.1.2/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649048 hstream-0.1.2/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3215 2024-05-11 04:07:02.605594 hstream-0.1.2/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      800 2024-05-11 01:21:34.649589 hstream-0.1.2/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649841 hstream-0.1.2/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      705 2024-05-11 12:14:20.156589 hstream-0.1.2/hstream/hs.py
--rw-r--r--   0        0        0      391 2024-05-11 11:50:20.040099 hstream-0.1.2/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.2/hstream/template.py
--rw-r--r--   0        0        0      161 2024-05-09 13:05:58.284121 hstream-0.1.2/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2453 2024-05-09 13:05:58.284396 hstream-0.1.2/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2465 2024-05-11 12:13:40.726351 hstream-0.1.2/hstream/utils.py
--rw-r--r--   0        0        0      523 2024-05-11 13:19:34.965468 hstream-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 hstream-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4136 2024-05-11 13:30:49.388722 hstream-0.1.3/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.3/hstream/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-09 13:05:58.281937 hstream-0.1.3/hstream/__main__.py
+-rw-r--r--   0        0        0     2091 2024-05-11 13:57:29.550245 hstream-0.1.3/hstream/cli.py
+-rw-r--r--   0        0        0    16829 2024-05-11 11:38:42.857136 hstream-0.1.3/hstream/components/components.py
+-rw-r--r--   0        0        0     4633 2024-05-09 13:05:58.283127 hstream-0.1.3/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-11 01:21:34.641755 hstream-0.1.3/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-11 01:21:34.644340 hstream-0.1.3/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      757 2024-05-11 03:52:48.159049 hstream-0.1.3/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      368 2024-05-11 04:02:12.326494 hstream-0.1.3/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7232 2024-05-11 12:14:46.432202 hstream-0.1.3/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      660 2024-05-11 01:21:34.646023 hstream-0.1.3/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-11 01:21:34.646562 hstream-0.1.3/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649048 hstream-0.1.3/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3215 2024-05-11 04:07:02.605594 hstream-0.1.3/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      800 2024-05-11 01:21:34.649589 hstream-0.1.3/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649841 hstream-0.1.3/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      705 2024-05-11 12:14:20.156589 hstream-0.1.3/hstream/hs.py
+-rw-r--r--   0        0        0      391 2024-05-11 11:50:20.040099 hstream-0.1.3/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.3/hstream/template.py
+-rw-r--r--   0        0        0      161 2024-05-09 13:05:58.284121 hstream-0.1.3/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2453 2024-05-09 13:05:58.284396 hstream-0.1.3/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2465 2024-05-11 12:13:40.726351 hstream-0.1.3/hstream/utils.py
+-rw-r--r--   0        0        0      523 2024-05-11 13:58:20.734970 hstream-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 hstream-0.1.3/PKG-INFO
```

### Comparing `hstream-0.1.2/README.md` & `hstream-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 Love Streamlit but:
 
 - impossible to customise beyond PoC phase
 - hard to reason about when extending and deploying
 - non-standard approach doesn't play nicely with existing ecosystems
 
-H-(html)-Stream is built with semantic html, CherryPy and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
+H-(html)-Stream is built with semantic html, Django and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
 
 ## Components
 
 `hs.markdown`
 
 `hs.text_input`
 
@@ -102,29 +102,23 @@
         hs.markdown('Thanks to: ')
         with hs.html('a', href='https://picocss.com'):
             hs.markdown('pico css')
 ```
 
 ![hstream card demo](demo/card_example.png)
 
-- `run_server`: Once you outgrown our framework it is easy to add custom functionality or piece by piece move to a custom web app.
-
-[Server Example](./demo/server_example.md)
-
-
 # Technologies
 
 Big thanks to the following libraries in particular
 
 - Streamlit
 - htmx
 - Yattag
 - pico css
-- CherryPy
-
+- Django
 
 # Features (WIP)
 
 - [x] live server reload on file change (through univorn)
 - [x] semantic html and basic html manipulation from within script
 - [x] basic components - see below
 - [x] swap stylesheet
```

### Comparing `hstream-0.1.2/hstream/cli.py` & `hstream-0.1.3/hstream/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import hstream
 import shutil
 
 @click.group()
 def cli():
     pass
 
-@click.command(help="Convert your script file to a Django app")
-@click.argument("file", type=click.Path(), help="Your script file currently running your app")
+@click.command()
+@click.argument("file", type=click.Path(), )
 def eject(file=Path("./app.py")):
     click.echo('Ejecting a django server...')
     file = Path(file)
     path_to_hstream_dir = os.path.dirname(os.path.abspath(hstream.__file__))
     django_server = Path(path_to_hstream_dir) / "django_server"
     destination_dir = "./"
 
@@ -31,22 +31,22 @@
         f.write(hs_view_contents)
 
     click.echo('Django server ejected successfully.')
     click.echo('You can now run:.')
     click.echo(click.style(f"     python manage.py runserver", fg='green'))
 
 
-@click.command(help="Run your script file")
-@click.argument("file", type=click.Path(), help = "The file to run. should contain something like`from hstream import hs \n hs.markdown('hi)` ")
+@click.command()
+@click.argument("file", type=click.Path(),)
 def run(file=Path("./app.py")):
     click.echo('Running server...')
     file = Path(file)
     run_server(file)
 
-@click.command(help="Initialize a new hstream project with an example file.")
+@click.command()
 def init():
     import urllib.request
     url = "https://raw.githubusercontent.com/conradbez/hstream/main/demo/example.py"
     response = urllib.request.urlopen(url)
     content = response.read().decode()
     if example := Path("example.py"):
         if example.exists():
```

### Comparing `hstream-0.1.2/hstream/components/components.py` & `hstream-0.1.3/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/components/styling_components.py` & `hstream-0.1.3/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/django_server/hs/session_utils.py` & `hstream-0.1.3/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/django_server/hs/views.py` & `hstream-0.1.3/hstream/django_server/hs/views.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/django_server/manage.py` & `hstream-0.1.3/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/django_server/root/settings.py` & `hstream-0.1.3/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/django_server/root/urls.py` & `hstream-0.1.3/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/hs.py` & `hstream-0.1.3/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/templates/format_html.html` & `hstream-0.1.3/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/hstream/utils.py` & `hstream-0.1.3/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.2/pyproject.toml` & `hstream-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 yattag = "^1.15.2"
-ipdb = "^0.13.13"
 markdown = "^3.6"
 beautifulsoup4 = "^4.12"
 django = "^5.0.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 ipykernel = "^6.29.4"
 pandas = "^2.2.2"
+ipdb = "^0.13.13"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hstream-0.1.2/PKG-INFO` & `hstream-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12,<5.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: django (>=5.0.6,<6.0.0)
-Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: markdown (>=3.6,<4.0)
 Requires-Dist: yattag (>=1.15.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # HStream
 
 Convert your script to interactive python web app `user_said = hs.text_input("What would you like to say:")`
@@ -78,15 +77,15 @@
 
 Love Streamlit but:
 
 - impossible to customise beyond PoC phase
 - hard to reason about when extending and deploying
 - non-standard approach doesn't play nicely with existing ecosystems
 
-H-(html)-Stream is built with semantic html, CherryPy and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
+H-(html)-Stream is built with semantic html, Django and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
 
 ## Components
 
 `hs.markdown`
 
 `hs.text_input`
 
@@ -121,29 +120,23 @@
         hs.markdown('Thanks to: ')
         with hs.html('a', href='https://picocss.com'):
             hs.markdown('pico css')
 ```
 
 ![hstream card demo](demo/card_example.png)
 
-- `run_server`: Once you outgrown our framework it is easy to add custom functionality or piece by piece move to a custom web app.
-
-[Server Example](./demo/server_example.md)
-
-
 # Technologies
 
 Big thanks to the following libraries in particular
 
 - Streamlit
 - htmx
 - Yattag
 - pico css
-- CherryPy
-
+- Django
 
 # Features (WIP)
 
 - [x] live server reload on file change (through univorn)
 - [x] semantic html and basic html manipulation from within script
 - [x] basic components - see below
 - [x] swap stylesheet
```

