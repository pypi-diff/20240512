# Comparing `tmp/sigaocaue_normalize_folder_name-0.1.0.tar.gz` & `tmp/sigaocaue_normalize_folder_name-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigaocaue_normalize_folder_name-0.1.0.tar", last modified: Sun May 12 14:58:42 2024, max compression
+gzip compressed data, was "sigaocaue_normalize_folder_name-0.1.1.tar", last modified: Sun May 12 15:14:48 2024, max compression
```

## Comparing `sigaocaue_normalize_folder_name-0.1.0.tar` & `sigaocaue_normalize_folder_name-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:42.257949 sigaocaue_normalize_folder_name-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-12 14:58:42.253949 sigaocaue_normalize_folder_name-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-12 14:58:38.000000 sigaocaue_normalize_folder_name-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:58:42.257949 sigaocaue_normalize_folder_name-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-12 14:58:38.000000 sigaocaue_normalize_folder_name-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:42.253949 sigaocaue_normalize_folder_name-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:42.253949 sigaocaue_normalize_folder_name-0.1.0/src/normalize_folder_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:38.000000 sigaocaue_normalize_folder_name-0.1.0/src/normalize_folder_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-12 14:58:38.000000 sigaocaue_normalize_folder_name-0.1.0/src/normalize_folder_name/normalized_folder_name_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:42.253949 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 14:58:42.000000 sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:14:48.322993 sigaocaue_normalize_folder_name-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-12 15:14:48.322993 sigaocaue_normalize_folder_name-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-12 15:14:41.000000 sigaocaue_normalize_folder_name-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:14:48.322993 sigaocaue_normalize_folder_name-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-12 15:14:46.000000 sigaocaue_normalize_folder_name-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:14:48.318993 sigaocaue_normalize_folder_name-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:14:48.322993 sigaocaue_normalize_folder_name-0.1.1/src/normalize_folder_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:14:41.000000 sigaocaue_normalize_folder_name-0.1.1/src/normalize_folder_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-12 15:14:41.000000 sigaocaue_normalize_folder_name-0.1.1/src/normalize_folder_name/normalized_folder_name_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:14:48.322993 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 15:14:48.000000 sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/top_level.txt
```

### Comparing `sigaocaue_normalize_folder_name-0.1.0/PKG-INFO` & `sigaocaue_normalize_folder_name-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigaocaue_normalize_folder_name
-Version: 0.1.0
+Version: 0.1.1
 Summary: O Normalize Folder Name CLI é uma ferramenta de linha de comando desenvolvida para auxiliar
 Home-page: https://github.com/sigaocaue/normalize_folder_name
 Author: Cauê Prado
 Author-email: caue.prado0@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 Esta ferramenta converte strings de entrada para um formato padronizado, substituindo espaços e caracteres especiais por underscores, removendo acentos e convertendo o texto para minúsculas. Isso facilita a criação de diretórios que são compatíveis com diversos sistemas operacionais e ambientes de desenvolvimento.
 
 ## Instalação
 
 Você pode instalar o **Normalize Folder Name CLI** diretamente via PyPI:
 
 ```bash
-pip install @sigaocaue/normalize-folder-name
+pip install sigaocaue-normalize-folder-name
 ```
 ## Uso
 Para usar a ferramenta, execute o comando a seguir no seu terminal:
 ```bash
 normalize_folder_name --text "Seu Texto Aqui"
 ```
 Isso irá gerar um nome de pasta normalizado baseado no texto fornecido.
```

### Comparing `sigaocaue_normalize_folder_name-0.1.0/README.md` & `sigaocaue_normalize_folder_name-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Esta ferramenta converte strings de entrada para um formato padronizado, substituindo espaços e caracteres especiais por underscores, removendo acentos e convertendo o texto para minúsculas. Isso facilita a criação de diretórios que são compatíveis com diversos sistemas operacionais e ambientes de desenvolvimento.
 
 ## Instalação
 
 Você pode instalar o **Normalize Folder Name CLI** diretamente via PyPI:
 
 ```bash
-pip install @sigaocaue/normalize-folder-name
+pip install sigaocaue-normalize-folder-name
 ```
 ## Uso
 Para usar a ferramenta, execute o comando a seguir no seu terminal:
 ```bash
 normalize_folder_name --text "Seu Texto Aqui"
 ```
 Isso irá gerar um nome de pasta normalizado baseado no texto fornecido.
```

### Comparing `sigaocaue_normalize_folder_name-0.1.0/setup.py` & `sigaocaue_normalize_folder_name-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sigaocaue_normalize_folder_name',
-    version='0.1.0',
+    version='0.1.1',
     author="Cauê Prado",
     author_email="caue.prado0@gmail.com",
     description="""
     O Normalize Folder Name CLI é uma ferramenta de linha de comando desenvolvida para auxiliar
     usuários a criarem um nome para suas pastas em um formato consistente, seguro e adequado para pastas de projetos
     de desenvolvimento de software.
     """,
```

### Comparing `sigaocaue_normalize_folder_name-0.1.0/src/normalize_folder_name/normalized_folder_name_cli.py` & `sigaocaue_normalize_folder_name-0.1.1/src/normalize_folder_name/normalized_folder_name_cli.py`

 * *Files identical despite different names*

### Comparing `sigaocaue_normalize_folder_name-0.1.0/src/sigaocaue_normalize_folder_name.egg-info/PKG-INFO` & `sigaocaue_normalize_folder_name-0.1.1/src/sigaocaue_normalize_folder_name.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigaocaue_normalize_folder_name
-Version: 0.1.0
+Version: 0.1.1
 Summary: O Normalize Folder Name CLI é uma ferramenta de linha de comando desenvolvida para auxiliar
 Home-page: https://github.com/sigaocaue/normalize_folder_name
 Author: Cauê Prado
 Author-email: caue.prado0@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 Esta ferramenta converte strings de entrada para um formato padronizado, substituindo espaços e caracteres especiais por underscores, removendo acentos e convertendo o texto para minúsculas. Isso facilita a criação de diretórios que são compatíveis com diversos sistemas operacionais e ambientes de desenvolvimento.
 
 ## Instalação
 
 Você pode instalar o **Normalize Folder Name CLI** diretamente via PyPI:
 
 ```bash
-pip install @sigaocaue/normalize-folder-name
+pip install sigaocaue-normalize-folder-name
 ```
 ## Uso
 Para usar a ferramenta, execute o comando a seguir no seu terminal:
 ```bash
 normalize_folder_name --text "Seu Texto Aqui"
 ```
 Isso irá gerar um nome de pasta normalizado baseado no texto fornecido.
```

