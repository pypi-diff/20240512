# Comparing `tmp/lnurl_nostr1-0.5.0rc5.tar.gz` & `tmp/lnurl_nostr1-0.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl_nostr1-0.5.0rc5.tar", max compression
+gzip compressed data, was "lnurl_nostr1-0.5.1rc1.tar", max compression
```

## Comparing `lnurl_nostr1-0.5.0rc5.tar` & `lnurl_nostr1-0.5.1rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.0rc5/LICENSE
--rwxr-xr-x   0        0        0     6290 2024-04-28 16:27:06.935463 lnurl_nostr1-0.5.0rc5/README.md
--rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.0rc5/lnurl/__init__.py
--rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.0rc5/lnurl/cli.py
--rw-r--r--   0        0        0     4885 2024-04-28 16:18:44.299319 lnurl_nostr1-0.5.0rc5/lnurl/core.py
--rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.0rc5/lnurl/exceptions.py
--rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.0rc5/lnurl/helpers.py
--rw-r--r--   0        0        0     5568 2024-04-28 16:18:44.300097 lnurl_nostr1-0.5.0rc5/lnurl/models.py
--rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.0rc5/lnurl/py.typed
--rw-r--r--   0        0        0     9969 2024-04-28 17:33:27.979186 lnurl_nostr1-0.5.0rc5/lnurl/types.py
--rw-r--r--   0        0        0     1962 2024-04-28 17:39:30.584004 lnurl_nostr1-0.5.0rc5/pyproject.toml
--rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.1rc1/LICENSE
+-rwxr-xr-x   0        0        0     6246 2024-05-11 23:54:04.691040 lnurl_nostr1-0.5.1rc1/README.md
+-rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.1rc1/lnurl/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.1rc1/lnurl/cli.py
+-rw-r--r--   0        0        0     6726 2024-05-11 20:59:34.262419 lnurl_nostr1-0.5.1rc1/lnurl/core.py
+-rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.1rc1/lnurl/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.1rc1/lnurl/helpers.py
+-rw-r--r--   0        0        0     5601 2024-05-11 21:00:28.213024 lnurl_nostr1-0.5.1rc1/lnurl/models.py
+-rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.1rc1/lnurl/py.typed
+-rw-r--r--   0        0        0     9119 2024-05-11 23:29:02.984282 lnurl_nostr1-0.5.1rc1/lnurl/types.py
+-rw-r--r--   0        0        0     1962 2024-05-11 23:43:24.886472 lnurl_nostr1-0.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7012 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.1rc1/PKG-INFO
```

### Comparing `lnurl_nostr1-0.5.0rc5/LICENSE` & `lnurl_nostr1-0.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc5/README.md` & `lnurl_nostr1-0.5.1rc1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 [![github-mypy-badge]][github-mypy]
 [![codecov-badge]][codecov]
 [![pypi-badge]][pypi]
 [![pypi-versions-badge]][pypi]
 [![license-badge]](LICENSE)
 
 
-A collection of helpers for building [LNURL][lnurl] support into wallets and services, with support for future *nostr1* protocol.
+A collection of helpers for building [LNURL][lnurl] support into wallets and services.
 
 Configuration
 -------------
 
 Developers can force strict RFC3986 validation for the URLs that the library encodes/decodes, using this env var:
 
 > LNURL_STRICT_RFC3986 = "0" by default (False)
 
 
 Basic usage
 -----------
 
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.encode('https://service.io/?q=3fc3645b439ce8e7')
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.encode('https://service.io/?q=3fc3645b439ce8e7')
 Lnurl('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', bech32=Bech32('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', hrp='lnurl', data=[13, 1, 26, 7, 8, 28, 3, 19, 7, 8, 23, 18, 30, 28, 27, 5, 14, 9, 27, 6, 18, 24, 27, 5, 5, 25, 20, 22, 30, 11, 25, 31, 14, 4, 30, 19, 6, 25, 19, 3, 6, 12, 27, 3, 8, 13, 11, 2, 6, 16, 25, 19, 18, 24, 27, 5, 7, 1, 18, 19, 14]), url=WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7'))
->>> lnurl_nostr1.decode('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9')
+>>> lnurl.decode('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9')
 WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7')
 ```
 
 The `Lnurl` object wraps a bech32 LNURL to provide some extra utilities.
 
 ```python
 from lnurl_nostr1 import Lnurl
@@ -74,23 +74,23 @@
 r = requests.get(lnurl.url)
 ```
 
 If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
 You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
 ```
 
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
```

### Comparing `lnurl_nostr1-0.5.0rc5/lnurl/__init__.py` & `lnurl_nostr1-0.5.1rc1/lnurl/__init__.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc5/lnurl/cli.py` & `lnurl_nostr1-0.5.1rc1/lnurl/cli.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc5/lnurl/helpers.py` & `lnurl_nostr1-0.5.1rc1/lnurl/helpers.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc5/lnurl/models.py` & `lnurl_nostr1-0.5.1rc1/lnurl/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     ClearnetUrl,
     DebugUrl,
     InitializationVector,
     LightningInvoice,
     LightningNodeUri,
     LnurlPayMetadata,
     Max144Str,
-    OnionUrl,
     Nostr1Url,
+    OnionUrl,
 )
 
 
 class LnurlPayRouteHop(BaseModel):
     node_id: str = Field(..., alias="nodeId")
     channel_update: str = Field(..., alias="channelUpdate")
 
