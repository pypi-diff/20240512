# Comparing `tmp/scicookie-0.8.1.tar.gz` & `tmp/scicookie-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.8.1.tar", max compression
+gzip compressed data, was "scicookie-0.8.2.tar", max compression
```

## Comparing `scicookie-0.8.1.tar` & `scicookie-0.8.2.tar`

### file list

```diff
@@ -1,88 +1,95 @@
--rw-r--r--   0        0        0     1508 2024-05-03 14:55:32.011097 scicookie-0.8.1/LICENSE
--rw-r--r--   0        0        0     4874 2024-05-03 14:55:32.011097 scicookie-0.8.1/docs/description.md
--rw-r--r--   0        0        0     2091 2024-05-03 14:56:49.847445 scicookie-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/__init__.py
--rw-r--r--   0        0        0      116 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/__main__.py
--rw-r--r--   0        0        0     5066 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/cli.py
--rw-r--r--   0        0        0     1860 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0    12724 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      971 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/logs.py
--rw-r--r--   0        0        0     1607 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/profile.py
--rw-r--r--   0        0        0     6460 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0     1380 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     4153 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/ui.py
--rw-r--r--   0        0        0      336 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     5119 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1208 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2051 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2939 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1392 2024-05-03 14:55:32.023097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1790 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     3254 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2812 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     4404 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
--rw-r--r--   0        0        0     3354 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
--rw-r--r--   0        0        0      108 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
--rw-r--r--   0        0        0     2229 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     3563 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0      432 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0      608 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/CMakeLists.txt
--rw-r--r--   0        0        0      618 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml
--rw-r--r--   0        0        0     1884 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
--rw-r--r--   0        0        0     4824 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/deps-pyproject.toml
--rw-r--r--   0        0        0      228 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch-pyproject.toml
--rw-r--r--   0        0        0      589 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs
--rw-r--r--   0        0        0      632 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp
--rw-r--r--   0        0        0      264 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin-pyproject.toml
--rw-r--r--   0        0        0      400 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
--rw-r--r--   0        0        0      223 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
--rw-r--r--   0        0        0      217 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
--rw-r--r--   0        0        0     3632 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
--rw-r--r--   0        0        0      275 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11-pyproject.toml
--rw-r--r--   0        0        0      247 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core-pyproject.toml
--rw-r--r--   0        0        0      497 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/setup.py
--rw-r--r--   0        0        0      226 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
--rw-r--r--   0        0        0      171 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/skcdemo.cpp
--rw-r--r--   0        0        0     6436 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6436 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0    19228 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
--rw-r--r--   0        0        0     5593 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
--rw-r--r--   0        0        0     1998 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       54 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
--rw-r--r--   0        0        0      182 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
--rw-r--r--   0        0        0       20 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0    14485 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1116 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3382 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0     1123 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      141 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4571 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rw-r--r--   0        0        0      719 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml
--rw-r--r--   0        0        0       17 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/styles.css
--rwxr-xr-x   0        0        0     5275 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      374 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       30 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
--rw-r--r--   0        0        0    16405 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6840 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     1554 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py
--rw-r--r--   0        0        0     1009 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
--rw-r--r--   0        0        0      892 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
--rw-r--r--   0        0        0      831 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      546 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0     2151 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
--rw-r--r--   0        0        0        0 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
--rw-r--r--   0        0        0       19 2024-05-03 14:55:32.027097 scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0     5638 1970-01-01 00:00:00.000000 scicookie-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1508 2024-05-11 23:13:27.875334 scicookie-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4875 2024-05-11 23:13:27.875334 scicookie-0.8.2/docs/description.md
+-rw-r--r--   0        0        0     2147 2024-05-11 23:14:41.674267 scicookie-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     4394 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1860 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0    12535 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      971 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1607 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profile.py
+-rw-r--r--   0        0        0     6460 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0     1380 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0       41 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/tools/__init__.py
+-rw-r--r--   0        0        0      965 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/tools/fix_eof.py
+-rw-r--r--   0        0        0     4153 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/ui.py
+-rw-r--r--   0        0        0      336 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     5119 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1208 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2051 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2939 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1390 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2720 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     3899 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2812 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     4404 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
+-rw-r--r--   0        0        0     3354 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
+-rw-r--r--   0        0        0      108 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
+-rw-r--r--   0        0        0     2229 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     6004 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     3563 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0      432 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     1809 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml
+-rw-r--r--   0        0        0     2633 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-pyproject.toml
+-rw-r--r--   0        0        0     1917 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/urls-pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch/pyproject.toml
+-rw-r--r--   0        0        0      681 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml
+-rw-r--r--   0        0        0      615 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs
+-rw-r--r--   0        0        0      347 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/pyproject.toml
+-rw-r--r--   0        0        0      402 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/main.cpp
+-rw-r--r--   0        0        0      830 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/meson.build
+-rw-r--r--   0        0        0      296 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/pyproject.toml
+-rw-r--r--   0        0        0      561 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm/pyproject.toml
+-rw-r--r--   0        0        0     3602 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml
+-rw-r--r--   0        0        0      281 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp
+-rw-r--r--   0        0        0      450 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/setup.py
+-rw-r--r--   0        0        0      321 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/CMakeLists.txt
+-rw-r--r--   0        0        0      195 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/main.cpp
+-rw-r--r--   0        0        0      329 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/pyproject.toml
+-rw-r--r--   0        0        0      401 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/setup.py
+-rw-r--r--   0        0        0     6436 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6436 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0    19228 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
+-rw-r--r--   0        0        0     5593 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
+-rw-r--r--   0        0        0     1998 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0    14485 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3383 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0     1123 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      141 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4518 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rw-r--r--   0        0        0      719 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml
+-rw-r--r--   0        0        0       17 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/styles.css
+-rwxr-xr-x   0        0        0     5275 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16405 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6840 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     1554 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py
+-rw-r--r--   0        0        0     1009 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
+-rw-r--r--   0        0        0      892 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
+-rw-r--r--   0        0        0      848 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0     2151 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
+-rw-r--r--   0        0        0       19 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 scicookie-0.8.2/PKG-INFO
```

### Comparing `scicookie-0.8.1/LICENSE` & `scicookie-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/docs/description.md` & `scicookie-0.8.2/docs/description.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
 - Python: Make sure you have Python installed on your system. You can check by
   running `python --version` or `python3 --version` in your terminal. If you
   don't have it, download it from [here](https://www.python.org/downloads/).
 
 **Installation**
 
