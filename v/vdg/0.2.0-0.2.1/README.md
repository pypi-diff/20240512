# Comparing `tmp/vdg-0.2.0.tar.gz` & `tmp/vdg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdg-0.2.0.tar", last modified: Sat May 11 10:55:39 2024, max compression
+gzip compressed data, was "vdg-0.2.1.tar", last modified: Sat May 11 12:12:39 2024, max compression
```

## Comparing `vdg-0.2.0.tar` & `vdg-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.630514 vdg-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 10:55:36.000000 vdg-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 10:55:36.000000 vdg-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:55:39.630514 vdg-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-11 10:55:36.000000 vdg-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:55:39.630514 vdg-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 10:55:36.000000 vdg-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/html.template
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/main.template
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/titles.template
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:12:39.907454 vdg-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 12:12:36.000000 vdg-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 12:12:36.000000 vdg-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-11 12:12:39.907454 vdg-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-11 12:12:36.000000 vdg-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:12:39.907454 vdg-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-11 12:12:36.000000 vdg-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:12:39.907454 vdg-0.2.1/vdg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:12:39.907454 vdg-0.2.1/vdg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/templates/html.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/templates/main.template
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/templates/titles.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-11 12:12:36.000000 vdg-0.2.1/vdg/templates/yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:12:39.907454 vdg-0.2.1/vdg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-11 12:12:39.000000 vdg-0.2.1/vdg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 12:12:39.000000 vdg-0.2.1/vdg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:12:39.000000 vdg-0.2.1/vdg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:12:39.000000 vdg-0.2.1/vdg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 12:12:39.000000 vdg-0.2.1/vdg.egg-info/top_level.txt
```

### Comparing `vdg-0.2.0/LICENSE` & `vdg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vdg-0.2.0/PKG-INFO` & `vdg-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-Metadata-Version: 2.1
-Name: vdg
-Version: 0.2.0
-Summary: VCB-Studio Draft Generator 发布稿生成器
-Author: diazchika
-Author-email: halberd-civic.0c@icloud.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 # VDG (VCB-S Draft Gen)
 
 ![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)
