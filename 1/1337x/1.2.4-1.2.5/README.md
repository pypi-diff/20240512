# Comparing `tmp/1337x-1.2.4.tar.gz` & `tmp/1337x-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1337x-1.2.4.tar", last modified: Thu Nov 24 07:43:20 2022, max compression
+gzip compressed data, was "1337x-1.2.5.tar", last modified: Sun May 12 13:52:20 2024, max compression
```

## Comparing `1337x-1.2.4.tar` & `1337x-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 07:43:20.841347 1337x-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 07:43:20.841347 1337x-1.2.4/1337x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10601 2022-11-24 07:43:20.000000 1337x-1.2.4/1337x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-24 07:43:20.000000 1337x-1.2.4/1337x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-24 07:43:20.000000 1337x-1.2.4/1337x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-24 07:43:20.000000 1337x-1.2.4/1337x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-24 07:43:20.000000 1337x-1.2.4/1337x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-11-24 07:43:11.000000 1337x-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10601 2022-11-24 07:43:20.841347 1337x-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9733 2022-11-24 07:43:11.000000 1337x-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 07:43:20.841347 1337x-1.2.4/py1337x/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-24 07:43:11.000000 1337x-1.2.4/py1337x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4702 2022-11-24 07:43:11.000000 1337x-1.2.4/py1337x/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-11-24 07:43:11.000000 1337x-1.2.4/py1337x/py1337x.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-24 07:43:20.841347 1337x-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-11-24 07:43:11.000000 1337x-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:52:20.690059 1337x-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:52:20.690059 1337x-1.2.5/1337x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-12 13:52:20.000000 1337x-1.2.5/1337x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-12 13:52:20.000000 1337x-1.2.5/1337x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:52:20.000000 1337x-1.2.5/1337x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-12 13:52:20.000000 1337x-1.2.5/1337x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 13:52:20.000000 1337x-1.2.5/1337x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-12 13:52:12.000000 1337x-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-12 13:52:20.690059 1337x-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-12 13:52:12.000000 1337x-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:52:20.690059 1337x-1.2.5/py1337x/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 13:52:12.000000 1337x-1.2.5/py1337x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-12 13:52:12.000000 1337x-1.2.5/py1337x/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-12 13:52:12.000000 1337x-1.2.5/py1337x/py1337x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 13:52:12.000000 1337x-1.2.5/py1337x/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:52:20.690059 1337x-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-12 13:52:12.000000 1337x-1.2.5/setup.py
```

### Comparing `1337x-1.2.4/1337x.egg-info/PKG-INFO` & `1337x-1.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: 1337x
-Version: 1.2.4
-Summary: Unofficial API of 1337x.to
-Home-page: https://github.com/hemantapkh/1337x
-Author: Hemanta Pokharel
-Author-email: hemantapkh@yahoo.com
-Project-URL: Documentation, https://github.com/hemantapkh/1337x/blob/main/README.md
-Project-URL: Issue tracker, https://github.com/hemantapkh/1337x/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <h2 align='center'>✖️Unofficial Python API Wrapper of 1337x</h2>
 <p align="center">
 <img src="https://github.com/hemantapkh/1337x/blob/main/images/1337x.png?raw=true" align="center" height=205 alt="1337x" />
 </p>
 <p align="center">
 <a href="https://pypi.org/project/1337x">
