# Comparing `tmp/xtn-tools-pro-1.0.0.0.4.tar.gz` & `tmp/xtn-tools-pro-1.0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.4.tar", last modified: Fri May 10 00:04:47 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.5.tar", last modified: Sun May 12 14:23:10 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.0.4.tar` & `xtn-tools-pro-1.0.0.0.5.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0      287 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1210 2024-05-10 00:03:27.000000 xtn-tools-pro-1.0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0     9842 2024-04-27 07:38:44.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     3502 2024-05-10 00:00:28.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools.py
--rw-rw-rw-   0        0        0     1512 2024-04-19 10:21:05.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_flie.py
--rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_time.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-12 14:22:55.000000 xtn-tools-pro-1.0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/MysqlDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0     9842 2024-04-27 07:38:44.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     4457 2024-05-12 08:36:29.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools.py
+-rw-rw-rw-   0        0        0     1517 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools_flie.py
+-rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools_time.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/utils/
+-rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/utils/__init__.py
+-rw-rw-rw-   0        0        0     8146 2024-05-12 11:55:54.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/utils/log.py
+-rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/utils/retry.py
+-rw-rw-rw-   0        0        0     6255 2024-05-12 11:19:21.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/utils/sql.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      613 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 14:23:10.000000 xtn-tools-pro-1.0.0.0.5/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # 说明：
 #    tools
 # History:
 # Date          Author    Version       Modification
 # --------------------------------------------------------------------------------------------------
 # 2024/4/17    xiatn     V00.01.000    新建
 # --------------------------------------------------------------------------------------------------
-import hashlib, json, math
+import hashlib, json, math,re
+from pprint import pformat
 from urllib.parse import urlencode
 
 
 def get_md5_32(s, is_upper=False):
     """
         获取文本的md5值 32位
     :param s: 文本
@@ -124,10 +125,52 @@
     """
     if limit <= 0:
         return 0
     # 根据总条数和limit计算总页数
     total_pages = math.ceil(total / limit)
     return total_pages
 
+def list_to_strtuple(datas):
+    """
+        列表转字符串
+    :param datas: datas: [1, 2]
+    :return: (1, 2) 字符串类型
+    """
+    data_str = str(tuple(datas))
+    data_str = re.sub(",\)$", ")", data_str)
+    return data_str
+
+
+
+
+def dumps_json(data,indent=4,sort_keys=False):
+    """
+        将JSON数据格式化为可打印的字符串
+    :param data:
+    :param indent: 每一级嵌套都使用4个空格进行缩进
+    :param sort_keys: 是否排序
+    :return:
+    """
+    try:
+        if isinstance(data, str):
+            data = get_str_to_json(data)
+
+        data = json.dumps(
+            data,
+            ensure_ascii=False,
+            indent=indent,
+            skipkeys=True,
+            sort_keys=sort_keys,
+            default=str,
+        )
+
+    except Exception as e:
+        data = pformat(data)
+
+    return data
+
+
+def split_image(img):
+    pass
 
 if __name__ == '__main__':
     pass
```

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_flie.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools_flie.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     sanitized_filename = sanitized_filename[:max_length]
     return sanitized_filename
 
 
 if __name__ == '__main__':
     pass
     print(get_file_extension('file/2024-04-19/BOSCH GEX 125-1A/125-1AE砂磨机操作说明书:[1]_jingyan.txt'))
-    print(get_check_filename('file/2024-04-19/BOSCH GEX 125-1A/125-1AE砂磨机操作说明书:[1]_jingyan.txt'))
+    print(get_file_check_filename('file/2024-04-19/BOSCH GEX 125-1A/125-1AE砂磨机操作说明书:[1]_jingyan.txt'))
```

### Comparing `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_time.py` & `xtn-tools-pro-1.0.0.0.5/xtn_tools_pro/tools_time.py`

 * *Files identical despite different names*

