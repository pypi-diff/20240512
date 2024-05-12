# Comparing `tmp/markdowntodocx-0.1.4.1.tar.gz` & `tmp/markdowntodocx-0.1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdowntodocx-0.1.4.1.tar", last modified: Thu Jan 18 10:51:34 2024, max compression
+gzip compressed data, was "markdowntodocx-0.1.5.0.tar", last modified: Sun May 12 18:01:28 2024, max compression
```

## Comparing `markdowntodocx-0.1.4.1.tar` & `markdowntodocx-0.1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-01-18 10:51:34.413716 markdowntodocx-0.1.4.1/
--rw-r--r--   0 barre     (1000) barre     (1000)     1064 2021-12-08 19:41:49.000000 markdowntodocx-0.1.4.1/LICENSE
--rw-r--r--   0 barre     (1000) barre     (1000)     4906 2024-01-18 10:51:34.413716 markdowntodocx-0.1.4.1/PKG-INFO
--rw-r--r--   0 barre     (1000) barre     (1000)     4637 2024-01-18 10:34:21.000000 markdowntodocx-0.1.4.1/README.md
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-01-18 10:51:34.410383 markdowntodocx-0.1.4.1/markdowntodocx/
--rw-r--r--   0 barre     (1000) barre     (1000)        0 2021-12-08 19:43:39.000000 markdowntodocx-0.1.4.1/markdowntodocx/__init__.py
--rw-r--r--   0 barre     (1000) barre     (1000)    29863 2024-01-18 10:49:34.000000 markdowntodocx-0.1.4.1/markdowntodocx/markdownconverter.py
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-01-18 10:51:34.413716 markdowntodocx-0.1.4.1/markdowntodocx.egg-info/
--rw-r--r--   0 barre     (1000) barre     (1000)     4906 2024-01-18 10:51:34.000000 markdowntodocx-0.1.4.1/markdowntodocx.egg-info/PKG-INFO
--rw-r--r--   0 barre     (1000) barre     (1000)      241 2024-01-18 10:51:34.000000 markdowntodocx-0.1.4.1/markdowntodocx.egg-info/SOURCES.txt
--rw-r--r--   0 barre     (1000) barre     (1000)        1 2024-01-18 10:51:34.000000 markdowntodocx-0.1.4.1/markdowntodocx.egg-info/dependency_links.txt
--rw-r--r--   0 barre     (1000) barre     (1000)       15 2024-01-18 10:51:34.000000 markdowntodocx-0.1.4.1/markdowntodocx.egg-info/top_level.txt
--rw-r--r--   0 barre     (1000) barre     (1000)       38 2024-01-18 10:51:34.413716 markdowntodocx-0.1.4.1/setup.cfg
--rw-r--r--   0 barre     (1000) barre     (1000)      618 2024-01-18 10:50:57.000000 markdowntodocx-0.1.4.1/setup.py
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-05-12 18:01:28.507943 markdowntodocx-0.1.5.0/
+-rw-r--r--   0 barre     (1000) barre     (1000)     1064 2021-12-08 19:41:49.000000 markdowntodocx-0.1.5.0/LICENSE
+-rw-r--r--   0 barre     (1000) barre     (1000)     4560 2024-05-12 18:01:28.507943 markdowntodocx-0.1.5.0/PKG-INFO
+-rw-r--r--   0 barre     (1000) barre     (1000)     4291 2024-04-02 15:36:42.000000 markdowntodocx-0.1.5.0/README.md
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-05-12 18:01:28.507943 markdowntodocx-0.1.5.0/markdowntodocx/
+-rw-r--r--   0 barre     (1000) barre     (1000)        0 2021-12-08 19:43:39.000000 markdowntodocx-0.1.5.0/markdowntodocx/__init__.py
+-rw-r--r--   0 barre     (1000) barre     (1000)    32537 2024-05-12 17:59:04.000000 markdowntodocx-0.1.5.0/markdowntodocx/markdownconverter.py
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2024-05-12 18:01:28.507943 markdowntodocx-0.1.5.0/markdowntodocx.egg-info/
+-rw-r--r--   0 barre     (1000) barre     (1000)     4560 2024-05-12 18:01:28.000000 markdowntodocx-0.1.5.0/markdowntodocx.egg-info/PKG-INFO
+-rw-r--r--   0 barre     (1000) barre     (1000)      241 2024-05-12 18:01:28.000000 markdowntodocx-0.1.5.0/markdowntodocx.egg-info/SOURCES.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)        1 2024-05-12 18:01:28.000000 markdowntodocx-0.1.5.0/markdowntodocx.egg-info/dependency_links.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)       15 2024-05-12 18:01:28.000000 markdowntodocx-0.1.5.0/markdowntodocx.egg-info/top_level.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)       38 2024-05-12 18:01:28.507943 markdowntodocx-0.1.5.0/setup.cfg
+-rw-r--r--   0 barre     (1000) barre     (1000)      625 2024-05-12 16:25:32.000000 markdowntodocx-0.1.5.0/setup.py
```

### Comparing `markdowntodocx-0.1.4.1/LICENSE` & `markdowntodocx-0.1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdowntodocx-0.1.4.1/PKG-INFO` & `markdowntodocx-0.1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdowntodocx
-Version: 0.1.4.1
+Version: 0.1.5.0
 Summary: Convert markdown inside Docx to docx styles
 Home-page: https://github.com/fbarre96/MarkDownToDocxStyle
 Author: Fabien Barre
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,26 +25,14 @@
 
 ```
 from markdowntodocx.markdownconverter import convertMarkdownInFile
 
 convertMarkdownInFile("/mypath/to/document.docx", "output_path.docx", {"Code Car":"CodeStyle"})
 ```
 
