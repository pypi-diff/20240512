# Comparing `tmp/gdown-5.1.0.tar.gz` & `tmp/gdown-5.2.0.tar.gz`

## Comparing `gdown-5.1.0.tar` & `gdown-5.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gdown-5.1.0/.gitattributes
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 gdown-5.1.0/Makefile
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 gdown-5.1.0/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 gdown-5.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 gdown-5.1.0/.github/ISSUE_TEMPLATE/1.bug_report.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gdown-5.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 gdown-5.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 gdown-5.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0   100269 2020-02-02 00:00:00.000000 gdown-5.1.0/.readme/cli.png
--rw-r--r--   0        0        0   112628 2020-02-02 00:00:00.000000 gdown-5.1.0/.readme/python.png
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/__init__.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/__main__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/_indent.py
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/cached_download.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/download.py
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/download_folder.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/exceptions.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/extractall.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 gdown-5.1.0/gdown/parse_url.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/test___main__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/test_cached_download.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/test_download.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/test_download_folder.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/test_parse_url.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/data/file_ids.csv
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/data/file_ids_large.csv
--rw-r--r--   0        0        0   244789 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/data/folder-page-sample.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 gdown-5.1.0/tests/data/folder_ids.csv
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 gdown-5.1.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 gdown-5.1.0/LICENSE
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 gdown-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 gdown-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gdown-5.2.0/.gitattributes
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 gdown-5.2.0/Makefile
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 gdown-5.2.0/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 gdown-5.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 gdown-5.2.0/.github/ISSUE_TEMPLATE/1.bug_report.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gdown-5.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 gdown-5.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 gdown-5.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0   100269 2020-02-02 00:00:00.000000 gdown-5.2.0/.readme/cli.png
+-rw-r--r--   0        0        0   112628 2020-02-02 00:00:00.000000 gdown-5.2.0/.readme/python.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/__init__.py
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/__main__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/_indent.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/cached_download.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/download.py
+-rw-r--r--   0        0        0    11085 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/download_folder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/exceptions.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/extractall.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 gdown-5.2.0/gdown/parse_url.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/test___main__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/test_cached_download.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/test_download.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/test_download_folder.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/test_parse_url.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/data/file_ids.csv
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/data/file_ids_large.csv
+-rw-r--r--   0        0        0   244789 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/data/folder-page-sample.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 gdown-5.2.0/tests/data/folder_ids.csv
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 gdown-5.2.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 gdown-5.2.0/LICENSE
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 gdown-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 gdown-5.2.0/PKG-INFO
```

### Comparing `gdown-5.1.0/Makefile` & `gdown-5.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/README.md` & `gdown-5.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <br>
   <br>
 </div>
 
 
 *Gdown* downloads a public file/folder from Google Drive.
 
-*Gdown* provides what's curl/wget doesn't for Google Drive:
+*Gdown* provides what curl/wget doesn't for Google Drive:
 - **Skip the security notice** allowing you to download large files (curl/wget fails);
 - **Recursive download** of files in a folder (maximum 50 files per folder);
 - **Specify download file format** for Google Slides/Sheet/Docs like PDF/XML/CSV.
 
 
 ## Installation
 
