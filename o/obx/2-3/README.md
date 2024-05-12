# Comparing `tmp/obx-2.tar.gz` & `tmp/obx-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obx-2.tar", last modified: Mon Feb 26 13:09:30 2024, max compression
+gzip compressed data, was "obx-3.tar", last modified: Sun May 12 06:28:49 2024, max compression
```

## Comparing `obx-2.tar` & `obx-3.tar`

### file list

```diff
@@ -1,24 +1,51 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-26 13:09:30.714496 obx-2/
--rw-r--r--   0 bart      (1000) bart      (1000)     1890 2024-02-26 13:09:30.714496 obx-2/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1363 2024-02-26 12:59:40.000000 obx-2/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-26 13:09:30.714496 obx-2/obx/
--rw-r--r--   0 bart      (1000) bart      (1000)     1339 2024-02-26 03:57:56.000000 obx-2/obx/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      714 2024-02-25 14:48:51.000000 obx-2/obx/brokers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1539 2024-02-25 14:49:09.000000 obx-2/obx/excepts.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6325 2024-02-26 03:53:29.000000 obx-2/obx/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1852 2024-02-26 03:54:22.000000 obx-2/obx/locates.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5450 2024-02-26 03:59:01.000000 obx-2/obx/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6007 2024-02-26 03:53:41.000000 obx-2/obx/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1914 2024-02-25 14:38:05.000000 obx-2/obx/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1236 2024-02-25 14:50:43.000000 obx-2/obx/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1860 2024-02-25 14:57:48.000000 obx-2/obx/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)      646 2024-02-25 14:38:05.000000 obx-2/obx/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-26 13:09:30.714496 obx-2/obx.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     1890 2024-02-26 13:09:30.000000 obx-2/obx.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      330 2024-02-26 13:09:30.000000 obx-2/obx.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-26 13:09:30.000000 obx-2/obx.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2024-02-26 13:09:30.000000 obx-2/obx.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-26 13:09:30.000000 obx-2/obx.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      699 2024-02-26 13:01:15.000000 obx-2/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-02-26 13:09:30.714496 obx-2/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-02-23 15:58:09.000000 obx-2/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.036146 obx-3/
+-rw-r--r--   0 bart      (1000) bart      (1001)     1833 2024-05-12 06:28:49.036146 obx-3/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1306 2024-05-12 06:27:07.000000 obx-3/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.032147 obx-3/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2554 2024-05-12 06:04:04.000000 obx-3/bin/obx
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1934 2024-05-12 06:04:23.000000 obx-3/bin/obxd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.032147 obx-3/obx/
+-rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:58:53.000000 obx-3/obx/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:58:53.000000 obx-3/obx/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:58:53.000000 obx-3/obx/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:58:53.000000 obx-3/obx/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:58:53.000000 obx-3/obx/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:58:53.000000 obx-3/obx/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:58:53.000000 obx-3/obx/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.036146 obx-3/obx/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      772 2024-05-12 06:04:49.000000 obx-3/obx/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:58:59.000000 obx-3/obx/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:58:59.000000 obx-3/obx/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      735 2024-05-12 06:13:41.000000 obx-3/obx/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:58:59.000000 obx-3/obx/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      706 2024-05-12 06:06:43.000000 obx-3/obx/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3554 2024-05-12 06:05:56.000000 obx-3/obx/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17337 2024-05-12 06:14:35.000000 obx-3/obx/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:58:59.000000 obx-3/obx/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 06:03:08.000000 obx-3/obx/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10786 2024-05-12 06:12:11.000000 obx-3/obx/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3148 2024-05-12 06:08:04.000000 obx-3/obx/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1156 2024-05-12 06:06:16.000000 obx-3/obx/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:58:59.000000 obx-3/obx/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5177 2024-05-12 06:10:09.000000 obx-3/obx/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3062 2024-05-12 06:08:29.000000 obx-3/obx/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5729 2024-05-12 06:03:08.000000 obx-3/obx/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:58:53.000000 obx-3/obx/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:58:53.000000 obx-3/obx/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:58:53.000000 obx-3/obx/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.032147 obx-3/obx.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     1833 2024-05-12 06:28:48.000000 obx-3/obx.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      767 2024-05-12 06:28:49.000000 obx-3/obx.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 06:28:48.000000 obx-3/obx.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-12 06:28:48.000000 obx-3/obx.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 06:28:14.000000 obx-3/obx.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)      766 2024-05-12 06:23:08.000000 obx-3/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-12 06:28:49.036146 obx-3/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      179 2024-05-12 06:21:25.000000 obx-3/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 06:28:49.036146 obx-3/tests/
+-rw-r--r--   0 bart      (1000) bart      (1001)    14351 2024-05-12 06:19:52.000000 obx-3/tests/test_github.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18423 2024-05-12 06:20:00.000000 obx-3/tests/test_hackernews.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      431 2024-05-12 06:20:34.000000 obx-3/tests/test_mixin.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      219 2024-05-12 06:19:37.000000 obx-3/tests/test_none.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4703 2024-05-12 06:20:51.000000 obx-3/tests/test_object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3458 2024-05-12 06:20:22.000000 obx-3/tests/test_opml.py
```

### Comparing `obx-2/PKG-INFO` & `obx-3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obx
-Version: 2
+Version: 3
 Summary: program your own commands
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/obx
 Project-URL: bugs, https://github.com/bthate/obx/issues
 Project-URL: source, https://github.com/bthate/obx
 Classifier: Development Status :: 3 - Alpha