-**To convert a python-docx Document object:**
-
-```
-from markdowntodocx.markdownconverter import convertMarkdownInFile
-
-res, msg = convertMarkdownInFile("examples/in_document.docx", "examples/out_document.docx", {"Code Car":"CodeStyle"})
-if res:
-    print("Success : output document path is "+msg)
-else:
-    print("Error in document : "+msg)
-```
-
 ## Styles and considerations
     You have to define styles in you word document in order to use Markdown **Headers/titles**, **Hyperlinks**, **Code formatting**, **Arrays**, **Unordered List**.
 
 This styles are either standard markdown or come from extended markdown : https://www.markdownguide.org/extended-syntax/
     
 
 * Emphasis (*italic*) `*Text*` or `_Text_`:  converts to word italic
```

### Comparing `markdowntodocx-0.1.4.1/README.md` & `markdowntodocx-0.1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,14 @@
 
 ```
 from markdowntodocx.markdownconverter import convertMarkdownInFile
 
 convertMarkdownInFile("/mypath/to/document.docx", "output_path.docx", {"Code Car":"CodeStyle"})
 ```
 
-**To convert a python-docx Document object:**
-
-```
-from markdowntodocx.markdownconverter import convertMarkdownInFile
-
-res, msg = convertMarkdownInFile("examples/in_document.docx", "examples/out_document.docx", {"Code Car":"CodeStyle"})
-if res:
-    print("Success : output document path is "+msg)
-else:
-    print("Error in document : "+msg)
-```
-
 ## Styles and considerations
     You have to define styles in you word document in order to use Markdown **Headers/titles**, **Hyperlinks**, **Code formatting**, **Arrays**, **Unordered List**.
 
 This styles are either standard markdown or come from extended markdown : https://www.markdownguide.org/extended-syntax/
     
 
 * Emphasis (*italic*) `*Text*` or `_Text_`:  converts to word italic
```

### Comparing `markdowntodocx-0.1.4.1/markdowntodocx/markdownconverter.py` & `markdowntodocx-0.1.5.0/markdowntodocx/markdownconverter.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import docx
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.constants import CONTENT_TYPE as CT
 import random
 from docx.shared import Cm
 from docx.enum.table import WD_ALIGN_VERTICAL # pylint: disable=no-name-in-module
 from docx.enum.text import WD_BREAK, WD_COLOR_INDEX
