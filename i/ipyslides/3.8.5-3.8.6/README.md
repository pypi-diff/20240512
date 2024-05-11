# Comparing `tmp/ipyslides-3.8.5.tar.gz` & `tmp/ipyslides-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.5.tar", last modified: Fri May 10 21:10:10 2024, max compression
+gzip compressed data, was "ipyslides-3.8.6.tar", last modified: Sat May 11 22:37:54 2024, max compression
```

## Comparing `ipyslides-3.8.5.tar` & `ipyslides-3.8.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 21:10:10.567577 ipyslides-3.8.5/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.5/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-10 21:10:10.565338 ipyslides-3.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 21:10:10.501006 ipyslides-3.8.5/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.5/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-10 21:08:52.000000 ipyslides-3.8.5/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 21:10:10.559369 ipyslides-3.8.5/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.5/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    39305 2024-05-10 10:28:28.000000 ipyslides-3.8.5/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6084 2024-05-10 20:38:34.000000 ipyslides-3.8.5/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.5/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.5/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.5/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.5/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.5/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-10 21:10:10.559369 ipyslides-3.8.5/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12864 2024-05-10 21:07:59.000000 ipyslides-3.8.5/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.5/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.5/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.5/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.5/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    21451 2024-05-10 05:55:37.000000 ipyslides-3.8.5/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28852 2024-05-08 00:37:24.000000 ipyslides-3.8.5/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28513 2024-05-08 18:39:39.000000 ipyslides-3.8.5/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15376 2024-05-10 05:56:13.000000 ipyslides-3.8.5/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.5/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47812 2024-05-10 09:58:54.000000 ipyslides-3.8.5/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.5/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.5/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.5/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.5/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.5/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-10 21:10:10.538520 ipyslides-3.8.5/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-10 21:10:09.000000 ipyslides-3.8.5/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-10 21:10:10.000000 ipyslides-3.8.5/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 21:10:09.000000 ipyslides-3.8.5/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-10 21:10:09.000000 ipyslides-3.8.5/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-10 21:10:09.000000 ipyslides-3.8.5/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 21:10:10.567858 ipyslides-3.8.5/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:37:54.700564 ipyslides-3.8.6/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.6/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-11 22:37:54.696465 ipyslides-3.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 22:37:54.560397 ipyslides-3.8.6/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.6/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-11 22:07:45.000000 ipyslides-3.8.6/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:37:54.689468 ipyslides-3.8.6/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.6/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    39305 2024-05-10 10:28:28.000000 ipyslides-3.8.6/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6084 2024-05-10 20:38:34.000000 ipyslides-3.8.6/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.6/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.8.6/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.8.6/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.8.6/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12158 2024-05-10 07:35:58.000000 ipyslides-3.8.6/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:37:54.693463 ipyslides-3.8.6/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12864 2024-05-10 21:19:34.000000 ipyslides-3.8.6/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.6/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.6/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.6/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.6/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23187 2024-05-11 22:30:33.000000 ipyslides-3.8.6/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.8.6/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-11 20:38:11.000000 ipyslides-3.8.6/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15376 2024-05-10 05:56:13.000000 ipyslides-3.8.6/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.6/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47973 2024-05-11 22:07:13.000000 ipyslides-3.8.6/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.8.6/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.6/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29250 2024-05-11 20:44:28.000000 ipyslides-3.8.6/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.6/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.6/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:37:54.625909 ipyslides-3.8.6/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-11 22:37:53.000000 ipyslides-3.8.6/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-11 22:37:54.000000 ipyslides-3.8.6/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 22:37:53.000000 ipyslides-3.8.6/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-11 22:37:53.000000 ipyslides-3.8.6/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 22:37:53.000000 ipyslides-3.8.6/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 22:37:54.700564 ipyslides-3.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.6/setup.py
```

### Comparing `ipyslides-3.8.5/LICENSE` & `ipyslides-3.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/PKG-INFO` & `ipyslides-3.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.5
+Version: 3.8.6
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.5/README.md` & `ipyslides-3.8.6/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.6/ipyslides/_base/_layout_css.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/_widgets.py` & `ipyslides-3.8.6/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/base.py` & `ipyslides-3.8.6/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/export_html.py` & `ipyslides-3.8.6/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/export_template.py` & `ipyslides-3.8.6/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/icons.py` & `ipyslides-3.8.6/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/intro.py` & `ipyslides-3.8.6/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.6/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/js/notes.js` & `ipyslides-3.8.6/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/navigation.py` & `ipyslides-3.8.6/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/notes.py` & `ipyslides-3.8.6/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/screenshot.py` & `ipyslides-3.8.6/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_base/settings.py` & `ipyslides-3.8.6/ipyslides/_base/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Author Notes: Classes in this module should only be instantiated in Slides class or it's parent class
 and then provided to other classes via composition, not inheritance.
 """
 
-import os
-import math
+import os, math
 
 from IPython.display import Image
 
 from ..formatters import fix_ipy_image, code_css
 from ..xmd import parse
 from ..utils import html, today, format_html, _sub_doc, _css_docstring
 from . import intro, styles, _layout_css
@@ -126,42 +125,49 @@
     def set_animation(self, main="slide_h", frame="appear"):
         "Set animation for slides and frames."
         if len(self._slides[:]) >= 1:
             self._slides[0]._set_overall_animation(main=main, frame=frame)
         else:
             raise RuntimeError("No slides yet to set animation.")
         return self # for chaining set_methods
+    
+    def set_theme(self, name:str):
+        "Set prefered theme."
+        themes = self.theme_dd.options
+        if name not in themes:
+            raise ValueError(f"name expect on the followings: {themes!r}")
+        self.theme_dd.value = name 
+        return self # for chaining set_methods
 
     @_sub_doc(colors=styles.theme_colors["Light"])
-    def set_theme_colors(self, colors={}):
+    def set_theme_colors(self, colors : dict):
         """Set theme colors. Only take effect when using custom theme.
         colors must be a dictionary with exactly like this:
         ```python
-        Slides.settings.set_theme_colors({colors})
+        {colors}
         ```
         """
         styles._validate_colors(colors)  # Validate colors before using and setting
         self._custom_colors = colors
         self.theme_dd.value = "Custom"  # Trigger theme update
         self._update_theme({'owner':self.theme_dd}) # This chnage is important to update layout theme as well
         return self # for chaining set_methods
 
     @_sub_doc(css_docstring=_css_docstring)
-    def set_css(self, css_dict={}):
+    def set_css(self, props: dict):
         """Set CSS for all slides. This loads on slides navigation, so you can include keyframes animations as well.
         Individual slide's CSS set by `slides[index].set_css` will override this.
         {css_docstring}
         """
         if len(self._slides[:]) >= 1:
-            self._slides[0]._set_overall_css(css_dict=css_dict)
+            self._slides[0]._set_overall_css(props)
         else:
             raise RuntimeError("No slides yet to set CSS.")
         return self # for chaining set_methods
 
-
     def set_bg_image(self, src=None, opacity=0.25, blur_radius=None):
         "Adds glassmorphic effect to the background with image. `src` can be a url or a local image path."
         if not src:
             self.widgets.htmls.glass.value = ""  # clear
             self._bg_image = ""
             return
 
@@ -251,20 +257,20 @@
             self._footer_kws["text"] = ""  # assign to text
         elif text and isinstance(text, str):
             self._footer_kws["text"] = text  # assign to text
         else:
             raise TypeError(f"text should be string or None, not {type(text)}")
 
         if self._slides.current:
-            self.get_footer(
+            self._get_footer(
                 self._slides.current, update_widget=True
             )  # Update footer immediately if slide there
         return self # for chaining set_methods
 
-    def get_footer(self, slide, update_widget=False):
+    def _get_footer(self, slide, update_widget=False):
         "Get footer text. `slide` is a slide object."
         if (type(slide).__name__ != "Slide") and (
             type(slide).__module__.split(".")[0] != "ipyslides"
         ):
             raise TypeError(f"slide should be Slide object, not {type(slide)}")
 
         number = slide.label if slide.label != "0" else ""
@@ -481,8 +487,36 @@
             self.widgets.quick_menu.layout.border = "1px solid var(--hover-bg)"
         else:
             self.btn_menu.icon = 'plus'
             self.widgets.quick_menu.layout.height = '0'
             self.widgets.quick_menu.layout.border = "none"
 
             if hasattr(self, '_hover_only') and self._hover_only:
-                self.btn_menu.add_class('Hover-Only')
+                self.btn_menu.add_class('Hover-Only')
+
+    def apply(self, **settings):
+        """Apply multiple settings at once. Top level keys should be function names without 'set_' and 
+        values should be dictionary of parameters to that function. For example:
+        ```python
+        Slides.settings.apply(
+            layout = {"aspect":1.6, "scroll":False},
+            footer = {0:"footer text", "numbering":True} # 0 key goes to first positional argument
+        )
+        ```
+        """
+        for key, kwargs in settings.items():
+            func = getattr(self, f"set_{key}", None)
+            if func is None:
+                attrs = [a[4:] for a in dir(self) if a.startswith("set_")]
+                raise AttributeError(f"Attribute {key!r} does not exists in settings!\nAllowed attributes are {attrs}.")
+            else:
+                if not isinstance(kwargs, dict):
+                    raise TypeError(f"value of {key!r} should be a dictionary of paraemetrs!")
+                
+                for kw in kwargs:
+                    if not isinstance(kw, (int, str)):
+                        raise TypeError(f"key in value of {key!r} should be int (for args) or str (for kwargs), got {type(kw)}")
+                
+                args = sorted([v for k,v in kwargs.items() if isinstance(k, int)]) # positional args should be in order
+                kwargs = {k:v for k,v in kwargs.items() if isinstance(k, str)} 
+                func(*args, **kwargs) # apply function
+
```

### Comparing `ipyslides-3.8.5/ipyslides/_base/slide.py` & `ipyslides-3.8.6/ipyslides/_base/slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         out = Output().add_class('SlideArea')
         with out:
             display(*self.contents)
         return display(out)
     
     def get_footer(self, update_widget = False): # Used here and export_html
         "Return footer of this slide. Optionally update footer widget."
-        return self._app.settings.get_footer(self, update_widget = update_widget)
+        return self._app.settings._get_footer(self, update_widget = update_widget)
         
     @property
     def frames(self):
         return tuple(self._frames)
     
     @property
     def proxies(self):
@@ -503,27 +503,27 @@
     def get_source(self, name = None):
         "Return source code of this slide, markdwon or python or None if no source exists."
         if self._source['text']:
             return self._app.code.from_string(**self._source, name = name)
         else:
             return self._app.code.cast('Source of a slide only exits if it is NOT created (most recently) using @Slides.frames decorator\n',language = 'markdown')
     
-    def _set_overall_css(self, css_dict={}):
+    def _set_overall_css(self, props: dict):
         self.__class__._overall_css = html('style','') # Reset overall CSS
         old_slide_css = self._css # Save old slide CSS without overall CSS
-        self.set_css(css_dict = css_dict) # Set this slide's CSS
+        self.set_css(props) # Set this slide's CSS
         self.__class__._overall_css = self.css # Set overall CSS from this slide's CSS, self.css takes both
         self._css = old_slide_css # Restore old slide CSS
     
     @_sub_doc(css_docstring = _css_docstring)
-    def set_css(self,css_dict = {}):
+    def set_css(self,props : dict):
         """Attributes at the root level of the dictionary will be applied to the slide. You can add CSS classes by `Slide.set_dom_classes`.
         use `ipyslides.Slides.settings.set_css` to set CSS for all slides at once.
         {css_docstring}"""
-        self._css = _format_css(css_dict, allow_root_attrs = True)
+        self._css = _format_css(props, allow_root_attrs = True)
         
         # See effect of changes
         if not self._app.running: # Otherwise it has side effects
             if self._app._slidelabel != self.label:
                 self._app._slidelabel = self.label # Go there to see effects
             else:
                 self._app._update_tmp_output(self.animation, self._css)
```

### Comparing `ipyslides-3.8.5/ipyslides/_base/styles.py` & `ipyslides-3.8.6/ipyslides/_base/styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     '@keyframes flowPrev':{
         'from' : {'transform': 'translateX(-50%)', 'opacity': 0},
         'to' : {'transform': 'translateX(0)', 'opacity': 1}
     },
 }) 
 }
   
-# This was 436 lines of code in CSS, css_dict is elegant + only 368 lines, clean CSS output is 462 lines
 def _validate_colors(colors):
     for key, value in colors.items():
         if not isinstance(value, str):
             raise TypeError(f'Color value for {key!r} must be a string')
         if not key in theme_colors['Light']:
             raise KeyError(f'Invalid color key {key!r}! Use one of {list(theme_colors["Light"].keys())}')
```

### Comparing `ipyslides-3.8.5/ipyslides/_base/widgets.py` & `ipyslides-3.8.6/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/_demo.py` & `ipyslides-3.8.6/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/core.py` & `ipyslides-3.8.6/ipyslides/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1055,14 +1055,15 @@
     _version = (
         _private_instance.version
     )  # This is for initial use, and will be overwritten by property version
     __doc__ = textwrap.dedent(
         """
     Interactive Slides in IPython Notebook. Only one instance can exist.
     `auto_focus` can be reset from settings and enable jumping back to slides after a cell is executed. 