@@ -76,15 +54,15 @@
 ### Quick Examples
 
 #### 1. Searching torrents
 ```python
 >>> from py1337x import py1337x
 
 # Using 1337x.tw and saving the cache in sqlite database which expires after 500 seconds
->>> torrents = py1337x(proxy='1337x.tw', cache='py1337xCache', cacheTime=500)
+>>> torrents = py1337x(proxy='1337x.to', cache='py1337xCache', cacheTime=500)
 
 >>> torrents.search('harry potter')
 {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50}
 
 # Searching harry potter in category movies and sort by seeders in descending order
 >>> torrents.search('harry potter', category='movies', sortBy='seeders', order='desc') 
 {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount': 50}
@@ -147,23 +125,21 @@
 ```
 
 **Proxy**
 
 If the default domain is banned in your country, you can use an alternative domain of 1337x. 
 
 - [`1337x.to`](https://1337x.to) (**default**)
-- [`1337x.tw`](https://www.1337x.tw)
-- [`1377x.to`](https://www.1377x.to)
-- [`1337xx.to`](https://www.1337xx.to)
 - [`1337x.st`](https://1337x.st)
 - [`x1337x.ws`](https://x1337x.ws)
 - [`x1337x.eu`](https://x1337x.eu)
 - [`x1337x.se`](https://x1337x.se)
-- [`1337x.is`](https://1337x.is)
-- [`1337x.gd`](https://1337x.gd)
+- [`1337x.so`](https://1337x.so)
+- [`1377x.to`](https://www.1377x.to) (unofficial)
+- [`1337xx.to`](https://www.1337xx.to) (unofficial)
 
 **cookie**
 
 Some of the proxies are protected with Cloudflare. For such proxies you need to pass a cookie value. To get a cookie go the the protected site from your browser, solve the captcha and copy the value of `cf_clearance`.
 
 ``Firefox: Inspect element > Storage > Cookies`` <br>
 ``Chrome: Inspect element > Application > Storage > Cookies``
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: 1337x Version: 1.2.4 Summary: Unofficial API of
-1337x.to Home-page: https://github.com/hemantapkh/1337x Author: Hemanta
-Pokharel Author-email: hemantapkh@yahoo.com Project-URL: Documentation, https:/
-/github.com/hemantapkh/1337x/blob/main/README.md Project-URL: Issue tracker,
-https://github.com/hemantapkh/1337x/issues Classifier: Development Status :: 5
-- Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Topic ::
-Internet Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
-:: Utilities Requires-Python: >=3.0 Description-Content-Type: text/markdown
-License-File: LICENSE
            ********** ?â???ï?¸?UUnnooffffiicciiaall PPyytthhoonn AAPPII WWrraappppeerr ooff 11333377xx **********
                                     [1337x]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_1_3_3_7_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_1_3_3_7_x_][https:
    //visitor-badge.laobi.icu/badge?page_id=hemantapkh.1337x]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]
    This is the unofficial API of 1337x. It supports all proxies of 1337x and
  almost all functions of 1337x. You can search, get trending, top and popular
  torrents. Furthermore, you can browse torrents of a certain category. It also
@@ -28,15 +16,15 @@
  sorting-methods) - [Contributing](#contributing) - [Projects using this API]
 (#projects-using-this-api) - [License](#license) ## Installation - Install via
   [PyPi](https://www.pypi.org/project/1337x) ```bash pip install 1337x ``` -
  Install from the source ```bash git clone https://github.com/hemantapkh/1337x
  && cd 1337x && python setup.py sdist && pip install dist/* ``` ## Start guide
 ### Quick Examples #### 1. Searching torrents ```python >>> from py1337x import
 py1337x # Using 1337x.tw and saving the cache in sqlite database which expires
-          after 500 seconds >>> torrents = py1337x(proxy='1337x.tw',
+          after 500 seconds >>> torrents = py1337x(proxy='1337x.to',
    cache='py1337xCache', cacheTime=500) >>> torrents.search('harry potter')
     {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50} #
   Searching harry potter in category movies and sort by seeders in descending
 order >>> torrents.search('harry potter', category='movies', sortBy='seeders',
 order='desc') {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount':
  50} # Viewing the 5th page of the result >>> torrents.search('harry potter',
 page=5) {'items': [...], 'currentPage': , 'itemCount': 20, 'pageCount': 50} ```
@@ -68,22 +56,22 @@
  ...', 'uploaderLink': '...', 'downloads': '5310', 'lastChecked': '44 seconds
      ago', 'uploadDate': '4 years ago', 'seeders': '36', 'leechers': '3',
    'magnetLink': '...', 'infoHash': '...'} ``` ## Detailed documentation ##
  Available attributes ```python from py1337x import py1337x torrents = py1337x
      (proxy='1337x.st', cookie='', cache='py1337xCache', cacheTime=86400,
     backend='sqlite') ``` **Proxy** If the default domain is banned in your
  country, you can use an alternative domain of 1337x. - [`1337x.to`](https://
-  1337x.to) (**default**) - [`1337x.tw`](https://www.1337x.tw) - [`1377x.to`]
- (https://www.1377x.to) - [`1337xx.to`](https://www.1337xx.to) - [`1337x.st`]
-(https://1337x.st) - [`x1337x.ws`](https://x1337x.ws) - [`x1337x.eu`](https://
-x1337x.eu) - [`x1337x.se`](https://x1337x.se) - [`1337x.is`](https://1337x.is)
- - [`1337x.gd`](https://1337x.gd) **cookie** Some of the proxies are protected
-  with Cloudflare. For such proxies you need to pass a cookie value. To get a
-cookie go the the protected site from your browser, solve the captcha and copy
-the value of `cf_clearance`. ``Firefox: Inspect element > Storage > Cookies``
+1337x.to) (**default**) - [`1337x.st`](https://1337x.st) - [`x1337x.ws`](https:
+   //x1337x.ws) - [`x1337x.eu`](https://x1337x.eu) - [`x1337x.se`](https://
+      x1337x.se) - [`1337x.so`](https://1337x.so) - [`1377x.to`](https://
+www.1377x.to) (unofficial) - [`1337xx.to`](https://www.1337xx.to) (unofficial)
+**cookie** Some of the proxies are protected with Cloudflare. For such proxies
+you need to pass a cookie value. To get a cookie go the the protected site from
+     your browser, solve the captcha and copy the value of `cf_clearance`.
+               ``Firefox: Inspect element > Storage > Cookies``
 ``Chrome: Inspect element > Application > Storage > Cookies`` **cache** Py1337x
 uses [requests-cache](https://pypi.org/project/requests-cache/) for caching to
 store data so that future requests for that data can be served faster. `cache`
   can be any of the following. - A boolean value: `True` for using cache and
 `False` for not using cache. (**cache is not used by default**) - Directory for
  storing the cache. **cacheTime** By default the cache expires after one day.
 You can change the cache expiration time by setting a custom `cacheTime`. - `-
```

### Comparing `1337x-1.2.4/LICENSE` & `1337x-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `1337x-1.2.4/PKG-INFO` & `1337x-1.2.5/1337x.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1337x
-Version: 1.2.4
+Version: 1.2.5
 Summary: Unofficial API of 1337x.to
 Home-page: https://github.com/hemantapkh/1337x
 Author: Hemanta Pokharel
 Author-email: hemantapkh@yahoo.com
 Project-URL: Documentation, https://github.com/hemantapkh/1337x/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/hemantapkh/1337x/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,31 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: attrs==23.2.0
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: bs4==0.0.2
+Requires-Dist: cattrs==23.2.3
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cloudscraper==1.2.71
+Requires-Dist: idna==3.7
+Requires-Dist: platformdirs==4.2.1
+Requires-Dist: pyparsing==3.1.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-cache==1.2.0
+Requires-Dist: requests-toolbelt==1.0.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: url-normalize==1.4.3
+Requires-Dist: urllib3==2.2.1
 
 
 <h2 align='center'>✖️Unofficial Python API Wrapper of 1337x</h2>
 <p align="center">
 <img src="https://github.com/hemantapkh/1337x/blob/main/images/1337x.png?raw=true" align="center" height=205 alt="1337x" />
 </p>
 <p align="center">
@@ -76,15 +93,15 @@
 ### Quick Examples
 
 #### 1. Searching torrents
 ```python
 >>> from py1337x import py1337x
 
 # Using 1337x.tw and saving the cache in sqlite database which expires after 500 seconds
->>> torrents = py1337x(proxy='1337x.tw', cache='py1337xCache', cacheTime=500)
+>>> torrents = py1337x(proxy='1337x.to', cache='py1337xCache', cacheTime=500)
 
 >>> torrents.search('harry potter')
 {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50}
 
 # Searching harry potter in category movies and sort by seeders in descending order
 >>> torrents.search('harry potter', category='movies', sortBy='seeders', order='desc') 
 {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount': 50}
@@ -147,23 +164,21 @@
 ```
 
 **Proxy**
 
 If the default domain is banned in your country, you can use an alternative domain of 1337x. 
 
 - [`1337x.to`](https://1337x.to) (**default**)
-- [`1337x.tw`](https://www.1337x.tw)
-- [`1377x.to`](https://www.1377x.to)
-- [`1337xx.to`](https://www.1337xx.to)
 - [`1337x.st`](https://1337x.st)
 - [`x1337x.ws`](https://x1337x.ws)
 - [`x1337x.eu`](https://x1337x.eu)
 - [`x1337x.se`](https://x1337x.se)
-- [`1337x.is`](https://1337x.is)
-- [`1337x.gd`](https://1337x.gd)
+- [`1337x.so`](https://1337x.so)
+- [`1377x.to`](https://www.1377x.to) (unofficial)
+- [`1337xx.to`](https://www.1337xx.to) (unofficial)
 
 **cookie**
 
 Some of the proxies are protected with Cloudflare. For such proxies you need to pass a cookie value. To get a cookie go the the protected site from your browser, solve the captcha and copy the value of `cf_clearance`.
 
 ``Firefox: Inspect element > Storage > Cookies`` <br>
 ``Chrome: Inspect element > Application > Storage > Cookies``
```

#### html2text {}

```diff
@@ -1,19 +1,26 @@
-Metadata-Version: 2.1 Name: 1337x Version: 1.2.4 Summary: Unofficial API of
+Metadata-Version: 2.1 Name: 1337x Version: 1.2.5 Summary: Unofficial API of
 1337x.to Home-page: https://github.com/hemantapkh/1337x Author: Hemanta
 Pokharel Author-email: hemantapkh@yahoo.com Project-URL: Documentation, https:/
 /github.com/hemantapkh/1337x/blob/main/README.md Project-URL: Issue tracker,
 https://github.com/hemantapkh/1337x/issues Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Topic ::
 Internet Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
 :: Utilities Requires-Python: >=3.0 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE Requires-Dist: attrs==23.2.0 Requires-Dist:
+beautifulsoup4==4.12.3 Requires-Dist: bs4==0.0.2 Requires-Dist: cattrs==23.2.3
+Requires-Dist: certifi==2024.2.2 Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cloudscraper==1.2.71 Requires-Dist: idna==3.7 Requires-Dist:
+platformdirs==4.2.1 Requires-Dist: pyparsing==3.1.2 Requires-Dist:
+requests==2.31.0 Requires-Dist: requests-cache==1.2.0 Requires-Dist: requests-
+toolbelt==1.0.0 Requires-Dist: six==1.16.0 Requires-Dist: soupsieve==2.5
+Requires-Dist: url-normalize==1.4.3 Requires-Dist: urllib3==2.2.1
            ********** ?â???ï?¸?UUnnooffffiicciiaall PPyytthhoonn AAPPII WWrraappppeerr ooff 11333377xx **********
                                     [1337x]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_1_3_3_7_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_1_3_3_7_x_][https:
    //visitor-badge.laobi.icu/badge?page_id=hemantapkh.1337x]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]
    This is the unofficial API of 1337x. It supports all proxies of 1337x and
  almost all functions of 1337x. You can search, get trending, top and popular
  torrents. Furthermore, you can browse torrents of a certain category. It also
@@ -28,15 +35,15 @@
  sorting-methods) - [Contributing](#contributing) - [Projects using this API]
 (#projects-using-this-api) - [License](#license) ## Installation - Install via
   [PyPi](https://www.pypi.org/project/1337x) ```bash pip install 1337x ``` -
  Install from the source ```bash git clone https://github.com/hemantapkh/1337x
  && cd 1337x && python setup.py sdist && pip install dist/* ``` ## Start guide
 ### Quick Examples #### 1. Searching torrents ```python >>> from py1337x import
 py1337x # Using 1337x.tw and saving the cache in sqlite database which expires
-          after 500 seconds >>> torrents = py1337x(proxy='1337x.tw',
+          after 500 seconds >>> torrents = py1337x(proxy='1337x.to',
    cache='py1337xCache', cacheTime=500) >>> torrents.search('harry potter')
     {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50} #
   Searching harry potter in category movies and sort by seeders in descending
 order >>> torrents.search('harry potter', category='movies', sortBy='seeders',
 order='desc') {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount':
  50} # Viewing the 5th page of the result >>> torrents.search('harry potter',
 page=5) {'items': [...], 'currentPage': , 'itemCount': 20, 'pageCount': 50} ```
@@ -68,22 +75,22 @@
  ...', 'uploaderLink': '...', 'downloads': '5310', 'lastChecked': '44 seconds
      ago', 'uploadDate': '4 years ago', 'seeders': '36', 'leechers': '3',
    'magnetLink': '...', 'infoHash': '...'} ``` ## Detailed documentation ##
  Available attributes ```python from py1337x import py1337x torrents = py1337x
      (proxy='1337x.st', cookie='', cache='py1337xCache', cacheTime=86400,
     backend='sqlite') ``` **Proxy** If the default domain is banned in your
  country, you can use an alternative domain of 1337x. - [`1337x.to`](https://
-  1337x.to) (**default**) - [`1337x.tw`](https://www.1337x.tw) - [`1377x.to`]
- (https://www.1377x.to) - [`1337xx.to`](https://www.1337xx.to) - [`1337x.st`]
-(https://1337x.st) - [`x1337x.ws`](https://x1337x.ws) - [`x1337x.eu`](https://
-x1337x.eu) - [`x1337x.se`](https://x1337x.se) - [`1337x.is`](https://1337x.is)
- - [`1337x.gd`](https://1337x.gd) **cookie** Some of the proxies are protected
-  with Cloudflare. For such proxies you need to pass a cookie value. To get a
-cookie go the the protected site from your browser, solve the captcha and copy
-the value of `cf_clearance`. ``Firefox: Inspect element > Storage > Cookies``
+1337x.to) (**default**) - [`1337x.st`](https://1337x.st) - [`x1337x.ws`](https:
+   //x1337x.ws) - [`x1337x.eu`](https://x1337x.eu) - [`x1337x.se`](https://
+      x1337x.se) - [`1337x.so`](https://1337x.so) - [`1377x.to`](https://
+www.1377x.to) (unofficial) - [`1337xx.to`](https://www.1337xx.to) (unofficial)
+**cookie** Some of the proxies are protected with Cloudflare. For such proxies
+you need to pass a cookie value. To get a cookie go the the protected site from
+     your browser, solve the captcha and copy the value of `cf_clearance`.
+               ``Firefox: Inspect element > Storage > Cookies``
 ``Chrome: Inspect element > Application > Storage > Cookies`` **cache** Py1337x
 uses [requests-cache](https://pypi.org/project/requests-cache/) for caching to
 store data so that future requests for that data can be served faster. `cache`
   can be any of the following. - A boolean value: `True` for using cache and
 `False` for not using cache. (**cache is not used by default**) - Directory for
  storing the cache. **cacheTime** By default the cache expires after one day.
 You can change the cache expiration time by setting a custom `cacheTime`. - `-
```

### Comparing `1337x-1.2.4/README.md` & `1337x-1.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+Metadata-Version: 2.1
+Name: 1337x
+Version: 1.2.5
+Summary: Unofficial API of 1337x.to
+Home-page: https://github.com/hemantapkh/1337x
+Author: Hemanta Pokharel
+Author-email: hemantapkh@yahoo.com
+Project-URL: Documentation, https://github.com/hemantapkh/1337x/blob/main/README.md
+Project-URL: Issue tracker, https://github.com/hemantapkh/1337x/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: attrs==23.2.0
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: bs4==0.0.2
+Requires-Dist: cattrs==23.2.3
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cloudscraper==1.2.71
+Requires-Dist: idna==3.7
+Requires-Dist: platformdirs==4.2.1
+Requires-Dist: pyparsing==3.1.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-cache==1.2.0
+Requires-Dist: requests-toolbelt==1.0.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: url-normalize==1.4.3
+Requires-Dist: urllib3==2.2.1
+
 
 <h2 align='center'>✖️Unofficial Python API Wrapper of 1337x</h2>
 <p align="center">
 <img src="https://github.com/hemantapkh/1337x/blob/main/images/1337x.png?raw=true" align="center" height=205 alt="1337x" />
 </p>
 <p align="center">
 <a href="https://pypi.org/project/1337x">
@@ -54,15 +93,15 @@
 ### Quick Examples
 
 #### 1. Searching torrents
 ```python
 >>> from py1337x import py1337x
 
 # Using 1337x.tw and saving the cache in sqlite database which expires after 500 seconds
->>> torrents = py1337x(proxy='1337x.tw', cache='py1337xCache', cacheTime=500)
+>>> torrents = py1337x(proxy='1337x.to', cache='py1337xCache', cacheTime=500)
 
 >>> torrents.search('harry potter')
 {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50}
 
 # Searching harry potter in category movies and sort by seeders in descending order
 >>> torrents.search('harry potter', category='movies', sortBy='seeders', order='desc') 
 {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount': 50}
@@ -125,23 +164,21 @@
 ```
 
 **Proxy**
 
 If the default domain is banned in your country, you can use an alternative domain of 1337x. 
 
 - [`1337x.to`](https://1337x.to) (**default**)
-- [`1337x.tw`](https://www.1337x.tw)
-- [`1377x.to`](https://www.1377x.to)
-- [`1337xx.to`](https://www.1337xx.to)
 - [`1337x.st`](https://1337x.st)
 - [`x1337x.ws`](https://x1337x.ws)
 - [`x1337x.eu`](https://x1337x.eu)
 - [`x1337x.se`](https://x1337x.se)
-- [`1337x.is`](https://1337x.is)
-- [`1337x.gd`](https://1337x.gd)
+- [`1337x.so`](https://1337x.so)
+- [`1377x.to`](https://www.1377x.to) (unofficial)
+- [`1337xx.to`](https://www.1337xx.to) (unofficial)
 
 **cookie**
 
 Some of the proxies are protected with Cloudflare. For such proxies you need to pass a cookie value. To get a cookie go the the protected site from your browser, solve the captcha and copy the value of `cf_clearance`.
 
 ``Firefox: Inspect element > Storage > Cookies`` <br>
 ``Chrome: Inspect element > Application > Storage > Cookies``
```

#### html2text {}

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1 Name: 1337x Version: 1.2.5 Summary: Unofficial API of
+1337x.to Home-page: https://github.com/hemantapkh/1337x Author: Hemanta
+Pokharel Author-email: hemantapkh@yahoo.com Project-URL: Documentation, https:/
+/github.com/hemantapkh/1337x/blob/main/README.md Project-URL: Issue tracker,
+https://github.com/hemantapkh/1337x/issues Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Topic ::
+Internet Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
+:: Utilities Requires-Python: >=3.0 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: attrs==23.2.0 Requires-Dist:
+beautifulsoup4==4.12.3 Requires-Dist: bs4==0.0.2 Requires-Dist: cattrs==23.2.3
+Requires-Dist: certifi==2024.2.2 Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cloudscraper==1.2.71 Requires-Dist: idna==3.7 Requires-Dist:
+platformdirs==4.2.1 Requires-Dist: pyparsing==3.1.2 Requires-Dist:
+requests==2.31.0 Requires-Dist: requests-cache==1.2.0 Requires-Dist: requests-
+toolbelt==1.0.0 Requires-Dist: six==1.16.0 Requires-Dist: soupsieve==2.5
+Requires-Dist: url-normalize==1.4.3 Requires-Dist: urllib3==2.2.1
            ********** ?â???ï?¸?UUnnooffffiicciiaall PPyytthhoonn AAPPII WWrraappppeerr ooff 11333377xx **********
                                     [1337x]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_1_3_3_7_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_1_3_3_7_x_][https:
    //visitor-badge.laobi.icu/badge?page_id=hemantapkh.1337x]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]
    This is the unofficial API of 1337x. It supports all proxies of 1337x and
  almost all functions of 1337x. You can search, get trending, top and popular
  torrents. Furthermore, you can browse torrents of a certain category. It also
@@ -16,15 +35,15 @@
  sorting-methods) - [Contributing](#contributing) - [Projects using this API]
 (#projects-using-this-api) - [License](#license) ## Installation - Install via
   [PyPi](https://www.pypi.org/project/1337x) ```bash pip install 1337x ``` -
  Install from the source ```bash git clone https://github.com/hemantapkh/1337x
  && cd 1337x && python setup.py sdist && pip install dist/* ``` ## Start guide
 ### Quick Examples #### 1. Searching torrents ```python >>> from py1337x import
 py1337x # Using 1337x.tw and saving the cache in sqlite database which expires
-          after 500 seconds >>> torrents = py1337x(proxy='1337x.tw',
+          after 500 seconds >>> torrents = py1337x(proxy='1337x.to',
    cache='py1337xCache', cacheTime=500) >>> torrents.search('harry potter')
     {'items': [...], 'currentPage': 1, 'itemCount': 20, 'pageCount': 50} #
   Searching harry potter in category movies and sort by seeders in descending
 order >>> torrents.search('harry potter', category='movies', sortBy='seeders',
 order='desc') {'items': [...], 'currentPage': 1, 'itemCount': 40, 'pageCount':
  50} # Viewing the 5th page of the result >>> torrents.search('harry potter',
 page=5) {'items': [...], 'currentPage': , 'itemCount': 20, 'pageCount': 50} ```
@@ -56,22 +75,22 @@
  ...', 'uploaderLink': '...', 'downloads': '5310', 'lastChecked': '44 seconds
      ago', 'uploadDate': '4 years ago', 'seeders': '36', 'leechers': '3',
    'magnetLink': '...', 'infoHash': '...'} ``` ## Detailed documentation ##
  Available attributes ```python from py1337x import py1337x torrents = py1337x
      (proxy='1337x.st', cookie='', cache='py1337xCache', cacheTime=86400,
     backend='sqlite') ``` **Proxy** If the default domain is banned in your
  country, you can use an alternative domain of 1337x. - [`1337x.to`](https://
-  1337x.to) (**default**) - [`1337x.tw`](https://www.1337x.tw) - [`1377x.to`]
- (https://www.1377x.to) - [`1337xx.to`](https://www.1337xx.to) - [`1337x.st`]
-(https://1337x.st) - [`x1337x.ws`](https://x1337x.ws) - [`x1337x.eu`](https://
-x1337x.eu) - [`x1337x.se`](https://x1337x.se) - [`1337x.is`](https://1337x.is)
- - [`1337x.gd`](https://1337x.gd) **cookie** Some of the proxies are protected
-  with Cloudflare. For such proxies you need to pass a cookie value. To get a
-cookie go the the protected site from your browser, solve the captcha and copy
-the value of `cf_clearance`. ``Firefox: Inspect element > Storage > Cookies``
+1337x.to) (**default**) - [`1337x.st`](https://1337x.st) - [`x1337x.ws`](https:
+   //x1337x.ws) - [`x1337x.eu`](https://x1337x.eu) - [`x1337x.se`](https://
+      x1337x.se) - [`1337x.so`](https://1337x.so) - [`1377x.to`](https://
+www.1377x.to) (unofficial) - [`1337xx.to`](https://www.1337xx.to) (unofficial)
+**cookie** Some of the proxies are protected with Cloudflare. For such proxies
+you need to pass a cookie value. To get a cookie go the the protected site from
+     your browser, solve the captcha and copy the value of `cf_clearance`.
+               ``Firefox: Inspect element > Storage > Cookies``
 ``Chrome: Inspect element > Application > Storage > Cookies`` **cache** Py1337x
 uses [requests-cache](https://pypi.org/project/requests-cache/) for caching to
 store data so that future requests for that data can be served faster. `cache`
   can be any of the following. - A boolean value: `True` for using cache and
 `False` for not using cache. (**cache is not used by default**) - Directory for
  storing the cache. **cacheTime** By default the cache expires after one day.
 You can change the cache expiration time by setting a custom `cacheTime`. - `-
```

### Comparing `1337x-1.2.4/py1337x/parser.py` & `1337x-1.2.5/py1337x/parser.py`

 * *Files identical despite different names*

### Comparing `1337x-1.2.4/py1337x/py1337x.py` & `1337x-1.2.5/py1337x/py1337x.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-import requests
+import cloudscraper
 import requests_cache
+
 from py1337x import parser
 
 
 class py1337x():
     def __init__(self, proxy=None, cookie=None, cache=None, cacheTime=86400, backend='sqlite'):
-        self.baseUrl = f'https://www.{proxy}' if proxy else 'https://www.1377x.to'
+        self.baseUrl = f'https://www.{proxy}' if proxy else 'https://www.1337x.to'
         self.headers = {
-            'user-agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:88.0) Gecko/20100101 Firefox/88.0',
-            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
-            'accept-language': 'en-US,en;q=0.5',
-            'upgrade-insecure-requests': '1',
-            'te': 'trailers'
-        }
+            'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.37',
+        } if cache else {}
 
         if cookie:
             self.headers['cookie'] = f'cf_clearance={cookie}'
 
-        self.requests = requests_cache.CachedSession(cache, expire_after=cacheTime, backend=backend) if cache else requests
+        self.requests = requests_cache.CachedSession(cache, expire_after=cacheTime, backend=backend) if cache else cloudscraper.create_scraper()
 
     #: Searching torrents
     def search(self, query, page=1, category=None, sortBy=None, order='desc'):
         query = '+'.join(query.split())
         category = category.upper() if category and category.lower() in ['xxx', 'tv'] else category.capitalize() if category else None
         url = f"{self.baseUrl}/{'sort-' if sortBy else ''}{'category-' if category else ''}search/{query}/{category+'/' if category else ''}{sortBy.lower()+'/' if sortBy else ''}{order.lower()+'/' if sortBy else ''}{page}/"
```

### Comparing `1337x-1.2.4/setup.py` & `1337x-1.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import setuptools
 
-with open("README.md", encoding="utf8") as fh:
-    readme = fh.read()
+with open("README.md", encoding="utf8") as f:
+    readme = f.read()
+    
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
 
 setuptools.setup(
     name="1337x",
-    version="1.2.4",
+    version="1.2.5",
     author="Hemanta Pokharel",
     author_email="hemantapkh@yahoo.com",
     description="Unofficial API of 1337x.to",
     long_description=readme,
     long_description_content_type="text/markdown",
-    install_requires=["requests", "bs4", "requests-cache"],
+    install_requires=requirements,
     url="https://github.com/hemantapkh/1337x",
     project_urls={
         "Documentation": "https://github.com/hemantapkh/1337x/blob/main/README.md",
         "Issue tracker": "https://github.com/hemantapkh/1337x/issues",
       },
     packages=setuptools.find_packages(),
     classifiers=[
```