-from docx.oxml.xmlchemy import OxmlElement
+from docx.oxml.parser import OxmlElement
 from docx.exceptions import InvalidXmlError
 from docx.oxml.ns import nsdecls
 from docx.oxml import parse_xml
 from docx.text.paragraph import Paragraph
 from docx.text.run import Run
 from docx.oxml.text.run import CT_R
+from docx.oxml.text.hyperlink import CT_Hyperlink
 #### Code rewritten and adapted to handle footnotes from baloo-docx ####
 from docx.opc.part import PartFactory
 from docx.opc.packuri import PackURI
 from docx.opc.part import XmlPart
 from docx.shared import RGBColor
 from docx.oxml.simpletypes import ST_DecimalNumber, ST_String
 from docx.opc.constants import NAMESPACE
@@ -123,19 +124,19 @@
 
     @classmethod
     def new (cls, _id):
         footnoteReference = OxmlElement('w:footnoteReference')
         footnoteReference._id = _id
         return footnoteReference
 
-class CT_Hyperlink(BaseOxmlElement):
-    @classmethod
-    def new (cls):
-        ref = OxmlElement('w:hyperlink')
-        return ref      
+# class CT_Hyperlink(BaseOxmlElement):
+#     @classmethod
+#     def new (cls):
+#         ref = OxmlElement('w:hyperlink')
+#         return ref      
 
 class CT_FootnoteRef (BaseOxmlElement):
     @classmethod
     def new (cls):
         ref = OxmlElement('w:footnoteRef')
         return ref       
 class FootnotesPart(XmlPart):
@@ -150,15 +151,15 @@
         return cls(partname, content_type, element, package)
 
 
 docx.oxml.register_element_cls('w:footnotes', CT_Footnotes)
 docx.oxml.register_element_cls('w:footnote', CT_Footnote)
 docx.oxml.register_element_cls('w:footnoteReference', CT_FNR)
 docx.oxml.register_element_cls('w:footnoteRef', CT_FootnoteRef)
-docx.oxml.register_element_cls('w:hyperlink', CT_Hyperlink)
+#docx.oxml.register_element_cls('w:hyperlink', CT_Hyperlink)
 PartFactory.part_type_for[CT.WML_FOOTNOTES] = FootnotesPart
 ##### END OF FOOTNOTES CODE ####
 #### EXTEND PARAGRAPH TO BE ABLE TO READ HYPERLINKS ####
 class Paragraph(docx.text.paragraph.Paragraph):
     def __init__(self, *args, **kwargs):
         super().__init__( *args, **kwargs)
     
@@ -189,62 +190,79 @@
             if isinstance(_elem, CT_Hyperlink):
                 for _r in _elem:
                     runs.append(Run(_r, _elem))
         return runs
 ####
 footnotes = {}
 default_styles_names = {
-        "Hyperlink": "Hyperlink",
-        "Code": "Code",
-        "Code Car": "Code Car",
-        "BulletList": "BulletList",
-        "Cell": "Cell",
-        "Header": "Header"
+        "Hyperlink": ("Hyperlink",),
+        "Code": ("Code", "macro"),
+        "Code Car": ("Code Car", "Macro Text Char"),
+        "BulletList": ("BulletList", "List Paragraph"),
+        "Cell": ("Cell", "No Spacing"),
+        "Header1": ("Heading 1", "Header"),
+        "Header2": ("Heading 2", "Header"),
+        "Header3": ("Heading 3", "Header"),
+        "Header4": ("Heading 4", "Header"),
+        "Header5": ("Heading 5", "Header"),
+        "Header6": ("Heading 6", "Header"),
     }
 styles = {}
-header_style = None
 code_style = None
 hyperlink_style = None
 
 def convertMarkdownInFile(infile, outfile, styles_names=None):
     global default_styles_names
     global styles
     if styles_names:
         for key, val in styles_names.items():
             default_styles_names[key] = val
     document = docx.Document(infile)
     for style in document.styles:
         styles[style.name] = style
