# Comparing `tmp/expr_codegen-0.6.4.tar.gz` & `tmp/expr_codegen-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expr_codegen-0.6.4.tar", last modified: Sat May 11 10:31:00 2024, max compression
+gzip compressed data, was "expr_codegen-0.6.5.tar", last modified: Sun May 12 13:30:20 2024, max compression
```

## Comparing `expr_codegen-0.6.4.tar` & `expr_codegen-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.048317 expr_codegen-0.6.4/expr_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/expr_codegen/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/latex/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/expr_codegen/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/pandas/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/pandas/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/pandas/template.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/expr_codegen/polars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/polars/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/polars/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/polars/template.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/expr_codegen/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/expr_codegen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-11 10:31:00.000000 expr_codegen-0.6.4/expr_codegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-11 10:31:00.000000 expr_codegen-0.6.4/expr_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:31:00.000000 expr_codegen-0.6.4/expr_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 10:31:00.000000 expr_codegen-0.6.4/expr_codegen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 10:31:00.000000 expr_codegen-0.6.4/expr_codegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 10:30:55.000000 expr_codegen-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:31:00.052317 expr_codegen-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/expr_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/expr_codegen/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/latex/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/expr_codegen/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/pandas/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/pandas/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/pandas/template.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/expr_codegen/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/polars/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/polars/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/polars/template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/expr_codegen/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/expr_codegen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-05-12 13:30:20.000000 expr_codegen-0.6.5/expr_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-12 13:30:20.000000 expr_codegen-0.6.5/expr_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:30:20.000000 expr_codegen-0.6.5/expr_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 13:30:20.000000 expr_codegen-0.6.5/expr_codegen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 13:30:20.000000 expr_codegen-0.6.5/expr_codegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-12 13:30:16.000000 expr_codegen-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:30:20.607822 expr_codegen-0.6.5/setup.cfg
```

### Comparing `expr_codegen-0.6.4/LICENSE` & `expr_codegen-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/PKG-INFO` & `expr_codegen-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.4
+Version: 0.6.5
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
@@ -71,27 +71,54 @@
 
 https://exprcodegen.streamlit.app
 
 初级用户可以直接访问此链接进行表达式转译，不需要另外安装软件。(此工具免费部署在国外，打开可能有些慢)
 
 更完整示例访问[alpha_examples](https://github.com/wukan1986/alpha_examples)
 
-## 使用方法
+## 使用示例
 
-运行`demo_cn.py`生成`output.py`，将此文件复制到其它项目中直接`import`使用即可。一般生成的文件不需要再修改。
+```python
+from expr_codegen.tool import codegen_exec
+
+
+def _code_block_():
+    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+
+    # 会在生成的代码中自动导入
+    from polars_ta.wq import cs_mad_zscore_resid
+
+    # 1. 下划线开头的变量只是中间变量，最终输出时会被剔除
+    _a = ts_returns(CLOSE, 1)
+    _b = ts_sum(min_(_a, 0) ** 2, 20)
+    _c = ts_sum(max_(_a, 0) ** 2, 20)
+    _d = ts_sum(_a ** 2, 20)
+    _e = (_b - _c) / _d
+    # 2. 下划线开头的变量可以重复使用。 多个复杂因子多行书写时有重复中间变时不再冲突
+    # 3. 下划线开头的变量循环赋值。 在调试时可快速用注释进行切换了
+    _e = cs_mad_zscore_resid(_e, LOG_MC_ZS, ONE)
+    RSJ = _e
+
+
+df = None  # 替换成真实的polars数据
+df = codegen_exec(_code_block_, df, output_file="output.py")
+
+
+```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
 ├─data
 │      prepare_date.py # 准备数据
 ├─examples
 │      alpha101.txt # WorldQuant Alpha101示例，可复制到`streamlit`应用
 │      demo_cn.py # 中文注释示例。演示如何将表达式转换成代码
+│      demo_express.py # 速成示例
 │      demo_exec_pl.py # 演示调用转换后代码并绘图
 │      demo_transformer.py # 演示将第三方表达式转成内部表达式
 │      output.py # 结果输出。可不修改代码，直接被其它项目导入
 │      show_tree.py # 画表达式树形图。可用于分析对比优化结果
 │      sympy_define.py # 符号定义，由于太多地方重复使用到，所以统一提取到此处
 ├─expr_codegen
 │   │  expr.py # 表达式处理基本函数
```

### Comparing `expr_codegen-0.6.4/README.md` & `expr_codegen-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,27 +21,54 @@
 
 https://exprcodegen.streamlit.app
 
 初级用户可以直接访问此链接进行表达式转译，不需要另外安装软件。(此工具免费部署在国外，打开可能有些慢)
 
 更完整示例访问[alpha_examples](https://github.com/wukan1986/alpha_examples)
 
-## 使用方法
+## 使用示例
 
-运行`demo_cn.py`生成`output.py`，将此文件复制到其它项目中直接`import`使用即可。一般生成的文件不需要再修改。
+```python
+from expr_codegen.tool import codegen_exec
+
+
+def _code_block_():
+    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+
+    # 会在生成的代码中自动导入
+    from polars_ta.wq import cs_mad_zscore_resid
+
+    # 1. 下划线开头的变量只是中间变量，最终输出时会被剔除
+    _a = ts_returns(CLOSE, 1)
+    _b = ts_sum(min_(_a, 0) ** 2, 20)
+    _c = ts_sum(max_(_a, 0) ** 2, 20)
+    _d = ts_sum(_a ** 2, 20)
+    _e = (_b - _c) / _d
+    # 2. 下划线开头的变量可以重复使用。 多个复杂因子多行书写时有重复中间变时不再冲突
+    # 3. 下划线开头的变量循环赋值。 在调试时可快速用注释进行切换了
+    _e = cs_mad_zscore_resid(_e, LOG_MC_ZS, ONE)
+    RSJ = _e
+
+
+df = None  # 替换成真实的polars数据
+df = codegen_exec(_code_block_, df, output_file="output.py")
+
+
+```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
 ├─data
 │      prepare_date.py # 准备数据
 ├─examples
 │      alpha101.txt # WorldQuant Alpha101示例，可复制到`streamlit`应用
 │      demo_cn.py # 中文注释示例。演示如何将表达式转换成代码
+│      demo_express.py # 速成示例
 │      demo_exec_pl.py # 演示调用转换后代码并绘图
 │      demo_transformer.py # 演示将第三方表达式转成内部表达式
 │      output.py # 结果输出。可不修改代码，直接被其它项目导入
 │      show_tree.py # 画表达式树形图。可用于分析对比优化结果
 │      sympy_define.py # 符号定义，由于太多地方重复使用到，所以统一提取到此处
 ├─expr_codegen
 │   │  expr.py # 表达式处理基本函数
```

### Comparing `expr_codegen-0.6.4/expr_codegen/codes.py` & `expr_codegen-0.6.5/expr_codegen/codes.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/dag.py` & `expr_codegen-0.6.5/expr_codegen/dag.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/expr.py` & `expr_codegen-0.6.5/expr_codegen/expr.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/latex/printer.py` & `expr_codegen-0.6.5/expr_codegen/latex/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/model.py` & `expr_codegen-0.6.5/expr_codegen/model.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/pandas/code.py` & `expr_codegen-0.6.5/expr_codegen/pandas/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/pandas/printer.py` & `expr_codegen-0.6.5/expr_codegen/pandas/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/pandas/template.py.j2` & `expr_codegen-0.6.5/expr_codegen/pandas/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/polars/code.py` & `expr_codegen-0.6.5/expr_codegen/polars/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/polars/printer.py` & `expr_codegen-0.6.5/expr_codegen/polars/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/polars/template.py.j2` & `expr_codegen-0.6.5/expr_codegen/polars/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/expr_codegen/tool.py` & `expr_codegen-0.6.5/expr_codegen/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,8 +259,11 @@
     if isinstance(code_block, str):
         source = code_block
     else:
         source = inspect.getsource(code_block)
 
     codes = _TOOL_._get_codes(source, extra_codes, output_file)
 
-    return _TOOL_.exec(codes, df_input)
+    if df_input is None:
+        return df_input
+    else:
+        return _TOOL_.exec(codes, df_input)
```

### Comparing `expr_codegen-0.6.4/expr_codegen.egg-info/PKG-INFO` & `expr_codegen-0.6.5/expr_codegen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.4
+Version: 0.6.5
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
@@ -71,27 +71,54 @@
 
 https://exprcodegen.streamlit.app
 
 初级用户可以直接访问此链接进行表达式转译，不需要另外安装软件。(此工具免费部署在国外，打开可能有些慢)
 
 更完整示例访问[alpha_examples](https://github.com/wukan1986/alpha_examples)
 
-## 使用方法
+## 使用示例
 
-运行`demo_cn.py`生成`output.py`，将此文件复制到其它项目中直接`import`使用即可。一般生成的文件不需要再修改。
+```python
+from expr_codegen.tool import codegen_exec
+
+
+def _code_block_():
+    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+
+    # 会在生成的代码中自动导入
+    from polars_ta.wq import cs_mad_zscore_resid
+
+    # 1. 下划线开头的变量只是中间变量，最终输出时会被剔除
+    _a = ts_returns(CLOSE, 1)
+    _b = ts_sum(min_(_a, 0) ** 2, 20)
+    _c = ts_sum(max_(_a, 0) ** 2, 20)
+    _d = ts_sum(_a ** 2, 20)
+    _e = (_b - _c) / _d
+    # 2. 下划线开头的变量可以重复使用。 多个复杂因子多行书写时有重复中间变时不再冲突
+    # 3. 下划线开头的变量循环赋值。 在调试时可快速用注释进行切换了
+    _e = cs_mad_zscore_resid(_e, LOG_MC_ZS, ONE)
+    RSJ = _e
+
+
+df = None  # 替换成真实的polars数据
+df = codegen_exec(_code_block_, df, output_file="output.py")
+
+
+```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
 ├─data
 │      prepare_date.py # 准备数据
 ├─examples
 │      alpha101.txt # WorldQuant Alpha101示例，可复制到`streamlit`应用
 │      demo_cn.py # 中文注释示例。演示如何将表达式转换成代码
+│      demo_express.py # 速成示例
 │      demo_exec_pl.py # 演示调用转换后代码并绘图
 │      demo_transformer.py # 演示将第三方表达式转成内部表达式
 │      output.py # 结果输出。可不修改代码，直接被其它项目导入
 │      show_tree.py # 画表达式树形图。可用于分析对比优化结果
 │      sympy_define.py # 符号定义，由于太多地方重复使用到，所以统一提取到此处
 ├─expr_codegen
 │   │  expr.py # 表达式处理基本函数
```

### Comparing `expr_codegen-0.6.4/expr_codegen.egg-info/SOURCES.txt` & `expr_codegen-0.6.5/expr_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.4/pyproject.toml` & `expr_codegen-0.6.5/pyproject.toml`

 * *Files identical despite different names*