+    `settings` are passed to `Slides.settings.apply` if you like to set during initialization.
     
     To suppress unwanted print from other libraries/functions, use:
     ```python
     with slides.suppress_stdout():
         some_function_that_prints() # This will not be printed
         print('This will not be printed either')
         display('Something') # This will be printed
@@ -1086,16 +1087,18 @@
         "Access current instnace without changing the settings."
         return _private_instance
 
     def __new__(
         cls,
         extensions=[],
         auto_focus = True,
+        **settings
         ):
         "Returns Same instance each time after applying given settings. Encapsulation."
         instance = cls.instance()
         instance.__doc__ = cls.__doc__  # copy docstring
         instance.extender.extend(extensions) # globally once
+        instance.settings.apply(**settings)
         instance.widgets.checks.focus.value = auto_focus # useful
         return instance
 
     # No need to define __init__, __new__ is enough to show signature and docs
```

### Comparing `ipyslides-3.8.5/ipyslides/formatters.py` & `ipyslides-3.8.6/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/source.py` & `ipyslides-3.8.6/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/utils.py` & `ipyslides-3.8.6/ipyslides/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 def _sub_doc(**kwargs):
     "Substitute docstring with given kwargs."
     def _inner(func):
         func.__doc__ = func.__doc__.format(**kwargs)
         return func
     return _inner
 