@@ -109,19 +109,19 @@
 id = "15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
 gdown.download_folder(id=id)
 ```
 
 
 ## FAQ
 
-### I get 'Permission Denied' error.
+### I get a 'Permission Denied' error.
 
 Have you made sure you set the file permission to 'Anyone with Link'?
 
-### I set the permission 'Anyone with Link', but still can't download.
+### I set the permission 'Anyone with Link', but I still can't download.
 
 Google restricts access to a file when the download is concentrated.
 If you can still access to the file from your browser, downloading cookies file might
 help. Follow this step: 1) download cookies.txt using browser extensions like
 ([Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc));
 2) mv the `cookies.txt` to `~/.cache/gdown/cookies.txt`; 3) run download again.
 If you're using `gdown>=5.0.0`, it should be able to use the cookies same as your browser.
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
                               ************ ggddoowwnn ************
            GGooooggllee DDrriivvee PPuubblliicc FFiillee DDoowwnnllooaaddeerr wwhheenn CCuurrll//WWggeett FFaaiillss
      [https://github.com/wkentaro/gdown/raw/main/.readme/cli.png][https://
             github.com/wkentaro/gdown/raw/main/.readme/python.png]
 
-*Gdown* downloads a public file/folder from Google Drive. *Gdown* provides
-what's curl/wget doesn't for Google Drive: - **Skip the security notice**
-allowing you to download large files (curl/wget fails); - **Recursive
-download** of files in a folder (maximum 50 files per folder); - **Specify
-download file format** for Google Slides/Sheet/Docs like PDF/XML/CSV. ##
-Installation _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_d_o_w_n_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_d_o_w_n_._s_v_g_]```bash pip install gdown # to upgrade pip
-install --upgrade gdown ``` ## Usage ### via Command Line ```bash $ gdown --
-help usage: gdown [-h] [-V] [-O OUTPUT] [-q] [--fuzzy] [--id] [--proxy PROXY]
-[--speed SPEED] [--no-cookies] [--no-check-certificate] [--continue] [--folder]
-[--remaining-ok] url_or_id ... $ # a large file (~500MB) $ gdown https://
-drive.google.com/uc?id=1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ md5sum
-fcn8s_from_caffe.npz 256c2a8235c1c65e62e48d3284fbd384 $ # same as the above but
-with the file ID $ gdown 1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ # a small file $
-gdown https://drive.google.com/uc?id=0B9P1L--7Wd2vU3VUVlFnbTgtS2c $ cat
-spam.txt spam $ # download with fuzzy extraction of a file ID $ gdown --fuzzy
-'https://drive.google.com/file/d/0B9P1L--7Wd2vU3VUVlFnbTgtS2c/
+*Gdown* downloads a public file/folder from Google Drive. *Gdown* provides what
+curl/wget doesn't for Google Drive: - **Skip the security notice** allowing you
+to download large files (curl/wget fails); - **Recursive download** of files in
+a folder (maximum 50 files per folder); - **Specify download file format** for
+Google Slides/Sheet/Docs like PDF/XML/CSV. ## Installation _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_d_o_w_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_g_d_o_w_n_._s_v_g_]```bash pip install gdown # to upgrade pip install --upgrade gdown
+``` ## Usage ### via Command Line ```bash $ gdown --help usage: gdown [-h] [-V]
+[-O OUTPUT] [-q] [--fuzzy] [--id] [--proxy PROXY] [--speed SPEED] [--no-
+cookies] [--no-check-certificate] [--continue] [--folder] [--remaining-ok]
+url_or_id ... $ # a large file (~500MB) $ gdown https://drive.google.com/
+uc?id=1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ md5sum fcn8s_from_caffe.npz
+256c2a8235c1c65e62e48d3284fbd384 $ # same as the above but with the file ID $
+gdown 1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ # a small file $ gdown https://
+drive.google.com/uc?id=0B9P1L--7Wd2vU3VUVlFnbTgtS2c $ cat spam.txt spam $ #
+download with fuzzy extraction of a file ID $ gdown --fuzzy 'https://
+drive.google.com/file/d/0B9P1L--7Wd2vU3VUVlFnbTgtS2c/
 view?usp=sharing&resourcekey=0-WWs_XOSctfaY_0-sJBKRSQ' $ cat spam.txt spam $ #
 --fuzzy option also works with Microsoft Powerpoint files $ gdown --fuzzy
 "https://docs.google.com/presentation/d/15umvZKlsJ3094HNg5S4vJsIhxcFlyTeK/
 edit?usp=sharing&ouid=117512221203072002113&rtpof=true&sd=true" $ # a folder $
 gdown https://drive.google.com/drive/folders/15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl
 -O /tmp/folder --folder $ # as an alternative to curl/wget $ gdown https://
 httpbin.org/ip -O ip.json $ cat ip.json { "origin": "126.169.213.247" } $ #
@@ -39,17 +39,17 @@
 7Wd2vNm9zMTJWOGxobkU/view?usp=sharing" gdown.download(url=url, output=output,
 fuzzy=True) # Cached download with identity check via MD5 (or SHA1, SHA256,
 etc). # Pass postprocess function e.g., extracting compressed file. md5 = "md5:
 fa837a88f0c40c513d975104edf3da17" gdown.cached_download(url, output, hash=hash,
 postprocess=gdown.extractall) # a folder url = "https://drive.google.com/drive/
 folders/15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl" gdown.download_folder(url) # same as
 the above, but with the folder ID id = "15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
-gdown.download_folder(id=id) ``` ## FAQ ### I get 'Permission Denied' error.
+gdown.download_folder(id=id) ``` ## FAQ ### I get a 'Permission Denied' error.
 Have you made sure you set the file permission to 'Anyone with Link'? ### I set
-the permission 'Anyone with Link', but still can't download. Google restricts
+the permission 'Anyone with Link', but I still can't download. Google restricts
 access to a file when the download is concentrated. If you can still access to
 the file from your browser, downloading cookies file might help. Follow this
 step: 1) download cookies.txt using browser extensions like ([Get cookies.txt
 LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/
 cclelndahbckbenkjhflpdbgdldlbecc)); 2) mv the `cookies.txt` to `~/.cache/gdown/
 cookies.txt`; 3) run download again. If you're using `gdown>=5.0.0`, it should
 be able to use the cookies same as your browser. ## License MIT