-    for style_name in default_styles_names.values():
-        if style_name not in styles:
-            return False, "Error in template. There is a style missing : "+str(style_name)
-    
-    global header_style
+    for key, style_name in default_styles_names.items():
+        if isinstance(style_name, tuple):
+            found = False
+            for name in style_name:
+                if name in styles:
+                    default_styles_names[key] = name
+                    found = True
+                    break
+            if not found and name != "Hyperlink":
+                return False, "Error in template. There is no "+str(name)+ " style in the doc. Searched for : "+str(key)
+        else:
+            if style_name not in styles and name != "Hyperlink":
+                return False, "Error in template. There is a style missing : "+str(style_name)
     global code_style
     global hyperlink_style
-    for x in styles:
-        if x == default_styles_names.get("Header", "Header"):
-            header_style = styles[default_styles_names.get("Header", "Header")]
-    if header_style is None:
-        raise KeyError("No style named "+default_styles_names.get("Header", "Header"))
-    code_style = styles[default_styles_names.get("Code Car", "Code Car")]
-    hyperlink_style = styles[default_styles_names.get("Hyperlink", "Hyperlink")]
+   
+    code_style = styles.get(default_styles_names.get("Code Car", "Code Car"), "macro")
+    hyperlink_style = styles.get(default_styles_names.get("Hyperlink", "Hyperlink"), None)
     markdownToWordInDocument(document)
     document.save(outfile)
     return True, outfile
     
 def markdownToWordInDocument(document):
     ps = getParagraphs(document)
     state = "normal"
     for paragraph in ps:
         state = markdownToWordInParagraph(document, paragraph, state)
     ps = getParagraphs(document)
     for paragraph in ps:
         state = markdownToWordInParagraphCar(document, paragraph, state)
     
+
+def markdownToWordFromString(string, outfile):
+    document = docx.Document()
+    paragraphs = string.replace("\r","").split("\n")
+    for para in paragraphs:
+        document.add_paragraph(para)
+    document.save(outfile)
+    return convertMarkdownInFile(outfile, outfile)
+    
 def getParagraphs(document):
     """ Retourne un generateur pour tous les paragraphes du document.
         La page d'entête n'étant pas incluse dans documents.paragraphs."""
     body = document._body._body # pylint: disable=protected-access
     ps = body.xpath('//w:p')
     for p in ps:
         yield Paragraph(p, document._body) # pylint: disable=protected-access
@@ -274,14 +292,16 @@
     fontB.subscript = fontA.subscript
     fontB.superscript = fontA.superscript
     fontB.size = fontA.size
     try:
         fontB.highlight_color = fontA.highlight_color
     except InvalidXmlError as e:
         pass
+    except ValueError as e:
+        pass
     fontB.color.rgb = fontA.color.rgb
 
 
 def markdownArrayToWordList(document, paragraph, state):
     table_line_regex = re.compile(r"^\|(?:[^|\n]*[^-|\n][^|\n]*\|)*\s*$", re.MULTILINE)
     matched = re.findall(table_line_regex, paragraph.text)
     if len(matched) == 0:
@@ -310,15 +330,15 @@
             end = paragraph.text.index(matched[-1], start+len(matched[0]))+len(matched[-1])
             text_end = paragraph.text[end:]
         except ValueError:
             text_end = ""
         paragraph.text = paragraph.text[:start-2].strip() # -2 for list marker + space
         for match in matched:
             new_p = insert_paragraph_after(paragraph)
-            new_p.style = "BulletList"
+            new_p.style = styles[default_styles_names.get("BulletList","BulletList")]
             r = new_p.add_run()
             r.add_text(match)
         if text_end.strip() != "":
             insert_paragraph_after(new_p, text_end)
         if paragraph.text.strip() == "":
             delete_paragraph(paragraph)
     return state
@@ -340,30 +360,30 @@
         insert_paragraph_after(paragraph, "```".join(text_bits[1:]))
         
     return state
 
 def markdownToWordInParagraph(document, paragraph, state):
     state = markdownArrayToWordList(document, paragraph, state)
     state = markdownUnorderedListToWordList(paragraph, styles[default_styles_names.get("BulletList","BulletList")], state)
