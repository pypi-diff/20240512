# Comparing `tmp/staging_cacao_accounting-0.0.1b20240511.tar.gz` & `tmp/staging_cacao_accounting-0.0.1b20240512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staging_cacao_accounting-0.0.1b20240511.tar", last modified: Sat May 11 22:54:43 2024, max compression
+gzip compressed data, was "staging_cacao_accounting-0.0.1b20240512.tar", last modified: Sat May 11 22:56:51 2024, max compression
```

## Comparing `staging_cacao_accounting-0.0.1b20240511.tar` & `staging_cacao_accounting-0.0.1b20240512.tar`

### file list

```diff
@@ -1,205 +1,2504 @@
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.087817 staging_cacao_accounting-0.0.1b20240511/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1166 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/Dockerfile
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11356 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/LICENSE
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28800 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/Licencias_de_Terceros.md
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/MANIFEST.in
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18934 2024-05-11 22:54:43.086817 staging_cacao_accounting-0.0.1b20240511/PKG-INFO
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4335 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/README.md
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.008815 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      684 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/I18N.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8159 2024-05-11 22:45:50.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      790 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/__main__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.008815 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1359 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.009816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/registros/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      675 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/registros/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.009816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/templates/
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.010815 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/templates/admin/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/templates/admin/modulos.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/templates/admin.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.010815 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ajax/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      764 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ajax/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.011816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2357 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.012816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      204 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/templates/app.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      627 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/templates/development.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.014816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3596 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1055 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/forms.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    26341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/permisos.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.015816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/registros/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      945 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/registros/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5351 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/roles.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.016816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1685 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/templates/login.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6697 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/templates/test_roles.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.017816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/bancos/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1126 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/bancos/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.017816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/bancos/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      332 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/bancos/templates/bancos.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1120 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/cli.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.018816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/compras/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1081 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/compras/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.018816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/compras/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/compras/templates/compras.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6678 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/config.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.020816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18243 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3871 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/auxiliares.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.020816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2325 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.020816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/catalogos/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11029 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/catalogos/base.csv
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2565 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/forms.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.025816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      998 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/ccosto.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      984 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/cuenta.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1101 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/entidad.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      969 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/moneda.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1032 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/periodo.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      989 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/proyecto.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      979 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/tasa_cambio.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      968 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/unidad.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.025816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.035816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      811 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3549 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      803 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8794 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2791 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2889 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2401 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2176 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1320 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1648 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2034 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1540 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      977 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2266 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1861 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1337 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.035816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/database/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    22209 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/database/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5564 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/database/helpers.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.036816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      861 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.037816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/base/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4885 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/base/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.037816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/dev/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    33257 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/dev/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2060 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/decorators.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/desktop.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.038816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/exceptions/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1283 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/exceptions/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      986 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/exceptions/mensajes.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.038816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/inventario/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1117 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/inventario/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.038816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/inventario/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      340 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/inventario/templates/inventario.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      783 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/loggin.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      813 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/metadata.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:42.993815 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/misc/
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.039816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/misc/ejemplos/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/misc/ejemplos/cacao-accounting.unit
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3923 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/modulos.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.039816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/registro/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6043 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/registro/__init__.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1989 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/server.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.040816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.042816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       32 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/cacaoaccounting.css
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1424 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/dashboard.css
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2590 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/purecss-treeview.css
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      722 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/signin.css
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      720 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/manifest.json
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.054816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Cacao Accounting SVG.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Cacao Accounting-01.png
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.057816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2212 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3851 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5536 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.062816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting-01.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting.png
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.066816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1150 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   270398 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4286 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9662 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    16958 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    61298 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    19765 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/brand.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting _logo.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    19765 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting _logo.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_logo.svg
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/circle-solid.svg
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.079816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-144x144.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    30582 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-192x192.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3820 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-36x36.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5627 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-48x48.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9202 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-72x72.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13210 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-96x96.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    16894 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-114x114.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18160 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-120x120.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-144x144.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    24785 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-152x152.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31048 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-180x180.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6938 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-57x57.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-60x60.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9202 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-72x72.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9743 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-76x76.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31156 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-precomposed.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31156 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1607 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-16x16.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3317 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-32x32.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13210 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-96x96.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1150 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon.ico
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-144x144.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    24371 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-150x150.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    67679 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-310x310.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8745 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-70x70.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon-16x16.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2212 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon-32x32.png
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1823 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/package-lock.json
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/package.json
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.081817 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1124 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/400.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1133 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/403.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1107 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/404.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1400 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/base.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8157 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/macros.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.081817 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/setup/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2863 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/setup/setup.html
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.081817 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/transaccion/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2723 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/transaccion/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.082816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/validaciones/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1243 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/validaciones/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.082816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ventas/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1048 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ventas/__init__.py
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.083816 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ventas/templates/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      325 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ventas/templates/ventas.html
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      934 2024-05-11 22:53:24.000000 staging_cacao_accounting-0.0.1b20240511/cacao_accounting/version.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1558 2024-05-11 22:50:08.000000 staging_cacao_accounting-0.0.1b20240511/pyproject.toml
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      248 2024-05-11 22:54:27.000000 staging_cacao_accounting-0.0.1b20240511/requirements.txt
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      187 2024-05-11 22:54:43.087817 staging_cacao_accounting-0.0.1b20240511/setup.cfg
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.086817 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18934 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/PKG-INFO
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7512 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)        1 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       54 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/entry_points.txt
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      217 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/requires.txt
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       17 2024-05-11 22:54:42.000000 staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:54:43.085816 staging_cacao_accounting-0.0.1b20240511/tests/
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       46 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/tests/test_basicos.py
--rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1070 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240511/wsgi.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.811537 staging_cacao_accounting-0.0.1b20240512/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1166 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/Dockerfile
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11356 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/LICENSE
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28800 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/Licencias_de_Terceros.md
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/MANIFEST.in
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18934 2024-05-11 22:56:51.811537 staging_cacao_accounting-0.0.1b20240512/PKG-INFO
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4335 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/README.md
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.157515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      684 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/I18N.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8159 2024-05-11 22:45:50.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      790 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/__main__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.161515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1359 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.162515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/registros/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      675 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/registros/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.162515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/templates/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.162515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/templates/admin/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/templates/admin/modulos.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/templates/admin.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.163515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ajax/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      764 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ajax/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.163515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2357 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.164515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      204 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/templates/app.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      627 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/templates/development.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.165515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3596 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1055 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/forms.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    26341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/permisos.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.165515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/registros/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      945 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/registros/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5351 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/roles.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.166515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1685 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/templates/login.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6697 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/templates/test_roles.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.166515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/bancos/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1126 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/bancos/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.166515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/bancos/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      332 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/bancos/templates/bancos.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1120 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/cli.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.166515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/compras/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1081 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/compras/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.167515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/compras/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/compras/templates/compras.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6678 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/config.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.167515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18243 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3871 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/auxiliares.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.168515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2325 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.168515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/catalogos/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11029 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/catalogos/base.csv
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2565 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/forms.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.171515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      998 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/ccosto.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      984 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/cuenta.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1101 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/entidad.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      969 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/moneda.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1032 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/periodo.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      989 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/proyecto.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      979 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/tasa_cambio.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      968 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/unidad.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.171515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.178516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      811 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3549 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      803 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8794 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2791 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2889 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2401 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2176 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1320 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1648 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2034 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1540 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      977 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2266 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1861 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1337 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.179515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/database/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    22209 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/database/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5564 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/database/helpers.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.180516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      861 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.181516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/base/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4885 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/base/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.181516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/dev/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    33257 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/dev/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2060 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/decorators.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/desktop.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.184516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/exceptions/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1283 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/exceptions/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      986 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/exceptions/mensajes.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.185515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/inventario/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1117 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/inventario/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.185515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/inventario/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      340 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/inventario/templates/inventario.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      783 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/loggin.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      813 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/metadata.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.138515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/misc/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.185515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/misc/ejemplos/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/misc/ejemplos/cacao-accounting.unit
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3923 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/modulos.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.186516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/registro/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6043 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/registro/__init__.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1989 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/server.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.187516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.189516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       32 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/cacaoaccounting.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1424 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/dashboard.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2590 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/purecss-treeview.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      722 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/signin.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      720 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/manifest.json
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.198516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Cacao Accounting SVG.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Cacao Accounting-01.png
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.200516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2212 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3851 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5536 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.204516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting-01.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting.png
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.208516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1150 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   270398 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4286 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9662 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    16958 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    61298 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    19765 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/brand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    27950 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting _logo.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    19765 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting _logo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    28208 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   451063 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   474061 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_logo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/circle-solid.svg
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.235516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-144x144.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    30582 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-192x192.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3820 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-36x36.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5627 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-48x48.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9202 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-72x72.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13210 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-96x96.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    16894 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-114x114.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18160 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-120x120.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-144x144.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    24785 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-152x152.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31048 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-180x180.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6938 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-57x57.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7341 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-60x60.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9202 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-72x72.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9743 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-76x76.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31156 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-precomposed.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    31156 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1607 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-16x16.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3317 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-32x32.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13210 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-96x96.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1150 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon.ico
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    23238 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-144x144.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    24371 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-150x150.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    67679 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-310x310.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8745 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-70x70.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon-16x16.png
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2212 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon-32x32.png
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.238516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1622 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/.package-lock.json
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.141515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.238516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.143515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.241516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/cjs/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2037 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/cjs/enums.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    30505 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/cjs/popper-base.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    40113 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    59692 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/cjs/popper.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.248516 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7344 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/createPopper.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.270517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      677 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1371 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3400 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2072 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      148 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getComputedStyle.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentElement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1227 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      142 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getHTMLElementScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      767 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      114 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeName.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2613 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      759 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      546 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      881 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      273 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      258 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      721 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      621 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      159 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/isLayoutViewport.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      440 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/isScrollParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      162 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/isTableElement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1177 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1335 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/enums.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/index.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.278517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2527 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3423 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5711 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1330 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4910 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1954 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      502 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/index.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1613 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      706 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6585 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      193 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/popper-base.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/popper-lite.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1090 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/popper.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/types.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.292517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1681 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1738 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/debounce.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      159 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/expandToHashMap.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       79 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getAltAxis.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       89 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getAltLen.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      125 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getBasePlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      117 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getFreshSideObject.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      127 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getMainAxisFromPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      248 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getOppositePlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      209 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getOppositeVariationPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       85 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/getVariation.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       84 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/math.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      184 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/mergePaddingObject.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1240 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      191 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/rectToClientRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      252 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/uniqueBy.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/userAgent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      262 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/esm/utils/within.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.297517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2479 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/enums.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1108 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/enums.min.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    32395 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper-base.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9780 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    42543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper-lite.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13566 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    63070 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    20122 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/dist/umd/popper.min.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.301517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7344 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/createPopper.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.314517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      677 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/contains.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1371 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3400 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2072 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      148 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1227 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      142 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      767 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      114 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2613 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      759 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      546 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      881 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      273 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      258 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      721 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      621 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      159 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      440 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      162 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1177 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1335 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/enums.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/index.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.318517 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2527 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3423 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/arrow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5711 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1330 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4910 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/flip.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1954 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/hide.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      502 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/index.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1613 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/offset.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      706 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6585 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      193 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/popper-base.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/popper-lite.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1090 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/popper.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/types.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.330518 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1681 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1738 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/debounce.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      159 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       79 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       89 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getAltLen.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      125 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      117 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      127 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      248 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      209 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       85 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/getVariation.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       84 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/math.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/mergeByName.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      184 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1240 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      191 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      252 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/userAgent.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      262 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/lib/utils/within.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4230 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/@popperjs/core/package.json
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.331518 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.145515 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.765537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    70329 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    51795 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    70403 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    51870 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    12065 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    10126 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    12058 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    10198 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   107823 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    85352 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   107691 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    85281 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   281046 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   232803 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   280259 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   232911 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.768537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   207819 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    80721 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   135829 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.esm.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    73935 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   145401 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    60635 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/dist/js/bootstrap.min.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.769537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.775537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2835 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/alert.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2825 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/base-component.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2463 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/button.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13420 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/carousel.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8838 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/collapse.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.778537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dom/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2115 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dom/data.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9438 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dom/event-handler.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2415 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dom/manipulator.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4220 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dom/selector-engine.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    15354 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11198 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/modal.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8264 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/offcanvas.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2669 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/popover.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9818 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    10426 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/tab.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6199 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/toast.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18395 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/tooltip.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.785537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4117 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/backdrop.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2050 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/component-functions.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2566 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/config.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3464 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/focustrap.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9316 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/index.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3922 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/sanitizer.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4698 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/scrollbar.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4360 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/swipe.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     4684 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/dist/util/template-factory.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      907 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/index.esm.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      874 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/index.umd.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.790537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1903 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/alert.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1932 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/base-component.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1625 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/button.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    11817 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/carousel.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7594 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/collapse.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.792537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dom/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1395 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dom/data.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8351 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dom/event-handler.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1658 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dom/manipulator.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3436 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dom/selector-engine.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    13205 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/dropdown.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9583 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/modal.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     6806 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/offcanvas.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1870 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/popover.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8474 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9068 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/tab.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     5039 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/toast.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    16031 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/tooltip.js
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.798537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3127 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/backdrop.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1114 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/component-functions.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1784 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/config.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2518 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/focustrap.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     7640 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/index.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2963 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/sanitizer.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3754 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/scrollbar.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3409 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/swipe.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3612 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/js/src/util/template-factory.js
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     9648 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap/package.json
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.334518 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)  1098145 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/bootstrap-icons.svg
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.336518 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    98255 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/bootstrap-icons.css
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    52358 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/bootstrap-icons.json
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    85875 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/bootstrap-icons.min.css
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:50.338518 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/fonts/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   176032 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/fonts/bootstrap-icons.woff
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   130396 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/font/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.752537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      476 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/0-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      507 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/0-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/0-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/0-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      250 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/1-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      279 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/1-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/1-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/1-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      854 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/123.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      457 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/2-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      477 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/2-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      484 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/2-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      564 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/2-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      607 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/3-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      642 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/3-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      634 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/3-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      714 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/3-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/4-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/4-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      428 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/4-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/4-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/5-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/5-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      521 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/5-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      601 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/5-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      617 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/6-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      640 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/6-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      662 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/6-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      727 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/6-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      251 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/7-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      279 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/7-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/7-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/7-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      686 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/8-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      717 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/8-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      737 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/8-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      804 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/8-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/9-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      597 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/9-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      620 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/9-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      684 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/9-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/activity.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      687 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/airplane-engines-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1025 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/airplane-engines.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      492 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/airplane-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      840 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/airplane.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      615 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alarm-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      689 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alarm.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alexa.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      264 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-bottom.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-center.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      315 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-end.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-middle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      315 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-start.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      281 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/align-top.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      839 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alipay.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      845 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alphabet-uppercase.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1038 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alphabet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      324 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1279 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/amazon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      230 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/amd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      432 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/android.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1401 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/android2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/app-indicator.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      278 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/app.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1430 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/apple.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      349 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/archive-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/archive.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      345 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-90deg-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-90deg-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      346 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-90deg-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-90deg-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      373 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-bar-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      373 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-bar-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      373 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-bar-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      374 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-bar-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      349 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-clockwise.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-counterclockwise.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      364 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-left-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-left-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      360 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-left-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      435 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-left-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      284 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      365 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-right-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      361 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-right-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      437 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-right-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      287 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-short.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      455 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      308 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      451 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-short.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      567 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-repeat.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      372 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-return-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-return-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      317 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      315 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right-short.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      438 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      742 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-through-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      946 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-through-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      362 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-left-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-left-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-left-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-left-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      281 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-right-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      361 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-right-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-right-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      432 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-right-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      284 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-short.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      355 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      308 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      461 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-angle-contract.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-angle-expand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      480 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-collapse-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-collapse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-expand-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      492 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-expand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      726 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-fullscreen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      695 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-move.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      349 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/arrows.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/aspect-ratio-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      472 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/aspect-ratio.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/asterisk.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      786 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/at.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      415 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/award-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      620 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/award.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      315 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/back.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      607 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      676 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      882 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      811 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      923 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      538 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack4-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backpack4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      452 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backspace-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backspace-reverse-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      577 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backspace-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      580 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/backspace.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      783 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-3d-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      843 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-3d.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      504 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-4k-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      540 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-4k.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      785 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-8k-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      854 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-8k.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      642 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-ad-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      695 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-ad.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-ar-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      596 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-ar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      783 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-cc-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      828 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-cc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      474 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-hd-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      522 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-hd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      784 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-sd-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      852 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-sd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-tm-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      453 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-tm.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-vo-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      640 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-vo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      501 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-vr-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      558 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-vr.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      626 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-wc-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      701 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/badge-wc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      379 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      471 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      270 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      348 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      367 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      535 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      305 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      736 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/balloon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      749 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/balloon-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      972 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/balloon-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      797 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/balloon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      257 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ban-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      284 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ban.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      812 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bandaid-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      959 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bandaid.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bank.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      422 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bank2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bar-chart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      309 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bar-chart-line-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      342 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bar-chart-line.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      527 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bar-chart-steps.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bar-chart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      559 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      738 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      581 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      447 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      461 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/basket3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      738 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/battery-charging.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/battery-full.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      362 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/battery-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      332 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/battery.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1505 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/behance.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bell-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bell-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      629 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bell-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bell.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      981 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bezier.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      767 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bezier2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      616 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bicycle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1589 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bing.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      628 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/binoculars-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1055 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/binoculars.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      872 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/blockquote-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      864 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/blockquote-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      477 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bluetooth.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      923 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/body-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      500 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/book-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      642 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/book-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      770 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/book.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      429 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      251 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      441 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      455 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      615 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-star-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      683 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-star.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      556 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      330 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmark.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmarks-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      442 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookmarks.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      293 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bookshelf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      714 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/boombox-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      754 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/boombox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      545 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bootstrap-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bootstrap-reboot.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bootstrap.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      229 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-all.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1149 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-bottom.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1125 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-center.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      940 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-inner.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1182 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1136 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-middle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      533 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-outer.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1152 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      704 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-style.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1160 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-top.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      369 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border-width.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1407 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/border.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bounding-box-circles.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      278 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bounding-box.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-down-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      530 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-down-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-down-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      537 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-down-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      546 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      548 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-up-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-up-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-in-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      542 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-up-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-up-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      538 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      480 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-seam-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box-seam.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      446 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box2-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      407 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box2-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      317 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/box2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      782 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/boxes.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      985 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/braces-asterisk.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      772 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/braces.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bricks.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      464 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/briefcase-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      539 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/briefcase.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-alt-high-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      581 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-alt-high.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      442 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-alt-low-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      480 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-alt-low.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      791 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-high-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      818 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-high.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      540 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-low-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      566 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brightness-low.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      252 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brilliance.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      590 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/broadcast-pin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/broadcast.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/browser-chrome.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1165 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/browser-edge.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1322 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/browser-firefox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2137 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/browser-safari.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      683 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brush-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1145 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/brush.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      334 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bucket-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      410 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bucket.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      703 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bug-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      812 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bug.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1045 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1081 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1002 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1093 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1049 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1114 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1150 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1071 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1162 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1133 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1587 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1069 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1145 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1161 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1196 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      994 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1502 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1040 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1076 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1092 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1108 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1010 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/building.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/buildings-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      644 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/buildings.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      434 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bullseye.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      898 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bus-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1047 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/bus-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/c-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      511 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/c-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/c-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      598 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/c-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      968 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cake-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1052 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cake.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1705 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cake2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2006 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cake2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      954 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calculator-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1006 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calculator.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      395 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      768 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-date-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      799 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-date.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      586 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-day-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      644 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-day.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      370 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-event-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-event.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      979 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-month-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1036 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-month.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      448 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-range-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-range.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      612 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-week-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      659 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-week.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      461 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      529 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      322 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      592 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      887 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-date-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      923 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-date.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      705 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-day-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      768 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-day.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-event-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      548 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-event.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      377 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      451 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      508 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      442 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1110 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-month-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1162 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-month.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      491 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      558 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-range-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      515 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-range.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      725 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-week-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      768 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-week.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      566 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      656 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      446 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      292 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-event-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-event.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      231 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      298 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-range-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-range.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-week-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3-week.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      666 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      465 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar4-event.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      482 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar4-range.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      701 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar4-week.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/calendar4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      399 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-reels-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      557 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-reels.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      324 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-video-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      392 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-video-off-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      521 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-video-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      427 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera-video.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      633 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/camera2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/capslock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      464 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/capslock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/capsule-pill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      279 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/capsule.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      875 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/car-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1220 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/car-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      719 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/card-checklist.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      545 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/card-heading.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      448 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/card-image.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      625 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/card-list.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      522 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/card-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      265 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-down-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      386 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-down-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      282 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      266 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-left-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      312 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-left-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      417 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-left-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      270 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      268 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-right-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      308 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-right-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      416 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-right-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      279 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      265 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      304 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-up-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      412 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-up-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      280 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/caret-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      529 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      569 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      464 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      440 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      513 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      554 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      602 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      635 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      465 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      453 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      512 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      538 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cart4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      948 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cash-coin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      369 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cash-stack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      328 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      477 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cassette-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      534 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cassette.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      465 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cast.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      743 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cc-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      786 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cc-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      793 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cc-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1622 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cc-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-dots-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      689 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-dots.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      328 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      671 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      364 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-dots-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      457 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-dots.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      264 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      869 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-quote-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      657 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-quote.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      537 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      941 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-quote-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      890 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-quote.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-dots-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      459 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-dots.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      267 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      342 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      435 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      816 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-quote-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      659 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-quote.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      393 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      539 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      343 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-dots-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      530 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-dots.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      372 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      902 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-quote-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      730 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-quote.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      610 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      414 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      457 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      770 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chat.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      372 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-all.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      339 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      369 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      321 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      376 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      271 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check2-all.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      369 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check2-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      434 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check2-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      271 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/check2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      470 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-contract.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      355 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-expand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      353 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      355 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-bar-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      299 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-compact-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      297 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-compact-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-compact-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      273 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-compact-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      408 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-contract.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      447 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-double-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      445 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-double-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      448 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-double-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-double-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      289 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-expand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      288 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      290 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      267 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/chevron-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      168 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      204 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/circle-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/circle-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      213 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      653 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      594 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-data-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      614 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-data.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      471 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      583 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      598 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      510 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      588 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      634 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      732 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-pulse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      635 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      715 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      488 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      619 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      634 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-data-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      663 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-data.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      510 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      696 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      676 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      551 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      605 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      631 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      759 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-pulse-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      770 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-pulse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      673 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      702 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clipboard2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      262 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      941 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clock-history.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      305 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      498 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-arrow-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      767 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-arrow-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      765 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      470 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      760 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      526 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-download-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      770 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-download.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      582 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-drizzle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      704 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-drizzle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      365 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      361 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-fog-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      483 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-fog.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      352 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-fog2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-fog2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      656 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-hail-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      786 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-hail.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-haze-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-haze.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-haze2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      497 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-haze2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-lightning-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-lightning-rain-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      863 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-lightning-rain.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-lightning.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      657 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      501 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-moon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      648 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-moon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      747 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      562 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-rain-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-rain-heavy-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      690 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-rain-heavy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      684 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-rain.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      426 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      670 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1266 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-sleet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1393 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-sleet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1509 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-snow-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1650 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-snow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      632 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-sun-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      778 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-sun.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      520 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-upload-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      806 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud-upload.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      597 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloud.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clouds-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      559 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/clouds.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      239 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloudy-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      370 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cloudy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      455 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/code-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/code-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      337 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/code.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      776 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/coin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      364 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/collection-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      438 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/collection-play-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      534 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/collection-play.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/collection.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      472 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/columns-gap.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      271 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/columns.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/command.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      307 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/compass-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/compass.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      533 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cone-striped.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      236 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cone.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1667 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/controller.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      693 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cookie.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/copy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      795 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cpu-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      887 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cpu.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      326 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card-2-back-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      407 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card-2-back.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      497 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card-2-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card-2-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      305 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      383 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/credit-card.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/crop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/crosshair.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/crosshair2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cup-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2113 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cup-hot-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2203 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cup-hot.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1081 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cup-straw.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      470 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cup.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      840 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-bitcoin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-dollar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      494 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-euro.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1031 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-exchange.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      504 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-pound.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-rupee.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/currency-yen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cursor-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      694 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cursor-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/cursor.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1662 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-circle-dotted.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      231 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      289 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      225 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1435 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-square-dotted.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      268 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      360 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      200 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1257 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1293 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1214 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1305 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1276 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1096 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1132 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1053 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1144 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1130 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1569 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1152 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1127 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1143 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1193 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1097 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1730 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1239 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1288 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1304 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1339 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1211 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/database.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      644 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/device-hdd-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      736 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/device-hdd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      588 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/device-ssd-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      660 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/device-ssd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diagram-2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      789 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diagram-2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      668 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diagram-3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      993 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diagram-3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      312 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diamond-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diamond-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/diamond.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      262 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-1-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      318 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      306 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      422 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-4-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      462 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      431 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-5-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      502 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-5.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      474 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-6-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      542 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dice-6.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      340 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/disc-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/disc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1149 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/discord.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      277 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/display-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      570 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/display.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      345 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/displayport-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      378 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/displayport.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/distribute-horizontal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/distribute-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      268 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/door-closed-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      288 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/door-closed.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/door-open-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      428 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/door-open.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      185 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dot.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      422 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/download.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      811 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dpad-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1085 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dpad.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      997 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dribbble.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/dropbox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/droplet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      624 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/droplet-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      607 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/droplet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1053 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/duffle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1161 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/duffle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ear-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      634 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      868 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/earbuds.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      379 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      405 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      484 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      338 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/easel3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      198 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/egg-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/egg-fried.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/egg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      325 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eject-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      365 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eject.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      676 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-angry-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      695 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-angry.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      787 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-astonished-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      876 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-astonished.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      585 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-dizzy-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      630 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-dizzy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-expressionless-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      419 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-expressionless.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      482 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-frown-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-frown.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      777 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-grimace-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      775 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-grimace.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      914 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-grin-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      957 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-grin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-heart-eyes-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-heart-eyes.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1157 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-kiss-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1105 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-kiss.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      560 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-laughing-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-laughing.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-neutral-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      423 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-neutral.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      482 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-smile-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      501 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-smile-upside-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-smile-upside-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-smile.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      600 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-sunglasses-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      650 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-sunglasses.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-surprise-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      401 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-surprise.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      846 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-tear-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      905 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-tear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-wink-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      631 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/emoji-wink.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      625 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-arrow-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      570 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      633 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-arrow-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1091 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-at-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1050 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-at.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      626 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      575 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-exclamation-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      349 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      702 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-open-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      750 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-open-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      663 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-open-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-open.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      496 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-paper-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      556 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-paper-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      681 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-paper-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-paper.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      590 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      539 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      631 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      580 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      669 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      618 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/envelope.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      398 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eraser-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eraser.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/escape.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      993 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ethernet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      805 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ev-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1129 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ev-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      657 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ev-station-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      708 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ev-station.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      318 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      429 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-diamond-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      548 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-diamond.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      247 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-octagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      553 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-octagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      354 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      412 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-triangle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      638 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation-triangle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      252 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      291 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exclude.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/explicit-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/explicit.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      350 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/exposure.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eye-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eye-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      797 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eye-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      519 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eye.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      459 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eyedropper.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      403 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/eyeglasses.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      435 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/facebook.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1233 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fan.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      450 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      353 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      417 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fast-forward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1164 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/feather.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      383 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/feather2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      366 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-arrow-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      348 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-arrow-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      445 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      473 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-bar-graph-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-bar-graph.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      618 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-binary-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      700 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-binary.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-break-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      367 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-break.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      332 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      426 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-code-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-code.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-diff-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-diff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-arrow-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      446 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      422 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-arrow-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      444 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      549 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-bar-graph-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-bar-graph.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      699 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-binary-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      701 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-binary.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      347 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-break-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-break.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      409 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      498 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-code-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-code.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-diff-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      486 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-diff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      633 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-easel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      636 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-easel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      474 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-excel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-excel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      289 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      481 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-font-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      504 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-font.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      508 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-image-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-image.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      675 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-lock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      682 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      475 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-lock2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      479 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-lock2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      581 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-medical-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      596 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-medical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      343 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      374 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      548 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-music-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-music.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1582 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-pdf-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1535 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-pdf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      410 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-person-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-person.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      401 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-play-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      416 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-play.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-post-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      453 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-post.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-ppt-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      426 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-ppt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      558 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-richtext-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-richtext.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      342 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-ruled-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      353 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-ruled.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      611 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-slides-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      613 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-slides.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-spreadsheet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-spreadsheet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      442 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-word-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      507 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-word.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      474 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      481 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      604 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-zip-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      573 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark-zip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      294 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-earmark.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-easel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      618 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-easel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      393 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-excel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      491 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-excel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      238 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      403 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-font-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      491 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-font.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      438 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-image-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-image.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      597 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-lock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      685 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-lock2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      476 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-lock2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      505 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-medical-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      577 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-medical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      265 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      361 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      473 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-music-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-music.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1510 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-pdf-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1516 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-pdf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-person-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      338 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-person.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      323 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-play-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      401 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-play.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      393 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      345 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-post-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      440 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-post.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      348 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-ppt-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-ppt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      479 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-richtext-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-richtext.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-ruled-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-ruled.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-slides-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      593 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-slides.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      339 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-spreadsheet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      400 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-spreadsheet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-text-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      472 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      412 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-word-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      510 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-word.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      395 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      487 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      528 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-zip-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      566 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file-zip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      281 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/file.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      350 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/files-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/files.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1018 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-aac.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-ai.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1109 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-bmp.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1464 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-cs.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2093 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-css.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1508 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-csv.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1604 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-doc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1708 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-docx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      570 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-exe.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      931 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-gif.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      949 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-heic.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-html.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      787 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-java.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1299 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-jpg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1192 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-js.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1750 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-json.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1262 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-jsx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      553 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-key.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      808 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-m4p.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      705 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-md.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      830 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-mdx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      952 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-mov.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1379 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-mp3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      845 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-mp4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      904 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-otf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      932 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-pdf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      889 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-php.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1194 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-png.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      875 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-ppt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      937 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-pptx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1505 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-psd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-py.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      765 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-raw.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      990 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-rb.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2335 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-sass.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2757 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-scss.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1026 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-sh.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1530 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-sql.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1557 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-svg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      497 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-tiff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1127 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-tsx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      423 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-ttf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-txt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      605 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-wav.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1017 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-woff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1129 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-xls.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1200 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-xlsx.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      558 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-xml.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      527 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filetype-yml.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      354 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/film.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      414 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      330 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      332 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      487 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      327 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/filter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2093 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fingerprint.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fire.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      652 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/flag-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1003 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/flag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      522 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/floppy-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/floppy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      401 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/floppy2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/floppy2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2977 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/flower1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      862 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/flower2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1691 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/flower3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      635 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      428 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      570 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      621 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      595 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-symlink-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      708 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-symlink.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      684 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      527 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      619 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder2-open.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/folder2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      348 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fonts.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/forward-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      482 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/forward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      322 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      909 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fuel-pump-diesel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      943 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fuel-pump-diesel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      628 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fuel-pump-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      682 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fuel-pump.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      540 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fullscreen-exit.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      536 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/fullscreen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      310 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/funnel-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/funnel.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      811 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gear-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1244 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gear-wide-connected.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1075 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gear-wide.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1507 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      479 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gem.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      432 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gender-ambiguous.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gender-female.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      307 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gender-male.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      269 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gender-neuter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      643 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gender-trans.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      234 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/geo-alt-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      463 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/geo-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      893 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/geo-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      920 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/geo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      497 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gift-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gift.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      511 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/git.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      708 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/github.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      471 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gitlab.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      717 2024-05-11 22:56:04.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe-americas.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1285 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe-asia-australia.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      800 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe-central-south-asia.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      826 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe-europe-africa.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1196 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1618 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/globe2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/google-play.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/google.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      566 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/gpu-card.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      401 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/graph-down-arrow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/graph-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      399 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/graph-up-arrow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/graph-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-1x2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-1x2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      561 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x2-gap-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      628 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x2-gap.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      764 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x3-gap-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      875 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x3-gap.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      428 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-3x3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      856 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grid.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      475 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grip-horizontal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      475 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/grip-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      246 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/h-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      277 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/h-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      283 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/h-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      364 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/h-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hammer.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-index-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-index-thumb-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1048 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-index-thumb.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1073 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-index.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      829 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-thumbs-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1563 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-thumbs-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      825 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-thumbs-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1591 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hand-thumbs-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/handbag-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      512 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/handbag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      815 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-network-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      595 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-network.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      445 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-rack-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      600 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-rack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      429 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-stack-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      597 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd-stack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      578 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdd.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      377 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdmi-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      416 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hdmi.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      303 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/headphones.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      502 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/headset-vr.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/headset.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      492 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart-arrow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      241 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      542 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart-pulse-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      806 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart-pulse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      458 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      290 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heartbreak-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      649 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heartbreak.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hearts.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heptagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      413 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heptagon-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      437 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/heptagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hexagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hexagon-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      331 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hexagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      592 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/highlighter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/highlights.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1067 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hospital-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1115 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hospital.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      619 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hourglass-bottom.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hourglass-split.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      617 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hourglass-top.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      700 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hourglass.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      544 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-add-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      542 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      580 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      556 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      501 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      477 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-door-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-door.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      592 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-exclamation-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      539 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1137 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-gear-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      993 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      571 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-lock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      571 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      592 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      627 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      415 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/house.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      535 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/houses-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      583 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/houses.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      346 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hr.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      343 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hurricane.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1342 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/hypnotize.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/image-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/image-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/image.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      516 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/images.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      462 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/inbox-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      560 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/inbox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      666 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/inboxes-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      865 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/inboxes.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      969 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/incognito.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      399 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/indent.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/infinity.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      427 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      452 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/info.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      876 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/input-cursor-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      398 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/input-cursor.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1596 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/instagram.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/intersect.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      631 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-album.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      675 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      677 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      605 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-bookmark-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      649 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-bookmark.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      658 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      763 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-code.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      864 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-medical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      593 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      643 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      809 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-richtext.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      748 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-text.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      719 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/journals.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      591 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/joystick.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      413 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/justify-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      415 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/justify-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      410 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/justify.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/kanban-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      513 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/kanban.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      283 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/key-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      628 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/key.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1831 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/keyboard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1856 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/keyboard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      299 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ladder.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1078 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lamp-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1140 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lamp.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      266 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/laptop-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/laptop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      537 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layer-backward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      533 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layer-forward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      399 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layers-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layers-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layers.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-sidebar-inset-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      380 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-sidebar-inset.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      314 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-sidebar-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      303 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-sidebar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      307 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-split.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-text-sidebar-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      501 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-text-sidebar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      503 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-text-window-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      494 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-text-window.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-three-columns.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      471 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/layout-wtf.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      529 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/life-preserver.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightbulb-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      519 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightbulb-off-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightbulb-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightbulb.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightning-charge-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightning-charge.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      294 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightning-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      383 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lightning.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1597 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/line.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/link-45deg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/link.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      666 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/linkedin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      701 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1117 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-columns-reverse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1119 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-columns.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      347 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-nested.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      973 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-ol.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1318 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-stars.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      627 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-task.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      441 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list-ul.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/list.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      271 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      334 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      674 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/luggage-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      737 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/luggage.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      886 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lungs-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1351 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/lungs.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      742 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/magic.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      222 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/magnet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      274 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/magnet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      512 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mailbox-flag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mailbox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mailbox2-flag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      472 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mailbox2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      449 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/map-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/map.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      469 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/markdown-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      656 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/markdown.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      449 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/marker-tip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mask.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      952 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mastodon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      483 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/medium.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      559 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/megaphone-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      750 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/megaphone.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      625 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/memory.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-app-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      589 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-app.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-button-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      654 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-button-wide-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      777 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-button-wide.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      708 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-button.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      590 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      588 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/menu-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      586 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/messenger.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      856 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/meta.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mic-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      526 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mic-mute-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mic-mute.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mic.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      768 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/microsoft-teams.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      236 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/microsoft.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      774 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/minecart-loaded.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      433 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/minecart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/modem-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      584 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/modem.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      906 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/moisture.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/moon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      982 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/moon-stars-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1154 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/moon-stars.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      566 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/moon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      492 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mortarboard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      605 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mortarboard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      846 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/motherboard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      947 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/motherboard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      228 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      293 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      623 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      874 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/mouse3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      423 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/music-note-beamed.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      555 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/music-note-list.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      335 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/music-note.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      376 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/music-player-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/music-player.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      600 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/newspaper.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1314 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nintendo-switch.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/node-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      455 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/node-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      379 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/node-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      500 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/node-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1644 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/noise-reduction.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      352 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nut-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nut.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      885 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nvidia.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      569 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nvme-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      672 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/nvme.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      386 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/octagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      414 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/octagon-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      425 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/octagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      479 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/opencollective.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/optical-audio-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      630 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/optical-audio.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      330 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/option.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      765 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/outlet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      356 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/p-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/p-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/p-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      469 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/p-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/paint-bucket.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      464 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/palette-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      789 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/palette.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      475 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/palette2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      305 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/paperclip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      259 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/paragraph.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      346 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pass-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      487 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pass.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/passport-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      499 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/passport.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      608 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1040 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      633 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-exclamation-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1005 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      545 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      977 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      596 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1027 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      897 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-question-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1304 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/patch-question.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      358 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      345 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      287 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      259 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pause.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      858 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/paypal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pc-display-horizontal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      509 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pc-display.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pc-horizontal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      601 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pci-card-network.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      991 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pci-card-sound.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      383 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pci-card.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      327 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/peace-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      375 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/peace.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pen-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      528 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      562 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pencil-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      575 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pencil-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      522 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pencil.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pentagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      380 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pentagon-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      473 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pentagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      361 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/people-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      698 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/people.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/percent.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      529 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      573 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-arms-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-badge-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-badge.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      631 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-bounding-box.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      388 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      565 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      323 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      577 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      546 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      431 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-add.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      479 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      450 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      888 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      409 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      447 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      513 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      222 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      983 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-gear.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      302 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-hearts.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      403 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-lines-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      374 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-raised-hand.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      567 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-rolodex.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      483 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-standing-dress.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-standing.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      519 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-vcard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      581 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-vcard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      407 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-video.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      459 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-video2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      438 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-video3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      705 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-walking.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      607 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-wheelchair.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      437 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-workspace.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      375 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/person.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      251 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1114 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-flip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      265 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-landscape-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      345 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-landscape.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      812 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-vibrate-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      958 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone-vibrate.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      330 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/phone.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      272 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pie-chart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      308 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pie-chart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1103 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/piggy-bank-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1544 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/piggy-bank.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      592 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin-angle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      986 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin-angle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin-map-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      447 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin-map.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      863 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      780 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pinterest.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      327 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pip-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      419 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/pip.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      299 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      376 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      266 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      272 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      278 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/play.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      787 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/playstation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      612 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plug-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      661 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plug.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      526 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plugin.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1707 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-circle-dotted.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      333 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      267 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      381 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-slash-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1476 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-square-dotted.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      313 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      244 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      643 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postage-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      699 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postage-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      630 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postage-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      674 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postage.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postcard-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postcard-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      547 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postcard-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      616 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/postcard.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      261 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/power.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/prescription.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      374 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/prescription2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/printer-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      553 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/printer.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/projector-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      480 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/projector.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1374 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/puzzle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2542 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/puzzle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      713 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/qr-code-scan.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      545 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/qr-code.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      673 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      715 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      782 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-diamond-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      922 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-diamond.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      654 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      876 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-octagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      927 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-octagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      713 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      786 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      626 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/question.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      699 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/quora.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      582 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/quote.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/r-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      408 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/r-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      431 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/r-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/r-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/radar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/radioactive.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      455 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rainbow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1223 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/receipt-cutoff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1719 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/receipt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      386 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reception-0.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      406 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reception-1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      426 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reception-2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      446 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reception-3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      467 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reception-4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      257 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      335 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      225 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      268 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      205 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      212 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      266 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      261 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/record2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      758 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/recycle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      984 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reddit.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      602 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/regex.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      580 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/repeat-1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/repeat.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      493 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reply-all-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      967 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reply-all.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      289 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reply-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      761 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/reply.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      446 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      365 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      411 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      389 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rewind.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      996 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/robot.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      896 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rocket-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1011 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rocket-takeoff-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1613 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rocket-takeoff.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1416 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rocket.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      868 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/router-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      946 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/router.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      391 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rss-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      499 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rss.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/rulers.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      690 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/safe-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      799 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/safe.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      959 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/safe2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1041 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/safe2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/save-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      437 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/save.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/save2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      416 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/save2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      415 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/scissors.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      489 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/scooter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      502 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/screwdriver.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sd-card-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      633 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sd-card.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      408 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/search-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      423 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/search-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      315 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/search.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      273 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/segmented-nav.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      665 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-arrow-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      608 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-arrow-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      663 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-arrow-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-arrow-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      601 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-check-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      552 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      519 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-dash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      470 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      543 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-exclamation-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      494 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      390 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      565 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      516 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      557 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      644 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      595 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      360 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/send.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      634 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/server.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      464 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shadows.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/share-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      440 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/share.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1064 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1047 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      639 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill-check.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      660 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill-exclamation.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      582 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      632 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      693 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      512 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      653 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-lock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1057 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-lock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      999 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1048 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      755 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-shaded.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      966 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1125 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      919 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shield.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      293 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shift-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shift.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      854 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shop-window.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      877 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      881 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/shuffle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      986 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-dead-end-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1121 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-dead-end.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1425 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-do-not-enter-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1456 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-do-not-enter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      347 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-side-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      488 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-side.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      337 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-t-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      481 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-t.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      387 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-y-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection-y.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      500 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-intersection.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      523 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-merge-left-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      658 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-merge-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      516 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-merge-right-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      680 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-merge-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      457 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-left-turn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      476 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-left-turn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      465 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-parking-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      489 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-parking.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      445 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-right-turn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-no-right-turn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      849 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-railroad-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      932 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-railroad.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1246 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-stop-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      482 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-stop-lights-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      611 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-stop-lights.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1340 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-stop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      454 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-left-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      615 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      459 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-right-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      614 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      511 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-slight-left-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      660 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-slight-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      496 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-slight-right-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      659 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-turn-slight-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      608 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-yield-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      906 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sign-yield.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1496 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      432 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost-2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      450 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost-2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      334 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      328 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost-split-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      363 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost-split.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      333 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/signpost.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      533 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sim-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      623 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sim-slash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      710 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sim-slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      655 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sim.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1297 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sina-weibo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      483 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      449 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-backward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      331 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      298 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      374 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      280 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      303 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-end.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      481 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      449 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      400 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      441 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-forward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      410 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      311 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      376 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      280 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      304 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skip-start.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1392 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/skype.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      971 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      251 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      312 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      251 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      287 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      224 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/slash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      485 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sliders.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      603 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sliders2-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      602 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sliders2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/smartwatch.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2370 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/snapchat.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      952 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/snow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1530 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/snow2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1104 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/snow3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      545 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-alpha-down-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-alpha-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      538 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-alpha-up-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-alpha-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      462 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-down-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      763 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-numeric-down-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      774 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-numeric-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      756 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-numeric-up-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      767 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-numeric-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-up-alt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      453 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sort-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      573 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/soundwave.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      949 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sourceforge.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/speaker-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/speaker.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      697 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/speedometer.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      866 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/speedometer2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1143 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/spellcheck.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      609 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/spotify.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      220 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      260 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/square-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      284 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      443 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stack-overflow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      606 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      399 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/star-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      617 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/star-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      623 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/star.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      998 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stars.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      826 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/steam.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stickies-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      518 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stickies.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      376 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sticky-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      416 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sticky.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop-btn-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      396 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop-btn.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      329 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      247 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      320 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      505 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stoplights-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stoplights.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      444 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stopwatch-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      487 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stopwatch.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      261 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/strava.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      568 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/stripe.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      478 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/subscript.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      223 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/substack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/subtract.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      367 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-club-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      980 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-club.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      270 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-diamond-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      424 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-diamond.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      316 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-heart-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      812 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-heart.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      434 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-spade-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      944 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suit-spade.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      462 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      383 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase-lg-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      468 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      586 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      360 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/suitcase2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      779 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sun-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      806 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sun.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      497 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sunglasses.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      649 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sunrise-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      685 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sunrise.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      650 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sunset-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      686 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/sunset.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      477 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/superscript.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/symmetry-horizontal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      344 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/symmetry-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      350 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/table.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      252 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tablet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      263 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tablet-landscape-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      341 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tablet-landscape.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      331 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tablet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      309 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tag-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tag.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      430 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tags-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      490 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tags.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      907 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/taxi-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1264 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/taxi-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      711 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telegram.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      521 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      679 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-forward-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      998 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-forward.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      660 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-inbound-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      979 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-inbound.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      588 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-minus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      942 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-minus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      659 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-outbound-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      978 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-outbound.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      638 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-plus-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      992 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      722 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-x-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1077 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      840 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/telephone.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1670 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tencent-qq.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      598 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      355 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      644 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      648 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal-split.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      723 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      454 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/terminal.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      412 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-center.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      512 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-indent-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      495 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-indent-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      408 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-left.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      413 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-paragraph.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      411 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-right.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      475 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/text-wrap.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      508 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/textarea-resize.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      710 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/textarea-t.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      492 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/textarea.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      394 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer-high.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      393 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer-low.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      816 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer-snow.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      828 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer-sun.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      350 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thermometer.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1061 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/threads-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      901 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/threads.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      282 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/three-dots-vertical.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      272 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/three-dots.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      382 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thunderbolt-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      429 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/thunderbolt.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      529 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket-detailed-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      666 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket-detailed.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      359 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      496 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket-perforated-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      640 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket-perforated.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      489 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ticket.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      275 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tiktok.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      284 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggle-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      218 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggle-on.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      296 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggle2-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      276 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggle2-on.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      393 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggles.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      431 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/toggles2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      922 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tools.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2177 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tornado.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      762 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-freight-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      915 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-freight-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      728 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      929 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1387 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-lightrail-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1562 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/train-lightrail-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      762 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/translate.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      692 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/transparency.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      441 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      539 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      503 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash2-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      418 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      577 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash3-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      656 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trash3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tree-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      579 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tree.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      511 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trello.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      286 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/triangle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      414 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/triangle-half.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      510 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/triangle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      607 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trophy-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      919 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/trophy.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      411 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tropical-storm.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      514 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/truck-flatbed.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/truck-front-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      809 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/truck-front.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      636 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/truck.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1785 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tsunami.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      255 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tv-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      614 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/tv.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      334 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/twitch.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      301 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/twitter-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      586 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/twitter.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      465 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-bold.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      254 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      460 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      623 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h3.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      335 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h4.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      516 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h5.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      630 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-h6.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-italic.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      574 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-strikethrough.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      319 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type-underline.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      619 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/type.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      740 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ubuntu.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      725 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ui-checks-grid.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      748 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ui-checks.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      487 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ui-radios-grid.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/ui-radios.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1171 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/umbrella-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1614 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/umbrella.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      402 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/unindent.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      249 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/union.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      583 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/unity.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      506 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/universal-access-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      400 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/universal-access.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      285 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/unlock-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      347 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/unlock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      762 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/upc-scan.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      371 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/upc.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      419 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/upload.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      228 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-c-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      288 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-c.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      298 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-drive-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      347 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-drive.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      333 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      375 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-micro-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      415 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-micro.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      368 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-mini-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      456 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-mini.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      438 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-plug-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      571 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-plug.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      660 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb-symbol.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/usb.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      692 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/valentine.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      681 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/valentine2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      524 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vector-pen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      408 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/view-list.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      428 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/view-stacked.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      755 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vignette.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      523 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vimeo.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      295 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vinyl-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      338 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vinyl.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1015 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/virus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      999 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/virus2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      307 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/voicemail.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      384 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-down-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      458 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-down.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      489 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-mute-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      551 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-mute.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      291 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-off-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      357 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      693 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-up-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      750 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/volume-up.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      364 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/vr.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wallet-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      369 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wallet.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      404 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wallet2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      525 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/watch.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1813 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/water.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      576 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/webcam-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      590 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/webcam.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1021 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wechat.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1189 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/whatsapp.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      486 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wifi-1.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      694 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wifi-2.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      945 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wifi-off.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      911 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wifi.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1291 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wikipedia.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      421 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wind.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      537 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-dash.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      532 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-desktop.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      559 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-dock.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      385 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-fullscreen.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      583 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-plus.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      436 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-sidebar.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      439 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-split.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      517 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-stack.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      662 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window-x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      419 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/window.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      266 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/windows.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1142 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wordpress.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      649 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wrench-adjustable-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      645 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wrench-adjustable-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      630 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wrench-adjustable.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      521 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/wrench.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      351 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-circle-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      420 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-circle.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      463 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-diamond-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      619 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-diamond.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      308 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-lg.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      559 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-octagon-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      632 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-octagon.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      397 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-square-fill.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      491 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x-square.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      331 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/x.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1252 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/xbox.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2422 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/yelp.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      386 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/yin-yang.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      893 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/youtube.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      531 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/zoom-in.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      484 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/icons/zoom-out.svg
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     3517 2024-05-11 22:56:03.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/node_modules/bootstrap-icons/package.json
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1823 2024-05-11 22:56:05.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/package-lock.json
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      563 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/package.json
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.802537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1124 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/400.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1133 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/403.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1107 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/404.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1400 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/base.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     8157 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/macros.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.802537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/setup/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2863 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/setup/setup.html
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.803537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/transaccion/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     2723 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/transaccion/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.803537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/validaciones/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1243 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/validaciones/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.803537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ventas/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1048 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ventas/__init__.py
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.804537 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ventas/templates/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      325 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ventas/templates/ventas.html
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      934 2024-05-11 22:56:23.000000 staging_cacao_accounting-0.0.1b20240512/cacao_accounting/version.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1558 2024-05-11 22:50:08.000000 staging_cacao_accounting-0.0.1b20240512/pyproject.toml
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      248 2024-05-11 22:54:27.000000 staging_cacao_accounting-0.0.1b20240512/requirements.txt
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      187 2024-05-11 22:56:51.812537 staging_cacao_accounting-0.0.1b20240512/setup.cfg
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.809537 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)    18934 2024-05-11 22:56:48.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)   181586 2024-05-11 22:56:50.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)        1 2024-05-11 22:56:48.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       54 2024-05-11 22:56:48.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/entry_points.txt
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)      217 2024-05-11 22:56:48.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/requires.txt
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       17 2024-05-11 22:56:48.000000 staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 wmoreno   (1000) wmoreno   (1000)        0 2024-05-11 22:56:51.809537 staging_cacao_accounting-0.0.1b20240512/tests/
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)       46 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/tests/test_basicos.py
+-rw-r--r--   0 wmoreno   (1000) wmoreno   (1000)     1070 2024-05-11 04:36:23.000000 staging_cacao_accounting-0.0.1b20240512/wsgi.py
```

### Comparing `staging_cacao_accounting-0.0.1b20240511/Dockerfile` & `staging_cacao_accounting-0.0.1b20240512/Dockerfile`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/LICENSE` & `staging_cacao_accounting-0.0.1b20240512/LICENSE`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/Licencias_de_Terceros.md` & `staging_cacao_accounting-0.0.1b20240512/Licencias_de_Terceros.md`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/PKG-INFO` & `staging_cacao_accounting-0.0.1b20240512/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging-cacao-accounting
-Version: 0.0.1b20240511
+Version: 0.0.1b20240512
 Summary: Accounting solution for the management of Accounts Payable, Accounts Receivable, Inventory, Treasury and General Accounting.
 Author-email: William Moreno Reyes <williamjmorenor@gmail.com>, BMO Soluciones <development@bmogroup.solutions>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `staging_cacao_accounting-0.0.1b20240511/README.md` & `staging_cacao_accounting-0.0.1b20240512/README.md`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/I18N.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/I18N.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/__main__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/__main__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/admin/registros/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/admin/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ajax/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ajax/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/app/templates/development.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/app/templates/development.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/forms.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/forms.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/permisos.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/permisos.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/registros/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/roles.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/roles.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/templates/login.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/auth/templates/test_roles.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/auth/templates/test_roles.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/bancos/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/bancos/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/cli.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/cli.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/compras/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/compras/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/config.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/config.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/auxiliares.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/auxiliares.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/ctas/catalogos/base.csv` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/ctas/catalogos/base.csv`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/forms.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/forms.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/ccosto.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/ccosto.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/cuenta.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/cuenta.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/entidad.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/entidad.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/moneda.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/moneda.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/periodo.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/periodo.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/proyecto.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/proyecto.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/tasa_cambio.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/tasa_cambio.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/registros/unidad.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/registros/unidad.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/contabilidad/templates/contabilidad.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/contabilidad/templates/contabilidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/database/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/database/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/database/helpers.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/database/helpers.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/base/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/base/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/datos/dev/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/datos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/decorators.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/decorators.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/exceptions/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/exceptions/mensajes.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/exceptions/mensajes.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/inventario/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/inventario/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/loggin.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/loggin.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/metadata.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/metadata.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/misc/ejemplos/cacao-accounting.unit` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/misc/ejemplos/cacao-accounting.unit`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/modulos.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/modulos.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/registro/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/registro/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/server.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/server.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/dashboard.css` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/purecss-treeview.css` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/purecss-treeview.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/css/signin.css` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/manifest.json` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/manifest.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Cacao Accounting SVG.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Cacao Accounting SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Cacao Accounting-01.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Cacao Accounting-01.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting-01.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting-01.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Web/Cacao Accounting.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Web/Cacao Accounting.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/brand.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/brand.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting _logo.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting _logo.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting _logo.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting _logo.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_accounting.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_accounting.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/cacao_logo.svg` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/cacao_logo.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-144x144.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-192x192.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-36x36.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-48x48.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-72x72.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/android-icon-96x96.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-114x114.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-120x120.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-144x144.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-152x152.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-180x180.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-57x57.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-60x60.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-72x72.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-76x76.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon-precomposed.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/apple-icon.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/apple-icon.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-16x16.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-32x32.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon-96x96.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/favicon.ico` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-144x144.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-150x150.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-310x310.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon/ms-icon-70x70.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon-16x16.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/media/favicon-32x32.png` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/media/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/package-lock.json` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/static/package.json` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/static/package.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/400.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/400.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/403.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/403.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/404.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/404.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/base.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/base.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/macros.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/macros.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/templates/setup/setup.html` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/templates/setup/setup.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/transaccion/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/transaccion/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/validaciones/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/validaciones/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/ventas/__init__.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/ventas/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/cacao_accounting/version.py` & `staging_cacao_accounting-0.0.1b20240512/cacao_accounting/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 
 APPNAME = "Cacao Accounting"
 APPAUTHOR = "William Moreno Reyes"
 MAYOR = "0"
 MENOR = "0"
 PATCH = "1"
-DATE = "20240511"
+DATE = "20240512"
 PRERELEASE = "b" + DATE
 VERSION = MAYOR + "." + MENOR + "." + PATCH + "." + PRERELEASE
```

### Comparing `staging_cacao_accounting-0.0.1b20240511/pyproject.toml` & `staging_cacao_accounting-0.0.1b20240512/pyproject.toml`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1b20240511/staging_cacao_accounting.egg-info/PKG-INFO` & `staging_cacao_accounting-0.0.1b20240512/staging_cacao_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging-cacao-accounting
-Version: 0.0.1b20240511
+Version: 0.0.1b20240512
 Summary: Accounting solution for the management of Accounts Payable, Accounts Receivable, Inventory, Treasury and General Accounting.
 Author-email: William Moreno Reyes <williamjmorenor@gmail.com>, BMO Soluciones <development@bmogroup.solutions>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `staging_cacao_accounting-0.0.1b20240511/wsgi.py` & `staging_cacao_accounting-0.0.1b20240512/wsgi.py`

 * *Files identical despite different names*