```

### Comparing `gdown-5.1.0/.github/FUNDING.yml` & `gdown-5.2.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/.github/ISSUE_TEMPLATE/1.bug_report.yml` & `gdown-5.2.0/.github/ISSUE_TEMPLATE/1.bug_report.yml`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/.github/workflows/release.yml` & `gdown-5.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/.readme/cli.png` & `gdown-5.2.0/.readme/cli.png`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/.readme/python.png` & `gdown-5.2.0/.readme/python.png`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/gdown/__main__.py` & `gdown-5.2.0/gdown/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,25 +54,32 @@
         action=_ShowVersionAction,
         help="display version",
         nargs=0,
     )
     parser.add_argument(
         "url_or_id", help="url or file/folder id (with --id) to download from"
     )
-    parser.add_argument("-O", "--output", help="output file name / path")
+    parser.add_argument(
+        "-O",
+        "--output",
+        help=(
+            f'output file name/path; end with "{os.path.sep}"'
+            "to create a new directory"
+        ),
+    )
     parser.add_argument(
         "-q",
         "--quiet",
         action="store_true",
         help="suppress logging except errors",
     )
     parser.add_argument(
         "--fuzzy",
         action="store_true",
-        help="(fild only) extract Google Drive's file ID",
+        help="(file only) extract Google Drive's file ID",
     )
     parser.add_argument(
         "--id",
         action="store_true",
         help="[DEPRECATED] flag to specify file/folder id instead of url",
     )
     parser.add_argument(
@@ -95,15 +102,16 @@
         help="don't check the server's TLS certificate",
     )
     parser.add_argument(
         "--continue",
         "-c",
         dest="continue_",
         action="store_true",
-        help="(file only) resume getting a partially-downloaded file",
+        help="resume getting partially-downloaded files while "
+        "skipping fully downloaded ones",
     )
     parser.add_argument(
         "--folder",
         action="store_true",
         help="download entire folder instead of a single file "
         "(max {max} files per folder)".format(max=MAX_NUMBER_FILES),
     )
@@ -154,14 +162,15 @@
                 quiet=args.quiet,
                 proxy=args.proxy,
                 speed=args.speed,
                 use_cookies=not args.no_cookies,
                 verify=not args.no_check_certificate,
                 remaining_ok=args.remaining_ok,
                 user_agent=args.user_agent,
+                resume=args.continue_,
             )
         else:
             download(
                 url=url,
                 output=args.output,
                 quiet=args.quiet,
                 proxy=args.proxy,
@@ -184,15 +193,15 @@
                 indent("\n".join(textwrap.wrap(str(e))), prefix="\t")
             ),
             file=sys.stderr,
         )
         sys.exit(1)
     except requests.exceptions.ProxyError as e:
         print(
-            "Failed to use proxy:\n\n{}\n\n" "Please check your proxy settings.".format(
+            "Failed to use proxy:\n\n{}\n\nPlease check your proxy settings.".format(
                 indent("\n".join(textwrap.wrap(str(e))), prefix="\t")
             ),
             file=sys.stderr,
         )
         sys.exit(1)
     except Exception as e:
         print(
```

### Comparing `gdown-5.1.0/gdown/cached_download.py` & `gdown-5.2.0/gdown/cached_download.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/gdown/download.py` & `gdown-5.2.0/gdown/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import email.utils
 import os
 import os.path as osp
 import re
 import shutil
 import sys
 import tempfile
 import textwrap
@@ -72,14 +73,25 @@
     if m:
         filename = m.groups()[0]
         return filename
 
     return None
 
 
+def _get_modified_time_from_response(response):
+    if "Last-Modified" not in response.headers:
+        return None
+
+    raw = response.headers["Last-Modified"]
+    if raw is None:
+        return None
+
+    return email.utils.parsedate_to_datetime(raw)
+
+
 def _get_session(proxy, use_cookies, user_agent, return_cookies_file=False):
     sess = requests.session()
 
     sess.headers.update({"User-Agent": user_agent})
 
     if proxy is not None:
         sess.proxies = {"http": proxy, "https": proxy}