@@ -17,19 +17,27 @@
 NAME
 
 ::
 
     OBX - program your own commands
 
 
+INSTALL
+
+::
+
+    $ pipx install obx
+    $ pipx ensurepath
+
+
 SYNOPSIS
 
 ::
 
-    >>> from obx import Object, dumps, loads
+    >>> from obx.object import Object, dumps, loads
     >>> o = Object()
     >>> o.a = "b"
     >>> txt = dumps(o)
     >>> loads(txt)
     {"a": "b"}
 
 
@@ -49,31 +57,24 @@
     method names. This makes storing and reading to/from json possible.
 
 
 CONTENT
 
 ::
 
-    obx.brokers     object broker
-    obx.excepts     deferred exception handling
-    obx.handler     event handler
-    obx.locates     find objects on disk
-    obx.objects     a clean namespace
-    obx.parsers     arguments parsing
-    obx.persist     object store
-    obx.repeats     repeaters
-    obx.threads	    threads
-    obx.workdir     directory to store objects
-
-
-INSTALL
-
-::
+    obx.broker     object broker
+    obx.client     clients
+    obx.disk       object store
+    obx.find       find objects on disk
+    obx.handler    event handler
+    obx.log        logging
+    obx.object     a clean namespace
+    obx.run        runtime
+    obx.threads	   threads
 
-    $ pip install obx
 
 
 AUTHOR
 
 ::
 
     Bart Thate <bthate@dds.nl>
```

### Comparing `obx-2/README.rst` & `obx-3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 NAME
 
 ::
 
     OBX - program your own commands
 
 
+INSTALL
+
+::
+
+    $ pipx install obx
+    $ pipx ensurepath
+
+
 SYNOPSIS
 
 ::
 
-    >>> from obx import Object, dumps, loads
+    >>> from obx.object import Object, dumps, loads
     >>> o = Object()
     >>> o.a = "b"
     >>> txt = dumps(o)
     >>> loads(txt)
     {"a": "b"}
 
 
@@ -33,31 +41,24 @@
     method names. This makes storing and reading to/from json possible.
 
 
 CONTENT
 
 ::
 
-    obx.brokers     object broker
-    obx.excepts     deferred exception handling
-    obx.handler     event handler
-    obx.locates     find objects on disk
-    obx.objects     a clean namespace
-    obx.parsers     arguments parsing
-    obx.persist     object store
-    obx.repeats     repeaters
-    obx.threads	    threads
-    obx.workdir     directory to store objects
-
-
-INSTALL
-
-::
+    obx.broker     object broker
+    obx.client     clients
+    obx.disk       object store
+    obx.find       find objects on disk
+    obx.handler    event handler
+    obx.log        logging
+    obx.object     a clean namespace
+    obx.run        runtime
+    obx.threads	   threads
 
-    $ pip install obx
 
 
 AUTHOR
 
 ::
 
     Bart Thate <bthate@dds.nl>
```

### Comparing `obx-2/obx/brokers.py` & `obx-3/obx/broker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,E0402
 
 
-"object cache"
+"broker"
 
 
-from .objects import Object, keys, values
+from .object import Object, keys
 
 
-def __dir__():
-    return (
-        'Broker',
-    )
+rpr = object.__repr__
 
 
-__all__ = __dir__()
+class Broker:
 
+    "Broker"
 
-rpr = object.__repr__
+    def __init__(self):
+        self.objs = Object()
 
+    def add(self, obj):
+        "add an object to the broker."
+        setattr(self.objs, rpr(obj), obj)
 
-class Broker(Object):
+    def first(self):
+        "return first object."
+        for key in keys(self.objs):
+            return getattr(self.objs, key)
 
-    objs = Object()
+    def get(self, orig):
+        "return object by origin (repr)"
+        return getattr(self.objs, orig, None)
 