-    state = mardownCodeBlockToWordStyle(paragraph, styles[default_styles_names.get("Code","Code")], state)
+    state = mardownCodeBlockToWordStyle(paragraph, styles.get(default_styles_names.get("Code","Code"), "Macro Text"), state)
     return state
 
 def setColor(paragraph, run, match):
     # match.group(0) is <color:RGB>text</color> 
     # match.group(1) is <color
     # match.group(2) is RGB>text
     # match.group(3) is </color>
     splitted = match.group(2).split(">")
     run.font.color.rgb = RGBColor.from_string(splitted[0])
     initial_len = len(run.text)
     run.text = ">".join(splitted[1:])
     return initial_len-len(run.text), False, "normal"
 
 def markdownToWordInParagraphCar(document, paragraph, state):
-    markdownHeaderToWordStyle(paragraph, header_style)
+    markdownHeaderToWordStyle(paragraph)
     transform_marker(paragraph, "==", setHighlight)
     transform_marker(paragraph, "**", setBold)
     transform_marker(paragraph, "__", setBold)
     transform_marker(paragraph, "*", setItalic)
     transform_marker(paragraph, "_", setItalic)
     transform_marker(paragraph, "~~", setStrike)
     transform_marker(paragraph, "`", setCode)
@@ -409,15 +429,18 @@
     else:
         transform_regex(paragraph, r"(https?:\/\/(?:www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b(?:[-a-zA-Z0-9()@:%_\+.~#?&//=]*[-a-zA-Z0-9@:%_\+.~#?&//=]))", (setHyperlink,))
     
     return state
 
 def setHyperlink(paragraph, run, match, **kwargs):
     run.font.underline = True
-    run.style = hyperlink_style
+    if hyperlink_style is not None:
+        run.style = hyperlink_style
+    else:
+        run.font.color.rgb = RGBColor.from_string("0000FF")
     deletedCars = len(run.text)
     try:
         link_text = match.group(2)
         link_url = match.group(4)
     except:
         link_text = kwargs.get("text", match.group(0))
         link_url = kwargs.get("url", match.group(0))
@@ -603,20 +626,23 @@
         for i, func in enumerate(funcs):
             run = paragraph.runs[runs[i][0] - deleted_runs]
             deleted_count, deleted_run, state = func(paragraph, run, match)
             deleted_runs += 1 if deleted_run else 0
             deletedCars += deleted_count
     return state
 
-def markdownHeaderToWordStyle(paragraph, header_style):
+def markdownHeaderToWordStyle(paragraph):
     
-    for match in re.finditer(r"^\s*#{1,6} (.+)$", paragraph.text, re.MULTILINE):
+    for match in re.finditer(r"^\s*(#{1,6}) (.+)$", paragraph.text, re.MULTILINE):
         paragraph.text = re.sub(r"^\s*#{1,6} ", "",paragraph.text)