@@ -116,15 +128,17 @@
     """Download file from URL.
 
     Parameters
     ----------
     url: str
         URL. Google Drive URL is also supported.
     output: str
-        Output filename. Default is basename of URL.
+        Output filename/directory. Default is basename of URL.
+        If output ends with separator '/' basename will be kept and the
+        parameter will be treated as parenting directory.
     quiet: bool
         Suppress terminal output. Default is False.
     proxy: str
         Proxy.
     speed: float
         Download byte size per second (e.g., 256KB/s = 256 * 1024).
     use_cookies: bool
@@ -134,15 +148,15 @@
         certificate is verified, or a string, in which case it must be a path
         to a CA bundle to use. Default is True.
     id: str
         Google Drive's file ID.
     fuzzy: bool
         Fuzzy extraction of Google Drive's file Id. Default is False.
     resume: bool
-        Resume the download from existing tmp file if possible.
+        Resume interrupted downloads while skipping completed ones.
         Default is False.
     format: str, optional
         Format of Google Docs, Spreadsheets and Slides. Default is:
             - Google Docs: 'docx'
             - Google Spreadsheet: 'xlsx'
             - Google Slides: 'pptx'
     user_agent: str, optional
@@ -260,32 +274,39 @@
             ).format(
                 indent("\n".join(textwrap.wrap(str(e))), prefix="\t"),
                 url_origin,
             )
             raise FileURLRetrievalError(message)
 
     filename_from_url = None
+    last_modified_time = None
     if gdrive_file_id and is_gdrive_download_link:
         filename_from_url = _get_filename_from_response(response=res)
+        last_modified_time = _get_modified_time_from_response(response=res)
     if filename_from_url is None:
         filename_from_url = osp.basename(url)
 
     if output is None:
         output = filename_from_url
 
     output_is_path = isinstance(output, str)
     if output_is_path and output.endswith(osp.sep):
         if not osp.exists(output):
             os.makedirs(output)
         output = osp.join(output, filename_from_url)
 
     if output_is_path:
+        if resume and os.path.isfile(output):
+            if not quiet:
+                print(f"Skipping already downloaded file {output}", file=sys.stderr)
+            return output
+
         existing_tmp_files = []
         for file in os.listdir(osp.dirname(output) or "."):
-            if file.startswith(osp.basename(output)):
+            if file.startswith(osp.basename(output)) and file.endswith(".part"):
                 existing_tmp_files.append(osp.join(osp.dirname(output), file))
         if resume and existing_tmp_files:
             if len(existing_tmp_files) != 1:
                 print(
                     "There are multiple temporary files to resume:",
                     file=sys.stderr,
                 )
@@ -300,26 +321,29 @@
                 return
             tmp_file = existing_tmp_files[0]
         else:
             resume = False
             # mkstemp is preferred, but does not work on Windows
             # https://github.com/wkentaro/gdown/issues/153
             tmp_file = tempfile.mktemp(
-                suffix=tempfile.template,
+                suffix=".part",
                 prefix=osp.basename(output),
                 dir=osp.dirname(output),
             )
         f = open(tmp_file, "ab")
     else:
         tmp_file = None
         f = output
 
     if tmp_file is not None and f.tell() != 0:
-        headers = {"Range": "bytes={}-".format(f.tell())}
+        start_size = f.tell()
+        headers = {"Range": "bytes={}-".format(start_size)}
         res = sess.get(url, headers=headers, stream=True, verify=verify)
+    else:
+        start_size = 0
 
     if not quiet:
         print(log_messages.get("start", "Downloading...\n"), file=sys.stderr, end="")
         if resume:
             print("Resume:", tmp_file, file=sys.stderr)
         if url_origin != url:
             print("From (original):", url_origin, file=sys.stderr)
@@ -333,17 +357,17 @@
             file=sys.stderr,
             end="",
         )
 
     try:
         total = res.headers.get("Content-Length")
         if total is not None:
-            total = int(total)
+            total = int(total) + start_size
         if not quiet:
-            pbar = tqdm.tqdm(total=total, unit="B", unit_scale=True)
+            pbar = tqdm.tqdm(total=total, unit="B", initial=start_size, unit_scale=True)
         t_start = time.time()
         for chunk in res.iter_content(chunk_size=CHUNK_SIZE):
             f.write(chunk)
             if not quiet:
                 pbar.update(len(chunk))
             if speed is not None:
                 elapsed_time_expected = 1.0 * pbar.n / speed
@@ -351,11 +375,14 @@
                 if elapsed_time < elapsed_time_expected:
                     time.sleep(elapsed_time_expected - elapsed_time)
         if not quiet:
             pbar.close()
         if tmp_file:
             f.close()
             shutil.move(tmp_file, output)
+        if output_is_path and last_modified_time:
+            mtime = last_modified_time.timestamp()
+            os.utime(output, (mtime, mtime))
     finally:
         sess.close()
 
     return output
```

### Comparing `gdown-5.1.0/gdown/download_folder.py` & `gdown-5.2.0/gdown/download_folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     proxy=None,
     speed=None,
     use_cookies=True,
     remaining_ok=False,
     verify=True,
     user_agent=None,
     skip_download: bool = False,
+    resume=False,
 ) -> Union[List[str], List[GoogleDriveFileToDownload], None]:
     """Downloads entire folder from URL.
 
     Parameters
     ----------
     url: str
         URL of the Google Drive folder.