@@ -37,15 +37,15 @@
 class MessageAction(LnurlPaySuccessAction):
     tag: Literal["message"] = "message"
     message: Max144Str
 
 
 class UrlAction(LnurlPaySuccessAction):
     tag: Literal["url"] = "url"
-    url: Union[ClearnetUrl, OnionUrl, DebugUrl, Nostr1Url]
+    url: Union[ClearnetUrl, OnionUrl, Nostr1Url, DebugUrl]
     description: Max144Str
 
 
 class LnurlResponseModel(BaseModel):
 
     class Config:
         allow_population_by_field_name = True
@@ -78,35 +78,35 @@
 
 class LnurlSuccessResponse(LnurlResponseModel):
     status: Literal["OK"] = "OK"
 
 
 class LnurlAuthResponse(LnurlResponseModel):
     tag: Literal["login"] = "login"
-    callback: Union[ClearnetUrl, OnionUrl, DebugUrl, Nostr1Url]
+    callback: Union[ClearnetUrl, OnionUrl, Nostr1Url, DebugUrl]
     k1: str
 
 
 class LnurlChannelResponse(LnurlResponseModel):
     tag: Literal["channelRequest"] = "channelRequest"
     uri: LightningNodeUri
-    callback: Union[ClearnetUrl, OnionUrl, DebugUrl, Nostr1Url]
+    callback: Union[ClearnetUrl, OnionUrl, Nostr1Url, DebugUrl]
     k1: str
 
 
 class LnurlHostedChannelResponse(LnurlResponseModel):
     tag: Literal["hostedChannelRequest"] = "hostedChannelRequest"
     uri: LightningNodeUri
     k1: str
     alias: Optional[str]
 
 
 class LnurlPayResponse(LnurlResponseModel):
     tag: Literal["payRequest"] = "payRequest"
-    callback: Union[ClearnetUrl, OnionUrl, DebugUrl, Nostr1Url]
+    callback: Union[ClearnetUrl, OnionUrl, Nostr1Url, DebugUrl]
     min_sendable: MilliSatoshi = Field(..., alias="minSendable", gt=0)
     max_sendable: MilliSatoshi = Field(..., alias="maxSendable", gt=0)
     metadata: LnurlPayMetadata
 
     @validator("max_sendable")
     def max_less_than_min(cls, value, values, **kwargs):  # noqa
         if "min_sendable" in values and value < values["min_sendable"]:
@@ -135,19 +135,20 @@
     )
 
 
 class LnurlPayActionResponse(LnurlResponseModel):
     pr: LightningInvoice
     success_action: Optional[Union[MessageAction, UrlAction, AesAction]] = Field(None, alias="successAction")
     routes: List[List[LnurlPayRouteHop]] = []
+    verify: Optional[str] = None
 
 
 class LnurlWithdrawResponse(LnurlResponseModel):
     tag: Literal["withdrawRequest"] = "withdrawRequest"
-    callback: Union[ClearnetUrl, OnionUrl, DebugUrl, Nostr1Url]
+    callback: Union[ClearnetUrl, OnionUrl, Nostr1Url, DebugUrl]
     k1: str
     min_withdrawable: MilliSatoshi = Field(..., alias="minWithdrawable", gt=0)
     max_withdrawable: MilliSatoshi = Field(..., alias="maxWithdrawable", gt=0)
     default_description: str = Field("", alias="defaultDescription")
 
     @validator("max_withdrawable")
     def max_less_than_min(cls, value, values, **kwargs):  # noqa
