# Comparing `tmp/DebugInfo-9.0.0.tar.gz` & `tmp/DebugInfo-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DebugInfo-9.0.0.tar", last modified: Tue Aug 15 09:23:21 2023, max compression
+gzip compressed data, was "DebugInfo-9.1.0.tar", last modified: Tue Aug 15 10:16:18 2023, max compression
```

## Comparing `DebugInfo-9.0.0.tar` & `DebugInfo-9.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-15 09:23:21.468964 DebugInfo-9.0.0/
--rw-rw-rw-   0        0        0    18431 2023-08-14 01:02:58.000000 DebugInfo-9.0.0/LICENSE
--rw-rw-rw-   0        0        0    11069 2023-08-15 09:23:21.467837 DebugInfo-9.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10472 2023-08-14 04:03:20.000000 DebugInfo-9.0.0/README.md
--rw-rw-rw-   0        0        0      677 2023-08-15 09:22:23.000000 DebugInfo-9.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-15 09:23:21.469461 DebugInfo-9.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-15 09:23:21.436078 DebugInfo-9.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-15 09:23:21.449298 DebugInfo-9.0.0/src/DebugInfo/
--rw-rw-rw-   0        0        0    37670 2023-08-15 09:22:23.000000 DebugInfo-9.0.0/src/DebugInfo/DebugInfo.py
--rw-rw-rw-   0        0        0       70 2023-08-14 01:02:58.000000 DebugInfo-9.0.0/src/DebugInfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-15 09:23:21.463831 DebugInfo-9.0.0/src/DebugInfo.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-08-15 09:23:21.000000 DebugInfo-9.0.0/src/DebugInfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-15 09:23:21.000000 DebugInfo-9.0.0/src/DebugInfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-15 09:23:21.000000 DebugInfo-9.0.0/src/DebugInfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-15 09:23:21.000000 DebugInfo-9.0.0/src/DebugInfo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-15 10:16:18.012794 DebugInfo-9.1.0/
+-rw-rw-rw-   0        0        0    18431 2023-08-14 01:02:58.000000 DebugInfo-9.1.0/LICENSE
+-rw-rw-rw-   0        0        0    11069 2023-08-15 10:16:18.011866 DebugInfo-9.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10472 2023-08-14 04:03:20.000000 DebugInfo-9.1.0/README.md
+-rw-rw-rw-   0        0        0      677 2023-08-15 10:15:10.000000 DebugInfo-9.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-15 10:16:18.012794 DebugInfo-9.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-15 10:16:17.970345 DebugInfo-9.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-15 10:16:17.983358 DebugInfo-9.1.0/src/DebugInfo/
+-rw-rw-rw-   0        0        0    38045 2023-08-15 10:15:10.000000 DebugInfo-9.1.0/src/DebugInfo/DebugInfo.py
+-rw-rw-rw-   0        0        0       70 2023-08-14 01:02:58.000000 DebugInfo-9.1.0/src/DebugInfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-15 10:16:17.992329 DebugInfo-9.1.0/src/DebugInfo.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-08-15 10:16:17.000000 DebugInfo-9.1.0/src/DebugInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-15 10:16:17.000000 DebugInfo-9.1.0/src/DebugInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-15 10:16:17.000000 DebugInfo-9.1.0/src/DebugInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-15 10:16:17.000000 DebugInfo-9.1.0/src/DebugInfo.egg-info/top_level.txt
```

### Comparing `DebugInfo-9.0.0/LICENSE` & `DebugInfo-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DebugInfo-9.0.0/PKG-INFO` & `DebugInfo-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DebugInfo
-Version: 9.0.0
+Version: 9.1.0
 Summary: 封装提供了一些调试常用方法，例如打印对齐，彩色文本，表格输出等
 Author-email: douyaoyuan <douyaoyuan@126.com>
 Project-URL: Homepage, https://gitee.com/DyyYq/DebugInfo.git
 Project-URL: Bug Tracker, https://gitee.com/DyyYq/DebugInfo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `DebugInfo-9.0.0/README.md` & `DebugInfo-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `DebugInfo-9.0.0/pyproject.toml` & `DebugInfo-9.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DebugInfo"