@@ -235,14 +236,19 @@
         certificate is verified, or a string, in which case it must be a path
         to a CA bundle to use. Default is True.
     user_agent: str, optional
         User-agent to use in the HTTP request.
     skip_download: bool, optional
         If True, return the list of files to download without downloading them.
         Defaults to False.
+    resume: bool
+        Resume interrupted transfers.
+        Completed output files will be skipped.
+        Partial tempfiles will be reused, if the transfer is incomplete.
+        Default is False.
 
     Returns
     -------
     files: List[str] or List[GoogleDriveFileToDownload] or None
         If dry_run is False, list of local file paths downloaded or None if failed.
         If dry_run is True, list of GoogleDriveFileToDownload that contains
         id, path, and local_path.
@@ -286,15 +292,15 @@
 
     if output is None:
         output = os.getcwd() + osp.sep
     if output.endswith(osp.sep):
         root_dir = osp.join(output, gdrive_file.name)
     else:
         root_dir = output
-    if not osp.exists(root_dir):
+    if not skip_download and not osp.exists(root_dir):
         os.makedirs(root_dir)
 
     files = []
     for id, path in directory_structure:
         local_path = osp.join(root_dir, path)
 
         if id is None:  # folder
@@ -303,22 +309,32 @@
             continue
 
         if skip_download:
             files.append(
                 GoogleDriveFileToDownload(id=id, path=path, local_path=local_path)
             )
         else:
+            if resume and os.path.isfile(local_path):
+                if not quiet:
+                    print(
+                        f"Skipping already downloaded file {local_path}",
+                        file=sys.stderr,
+                    )
+                files.append(local_path)
+                continue
+
             local_path = download(
                 url="https://drive.google.com/uc?id=" + id,
                 output=local_path,
                 quiet=quiet,
                 proxy=proxy,
                 speed=speed,
                 use_cookies=use_cookies,
                 verify=verify,
+                resume=resume,
             )
             if local_path is None:
                 if not quiet:
                     print("Download ended unsuccessfully", file=sys.stderr)
                 return None
             files.append(local_path)
     if not quiet:
```

### Comparing `gdown-5.1.0/gdown/extractall.py` & `gdown-5.2.0/gdown/extractall.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/gdown/parse_url.py` & `gdown-5.2.0/gdown/parse_url.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/tests/test___main__.py` & `gdown-5.2.0/tests/test___main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,39 @@
+import hashlib
 import os
-import shlex
 import subprocess
 import sys
 import tempfile
 
 from gdown.cached_download import _assert_filehash
+from gdown.cached_download import _compute_filehash
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 
 def _test_cli_with_md5(url_or_id, md5, options=None):
-    with tempfile.NamedTemporaryFile() as f:
-        cmd = f"gdown {url_or_id} -O {f.name}"
+    # We can't use NamedTemporaryFile because Windows doesn't allow the subprocess
+    # to write the file created by the parent process.
+    with tempfile.TemporaryDirectory() as d:
+        file_path = os.path.join(d, "file")
+        cmd = ["gdown", "--no-cookies", url_or_id, "-O", file_path]
         if options is not None:
-            cmd = f"{cmd} {options}"
-        subprocess.call(shlex.split(cmd))
-        _assert_filehash(path=f.name, hash=f"md5:{md5}")
+            cmd.extend(options)
+        subprocess.call(cmd)
+        _assert_filehash(path=file_path, hash=f"md5:{md5}")
 
 
 def _test_cli_with_content(url_or_id, content):
-    with tempfile.NamedTemporaryFile() as f:
-        subprocess.call(shlex.split(f"gdown {url_or_id} -O {f.name}"))
-        with open(f.name) as f:
+    # We can't use NamedTemporaryFile because Windows doesn't allow the subprocess
+    # to write the file created by the parent process.
+    with tempfile.TemporaryDirectory() as d:
+        file_path = os.path.join(d, "file")
+        cmd = ["gdown", "--no-cookies", url_or_id, "-O", file_path]
+        subprocess.call(cmd)
+        with open(file_path) as f:
             assert f.read() == content
 
 
 def test_download_from_url_other_than_gdrive():
     url = "https://raw.githubusercontent.com/wkentaro/gdown/3.1.0/gdown/__init__.py"
     md5 = "2a51927dde6b146ce56b4d89ebbb5268"
     _test_cli_with_md5(url_or_id=url, md5=md5)
@@ -59,49 +67,63 @@
             continue
     else:
         file_ids, _ = zip(*file_id_and_md5s)
         raise AssertionError(f"Failed to download any of the files: {file_ids}")
 
 
 def test_download_and_extract():