-- Install Cookieninja (if not already installed): Open your terminal and run the
-  following command: `pip install scicookie`
+- Install Cookiecutter (if not already installed): Open your terminal and run
+  the following command: `pip install scicookie`
 
 **Project Creation**
 
 1. Navigate to your desired project directory: Use the `cd` command to navigate
    to the directory where you want to create your new Python package project.
    For example: `cd ~/dev/my-python-projects` (Replace
    `~/dev/my-python-projects` with your preferred directory path.)
```

### Comparing `scicookie-0.8.1/pyproject.toml` & `scicookie-0.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.8.1"  # semantic-release
+version = "0.8.2"  # semantic-release
 description = "Cookiecutter template for a Python package"
 readme = "docs/description.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD-3-Clause"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
@@ -13,20 +13,20 @@
 ]
 
 [tool.poetry.scripts]
 "scicookie" = "scicookie.__main__:app"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
-cookieninja = "1.0.0"
-sh = ">=2.0.4"
+cookiecutter = "2.6.0"
 colorama = ">=0.4.6"
 inquirer = ">=3.1.3"
 pyyaml = ">=6.0.1"
-nodejs-wheel = ">=20.12"
+nodejs-wheel = ">=20.13.0-1"
+pre-commit-hooks = ">=0.4.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7"
 pre-commit = ">=3"
 ruff = ">=0.2.0"
 mypy = ">=1.5"