```

### Comparing `lnurl_nostr1-0.5.0rc5/lnurl/types.py` & `lnurl_nostr1-0.5.1rc1/lnurl/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ConstrainedStr,
     HttpUrl,
     Json,
     ValidationError,
     parse_obj_as,
     validator,
 )
-from pydantic.errors import UrlHostTldError, UrlSchemeError, UrlPortError, UrlHostError
+from pydantic.errors import UrlHostTldError, UrlSchemeError
 from pydantic.networks import Parts
 from pydantic.validators import str_validator
 
 from .exceptions import InvalidLnurlPayMetadata
 from .helpers import _bech32_decode, _lnurl_clean, lnurl_decode
 
 
@@ -99,18 +99,15 @@
     """Unsecure web URL, to make developers life easier."""
 
     allowed_schemes = {"http"}
 
     @classmethod
     def validate_host(cls, parts: Parts) -> Tuple[str, Optional[str], str, bool]:
         host, tld, host_type, rebuild = super().validate_host(parts)
-        allowed_hosts = ["127.0.0.1", "0.0.0.0"] + [
-            h for h in os.environ.get("LNURL_UNSECURE_HOSTS", "").split(" ") if h != ""
-        ]
-        if host not in allowed_hosts:
+        if host not in ["127.0.0.1", "0.0.0.0"]:
             raise UrlSchemeError()
         return host, tld, host_type, rebuild
 
 
 class ClearnetUrl(Url):
     """Secure web URL."""
 
@@ -125,48 +122,24 @@
     @classmethod
     def validate_host(cls, parts: Parts) -> Tuple[str, Optional[str], str, bool]:
         host, tld, host_type, rebuild = super().validate_host(parts)
         if tld != "onion":
             raise UrlHostTldError()
         return host, tld, host_type, rebuild
 
-class UrlPortNotAllowedError(UrlPortError):
-    msg_template = 'URL port not allowed'
-
 class Nostr1Url(Url):
-    """Nostr1 URL."""
-
-    allowed_schemes = {"nostr1"}
-
-    tld_required = False
-
-    @staticmethod
-    def _validate_port(port: Optional[str]) -> None:
-        if port is not None:
-            raise UrlPortNotAllowedError()
-
-    @staticmethod
-    def get_default_parts(parts: 'Parts') -> 'Parts':
-        return {}
+    """Nostr DM service, version 1."""
 
-    @classmethod
-    def validate_parts(cls, parts: 'Parts', validate_port: bool = True) -> 'Parts':
-        return super().validate_parts(parts, validate_port=True)
+    allowed_schemes = {"http"}
 
     @classmethod
     def validate_host(cls, parts: Parts) -> Tuple[str, Optional[str], str, bool]:
         host, tld, host_type, rebuild = super().validate_host(parts)
-        if tld or not host:
-            raise UrlHostError()
-        try:
-            hrp, data = _bech32_decode(host)
-        except:
-            raise UrlHostError()
-        if hrp != 'npub' or len(data) != 52:
-            raise UrlHostError()
+        if tld != "nostr1":
+            raise UrlHostTldError()
         return host, tld, host_type, rebuild
 
 class LightningInvoice(Bech32):
     """Bech32 Lightning invoice."""
 
 
 class LightningNodeUri(ReprMixin, str):
@@ -201,24 +174,24 @@
 
 class Lnurl(ReprMixin, str):
     __slots__ = ("bech32", "url")
 
     def __new__(cls, lightning: str, **_) -> "Lnurl":
         return str.__new__(cls, _lnurl_clean(lightning))
 
-    def __init__(self, lightning: str, *, url: Optional[Union[OnionUrl, ClearnetUrl, DebugUrl, Nostr1Url]] = None):
+    def __init__(self, lightning: str, *, url: Optional[Union[OnionUrl, Nostr1Url, ClearnetUrl, DebugUrl]] = None):
         bech32 = _lnurl_clean(lightning)
         str.__init__(bech32)
         self.bech32 = Bech32(bech32)
         self.url = url if url else self.__get_url__(bech32)
 
     @classmethod
-    def __get_url__(cls, bech32: str) -> Union[OnionUrl, ClearnetUrl, DebugUrl, Nostr1Url]:
+    def __get_url__(cls, bech32: str) -> Union[OnionUrl, Nostr1Url, ClearnetUrl, DebugUrl]:
         url: str = lnurl_decode(bech32)
-        return parse_obj_as(Union[OnionUrl, ClearnetUrl, DebugUrl, Nostr1Url], url)  # type: ignore
+        return parse_obj_as(Union[OnionUrl, Nostr1Url, ClearnetUrl, DebugUrl], url)  # type: ignore
 
     @classmethod
     def __get_validators__(cls):
         yield str_validator
         yield cls.validate
 
     @classmethod