+[![Deploy to PyPI](https://github.com/diazchika/vdg/actions/workflows/python-publish.yml/badge.svg)](https://github.com/diazchika/vdg/actions/workflows/python-publish.yml)
 
 ## Introduction
 
 主要是使用 Jinja2 对 HTML 模版进行填充以达到生成发布稿的效果。只需要把发布信息填写在 YAML 文件里就可以轻松生成三分发布稿（并不是终稿）✌️。
 
 [生成样品](https://github.com/diazchika/vdg/tree/main/test)
 
@@ -24,24 +14,32 @@
 
 ## Usage
 
 ### 生成新 YAML 文件
 
 `vdg new --path <path>`
 
-会在`<path>`路径下生成 `config.yaml`，里面很多空要填...
+会在`<path>`路径下生成 `config.yaml`，里面很多发布信息要填...
 
 `<path>` 默认为 `config.yaml`
 
 YAML 里具体有什么看[这里](https://github.com/diazchika/vdg/blob/main/vdg/templates/yaml.template)。
 
 ### 生成发布稿件
 
 `vdg gen --path <path-to-yaml>`
 
 会读取`<path-to-yaml>`指定的 yaml 文件，并根据它生成发布稿。
 
 `<path>` 默认为 `config.yaml`
 
+### 其他
+
+`vdg -h`
+
+## 点评
+
+diazchika: 总之就是一道大型填空题
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `vdg-0.2.0/setup.py` & `vdg-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="vdg",
-    version="0.2.0",
+    version="0.2.1",
     author="diazchika",
     author_email="halberd-civic.0c@icloud.com",
     description="VCB-Studio Draft Generator 发布稿生成器",
     long_description=read('README.md'),
     packages=find_packages(),
     include_package_data=True,
     package_data={
@@ -25,8 +25,12 @@
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
+    project_urls={
+        'github': 'https://github.com/diazchika/vdg',
+        'VCB-Studio': 'https:///vcb-s.com',
+    }
 )
```

### Comparing `vdg-0.2.0/vdg/core.py` & `vdg-0.2.1/vdg/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     Generate Markdown release draft.
     :param html_draft_str: HTML 发布稿字符串
     :param comparison_md: Markdown格式的对比图字符串
     :return:
     """
     # Initialize the HTML to Markdown converter
     converter = html2text.HTML2Text()
+    converter.body_width = 0
     converter.ignore_links = True
 
     # Convert HTML to Markdown
     markdown_content = converter.handle(html_draft_str)
 
     # Split the Markdown content at the last occurrence of '* * *' and append the comparison section
     blocks = markdown_content.rsplit('* * *', 1)
@@ -180,15 +181,16 @@
             file.write(titles_content)
     except IOError as exc:
         print(f"Error writing to file: {exc}")
 
     print(f"稿件 诞生在 {output_dir}")
 
 
-def create_yaml_config(destination_path: Union[str, Path], template_path: Union[str, Path] = 'templates/yaml.template') -> None:
+def create_yaml_config(destination_path: Union[str, Path],
+                       template_path: Union[str, Path] = 'templates/yaml.template') -> None:
     """
     复制一份 YAML 模版到 destination_path
 
     Args:
         destination_path (Union[str, Path]): The directory where the config.yaml file will be created.
         template_path (Union[str, Path], optional): The path to the YAML template file. Defaults to 'yaml.template'.
     """
@@ -199,7 +201,28 @@
 
     output_path = Path(destination_path)
     with open(output_path, "w") as f:
         f.write(yaml_str)
 
     # User Prompt
     print(f"config.yaml 诞生在 {output_path}")
+
+
+def generate_links(path_to_yaml) -> None:
+    """Generate drafts based on the provided YAML configuration."""
+    with open(path_to_yaml, "r") as file:
+        release_info = yaml.safe_load(file)
+
+    # project_name = release_info.get("filename")
+    links = release_info.get("BT站链接")
+
+    # output_dir = Path(path_to_yaml).parent
+    # output_dir.mkdir(parents=True, exist_ok=True)
+
+    # file_paths = output_dir / f"{project_name}_links.txt"
+
+    # with file_paths.open("w") as file:
+    for link in links.split('\n'):
+        if link != "":
+            print(f'<a href="{link}" rel="noopener" target="_blank">{link}</a>\n')
+
+    # print(f"Links 诞生在 {output_dir}")
```

### Comparing `vdg-0.2.0/vdg/main.py` & `vdg-0.2.1/vdg/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import argparse
 
-from vdg.core import generate_drafts, create_yaml_config
+from vdg.core import *
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="发布稿生成器。")
     subparsers = parser.add_subparsers(dest='command', required=True)
 
-    parser_new = subparsers.add_parser('new', help='生成新的发布稿模版 YAML。默认在当前目录生成，传 -p/--path <path> 指定路径')
+    parser_new = subparsers.add_parser('new', help='生成新的发布稿模版 YAML。vdg new -h')
     parser_new.add_argument('-p', '--path', type=str, help='YAML文件路径', default='./config.yaml')
 
-    parser_gen = subparsers.add_parser('gen', help='根据YAML生成发布稿。默认当前目录下的 config.yaml，传 -p/--path <path> 指定路径')
+    parser_gen = subparsers.add_parser('gen', help='根据YAML在当前目录下生成发布稿。vdg gen -h')
     parser_gen.add_argument('-p', '--path', type=str, help='YAML文件路径', default='./config.yaml')
+    parser_gen.add_argument('-l', '--links', action='store_true', help='输出方便在主站粘贴的BT站点链接。')
 
     args = parser.parse_args()
 
     return args
 
 
 def main():
     args = parse_args()
 
     if args.command == 'new':
         create_yaml_config(args.path)
-    elif args.command == 'gen':
+    elif args.command == 'gen' and not args.links:
         generate_drafts(args.path)
+    elif args.command == 'gen' and args.links:
+        generate_links(args.path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vdg-0.2.0/vdg/templates/html.template` & `vdg-0.2.1/vdg/templates/html.template`

 * *Files identical despite different names*

### Comparing `vdg-0.2.0/vdg/templates/main.template` & `vdg-0.2.1/vdg/templates/main.template`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,17 @@
 
 <del><a href="https://share.dmhy.org/topics/view/xxxx.html" rel="noopener" target="_blank">https://share.dmhy.org/topics/view/xxxx.html</a></del>
 
 <del><a href="https://nyaa.si/view/xxxxxx" rel="noopener" target="_blank">https://nyaa.si/view/xxxxxx</a></del>
 [/box]
 {% endif %}
 
-<!-- Image Credit: <a href="{{主站图片来源链接}}" rel="noopener" target="_blank">{{主站图片原作者ID}}</a> -->
-
+{% if 主站图片原作者ID %}
+Image Credit: <a href="{{主站图片来源链接}}" rel="noopener" target="_blank">{{主站图片原作者ID}}</a>
+{% endif %}
 <label for="medie-info-switch" class="btn btn-inverse-primary" title="展开MediaInfo">MediaInfo</label>
 
 <pre class="js-medie-info-detail medie-info-detail" style="display: none;">
 {{MediaInfo}}
 </pre>
 
 {% if 重发 %}
```

#### html2text {}

```diff
@@ -11,12 +11,14 @@
 _w_w_w_._a_c_g_n_x_._s_e_/_s_h_o_w_-_x_x_x_x_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_a_c_g_._r_i_p_/_t_/_x_x_x_x_x_x _h_t_t_p_s_:_/_/
 _s_h_a_r_e_._d_m_h_y_._o_r_g_/_t_o_p_i_c_s_/_v_i_e_w_/_x_x_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_n_y_a_a_._s_i_/_v_i_e_w_/_x_x_x_x_x_x [/box] {%
 endif %} {% if éå %}
 ===============================================================================
 æ§åæ§½ [box style="download"] 10-bit 1080p AVC _h_t_t_p_s_:_/_/_b_a_n_g_u_m_i_._m_o_e_/_t_o_r_r_e_n_t_/
 _x_x_x_x_x_x_x_x _h_t_t_p_s_:_/_/_s_h_a_r_e_._a_c_g_n_x_._s_e_/_s_h_o_w_-_x_x_x_x_x_x_x_x_x_x_x_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_w_w_w_._a_c_g_n_x_._s_e_/
 _s_h_o_w_-_x_x_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_a_c_g_._r_i_p_/_t_/_x_x_x_x_x_x _h_t_t_p_s_:_/_/_s_h_a_r_e_._d_m_h_y_._o_r_g_/_t_o_p_i_c_s_/_v_i_e_w_/
-_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_n_y_a_a_._s_i_/_v_i_e_w_/_x_x_x_x_x_x [/box] {% endif %} MediaInfo
+_x_x_x_x_._h_t_m_l _h_t_t_p_s_:_/_/_n_y_a_a_._s_i_/_v_i_e_w_/_x_x_x_x_x_x [/box] {% endif %} {% if
+ä¸»ç«å¾çåä½èID %} Image Credit: _{_{_ä_¸_»_ç_«__å__¾_ç___å___ä_½__è___I_D_}_} {% endif
+%} MediaInfo
 {{MediaInfo}}
 {% if éå %} [box style="info"]
 æ¬é¡µé¢çä½åå·²è¢«æ´æ°çåéæ¿ä»£ï¼è¯·ç§»æ­¥ä¸è½½æ°çï¼ _h_t_t_p_s_:
 _/_/_v_c_b_-_s_._c_o_m_/_a_r_c_h_i_v_e_s_/_x_x_x_x [/box] {% endif %}
```

### Comparing `vdg-0.2.0/vdg/templates/yaml.template` & `vdg-0.2.1/vdg/templates/yaml.template`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 # 画质吐槽
 画质吐槽: |
 画质吐槽英文: |
 
 # 发布吐槽
 发布吐槽: |
 
+BT站链接: |
+
 对比图HTML: |
 对比图MD: |
 
 # SAYA IS ∞ LOLICON!
 MediaInfo: |
 
 # 用于程序运行时添加 HTML 换行符
```

### Comparing `vdg-0.2.0/vdg.egg-info/PKG-INFO` & `vdg-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: vdg
-Version: 0.2.0
+Version: 0.2.1
 Summary: VCB-Studio Draft Generator 发布稿生成器
 Author: diazchika
 Author-email: halberd-civic.0c@icloud.com
+Project-URL: github, https://github.com/diazchika/vdg
+Project-URL: VCB-Studio, https:///vcb-s.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 # VDG (VCB-S Draft Gen)
 
 ![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)
+[![Deploy to PyPI](https://github.com/diazchika/vdg/actions/workflows/python-publish.yml/badge.svg)](https://github.com/diazchika/vdg/actions/workflows/python-publish.yml)
 
 ## Introduction
 
 主要是使用 Jinja2 对 HTML 模版进行填充以达到生成发布稿的效果。只需要把发布信息填写在 YAML 文件里就可以轻松生成三分发布稿（并不是终稿）✌️。
 
 [生成样品](https://github.com/diazchika/vdg/tree/main/test)
 
@@ -24,24 +27,32 @@
 
 ## Usage
 
 ### 生成新 YAML 文件
 
 `vdg new --path <path>`
 
-会在`<path>`路径下生成 `config.yaml`，里面很多空要填...
+会在`<path>`路径下生成 `config.yaml`，里面很多发布信息要填...
 
 `<path>` 默认为 `config.yaml`
 
 YAML 里具体有什么看[这里](https://github.com/diazchika/vdg/blob/main/vdg/templates/yaml.template)。
 
 ### 生成发布稿件
 
 `vdg gen --path <path-to-yaml>`
 
 会读取`<path-to-yaml>`指定的 yaml 文件，并根据它生成发布稿。
 
 `<path>` 默认为 `config.yaml`
 
+### 其他
+
+`vdg -h`
+
+## 点评
+
+diazchika: 总之就是一道大型填空题
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