-_css_docstring = """`css_dict` is a nested dict of css selectors and properties. There are few special rules in `css_dict`:
+_css_docstring = """`props` is a nested dict of css selectors and properties. There are few special rules in `props`:
 
 - All nested selectors are joined with space, so '.A': {'.B': ... } becomes '.A .B {...}' in CSS.
 - A '^' in start of a selector joins to parent selector without space, so '.A': {'^:hover': ...} becomes '.A:hover {...}' in CSS. You can also use '.A:hover' directly but it will restrict other nested keys to hover only.
 - A '<' in start of a nested selector makes it root selector, so '.A': {'<.B': ...} becomes '.A {}\n.B {...}' in CSS.
 - A list/tuple of values for a key in dict generates CSS fallback, so '.A': {'font-size': ('20px','2em')} becomes '.A {font-size: 20px; font-size: 2em;}' in CSS.
 
 Read about specificity of CSS selectors [here](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity).
@@ -280,36 +280,38 @@
     content = re.sub(r'\$', ',', content) # Replace $ with ,
     content = re.sub(r'\n\s+\n|\n\n','\n', content) # Remove empty lines after tab is replaced above
     content = re.sub('\t', '    ', content) # 4 space instead of tab is bettter option
     content = re.sub(r'\^',' ', content) # Remove left over ^ from start of main selector
         
     return content
 