-    cmd = "gdown https://github.com/wkentaro/gdown/archive/refs/tags/v4.0.0.tar.gz -O - | tar zxvf -"  # noqa: E501
+    cmd = "gdown --no-cookies https://github.com/wkentaro/gdown/archive/refs/tags/v4.0.0.tar.gz -O - | tar zxvf -"  # noqa: E501
     with tempfile.TemporaryDirectory() as d:
         subprocess.call(cmd, shell=True, cwd=d)
         assert os.path.exists(os.path.join(d, "gdown-4.0.0/gdown/__init__.py"))
 
 
 def test_download_folder_from_gdrive():
     with open(os.path.join(here, "data/folder_ids.csv")) as f:
         folder_id_and_md5s = [
             [x.strip() for x in folder_id.split(",")] for folder_id in f
         ]
 
     for folder_id, md5 in folder_id_and_md5s:
         with tempfile.TemporaryDirectory() as d:
-            cmd = f"gdown {folder_id} -O {d} --folder"
-            subprocess.call(shlex.split(cmd))
+            cmd = ["gdown", "--no-cookies", folder_id, "-O", d, "--folder"]
+            subprocess.call(cmd)
 
-            cmd = "find . -type f -exec md5sum {} \\; | awk '{print $1}' | sort | md5sum | awk '{print $1}'"  # noqa: E501
-            md5_actual = (
-                subprocess.check_output(cmd, shell=True, cwd=d).decode().strip()
-            )
+            md5s_actual = []
+            for dirpath, dirnames, filenames in os.walk(d):
+                for filename in filenames:
+                    md5_actual = _compute_filehash(
+                        path=os.path.join(dirpath, filename), algorithm="md5"
+                    )[len("md5:") :]
+                    md5s_actual.append(md5_actual)
+
+            md5_actual = hashlib.md5(
+                ("".join(x + "\n" for x in sorted(md5s_actual))).encode()
+            ).hexdigest()
         try:
             assert md5_actual == md5
             break
         except AssertionError as e:
             print(e, file=sys.stderr)
     else:
         file_ids, md5s = zip(*folder_id_and_md5s)
         raise AssertionError(f"Failed to download any of the folders: {file_ids}")
 
 
 def test_download_a_folder_with_remining_ok_false():
     with tempfile.TemporaryDirectory() as d:
-        cmd = f"gdown https://drive.google.com/drive/folders/1gd3xLkmjT8IckN6WtMbyFZvLR4exRIkn -O {d} --folder"  # noqa: E501
-    assert subprocess.call(shlex.split(cmd)) == 1
+        cmd = [
+            "gdown",
+            "--no-cookies",
+            "https://drive.google.com/drive/folders/1gd3xLkmjT8IckN6WtMbyFZvLR4exRIkn",
+            "-O",
+            d,
+            "--folder",
+        ]
+    assert subprocess.call(cmd) == 1
 
 
 # def test_download_docs_from_gdrive():
 #     file_id = "1TFYNzuZJTgNGzGmjraZ58ZVOh9_YoKeBnU-opWgXQL4"
 #     md5 = "6c17d87d3d01405ac5c9bb65ee2d2fc2"
 #     _test_cli_with_md5(url_or_id=file_id, md5=md5, options="--format txt")
 #
@@ -111,20 +133,20 @@
 #     md5 = "5be20dd8a23afa06365714edc24856f3"
 #     _test_cli_with_md5(url_or_id=file_id, md5=md5, options="--format pdf")
 
 
 def test_download_slides_from_gdrive():
     file_id = "13AhW1Z1GYGaiTpJ0Pr2TTXoQivb6jx-a"
     md5 = "96704c6c40e308a68d3842e83a0136b9"
-    _test_cli_with_md5(url_or_id=file_id, md5=md5, options="--format pdf")
+    _test_cli_with_md5(url_or_id=file_id, md5=md5, options=["--format", "pdf"])
 
 
 def test_download_a_folder_with_file_content_more_than_the_limit():
     url = "https://drive.google.com/drive/folders/1gd3xLkmjT8IckN6WtMbyFZvLR4exRIkn"
 
     with tempfile.TemporaryDirectory() as d:
-        cmd = f"gdown {url} -O {d} --folder --remaining-ok"
-        subprocess.check_call(shlex.split(cmd))
+        cmd = ["gdown", "--no-cookies", url, "-O", d, "--folder", "--remaining-ok"]
+        subprocess.check_call(cmd)
 
         filenames = sorted(os.listdir(d))
         for i in range(50):
             assert filenames[i] == f"file_{i:02d}.txt"
```

### Comparing `gdown-5.1.0/tests/test_cached_download.py` & `gdown-5.2.0/tests/test_cached_download.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/tests/test_download_folder.py` & `gdown-5.2.0/tests/test_download_folder.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/tests/test_parse_url.py` & `gdown-5.2.0/tests/test_parse_url.py`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/tests/data/folder-page-sample.html` & `gdown-5.2.0/tests/data/folder-page-sample.html`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/LICENSE` & `gdown-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdown-5.1.0/pyproject.toml` & `gdown-5.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,15 @@
   "build",
   "mypy",
   "pytest",
   "pytest-xdist",
   "ruff",
   "twine",
   "types-requests",