@@ -243,18 +216,18 @@
 
     @validator("address")
     def is_valid_email_address(cls, email: str) -> bool:
         email_regex = r"[A-Za-z0-9\._%+-]+@[A-Za-z0-9\.-]+\.[A-Za-z]{2,63}"
         return re.fullmatch(email_regex, email) is not None
 
     @classmethod
-    def __get_url__(cls, address: str) -> Union[OnionUrl, ClearnetUrl, DebugUrl, Nostr1Url]:
+    def __get_url__(cls, address: str) -> Union[OnionUrl, Nostr1Url, ClearnetUrl, DebugUrl]:
         name, domain = address.split("@")
         url = ("http://" if domain.endswith(".onion") else "https://") + domain + "/.well-known/lnurlp/" + name
-        return parse_obj_as(Union[OnionUrl, ClearnetUrl, DebugUrl, Nostr1Url], url)  # type: ignore
+        return parse_obj_as(Union[OnionUrl, Nostr1Url, ClearnetUrl, DebugUrl], url)  # type: ignore
 
 
 class LnurlPayMetadata(ReprMixin, str):
     valid_metadata_mime_types = {"text/plain", "image/png;base64", "image/jpeg;base64"}
 
     __slots__ = ("_list",)
```

### Comparing `lnurl_nostr1-0.5.0rc5/pyproject.toml` & `lnurl_nostr1-0.5.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnurl_nostr1"
-version = "0.5.0rc5"
+version = "0.5.1rc1"
 description = "LNURL implementation for Python, with support for future nostr1 protocol."
 authors = ["Alan Bits <alan@lnbits.com>", "Oren <orenz0@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "*.py", from = "lnurl", to = "lnurl_nostr1"},
   {include = "py.typed", from = "lnurl", to = "lnurl_nostr1/py.typed"},
```

### Comparing `lnurl_nostr1-0.5.0rc5/PKG-INFO` & `lnurl_nostr1-0.5.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnurl_nostr1
-Version: 0.5.0rc5
+Version: 0.5.1rc1
 Summary: LNURL implementation for Python, with support for future nostr1 protocol.
 License: MIT
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,32 +26,32 @@
 [![github-mypy-badge]][github-mypy]
 [![codecov-badge]][codecov]
 [![pypi-badge]][pypi]
 [![pypi-versions-badge]][pypi]
 [![license-badge]](LICENSE)
 
 
-A collection of helpers for building [LNURL][lnurl] support into wallets and services, with support for future *nostr1* protocol.
+A collection of helpers for building [LNURL][lnurl] support into wallets and services.
 
 Configuration
 -------------
 
 Developers can force strict RFC3986 validation for the URLs that the library encodes/decodes, using this env var:
 
 > LNURL_STRICT_RFC3986 = "0" by default (False)
 
 
 Basic usage
 -----------
 
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.encode('https://service.io/?q=3fc3645b439ce8e7')
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.encode('https://service.io/?q=3fc3645b439ce8e7')
 Lnurl('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', bech32=Bech32('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9', hrp='lnurl', data=[13, 1, 26, 7, 8, 28, 3, 19, 7, 8, 23, 18, 30, 28, 27, 5, 14, 9, 27, 6, 18, 24, 27, 5, 5, 25, 20, 22, 30, 11, 25, 31, 14, 4, 30, 19, 6, 25, 19, 3, 6, 12, 27, 3, 8, 13, 11, 2, 6, 16, 25, 19, 18, 24, 27, 5, 7, 1, 18, 19, 14]), url=WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7'))
->>> lnurl_nostr1.decode('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9')
+>>> lnurl.decode('LNURL1DP68GURN8GHJ7UM9WFMXJCM99E5K7TELWY7NXENRXVMRGDTZXSENJCM98PJNWXQ96S9')
 WebUrl('https://service.io/?q=3fc3645b439ce8e7', scheme='https', host='service.io', tld='io', host_type='domain', path='/', query='q=3fc3645b439ce8e7')
 ```
 
 The `Lnurl` object wraps a bech32 LNURL to provide some extra utilities.
 
 ```python
 from lnurl_nostr1 import Lnurl
@@ -95,23 +95,23 @@
 r = requests.get(lnurl.url)
 ```
 
 If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
 You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
 ```python
->>> import lnurl_nostr1
->>> lnurl_nostr1.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+>>> import lnurl_nostr1 as lnurl
+>>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
 ```
 
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
```