-        paragraph.style = header_style
-
+        headersize = len(match.group(1))
+        header_style = styles.get(default_styles_names.get("Header"+str(headersize), "Heading "+str(headersize)), None)
+        if header_style is not None:
+            paragraph.style = header_style
+        
 
 def getRunsIndexFromPositions(paragraph, positions):
     """returns a list of tuples (runIndex, positionInRun) for each caracter position in the list positions
     example:
         paragraph.text is "This is an *example* of a paragraph"
         runs look like this:
             [
@@ -724,14 +750,16 @@
 
 
 def set_hyperlink(paragraph, run, url, text, style):
     # This gets access to the document.xml.rels file and gets a new relation id value
     run.font.underline = True
     if style is not None:
         run.style = style
+    else:
+        run.font.color.rgb = RGBColor(0, 0, 255)
     part = paragraph.part
     r_id = part.relate_to(url, docx.opc.constants.RELATIONSHIP_TYPE.HYPERLINK, is_external=True)
     index_in_paragraph = paragraph._p.index(run.element)
     # Create the w:hyperlink tag and add needed values
     hyperlink = docx.oxml.shared.OxmlElement('w:hyperlink')
     hyperlink.set(docx.oxml.shared.qn('r:id'), r_id, )
     run.element.text = text
@@ -760,12 +788,66 @@
         new_para.add_run(text)
     if style is not None:
         new_para.style = style
     return new_para
 
 
 if __name__ == '__main__':
-    res, msg = convertMarkdownInFile("examples/in_document.docx", "examples/out_document.docx", {"Header":"Header","Code Car":"CodeStyle"})
+    #res, msg = convertMarkdownInFile("examples/in_document.docx", "examples/out_document.docx", {"Header":"Header","Code Car":"CodeStyle"})
+    res, msg = markdownToWordFromString("""# H1 Header: Welcome to My Markdown Guide!
+
+## H2 Header: Quick Overview
+Markdown is a lightweight markup language that you can use to add formatting elements to plaintext text documents. Created by John Gruber in 2004, Markdown is now one of the world’s most popular markup languages.
+
+### H3 Header: What Markdown Can Do
+
+#### H4 Header: Formatting Text
+You can do numerous things with Markdown format, including:
+
+- **Bold** text
+- *Italic* text
+- **_Combined emphasis_**
+
+> **Note:** Markdown is not the same as Markup. They’re different, remember!
+
+#### H4 Header: Creating Lists
+
+##### H5 Header: Unordered Lists
+- Item one
+- Item two
+  - Sub Item one
+  - Sub Item two
+
+##### H5 Header: Ordered Lists
+1. First item
+2. Second item
+    1. Subitem
+    2. Subitem
+
+#### H4 Header: Adding Links and Images
+
+Here is a clickable link to [OpenAI](https://www.openai.com), the organization behind Assistant.
+
+Here is an image:
+
+[Alt text for image](https://via.placeholder.com/150)
+
+#### H4 Header: Inserting Code
+
+```python
+# This is some Python code
+def say_hello(name):
+    print("Hello, " + name)
+```
+
+##### H5 Header: Inline Code
+You can also use inline `code` within your text.
+
+### H3 Header: Using Blockquotes
+
+> Markdown uses email-style > characters for blockquoting.
+> It’s very handy for email mimicking."""
+, "examples/out_string.docx")
     if res:
         print("Success : output document path is "+msg)
     else:
         print("Error in document : "+msg)
```

### Comparing `markdowntodocx-0.1.4.1/markdowntodocx.egg-info/PKG-INFO` & `markdowntodocx-0.1.5.0/markdowntodocx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdowntodocx
-Version: 0.1.4.1
+Version: 0.1.5.0
 Summary: Convert markdown inside Docx to docx styles
 Home-page: https://github.com/fbarre96/MarkDownToDocxStyle
 Author: Fabien Barre
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,26 +25,14 @@
 
 ```
 from markdowntodocx.markdownconverter import convertMarkdownInFile
 
 convertMarkdownInFile("/mypath/to/document.docx", "output_path.docx", {"Code Car":"CodeStyle"})
 ```
 
-**To convert a python-docx Document object:**
-
-```
-from markdowntodocx.markdownconverter import convertMarkdownInFile
-
-res, msg = convertMarkdownInFile("examples/in_document.docx", "examples/out_document.docx", {"Code Car":"CodeStyle"})
-if res:
-    print("Success : output document path is "+msg)
-else:
-    print("Error in document : "+msg)
-```
-
 ## Styles and considerations
     You have to define styles in you word document in order to use Markdown **Headers/titles**, **Hyperlinks**, **Code formatting**, **Arrays**, **Unordered List**.
 
 This styles are either standard markdown or come from extended markdown : https://www.markdownguide.org/extended-syntax/
     
 
 * Emphasis (*italic*) `*Text*` or `_Text_`:  converts to word italic
```

### Comparing `markdowntodocx-0.1.4.1/setup.py` & `markdowntodocx-0.1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='markdowntodocx',
     packages=find_packages(include=['markdowntodocx']),
-    version='0.1.4.1',
+    version='0.1.5.0',
     url="https://github.com/fbarre96/MarkDownToDocxStyle",
     description='Convert markdown inside Docx to docx styles',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Fabien Barre',
     license='MIT',
-    setup_requires=['python-docx',"requests"],
+    setup_requires=['python-docx>=1.1.2',"requests"],
 )
```