-version = "9.0.0"
+version = "9.1.0"
 authors = [
   { name="douyaoyuan", email="douyaoyuan@126.com" },
 ]
 description = "封装提供了一些调试常用方法，例如打印对齐，彩色文本，表格输出等"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `DebugInfo-9.0.0/src/DebugInfo/DebugInfo.py` & `DebugInfo-9.1.0/src/DebugInfo/DebugInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,32 +699,32 @@
     # endregion
 
     # region 表格操作
     def 准备表格(self):
         self.__表格 = []
 
         class 次次级方法类:
-            def 修饰方法(self, callable) -> None:
+            def 修饰方法(self, 方法: callable = None) -> None:
                 pass
 
         class 添加多行次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         class 次级方法类:
-            def 添加一行(self, *args) -> 次次级方法类:
+            def 添加一行(self, *元素列表) -> 次次级方法类:
                 pass
 
-            def 添加一调试行(self, *args) -> 次次级方法类:
+            def 添加一调试行(self, *元素列表) -> 次次级方法类:
                 pass
 
-            def 添加多行(self, *args, **kwargs) -> 添加多行次级方法类:
+            def 添加多行(self, 行列表: list or tuple, 拆分列数: int = -1, 拆分行数: int = -1) -> 添加多行次级方法类:
                 pass
 
-            def 添加多调试行(self, *args, **kwargs) -> 添加多行次级方法类:
+            def 添加多调试行(self, 行列表: list or tuple, 拆分列数: int = -1, 拆分行数: int = -1) -> 添加多行次级方法类:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.添加一行 = self.添加一行
         次级方法.添加一调试行 = self.添加一调试行
         次级方法.添加多行 = self.添加多行
         次级方法.添加多调试行 = self.添加多调试行
@@ -734,18 +734,18 @@
     def 添加一行(self, *元素列表):
         if len(元素列表) == 1 and type(元素列表[0]) in [list, tuple]:
             self.__添加一行(元素列表[0])
         elif len(元素列表) > 0:
             self.__添加一行(元素列表)
 
         class 次级方法类:
-            def 修饰方法(self, callable) -> None:
+            def 修饰方法(self, 方法: callable = None) -> None:
                 pass
 
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.修饰方法 = self.__修饰最后一行
         次级方法.展示表格 = self.展示表格
 
         return 次级方法
@@ -753,15 +753,15 @@
     def 添加空行(self, 空行数量: int = 1):
         if 空行数量 < 1:
             return None
         for 次数 in range(空行数量):
             self.__添加一行([''])
 
         class 次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.展示表格 = self.展示表格
 
         return 次级方法
 
@@ -779,31 +779,31 @@
             else:
                 计算拆分列数: int = (len(行列表) / 拆分行数).__ceil__()
                 self.添加多行(行列表=行列表, 拆分列数=计算拆分列数)
         else:
             self.__添加一行([str(行列表)])
 
         class 次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.展示表格 = self.展示表格
 
         return 次级方法
 
     def 添加一调试行(self, *元素列表):
         if self.__调试状态:
             self.添加一行(*元素列表)
 
         class 次级方法类:
-            def 修饰方法(self, callable) -> None:
+            def 修饰方法(self, 方法: callable = None) -> None:
                 pass
 
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         if self.__调试状态:
             次级方法.修饰方法 = self.__修饰最后一行
             次级方法.展示表格 = self.展示表格
         else:
@@ -813,15 +813,15 @@
         return 次级方法
 
     def 添加多调试行(self, 行列表: list or tuple, 拆分列数: int = -1, 拆分行数: int = -1):
         if self.__调试状态:
             self.添加多行(行列表, 拆分列数, 拆分行数)
 
         class 次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         if self.__调试状态:
             次级方法.展示表格 = self.展示表格
         else:
             次级方法.展示表格 = self.__空方法
@@ -829,22 +829,22 @@
         return 次级方法
 
     def 上下颠倒表格(self):
         if self.__表格:
             self.__表格.reverse()
 
         class 次次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         class 次级方法类:
             def 左右颠倒表格(self) -> 次次级方法类:
                 pass
 
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.左右颠倒表格 = self.左右颠倒表格
         次级方法.展示表格 = self.展示表格
 
         return 次级方法
@@ -862,22 +862,22 @@
                     else:
                         这一行.append("")
                 这一行.reverse()
                 临时表格.append(这一行)
             self.__表格 = 临时表格
 
         class 次次级方法类:
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         class 次级方法类:
             def 上下颠倒表格(self) -> 次次级方法类:
                 pass
 
-            def 展示表格(self) -> None:
+            def 展示表格(self, 列间距: int = 2) -> None:
                 pass
 
         次级方法: 次级方法类 = 次级方法类()
         次级方法.上下颠倒表格 = self.上下颠倒表格
         次级方法.展示表格 = self.展示表格
 
         return 次级方法
```

### Comparing `DebugInfo-9.0.0/src/DebugInfo.egg-info/PKG-INFO` & `DebugInfo-9.1.0/src/DebugInfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DebugInfo
-Version: 9.0.0
+Version: 9.1.0
 Summary: 封装提供了一些调试常用方法，例如打印对齐，彩色文本，表格输出等
 Author-email: douyaoyuan <douyaoyuan@126.com>
 Project-URL: Homepage, https://gitee.com/DyyYq/DebugInfo.git
 Project-URL: Bug Tracker, https://gitee.com/DyyYq/DebugInfo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