@@ -53,16 +53,17 @@
     | src/scicookie/hooks/*
 )'''  # TOML's single-quoted strings do not require escaping backslashes
 
 [[tool.mypy.overrides]]
 module = [
   "colorama",
   "inquirer",
-  "sh",
+  "cookiecutter.main",
   "yaml",
+  "pre_commit_hooks",
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 79
 force-exclude = true
 src = ["./"]
```

### Comparing `scicookie-0.8.1/src/scicookie/cli.py` & `scicookie-0.8.2/src/scicookie/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Module with CLI functions."""
 
 import argparse
 import json
-import os
-import sys
 
 from pathlib import Path
 from typing import Union
 
-import sh
+from cookiecutter.main import cookiecutter
 
 from scicookie.logs import SciCookieErrorType, SciCookieLogs
 from scicookie.profile import Profile
 from scicookie.ui import make_questions
 
 PACKAGE_PATH = Path(__file__).parent
 COOKIECUTTER_FILE_PATH = PACKAGE_PATH / "cookiecutter.json"
@@ -54,18 +52,17 @@
 
     if isinstance(answer_definition, str):
         return answer_definition
 
     return answer_definition[0]
 
 
-def call_cookiecutter(profile: Profile, answers: dict):  # noqa: PLR0912
-    """Call cookiecutter/cookieninja with the parameters from the TUI."""
+def call_cookiecutter(profile: Profile, answers: dict):
+    """Call cookiecutter/cookiecutter with the parameters from the TUI."""
     answers_profile = {}
-    cookie_args = []
     questions = profile.config
 
     with open(COOKIECUTTER_FILE_PATH) as f:
         cookiecutter_config = json.load(f)
 
     # fill the answers with default value
     for question_id, question in questions.items():
@@ -96,40 +93,16 @@
             answers_profile[question_id] = answer
             continue
 
         for choice in answer:
             choice_id = f"use_{choice.replace('-', '_')}"
             answers_profile[choice_id] = "yes"
 
-    for question_id, answer in answers_profile.items():
-        cookie_args.append(f"{question_id}={answer}")
-
-    sh_extras = {
-        "_in": sys.stdin,
-        "_out": sys.stdout,
-        "_err": sys.stderr,
-        "_no_err": True,
-        "_env": os.environ,
-        "_bg": True,
-        "_bg_exc": False,
-    }
-
-    p = sh.cookieninja("--no-input", PACKAGE_PATH, *cookie_args, **sh_extras)
-
-    try:
-        p.wait()
-    except sh.ErrorReturnCode as e:
-        SciCookieLogs.raise_error(
-            str(e), SciCookieErrorType.SH_ERROR_RETURN_CODE
-        )
-    except KeyboardInterrupt:
-        pid = p.pid
-        p.kill()
-        SciCookieLogs.raise_error(
-            f"Process {pid} killed.", SciCookieErrorType.SH_KEYBOARD_INTERRUPT
+        cookiecutter(
+            str(PACKAGE_PATH), no_input=True, extra_context=answers_profile
         )
 
 
 def app():
     """Run SciCookie."""
     # note: this parameter should be provided by a CLI argument
```

### Comparing `scicookie-0.8.1/src/scicookie/cookiecutter.json` & `scicookie-0.8.2/src/scicookie/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.8.2/src/scicookie/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import datetime
 import os
 import shutil
 import subprocess
 
 from pathlib import Path
 
+from scicookie.tools import fix_eof
+
 PROJECT_DIRECTORY = Path(os.path.abspath(os.path.curdir)).resolve()
 
 UNUSED_DOCS_DIRS = [
     PROJECT_DIRECTORY / 'docs-mkdocs',
     PROJECT_DIRECTORY / 'docs-sphinx',
     PROJECT_DIRECTORY / 'docs-jupyter-book',
     PROJECT_DIRECTORY / 'docs-quarto',
@@ -24,14 +26,16 @@
 
 USE_SRC_LAYOUT = {{ cookiecutter.project_layout == "src" }}
 if USE_SRC_LAYOUT:
     PACKAGE_PATH = PROJECT_DIRECTORY / "src" / "{{ cookiecutter.package_slug}}"
 else:
     PACKAGE_PATH = PROJECT_DIRECTORY / "{{ cookiecutter.package_slug}}"
 
+COMPILE_SOURCE_DIR = PROJECT_DIRECTORY / "src"
+
 USE_BLACK = {{ cookiecutter.use_black == "yes" }}
 USE_BANDIT = {{ cookiecutter.use_bandit == "yes" }}
 USE_CONTAINERS = {{ cookiecutter.use_containers in ['Docker', 'Podman'] }}
 USE_CLI = {{ cookiecutter.command_line_interface != "None" }}
 USE_CONDA = {{ cookiecutter.use_conda == "yes" }}
 USE_MAKE = {{ cookiecutter.use_make == "yes" }}
 USE_MAKIM = {{ cookiecutter.use_makim == "yes" }}
@@ -190,88 +194,104 @@
 def clean_up_cli():
     if not USE_CLI:
         remove_package_file("__main__.py")
         remove_package_file("cli.py")
 
 
 def clean_up_build_system():
-    build_system_dir = PROJECT_DIRECTORY / "build-system"
+    build_system_base_dir = PROJECT_DIRECTORY / "build-system"
+    build_system_dir = build_system_base_dir / BUILD_SYSTEM
+
+    os.makedirs(COMPILE_SOURCE_DIR, exist_ok=True)
 
-    if BUILD_SYSTEM == "poetry":
+    if BUILD_SYSTEM == "flit":
         shutil.move(
-            build_system_dir / "poetry-pyproject.toml",
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
-    elif BUILD_SYSTEM == "flit":
+    elif BUILD_SYSTEM == "hatch":
         shutil.move(
-            build_system_dir / "flit-pyproject.toml",
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
-    elif BUILD_SYSTEM == "mesonpy":
+    elif BUILD_SYSTEM == "maturin":
         shutil.move(
-            build_system_dir / "mesonpy-pyproject.toml",
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
         shutil.move(
-            build_system_dir / "meson.build",
-            PROJECT_DIRECTORY / 'meson.build'
+            build_system_dir / "Cargo.toml",
+            PROJECT_DIRECTORY / 'Cargo.toml'
         )
-    elif BUILD_SYSTEM == "setuptools":
         shutil.move(
-            build_system_dir / "setuptools-pyproject.toml",
-            PROJECT_DIRECTORY / 'pyproject.toml'
+            build_system_dir / "lib.rs",
+            COMPILE_SOURCE_DIR / 'lib.rs'
         )
-    elif BUILD_SYSTEM == "pdm":
+    elif BUILD_SYSTEM == "mesonpy":
+        os.makedirs(COMPILE_SOURCE_DIR, exist_ok=True)
         shutil.move(
-            build_system_dir / "pdm-pyproject.toml",
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
-    elif BUILD_SYSTEM == "hatch":
         shutil.move(
-            build_system_dir / "hatch-pyproject.toml",
-            PROJECT_DIRECTORY / 'pyproject.toml'
+            build_system_dir / "meson.build",
+            PROJECT_DIRECTORY / 'meson.build'
         )
-    elif BUILD_SYSTEM == "maturin":
         shutil.move(
-            build_system_dir / "maturin-pyproject.toml",
+            build_system_dir / "main.cpp",
+            COMPILE_SOURCE_DIR / 'main.cpp'
+        )
+    elif BUILD_SYSTEM == "pdm":
+        shutil.move(
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
+    elif BUILD_SYSTEM == "poetry":
         shutil.move(
-            build_system_dir / "Cargo.toml",
-            PROJECT_DIRECTORY / 'Cargo.toml'
+            build_system_dir / "pyproject.toml",
+            PROJECT_DIRECTORY / 'pyproject.toml'
         )
-    elif BUILD_SYSTEM == "scikit-build-core":
+    elif BUILD_SYSTEM == "pybind11":
         shutil.move(
-            build_system_dir / "scikit-build-core-pyproject.toml",
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
         shutil.move(
             build_system_dir / "CMakeLists.txt",
             PROJECT_DIRECTORY / 'CMakeLists.txt'
         )
         shutil.move(
-            build_system_dir / "skcdemo.cpp",
-            PROJECT_DIRECTORY / 'skcdemo.cpp'
+            build_system_dir / "setup.py",
+            PROJECT_DIRECTORY / 'setup.py'
         )
-    elif BUILD_SYSTEM == "pybind11":
         shutil.move(
-            build_system_dir / "pybind11-pyproject.toml",
+            build_system_dir / "main.cpp",
+            COMPILE_SOURCE_DIR / 'main.cpp'
+        )
+    elif BUILD_SYSTEM == "scikit-build-core":
+        shutil.move(
+            build_system_dir / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
         shutil.move(
             build_system_dir / "CMakeLists.txt",
             PROJECT_DIRECTORY / 'CMakeLists.txt'
         )
         shutil.move(
-            build_system_dir / "setup.py",
-            PROJECT_DIRECTORY / 'setup.py'
+            build_system_dir / "main.cpp",
+            COMPILE_SOURCE_DIR / 'main.cpp'
+        )
+    elif BUILD_SYSTEM == "setuptools":
+        shutil.move(
+            build_system_dir / "pyproject.toml",
+            PROJECT_DIRECTORY / 'pyproject.toml'
         )
     else:
         shutil.move(
-            build_system_dir / "base-pyproject.toml",
+            build_system_base_dir / "base" / "pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
         )
     remove_dir("build-system")
 
 
 def http2ssh(url):
     url = url.replace("https://", "git@")
@@ -280,28 +300,34 @@
 def clean_up_linter():
     if not USE_MYPY:
         remove_package_file("py.typed")
 
     if not USE_PRE_COMMIT:
         remove_project_file(".pre-commit-config.yaml")
 
-    # Auto format files with prettier
+    # Auto format tools
+    # -----------------
+
+    # prettier
     subprocess.call([
         "npx",
         "--yes",
         "prettier",
         "--write",
         "--ignore-unknown",
         PROJECT_DIRECTORY
     ])
 
     if not USE_PRETTIER:
         remove_project_file(".prettierrc.yaml")
         remove_project_file(".prettierignore")
 
+    # fix end of file
+    fix_eof.run(PROJECT_DIRECTORY)
+
 
 def prepare_git() -> None:
     git_https_origin = http2ssh("{{cookiecutter.git_https_origin}}")
     git_https_upstream = http2ssh("{{cookiecutter.git_https_upstream}}")
     git_main_branch = http2ssh("{{cookiecutter.git_main_branch}}")
     unique_id = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
     git_new_branch = f"initial-from-scicookie-{unique_id}"
@@ -361,39 +387,17 @@
     subprocess.call(["git", "add", "."])
     subprocess.call([
         "git", "commit", "-m", "Initial commit from SciCookie", "--no-verify"
     ])
     subprocess.call(["git", "branch", "-D", git_stash_branch])
 
 
-def add_binding_source_files():
-    if BUILD_SYSTEM == "maturin":
-        build_system_dir = PROJECT_DIRECTORY / "build-system"
-        src_system_dir = PROJECT_DIRECTORY/ "src"
-        if USE_SRC_LAYOUT :
-            shutil.move(build_system_dir / "lib.rs", "src")
-        else:
-            os.makedir(src_system_dir)
-            shutil.move(build_system_dir / "lib.rs", src_system_dir)
-    elif BUILD_SYSTEM == "pybind11" :
-        build_system_dir = PROJECT_DIRECTORY / "build-system"
-        src_system_dir = PROJECT_DIRECTORY/ "src"
-        if USE_SRC_LAYOUT :
-            shutil.move(build_system_dir / "main.cpp", "src")
-        else:
-            os.makedir(src_system_dir)
-            shutil.move(build_system_dir / "main.cpp", src_system_dir)
-    else:
-        pass
-
-
 def post_gen():
     # keep this one first, because it changes the package folder
     clean_up_project_layout()
-    add_binding_source_files()
     clean_up_automation()
     clean_up_cli()
     clean_up_code_of_conduct()
     clean_up_conda()
     clean_up_containers()
     clean_up_docs()
     clean_up_governance()
```

### Comparing `scicookie-0.8.1/src/scicookie/logs.py` & `scicookie-0.8.2/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/profile.py` & `scicookie-0.8.2/src/scicookie/profile.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/profiles/base.yaml` & `scicookie-0.8.2/src/scicookie/profiles/base.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/profiles/osl.yaml` & `scicookie-0.8.2/src/scicookie/profiles/osl.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/ui.py` & `scicookie-0.8.2/src/scicookie/ui.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## Pull Request description
 
 <!-- Describe the purpose of your PR and the changes you have made. -->
 
 <!-- Which issue this PR aims to resolve or fix? E.g.:
-Fixes #004
+Fixes #4
 -->
 
 ## How to test these changes
 
 <!-- Example:
 
 * run `$ abc -p 1234`
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,50 @@
+{%- raw -%}
 name: main
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
-  build:
+  check-branch:
+    if: ${{ github.event_name == 'pull_request' }}
+    runs-on: ubuntu-latest
+    timeout-minutes: 2
+    concurrency:
+      group: check-pr-${{ github.ref }}
+      cancel-in-progress: true
+
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - name: Check if the PR's branch is updated
+        uses: osl-incubator/gh-check-pr-is-updated@1.0.0
+        with:
+          remote_branch: origin/main
+          pr_sha: ${{ github.event.pull_request.head.sha }}
+
+  test:
     runs-on: ubuntu-latest
     timeout-minutes: 10
     concurrency:
-      group: ci-${{ "{{ github.ref }}" }}
+      group: ci-${{ github.event_name }}-${{ github.ref }}
       cancel-in-progress: true
 
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
       - uses: actions/checkout@v3
+{%- endraw %}
 {% if cookiecutter.use_conda == "yes" %}
       - uses: conda-incubator/setup-miniconda@v3
         with:
           miniforge-version: latest
           environment-file: conda/dev.yaml
           channels: conda-forge,nodefaults
           activate-environment: {{ cookiecutter.project_slug }}
@@ -34,15 +55,15 @@
         with:
           python-version: "pypy3.9"
 
       - name: Create virtual environment
         run: source {{ cookiecutter.project_slug }}/bin/activate
 
       - name: Install build-system
-        run: pip install -r requests.txt
+        run: pip install -r requirements.txt
 {%- endif %}
       - name: Install dependencies
         run: |
           {%- if cookiecutter.build_system == "poetry" %}
           poetry install
           {%- elif cookiecutter.build_system == "flit" %}
           flit install
@@ -52,20 +73,28 @@
           pip install .
           {%- endif %}
 
       - name: Run tests
         run: |
           {%- if cookiecutter.use_makim == "yes" %}
           makim tests.unit
-          {%- else %}
+          {%- elif cookiecutter.use_make == "yes" %}
           make test
+          {%- else %}
+          # add your command for running tests here
           {%- endif %}
 
       - name: Run style checks
         if: success() || failure()
         run: |
+          {%- if cookiecutter.use_pre_commit == "yes" %}
           pre-commit install
           {%- if cookiecutter.use_makim == "yes" %}
           makim tests.linter
-          {%- else %}
+          {%- elif cookiecutter.use_make == "yes" %}
           make lint
+          {%- else %}
+          # add your command for running the linter here
+          {%- endif %}
+          {%- else %}
+          # add your command for running the linter here
           {%- endif %}
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% if cookiecutter.project_license == 'MIT' -%}
+{%- if cookiecutter.project_license == 'MIT' -%}
 MIT License
 
 Copyright (c) {% now 'local', '%Y' %}, {{ cookiecutter.author_full_name }}
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -16,16 +16,16 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-{% elif cookiecutter.project_license == 'BSD 3 Clause' %}
 
+{%- elif cookiecutter.project_license == 'BSD 3 Clause' -%}
 BSD License
 
 Copyright (c) {% now 'local', '%Y' %}, {{ cookiecutter.author_full_name }}
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -47,15 +47,16 @@
 IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
-{% elif cookiecutter.project_license == 'ISC license' -%}
+
+{%- elif cookiecutter.project_license == 'ISC license' -%}
 ISC License
 
 Copyright (c) {% now 'local', '%Y' %}, {{ cookiecutter.author_full_name }}
 
 Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
@@ -71,15 +72,16 @@
 http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-{% elif cookiecutter.project_license == 'GNU General Public License v3' -%}
+
+{%- elif cookiecutter.project_license == 'GNU General Public License v3' -%}
 GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007
 
     {{ cookiecutter.project_short_description }}
     Copyright (C) {% now 'local', '%Y' %}  {{ cookiecutter.author_full_name }}
 
     This program is free software: you can redistribute it and/or modify
@@ -104,8 +106,8 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <http://www.gnu.org/philosophy/why-not-lgpl.html>.
-{% endif -%}
+{%- endif -%}
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [package]
-name = "{{ cookiecutter.project_slug }}"
-version = "0.1.0"
+name = "{{ cookiecutter.package_slug }}"
+version = "{{ cookiecutter.project_version }}"
 authors = ["{{ cookiecutter.author_full_name }} <{{ cookiecutter.author_email }}>"]
 edition = "2021"
 
 [lib]
-name = "_core"
+name = "{{ cookiecutter.package_slug }}"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [dependencies]
 rand = "0.8.4"
 
 [dependencies.pyo3]
 version = "0.19.1"
-# "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
-# "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
+# "extension-module" tells pyo3 we want to build an extension module (skips
+#   linking against libpython.so)
+# "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with
+#   minimum Python version 3.8
 features = ["extension-module", "abi3-py38"]
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -82,9 +82,7 @@
 check_untyped_defs = true
 strict = true
 ignore_missing_imports = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
 {% endif -%}
-{# keep this line at the end of the file #}
-# Add more configuration here!
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     x - y
 }
 
 /// A Python module implemented in Rust. The name of this function must match
 /// the `lib.name` setting in the `Cargo.toml`, else Python will not be able to
 /// import the module.
 #[pymodule]
-fn _core(_py: Python, m: &PyModule) -> PyResult<()> {
+fn {{ cookiecutter.package_slug }}(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(add, m)?)?;
     m.add_function(wrap_pyfunction!(subtract, m)?)?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
 
     Ok(())
 }
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -116,9 +116,8 @@
 {% endif -%}
 {%- if cookiecutter.use_makim == "yes" -%}
 makim = "1.15.1"
 {% endif -%}
 # 'PosixPath' object has no attribute 'endswith'
 virtualenv = "<=20.25.1"
 
-{% include "build-system/base-pyproject.toml" %}
-{#- keep this line at the end of the file -#}
+{% include "build-system/base/dev-deps-config-pyproject.toml" %}
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
   lifecycle and resources. This integration has improved our development and
   deployment processes, making them more efficient and streamlined.
 {%+ endif %}
 - TODO
 
 ## Credits
 
-This package was created with Cookieninja and the
+This package was created with Cookiecutter and the
 [osl-incubator/scicookie](https://github.com/osl-incubator/scicookie) project
 template.
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,17 @@
             show_category_heading: true
             show_root_full_path: false
             show_root_heading: true
             show_root_toc_entry: true
             show_source: false
             show_modules: true
   - mkdocs-jupyter:
-      execute: true
+      execute: false
       ignore:
         - "*.py"
-      # execute_ignore: "tutorial/*Geospatial*.ipynb"
       include_source: true
       theme: dark
   - literate-nav
 markdown_extensions:
   - admonition
   - attr_list
   - codehilite
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """{{ cookiecutter.project_name }}."""
 {%- if cookiecutter.use_black == "yes" %}
   {%- set QUOTE = '"' -%}
 {%- else %}
   {%- set QUOTE = "'" -%}
 {%- endif %}
-{% if cookiecutter.build_system == "hatch" -%}
+{% if cookiecutter.build_system in ["hatch", "pdm", "flit"] -%}
 __version__ = {{ QUOTE }}{{ cookiecutter.project_version }}{{ QUOTE }}
 {%- else %}
 from importlib import metadata as importlib_metadata
 
 
 def get_version() -> str:
     """Return the program version."""
```

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py` & `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.1/PKG-INFO` & `scicookie-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.8.1
+Version: 0.8.2
 Summary: Cookiecutter template for a Python package
 License: BSD-3-Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6)
-Requires-Dist: cookieninja (==1.0.0)
+Requires-Dist: cookiecutter (==2.6.0)
 Requires-Dist: inquirer (>=3.1.3)
-Requires-Dist: nodejs-wheel (>=20.12)
+Requires-Dist: nodejs-wheel (>=20.13.0-1)
+Requires-Dist: pre-commit-hooks (>=0.4.6)
 Requires-Dist: pyyaml (>=6.0.1)
-Requires-Dist: sh (>=2.0.4)
 Description-Content-Type: text/markdown
 
 ![CI](https://img.shields.io/github/actions/workflow/status/osl-incubator/scicookie/main.yaml?logo=github&label=CI)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scicookie)](https://pypi.org/project/scicookie/)
 [![Package Version](https://img.shields.io/pypi/v/scicookie?color=blue)](https://pypi.org/project/scicookie/)
 ![License](https://img.shields.io/pypi/l/scicookie?color=blue)
 ![Discord](https://img.shields.io/discord/796786891798085652?logo=discord&color=blue)
@@ -79,16 +79,16 @@
 
 - Python: Make sure you have Python installed on your system. You can check by
   running `python --version` or `python3 --version` in your terminal. If you
   don't have it, download it from [here](https://www.python.org/downloads/).
 
 **Installation**
 
-- Install Cookieninja (if not already installed): Open your terminal and run the
-  following command: `pip install scicookie`
+- Install Cookiecutter (if not already installed): Open your terminal and run
+  the following command: `pip install scicookie`
 
 **Project Creation**
 
 1. Navigate to your desired project directory: Use the `cd` command to navigate
    to the directory where you want to create your new Python package project.
    For example: `cd ~/dev/my-python-projects` (Replace
    `~/dev/my-python-projects` with your preferred directory path.)
```