-def _format_css(css_dict, allow_root_attrs = False):
+def _format_css(props : dict, allow_root_attrs = False):
+    if not isinstance(props, dict):
+        raise TypeError("props should be a dictionay of CSS selectors and properties.")
     uclass = get_unique_css_class()
     _all_css = '' # All css
-    root_attrs = {k:v for k,v in css_dict.items() if not isinstance(v,dict)}
+    root_attrs = {k:v for k,v in props.items() if not isinstance(v,dict)}
     allowed_attrs = {k:v for k,v in root_attrs.items() if "background" in k} # only allow background CSS to change at root
     if allow_root_attrs:
         if allowed_attrs: # Applies to background mostly
             _all_css += _build_css((f'{uclass}.SlidesWrapper, {uclass} .NavWrapper, {uclass} .BackLayer .Front',), allowed_attrs)
             if (root_attrs := {k:v for k,v in root_attrs.items() if k not in allowed_attrs}):
-                print(f'Skipping attributes: \n{root_attrs}\nat root level of css_dict!\nOnly background-related attributes are allowed at top!' )
+                print(f'Skipping attributes: \n{root_attrs}\nat root level of props!\nOnly background-related attributes are allowed at top!' )
 
     if root_attrs and not allow_root_attrs:
-        print(f'Skipping attributes: \n{root_attrs}\nat root level of css_dict!')
+        print(f'Skipping attributes: \n{root_attrs}\nat root level of props!')
     
-    css_dict = {k:v for k,v in css_dict.items() if isinstance(v,dict)} # Remove root attrs after they are set above for background, no more use
-    _all_css += _build_css((f'{uclass} .SlideArea',),css_dict) # Build css from dict
+    props = {k:v for k,v in props.items() if isinstance(v,dict)} # Remove root attrs after they are set above for background, no more use
+    _all_css += _build_css((f'{uclass} .SlideArea',),props) # Build css from dict
     return html('style', _all_css)
     
 @_sub_doc(css_docstring = _css_docstring)
-def format_css(css_dict):
+def format_css(props : dict):
     "{css_docstring}"
-    return _format_css(css_dict, allow_root_attrs = False)
+    return _format_css(props, allow_root_attrs = False)
 
 def alt(widget, func):
     """Display `widget` for slides and output of `func(widget)` will be and displayed only in exported formats as HTML.
     `func` should return possible HTML representation (provided by user) of widget as string.
     
     ```python run source
     import ipywidgets as ipw
```

### Comparing `ipyslides-3.8.5/ipyslides/writer.py` & `ipyslides-3.8.6/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides/xmd.py` & `ipyslides-3.8.6/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.6/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.5
+Version: 3.8.6
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.5/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.6/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.5/setup.py` & `ipyslides-3.8.6/setup.py`

 * *Files identical despite different names*