-    @staticmethod
-    def add(obj):
-        setattr(Broker.objs, rpr(obj), obj)
-
-    @staticmethod
-    def all():
-        return values(Broker.objs)
-
-    @staticmethod
-    def first():
-        for key in keys(Broker.objs):
-            return getattr(Broker.objs, key)
-
-    @staticmethod
-    def get(orig):
-        return getattr(Broker.objs, orig, None)
-
-    @staticmethod
-    def remove(obj):
-        delattr(Broker.objs, rpr(obj))
+    def remove(self, obj):
+        "remove object from broker"
+        delattr(self.objs, rpr(obj))
+
+
+def __dir__():
+    return (
+        'Broker',
+    )
```

### Comparing `obx-2/obx/handler.py` & `obx-3/obx/object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,275 +1,273 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402
 
 
-"handler"
+"clean namespace"
 
 
-import inspect
-import queue
-import threading
-import time
+import json
+import pathlib
 import _thread
 
 
-from .objects import Default, Object, spl
-from .persist import Persist
-from .brokers import Broker
-from .excepts import Error
-from .threads import launch
-
-
-class Command(Object):
-
-    cmds = Object()
-
-    @staticmethod
-    def add(func):
-        setattr(Command.cmds, func.__name__, func)
-
-
-class Message(Default):
-
-    def __init__(self):
-        Default.__init__(self)
-        self._ready  = threading.Event()
-        self._thr    = None
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-        self.type    = "event"
-
-    def ready(self):
-        self._ready.set()
-
-    def reply(self, txt):
-        self.result.append(txt)
-
-    def show(self):
-        bot = Broker.get(self.orig)
-        for txt in self.result:
-            bot.say(self.channel, txt)
-
-    def wait(self):
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
-
-
-class Handler(Object):
-
-    def __init__(self):
-        Object.__init__(self)
-        self.cbs      = Object()
-        self.queue    = queue.Queue()
-        self.stopped  = threading.Event()
-        self.threaded = True
-        Broker.add(self)
-
-    def callback(self, evt):
-        func = getattr(self.cbs, evt.type, None)
-        if not func:
-            evt.ready()
-            return
-        if self.threaded:
-            evt._thr = launch(func, evt)
-        else:
-            func(evt)
-            evt.ready()
-
-    def loop(self):
-        while not self.stopped.is_set():
-            try:
-                evt = self.poll()
-                self.callback(evt)
-            except (KeyboardInterrupt, EOFError):
-                _thread.interrupt_main()
-
-    def poll(self):
-        return self.queue.get()
-
-    def put(self, evt):
-        self.queue.put_nowait(evt)
-
-    def register(self, typ, cbs):
-        setattr(self.cbs, typ, cbs)
+lock = _thread.allocate_lock()
 
-    def start(self):
-        launch(self.loop)
 
-    def stop(self):
-        self.stopped.set()
+class Object: # pylint: disable=R0902
 
+    "Object"
 
-class Client(Handler):
+    def __contains__(self, key):
+        return key in dir(self)
 
-    def __init__(self):
-        Handler.__init__(self)
-        self.register("command", command)
+    def __iter__(self):
+        return iter(self.__dict__)
 
-    def announce(self, txt):
-        self.raw(txt)
+    def __len__(self):
+        return len(self.__dict__)
 
-    def say(self, channel, txt):
-        self.raw(txt)
+    def __str__(self):
+        return str(self.__dict__)
 
-    def show(self, evt):
-        for txt in evt.result:
-            self.say(evt.channel, txt)
 
-    def raw(self, txt):
-        pass
+class Default(Object): # pylint: disable=R0902,R0903
 
+    "Default"
 
-"utility"
+    def __getattr__(self, key):
+        return self.__dict__.get(key, "")
 
 
-def cmnd(txt, out):
-    clt = Client()
-    clt.raw = out
-    evn = Message()
-    evn.orig = object.__repr__(clt)
-    evn.txt = txt
-    command(evn)
-    evn.wait()
-    return evn
+def construct(obj, *args, **kwargs):
+    "construct an object from provided arguments."
+    if args:
+        val = args[0]
+        if isinstance(val, zip):
+            update(obj, dict(val))
+        elif isinstance(val, dict):
+            update(obj, val)
+        elif isinstance(val, Object):
+            update(obj, vars(val))
+    if kwargs:
+        update(obj, kwargs)
 
 
-def command(evt):
-    parse_cmd(evt)
-    func = getattr(Command.cmds, evt.cmd, None)
-    if func:
+def edit(obj, setter, skip=False):
+    "edit an object from provided dict/dict-like."
+    for key, val in items(setter):
+        if skip and val == "":
+            continue
         try:
-            func(evt)
-            evt.show()
-        except Exception as exc:
-            Error.add(exc)
-    evt.ready()
-
-
-def forever():
-    while 1:
+            setattr(obj, key, int(val))
+            continue
+        except ValueError:
+            pass
         try:
-            time.sleep(1.0)
-        except (KeyboardInterrupt, EOFError):
-            _thread.interrupt_main()
+            setattr(obj, key, float(val))
+            continue
+        except ValueError:
+            pass
+        if val in ["True", "true"]:
+            setattr(obj, key, True)
+        elif val in ["False", "false"]:
+            setattr(obj, key, False)
+        else:
+            setattr(obj, key, val)
 
 
-def laps(seconds, short=True):
+def fmt(obj, args=None, skip=None, plain=False):
+    "format an object to a printable string."
+    if args is None:
+        args = keys(obj)
+    if skip is None:
+        skip = []
     txt = ""
-    nsec = float(seconds)
-    if nsec < 1:
-        return f"{nsec:.2f}s"
-    yea = 365*24*60*60
-    week = 7*24*60*60
-    nday = 24*60*60
-    hour = 60*60
-    minute = 60
-    yeas = int(nsec/yea)
-    nsec -= yeas*yea
-    weeks = int(nsec/week)
-    nsec -= weeks*week
-    nrdays = int(nsec/nday)
-    nsec -= nrdays*nday
-    hours = int(nsec/hour)
-    nsec -= hours*hour
-    minutes = int(nsec/minute)
-    nsec -= int(minute*minutes)
-    sec = int(nsec)
-    if yeas:
-        txt += f"{yeas}y"
-    if weeks:
-        nrdays += weeks * 7
-    if nrdays:
-        txt += f"{nrdays}d"
-    if short and txt:
-        return txt.strip()
-    if hours:
-        txt += f"{hours}h"
-    if minutes:
-        txt += f"{minutes}m"
-    if sec:
-        txt += f"{sec}s"
-    txt = txt.strip()
-    return txt
-
-
-def parse_cmd(obj, txt=None):
-    args = []
-    obj.args    = obj.args or []
-    obj.cmd     = obj.cmd or ""
-    obj.gets    = obj.gets or Default()
-    obj.hasmods = obj.hasmod or False
-    obj.index   = None
-    obj.mod     = obj.mod or ""
-    obj.opts    = obj.opts or ""
-    obj.result  = obj.reult or []
-    obj.sets    = obj.sets or Default()
-    obj.txt     = txt or obj.txt or ""
-    obj.otxt    = obj.txt
-    _nr = -1
-    for spli in obj.otxt.split():
-        if spli.startswith("-"):
-            try:
-                obj.index = int(spli[1:])
-            except ValueError:
-                obj.opts += spli[1:]
-            continue
-        if "==" in spli:
-            key, value = spli.split("==", maxsplit=1)
-            if key in obj.gets:
-                val = getattr(obj.gets, key)
-                value = val + "," + value
-            setattr(obj.gets, key, value)
+    for key in args:
+        if key.startswith("__"):
             continue
-        if "=" in spli:
-            key, value = spli.split("=", maxsplit=1)
-            if key == "mod":
-                obj.hasmods = True
-                if obj.mod:
-                    obj.mod += f",{value}"
-                else:
-                    obj.mod = value
-                continue
-            setattr(obj.sets, key, value)
+        if key in skip:
             continue
-        _nr += 1
-        if _nr == 0:
-            obj.cmd = spli
+        value = getattr(obj, key, None)
+        if value is None:
             continue
-        args.append(spli)
-    if args:
-        obj.args = args
-        obj.txt  = obj.cmd or ""
-        obj.rest = " ".join(obj.args)
-        obj.txt  = obj.cmd + " " + obj.rest
-    else:
-        obj.txt = obj.cmd or ""
+        if plain:
+            txt += f"{value} "
+        elif isinstance(value, str) and len(value.split()) >= 2:
+            txt += f'{key}="{value}" '
+        else:
+            txt += f"{key}={value} "
+    return txt.strip()
 
 
+def fqn(obj):
+    "return full qualified name of an object."
+    kin = str(type(obj)).split()[-1][1:-2]
+    if kin == "type":
+        kin = obj.__name__
+    return kin
+
+
+def items(obj):
+    "return the items of an object."
+    if isinstance(obj, type({})):
+        return obj.items()
+    return obj.__dict__.items()
+
+
+def keys(obj):
+    "return keys of an object."
+    if isinstance(obj, type({})):
+        return obj.keys()
+    return list(obj.__dict__.keys())
+
+
+def read(obj, pth):
+    "read an object from file path."
+    with lock:
+        with open(pth, 'r', encoding='utf-8') as ofile:
+            update(obj, load(ofile))
+
+
+def search(obj, selector):
+    "check if object matches provided values."
+    res = False
+    if not selector:
+        return True
+    for key, value in items(selector):
+        val = getattr(obj, key, None)
+        if str(value).lower() in str(val).lower():
+            res = True
+        else:
+            res = False
+            break
+    return res
 