+  "types-setuptools",
 ]
 
 [project.urls]
 Homepage = "https://github.com/wkentaro/gdown"
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
@@ -96,9 +97,9 @@
 
 # Like Black, respect magic trailing commas.
 skip-magic-trailing-comma = false
 
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
```

### Comparing `gdown-5.1.0/PKG-INFO` & `gdown-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gdown
-Version: 5.1.0
+Version: 5.2.0
 Summary: Google Drive Public File/Folder Downloader
 Project-URL: Homepage, https://github.com/wkentaro/gdown
 Author-email: Kentaro Wada <www.kentaro.wada@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: curl,download,google-drive,wget
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,29 +29,30 @@
 Requires-Dist: build; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Requires-Dist: twine; extra == 'test'
 Requires-Dist: types-requests; extra == 'test'
+Requires-Dist: types-setuptools; extra == 'test'
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>gdown</h1>
   <p><b>Google Drive Public File Downloader when Curl/Wget Fails</b></p>
   <img src="https://github.com/wkentaro/gdown/raw/main/.readme/cli.png" width="80%">
   <img src="https://github.com/wkentaro/gdown/raw/main/.readme/python.png" width="80%">
   <br>
   <br>
 </div>
 
 
 *Gdown* downloads a public file/folder from Google Drive.
 
-*Gdown* provides what's curl/wget doesn't for Google Drive:
+*Gdown* provides what curl/wget doesn't for Google Drive:
 - **Skip the security notice** allowing you to download large files (curl/wget fails);
 - **Recursive download** of files in a folder (maximum 50 files per folder);
 - **Specify download file format** for Google Slides/Sheet/Docs like PDF/XML/CSV.
 
 
 ## Installation
 
@@ -146,19 +147,19 @@
 id = "15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
 gdown.download_folder(id=id)
 ```
 
 
 ## FAQ
 
-### I get 'Permission Denied' error.
+### I get a 'Permission Denied' error.
 
 Have you made sure you set the file permission to 'Anyone with Link'?
 
-### I set the permission 'Anyone with Link', but still can't download.
+### I set the permission 'Anyone with Link', but I still can't download.
 
 Google restricts access to a file when the download is concentrated.
 If you can still access to the file from your browser, downloading cookies file might
 help. Follow this step: 1) download cookies.txt using browser extensions like
 ([Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc));
 2) mv the `cookies.txt` to `~/.cache/gdown/cookies.txt`; 3) run download again.
 If you're using `gdown>=5.0.0`, it should be able to use the cookies same as your browser.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gdown Version: 5.1.0 Summary: Google Drive Public
+Metadata-Version: 2.3 Name: gdown Version: 5.2.0 Summary: Google Drive Public
 File/Folder Downloader Project-URL: Homepage, https://github.com/wkentaro/gdown
 Author-email: Kentaro Wada
 gmail.com> License: MIT License-File: LICENSE Keywords: curl,download,google-
 drive,wget Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -12,37 +12,38 @@
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4 Requires-Dist: filelock Requires-Dist: requests
 [socks] Requires-Dist: tqdm Provides-Extra: test Requires-Dist: build; extra ==
 'test' Requires-Dist: mypy; extra == 'test' Requires-Dist: pytest; extra ==
 'test' Requires-Dist: pytest-xdist; extra == 'test' Requires-Dist: ruff; extra
 == 'test' Requires-Dist: twine; extra == 'test' Requires-Dist: types-requests;
-extra == 'test' Description-Content-Type: text/markdown
+extra == 'test' Requires-Dist: types-setuptools; extra == 'test' Description-
+Content-Type: text/markdown
                               ************ ggddoowwnn ************
            GGooooggllee DDrriivvee PPuubblliicc FFiillee DDoowwnnllooaaddeerr wwhheenn CCuurrll//WWggeett FFaaiillss
      [https://github.com/wkentaro/gdown/raw/main/.readme/cli.png][https://
             github.com/wkentaro/gdown/raw/main/.readme/python.png]
 
-*Gdown* downloads a public file/folder from Google Drive. *Gdown* provides
-what's curl/wget doesn't for Google Drive: - **Skip the security notice**
-allowing you to download large files (curl/wget fails); - **Recursive
-download** of files in a folder (maximum 50 files per folder); - **Specify
-download file format** for Google Slides/Sheet/Docs like PDF/XML/CSV. ##
-Installation _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_d_o_w_n_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_d_o_w_n_._s_v_g_]```bash pip install gdown # to upgrade pip
-install --upgrade gdown ``` ## Usage ### via Command Line ```bash $ gdown --
-help usage: gdown [-h] [-V] [-O OUTPUT] [-q] [--fuzzy] [--id] [--proxy PROXY]
-[--speed SPEED] [--no-cookies] [--no-check-certificate] [--continue] [--folder]
-[--remaining-ok] url_or_id ... $ # a large file (~500MB) $ gdown https://
-drive.google.com/uc?id=1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ md5sum
-fcn8s_from_caffe.npz 256c2a8235c1c65e62e48d3284fbd384 $ # same as the above but
-with the file ID $ gdown 1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ # a small file $
-gdown https://drive.google.com/uc?id=0B9P1L--7Wd2vU3VUVlFnbTgtS2c $ cat
-spam.txt spam $ # download with fuzzy extraction of a file ID $ gdown --fuzzy
-'https://drive.google.com/file/d/0B9P1L--7Wd2vU3VUVlFnbTgtS2c/
+*Gdown* downloads a public file/folder from Google Drive. *Gdown* provides what
+curl/wget doesn't for Google Drive: - **Skip the security notice** allowing you
+to download large files (curl/wget fails); - **Recursive download** of files in
+a folder (maximum 50 files per folder); - **Specify download file format** for
+Google Slides/Sheet/Docs like PDF/XML/CSV. ## Installation _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_d_o_w_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_g_d_o_w_n_._s_v_g_]```bash pip install gdown # to upgrade pip install --upgrade gdown
+``` ## Usage ### via Command Line ```bash $ gdown --help usage: gdown [-h] [-V]
+[-O OUTPUT] [-q] [--fuzzy] [--id] [--proxy PROXY] [--speed SPEED] [--no-
+cookies] [--no-check-certificate] [--continue] [--folder] [--remaining-ok]
+url_or_id ... $ # a large file (~500MB) $ gdown https://drive.google.com/
+uc?id=1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ md5sum fcn8s_from_caffe.npz
+256c2a8235c1c65e62e48d3284fbd384 $ # same as the above but with the file ID $
+gdown 1l_5RK28JRL19wpT22B-DY9We3TVXnnQQ $ # a small file $ gdown https://
+drive.google.com/uc?id=0B9P1L--7Wd2vU3VUVlFnbTgtS2c $ cat spam.txt spam $ #
+download with fuzzy extraction of a file ID $ gdown --fuzzy 'https://
+drive.google.com/file/d/0B9P1L--7Wd2vU3VUVlFnbTgtS2c/
 view?usp=sharing&resourcekey=0-WWs_XOSctfaY_0-sJBKRSQ' $ cat spam.txt spam $ #
 --fuzzy option also works with Microsoft Powerpoint files $ gdown --fuzzy
 "https://docs.google.com/presentation/d/15umvZKlsJ3094HNg5S4vJsIhxcFlyTeK/
 edit?usp=sharing&ouid=117512221203072002113&rtpof=true&sd=true" $ # a folder $
 gdown https://drive.google.com/drive/folders/15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl
 -O /tmp/folder --folder $ # as an alternative to curl/wget $ gdown https://
 httpbin.org/ip -O ip.json $ cat ip.json { "origin": "126.169.213.247" } $ #
@@ -58,17 +59,17 @@
 7Wd2vNm9zMTJWOGxobkU/view?usp=sharing" gdown.download(url=url, output=output,
 fuzzy=True) # Cached download with identity check via MD5 (or SHA1, SHA256,
 etc). # Pass postprocess function e.g., extracting compressed file. md5 = "md5:
 fa837a88f0c40c513d975104edf3da17" gdown.cached_download(url, output, hash=hash,
 postprocess=gdown.extractall) # a folder url = "https://drive.google.com/drive/
 folders/15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl" gdown.download_folder(url) # same as
 the above, but with the folder ID id = "15uNXeRBIhVvZJIhL4yTw4IsStMhUaaxl"
-gdown.download_folder(id=id) ``` ## FAQ ### I get 'Permission Denied' error.
+gdown.download_folder(id=id) ``` ## FAQ ### I get a 'Permission Denied' error.
 Have you made sure you set the file permission to 'Anyone with Link'? ### I set
-the permission 'Anyone with Link', but still can't download. Google restricts
+the permission 'Anyone with Link', but I still can't download. Google restricts
 access to a file when the download is concentrated. If you can still access to
 the file from your browser, downloading cookies file might help. Follow this
 step: 1) download cookies.txt using browser extensions like ([Get cookies.txt
 LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/
 cclelndahbckbenkjhflpdbgdldlbecc)); 2) mv the `cookies.txt` to `~/.cache/gdown/
 cookies.txt`; 3) run download again. If you're using `gdown>=5.0.0`, it should
 be able to use the cookies same as your browser. ## License MIT
```