-def scan(pkg, modstr, initer=False, disable="", wait=True):
-    mds = []
-    for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
+
+def update(obj, data, empty=True):
+    "update an object."
+    for key, value in items(data):
+        if empty and not value:
             continue
-        for _key, cmd in inspect.getmembers(module, inspect.isfunction):
-            if 'event' in cmd.__code__.co_varnames:
-                Command.add(cmd)
-        for _key, clz in inspect.getmembers(module, inspect.isclass):
-            if not issubclass(clz, Object):
-                continue
-            Persist.add(clz)
-        if initer and "init" in dir(module):
-            module._thr = launch(module.init, name=f"init {modname}")
-            mds.append(module)
-    if wait and initer:
-        for mod in mds:
-            mod._thr.join()
-    return mds
+        setattr(obj, key, value)
+
+
+def values(obj):
+    "return values of an object."
+    return obj.__dict__.values()
+
+
+def write(obj, pth):
+    "write an object to disk."
+    with lock:
+        path = pathlib.Path(pth)
+        path.parent.mkdir(parents=True, exist_ok=True)
+        with open(pth, 'w', encoding='utf-8') as ofile:
+            dump(obj, ofile, indent=4)
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    "ObjectDecoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONDecoder.__init__(self, *args, **kwargs)
+
+    def decode(self, s, _w=None):
+        "decoding string to object."
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        "decode partial string to object."
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None):
+    "construct object from dict."
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw):
+    "load object from file."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw):
+    "load object from string."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    "ObjectEncoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONEncoder.__init__(self, *args, **kwargs)
+
+    def default(self, o):
+        "return stringable value."
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return o.__dict__
+
+    def encode(self, o) -> str:
+        "encode object to string."
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(self, o, _one_shot=False):
+        "loop over object to encode to string."
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw):
+    "dump object to file."
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
+def dumps(*args, **kw):
+    "dump object to string."
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
+
+
+def __dir__():
+    return (
+        'Object',
+        'Default',
+        'construct',
+        'dump',
+        'dumps',
+        'edit',
+        'fmt',
+        'fqn',
+        'hook',
+        'items',
+        'keys',
+        'load',
+        'loads',
+        'read',
+        'search',
+        'update',
+        'values',
+        'write'
+    )
```

### Comparing `obx-2/obx/locates.py` & `obx-3/obx/find.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-# This file is placed in the Public Domain
-#
-# pylint: disable=C,R,W0105
+# This file is placed in the Public Domain.
 
 
-"find objects"
+"find"
 
 
 import os
 import time
 
 
-from .objects import Default, fqn, search, update
-from .persist import fetch, long, strip
-from .workdir import store
+from .disk import fetch, long, store, strip
+from .object import Default, fqn, search, update
 
 
-def __dir__():
-    return (
-        'find',
-        'fns',
-        'last'
-    )
+def fns(mtc=""):
+    "show list of files."
+    dname = ''
+    pth = store(mtc)
+    for rootdir, dirs, _files in os.walk(pth, topdown=False):
+        if dirs:
+            for dname in sorted(dirs):
+                if dname.count('-') == 2:
+                    ddd = os.path.join(rootdir, dname)
+                    fls = sorted(os.listdir(ddd))
+                    for fll in fls:
+                        yield strip(os.path.join(ddd, fll))
 
 
-__all__ = __dir__()
+def fntime(daystr):
+    "convert file name to it's saved time."
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    timed = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        timed += float('.' + rest)
+    return timed
 
 
 def find(mtc, selector=None, index=None, deleted=False):
+    "find object matching the selector dict."
     clz = long(mtc)
-    nr = -1
+    nrs = -1
     for fnm in sorted(fns(clz), key=fntime):
         obj = Default()
         fetch(obj, fnm)
         if not deleted and '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
-        nr += 1 
-        if index is not None and nr != int(index):
+        nrs += 1
+        if index is not None and nrs != int(index):
             continue
         yield (fnm, obj)
 
 
-def fns(mtc=""):
-    dname = ''
-    pth = store(mtc)
-    for rootdir, dirs, _files in os.walk(pth, topdown=False):
-        if dirs:
-            for dname in sorted(dirs):
-                if dname.count('-') == 2:
-                    ddd = os.path.join(rootdir, dname)
-                    fls = sorted(os.listdir(ddd))
-                    for fll in fls:
-                        yield strip(os.path.join(ddd, fll))
-
-
 def last(obj, selector=None):
+    "return last object saved."
     if selector is None:
         selector = {}
     result = sorted(
                     find(fqn(obj), selector),
                     key=lambda x: fntime(x[0])
                    )
+    res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
-        return inp[0]
-
+        res = inp[0]
+    return res
 
-"utility"
 
-
-def fntime(daystr):
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    timed = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        timed += float('.' + rest)
-    return timed
+def __dir__():
+    return (
+        'fns',
+        'fntime',
+        'find',
+        'last'
+    )
```

### Comparing `obx-2/obx/parsers.py` & `obx-3/obx/modules/tmr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0718,W0702,E0402
 
 
-"parsing text"
+"timer"
 
 
 import datetime
-import os
 import re
 import time as ttime
 
 
-from .objects import Default
+from ..client    import laps
+from ..handler   import Event
+from ..find      import find
+from ..object    import update
+from ..run       import broker
+from ..thread    import Timer, launch
+from ..disk      import sync
 
 
-def __dir__():
-    return (
-        'NoDate',
-        'fntime',
-        'laps',
-        'parse_cmd',
-        'parse_time',
-        'spl'
-    )
-
-
-__all__ = __dir__()
+def init():
+    "start timers."
+    for _fn, obj in find("timer"):
+        if "time" not in obj:
+            continue
+        diff = float(obj.time) - ttime.time()
+        if diff > 0:
+            bot = broker.first()
+            evt = Event()
+            update(evt, obj)
+            evt.orig = object.__repr__(bot)
+            timer = Timer(diff, evt.show)
+            launch(timer.start)
 
 
 MONTHS = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
@@ -52,59 +56,57 @@
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    pass
+    "NoDate"
 
 
 def extract_date(daystr):
+    "extract date from string."
+    res = None
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
+            break
         except ValueError:
             res = None
-        if res:
-            return res
-
-
-def fntime(daystr):
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    timed = ttime.mktime(ttime.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        timed += float('.' + rest)
-    return timed
+    return res
 
 
 def get_day(daystr):
+    "return day from string."
+    day = None
+    month = None
+    yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
-        (day, month, yea) = ymdre.groups()
+        if ymdre:
+            (day, month, yea) = ymdre.groups()
     except ValueError:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
-            (day, month) = ymre.groups()
-            yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex:
+            if ymre:
+                (day, month) = ymre.groups()
+                yea = ttime.strftime("%Y", ttime.localtime())
+        except Exception as ex: # pylint: disable=W0212
             raise NoDate(daystr) from ex
-    day = int(day)
-    month = int(month)
-    yea = int(yea)
-    date = "%s %s %s" % (day, MONTHS[month], yea)
-    return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
+    if day:
+        day = int(day)
+        month = int(month)
+        yea = int(yea)
+        date = f"{day} {MONTHS[month]} {yea}"
+        return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
+    raise NoDate(daystr)
 
 
 def get_hour(daystr):
+    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -118,117 +120,27 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
+    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
-def laps(seconds, short=True):
-    txt = ""
-    nsec = float(seconds)
-    if nsec < 1:
-        return f"{nsec:.2f}s"
-    yea = 365*24*60*60
-    week = 7*24*60*60
-    nday = 24*60*60
-    hour = 60*60
-    minute = 60
-    yeas = int(nsec/yea)
-    nsec -= yeas*yea
-    weeks = int(nsec/week)
-    nsec -= weeks*week
-    nrdays = int(nsec/nday)
-    nsec -= nrdays*nday
-    hours = int(nsec/hour)
-    nsec -= hours*hour
-    minutes = int(nsec/minute)
-    nsec -= int(minute*minutes)
-    sec = int(nsec)
-    if yeas:
-        txt += f"{yeas}y"
-    if weeks:
-        nrdays += weeks * 7
-    if nrdays:
-        txt += f"{nrdays}d"
-    if short and txt:
-        return txt.strip()
-    if hours:
-        txt += f"{hours}h"
-    if minutes:
-        txt += f"{minutes}m"
-    if sec:
-        txt += f"{sec}s"
-    txt = txt.strip()
-    return txt
-
-
-def parse_cmd(obj, txt=None):
-    args = []
-    obj.args    = obj.args or []
-    obj.cmd     = obj.cmd or ""
-    obj.gets    = obj.gets or Default()
-    obj.hasmods = obj.hasmod or False
-    obj.index   = None
-    obj.mod     = obj.mod or ""
-    obj.opts    = obj.opts or ""
-    obj.result  = obj.reult or []
-    obj.sets    = obj.sets or Default()
-    obj.txt     = txt or obj.txt or ""
-    obj.otxt    = obj.txt
-    _nr = -1
-    for spli in obj.otxt.split():
-        if spli.startswith("-"):
-            try:
-                obj.index = int(spli[1:])
-            except ValueError:
-                obj.opts += spli[1:]
-            continue
-        if "==" in spli:
-            key, value = spli.split("==", maxsplit=1)
-            if key in obj.gets:
-                val = getattr(obj.gets, key)
-                value = val + "," + value
-            setattr(obj.gets, key, value)
-            continue
-        if "=" in spli:
-            key, value = spli.split("=", maxsplit=1)
-            if key == "mod":
-                obj.hasmods = True
-                if obj.mod:
-                    obj.mod += f",{value}"
-                else:
-                    obj.mod = value
-                continue
-            setattr(obj.sets, key, value)
-            continue
-        _nr += 1
-        if _nr == 0:
-            obj.cmd = spli
-            continue
-        args.append(spli)
-    if args:
-        obj.args = args
-        obj.txt  = obj.cmd or ""
-        obj.rest = " ".join(obj.args)
-        obj.txt  = obj.cmd + " " + obj.rest
-    else:
-        obj.txt = obj.cmd or ""
-
-
 def parse_time(txt):
+    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -242,33 +154,75 @@
             target = to_day(today())
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
-def spl(txt):
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
-
-
 def to_day(daystr):
+    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
+    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
+            break
         except ValueError:
             res = None
-        if res:
-            return res
         line = ""
+    return res
 
 
 def today():
+    "return date."
     return str(datetime.datetime.today()).split()[0]
+
+
+def tmr(event):
+    "add a timer."
+    result = ""
+    if not event.rest:
+        nmr = 0
+        for _fn, obj in find('timer'):
+            lap = float(obj.time) - ttime.time()
+            if lap > 0:
+                event.reply(f'{nmr} {obj.txt} {laps(lap)}')
+                nmr += 1
+        return result
+    seconds = 0
+    line = ""
+    for word in event.args:
+        if word.startswith("+"):
+            try:
+                seconds = int(word[1:])
+            except (ValueError, IndexError):
+                event.reply(f"{seconds} is not an integer")
+                return result
+        else:
+            line += word + " "
+    if seconds:
+        target = ttime.time() + seconds
+    else:
+        try:
+            target = get_day(event.rest)
+        except NoDate:
+            target = to_day(today())
+        hour =  get_hour(event.rest)
+        if hour:
+            target += hour
+    if not target or ttime.time() > target:
+        event.reply("already passed given time.")
+        return result
+    event.time = target
+    diff = target - ttime.time()
+    event.reply("ok " +  laps(diff))
+    event.result = []
+    event.result.append(event.rest)
+    timer = Timer(diff, event.show, thrname=event.cmd)
+    update(timer, event)
+    sync(timer)
+    launch(timer.start)
+    return result
```

### Comparing `obx-2/obx/persist.py` & `obx-3/obx/disk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,122 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"eternity"
+"disk"
 
 
 import datetime
+import inspect
 import os
 import pathlib
-import _thread
 
 
-from .objects import Object, dump, fqn, load, update
-from .workdir import store, types
+from .object import Object, fqn, read, write
 
 
-def __dir__():
-    return (
-        'Persist',
-        'ident',
-        'fetch',
-        'read',
-        'sync',
-        'write'
-    )
-
-
-__all__ = __dir__()
+class Workdir(Object): # pylint: disable=R0903
 
+    "Workdir"
 
-lock = _thread.allocate_lock()
+    workdir = ""
 
 
-class Persist(Object):
-
-    classes = Object()
-
-    @staticmethod
-    def add(clz):
-        if not clz:
-            return
-        name = str(clz).split()[1][1:-2]
-        setattr(Persist.classes, name, clz)
-
-
-def long(name):
-    split = name.split(".")[-1].lower()
-    res = name
-    for named in Persist.classes:
-        if split in named.split(".")[-1].lower():
-            res = named
-            break
-    if "." not in res:
-        for fnm in types():
-            claz = fnm.split(".")[-1]
-            if fnm == claz.lower():
-                res = fnm
-    return res
+def fetch(obj, pth):
+    "read object from disk."
+    pth2 = store(pth)
+    read(obj, pth2)
+    return strip(pth)
 
 
 def ident(obj):
+    "return an id for an object."
     return os.path.join(
                         fqn(obj),
                         os.path.join(*str(datetime.datetime.now()).split())
                        )
 
 
-def fetch(obj, pth):
-    pth2 = store(pth)
-    read(obj, pth2)
-    return strip(pth)
+def lsstore():
+    "return types stored."
+    return os.listdir(store())
+
+
+def skel():
+    "create directory,"
+    pth  = os.path.join(Workdir.workdir, "store", "")
+    path = pathlib.Path(pth)
+    path.mkdir(parents=True, exist_ok=True)
+
 
+def store(pth=""):
+    "return objects directory."
+    return os.path.join(Workdir.workdir, "store", pth)
 
-def read(obj, pth):
-    with lock:
-        with open(pth, 'r', encoding='utf-8') as ofile:
-            update(obj, load(ofile))
+
+def strip(pth, nmr=3):
+    "reduce to path with directory."
+    return os.sep.join(pth.split(os.sep)[-nmr:])
 
 
 def sync(obj, pth=None):
+    "sync object to disk."
     if pth is None:
         pth = ident(obj)
     pth2 = store(pth)
     write(obj, pth2)
     return pth
 
 
-def write(obj, pth):
-    with lock:
-        cdir(os.path.dirname(pth))
-        with open(pth, 'w', encoding='utf-8') as ofile:
-            dump(obj, ofile, indent=4)
+class Whitelist(Object): # pylint: disable=R0903
+
+    "Whitelist"
 
+    classes = Object()
 
-"utilities"
 
+def scancls(mod) -> None:
+    "scan module for classes."
+    for key, clz in inspect.getmembers(mod, inspect.isclass):
+        if key.startswith("cb"):
+            continue
+        if not issubclass(clz, Object):
+            continue
+        whitelist(clz)
 
-def cdir(pth) -> None:
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
 
+def whitelist(clz):
+    "add class to whitelist."
+    name = str(clz).split()[1][1:-2]
+    setattr(Whitelist.classes, name, clz)
 
-def strip(pth, nmr=3):
-    return os.sep.join(pth.split(os.sep)[-nmr:])
+
+def long(name):
+    "match from single name to long name."
+    split = name.split(".")[-1].lower()
+    res = name
+    for named in Whitelist.classes:
+        if split in named.split(".")[-1].lower():
+            res = named
+            break
+    if "." not in res:
+        for fnm in lsstore():
+            claz = fnm.split(".")[-1]
+            if fnm == claz.lower():
+                res = fnm
+    return res
+
+
+def __dir__():
+    return (
+        'Whitelist',
+        'Workdir',
+        'fetch',
+        'ident',
+        'lsstore',
+        'long',
+        'scancls',
+        'skel',
+        'store',
+        'strip',
+        'sync',
+        'whitelist'
+    )
```

### Comparing `obx-2/obx.egg-info/PKG-INFO` & `obx-3/obx.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obx
-Version: 2
+Version: 3
 Summary: program your own commands
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/obx
 Project-URL: bugs, https://github.com/bthate/obx/issues
 Project-URL: source, https://github.com/bthate/obx
 Classifier: Development Status :: 3 - Alpha
@@ -17,19 +17,27 @@
 NAME
 
 ::
 
     OBX - program your own commands
 
 
+INSTALL
+
+::
+
+    $ pipx install obx
+    $ pipx ensurepath
+
+
 SYNOPSIS
 
 ::
 
-    >>> from obx import Object, dumps, loads
+    >>> from obx.object import Object, dumps, loads
     >>> o = Object()
     >>> o.a = "b"
     >>> txt = dumps(o)
     >>> loads(txt)
     {"a": "b"}
 
 
@@ -49,31 +57,24 @@
     method names. This makes storing and reading to/from json possible.
 
 
 CONTENT
 
 ::
 
-    obx.brokers     object broker
-    obx.excepts     deferred exception handling
-    obx.handler     event handler
-    obx.locates     find objects on disk
-    obx.objects     a clean namespace
-    obx.parsers     arguments parsing
-    obx.persist     object store
-    obx.repeats     repeaters
-    obx.threads	    threads
-    obx.workdir     directory to store objects
-
-
-INSTALL
-
-::
+    obx.broker     object broker
+    obx.client     clients
+    obx.disk       object store
+    obx.find       find objects on disk
+    obx.handler    event handler
+    obx.log        logging
+    obx.object     a clean namespace
+    obx.run        runtime
+    obx.threads	   threads
 
-    $ pip install obx
 
 
 AUTHOR
 
 ::
 
     Bart Thate <bthate@dds.nl>
```

