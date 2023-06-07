# Comparing `tmp/mwxlib-0.84.9-py3-none-any.whl.zip` & `tmp/mwxlib-0.85.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162167 bytes, number of entries: 22
+Zip file size: 162106 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-03 17:04 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43499 b- defN 23-Jun-03 17:04 mwx/controls.py
--rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-05 06:58 mwx/framework.py
--rw-rw-rw-  2.0 fat    68716 b- defN 23-Jun-05 06:02 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73681 b- defN 23-Jun-05 06:59 mwx/framework.py
+-rw-rw-rw-  2.0 fat    68631 b- defN 23-Jun-05 07:49 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-Jun-03 17:04 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-Jun-03 17:04 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27598 b- defN 23-Jun-03 17:04 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138759 b- defN 23-Jun-05 06:58 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37431 b- defN 23-Jun-05 06:58 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   138916 b- defN 23-Jun-07 01:03 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37369 b- defN 23-Jun-05 06:59 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-Jun-03 17:04 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-Jun-03 17:04 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-Jun-03 17:04 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-Jun-03 17:04 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-03 17:04 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-05 06:58 mwxlib-0.84.9.dist-info/RECORD
-22 files, 614606 bytes uncompressed, 159665 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-07 04:01 mwxlib-0.85.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-07 04:01 mwxlib-0.85.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 04:01 mwxlib-0.85.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-07 04:01 mwxlib-0.85.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-07 04:01 mwxlib-0.85.0.dist-info/RECORD
+22 files, 614481 bytes uncompressed, 159604 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.9.dist-info/LICENSE
+Filename: mwxlib-0.85.0.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.9.dist-info/METADATA
+Filename: mwxlib-0.85.0.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.9.dist-info/WHEEL
+Filename: mwxlib-0.85.0.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.9.dist-info/top_level.txt
+Filename: mwxlib-0.85.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.9.dist-info/RECORD
+Filename: mwxlib-0.85.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.84.9"
+__version__ = "0.85.0"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -1587,16 +1587,14 @@
         if traceable:
             book.handler.bind('pointer_set', _F(self.start_trace, book=book))
             book.handler.bind('pointer_unset', _F(self.stop_trace, book=book))
         else:
             book.handler.unbind('pointer_set')
             book.handler.unbind('pointer_unset')
     
-    set_traceable = set_hookable # for backward compatibility
-    
     def start_trace(self, line, book):
         if not self.debugger.busy:
             self.debugger.unwatch()
             self.debugger.editor = book
             self.debugger.watch((book.buffer.filename, line+1))
             self.debugger.send_input('') # clear input
         book.buffer.del_marker(4)
@@ -1708,16 +1706,14 @@
     ## --------------------------------
     
     def get_all_pages(self, type=None):
         """Yields all pages of the specified type in the notebooks."""
         yield from self.console.get_pages(type)
         yield from self.ghost.get_pages(type)
     
-    get_pages = get_all_pages # for backward compatibility
-    
     @property
     def all_books(self):
         """Yields all books in the notebooks."""
         yield from self.get_all_pages(type(self.Log))
     
     @property
     def current_shell(self):
```

## mwx/graphman.py

```diff
@@ -1534,15 +1534,15 @@
         """Load buffers from paths to the view window.
         
         If no view given, the currently selected view is chosen.
         """
         if view not in self.graphic_windows:
             view = self.selected_view
         
-        if isinstance(paths, str): # for single frame: backward compatibility
+        if isinstance(paths, str): # for single frame
             paths = [paths]
         
         if paths is None:
             with wx.FileDialog(self, "Open image files",
                     wildcard='|'.join(self.wildcards),
                     style=wx.FD_OPEN|wx.FD_MULTIPLE|wx.FD_FILE_MUST_EXIST) as dlg:
                 if dlg.ShowModal() != wx.ID_OK:
@@ -1751,22 +1751,21 @@
 
 
 if __name__ == "__main__":
     app = wx.App()
     frm = Frame(None)
     
     frm.handler.debug = 0
-    frm.graph.handler.debug = 4
+    frm.graph.handler.debug = 0
     frm.output.handler.debug = 0
     
-    frm.load_buffer(r"C:\usr\home\lib\python\demo\sample.bmp")
-    frm.load_buffer(r"C:\usr\home\lib\python\demo\sample2.tif")
+    frm.load_frame([r"C:\usr\home\lib\python\demo\sample.bmp",
+                    r"C:\usr\home\lib\python\demo\sample2.tif",
+                    ])
     frm.graph.load(np.random.randn(1024,1024))
     
     ## Note: 次の二つは別モジュール扱い
     ## frm.load_plug("demo.template.py", show=1, force=1)
     ## frm.load_plug("demo/template.py", show=1, force=1)
     
-    frm.load_plug(r"C:\usr\home\lib\python\demo\template.py", show=1, dock=4)
-    
     frm.Show()
     app.MainLoop()
```

## mwx/nutshell.py

```diff
@@ -791,15 +791,15 @@
         """Called when a line of text selection is changing."""
         p = self.PositionFromPoint(evt.Position) #<wx._core.MouseEvent>
         po, qo = self.__anchors
         if self.__margin:
             if p >= po:
                 lc = self.LineFromPosition(p)
                 text = self.GetLine(lc)
-                self.cpos = p + len(text)
+                self.cpos = p + len(text.encode()) # Count bytes.
                 self.anchor = po
                 if not self.GetFoldExpanded(lc): # Select more lines hidden if folded.
                     self.CharRightExtend()
                     self.__anchors[1] = self.cpos
             else:
                 self.cpos = p
                 self.anchor = qo
@@ -1048,15 +1048,19 @@
             self.goto_char(p)
             self.goto_char(self.bol)
             self.mark = self.cpos
             self.EnsureVisible(self.cline)
             yield err
     
     def grep(self, pattern, flags=re.M):
-        yield from re.finditer(pattern, self.Text, flags)
+        ## Note: Count bytes; Use self.GetTextRange(p,q).
+        yield from re.finditer(pattern.encode(), self.TextRaw, flags)
+        
+        ## Note: Count multi-byte chars; Use self.Text[p:q].
+        ## yield from re.finditer(pattern, self.Text, flags)
     
     def search_text(self, text):
         """Yields raw-positions where `text` is found."""
         word = text.encode()
         raw = self.TextRaw
         pos = -1
         while 1:
@@ -2094,16 +2098,14 @@
         with wx.FileDialog(self, "Save buffer as",
                 defaultFile=name,
                 wildcard='|'.join(self.wildcards),
                 style=wx.FD_SAVE|wx.FD_OVERWRITE_PROMPT) as dlg:
             if dlg.ShowModal() == wx.ID_OK:
                 return self.save_file(dlg.Path, buf)
     
-    save_as_buffer = save_buffer_as # for backward compatibility
-    
     def save_all_buffers(self):
         for buf in self.all_buffers:
             if buf.need_buffer_save:
                 self.save_buffer(buf)
     
     def open_buffer(self):
         """Confirm the open with the dialog."""
```

## mwx/utilus.py

```diff
@@ -542,16 +542,14 @@
     default_state = None
     current_state = property(lambda self: self.__state)
     previous_state = property(lambda self: self.__prev_state)
     
     current_event = property(lambda self: self.__event)
     previous_event = property(lambda self: self.__prev_event)
     
-    event = current_event # for backward compatibility
-    
     @current_state.setter
     def current_state(self, state):
         self.__state = state
         self.__event = '*forced*'
         self.__debcall__(self.__event)
     
     def clear(self, state):
```

## Comparing `mwxlib-0.84.9.dist-info/LICENSE` & `mwxlib-0.85.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.9.dist-info/METADATA` & `mwxlib-0.85.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.9
+Version: 0.85.0
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.84.9.dist-info/RECORD` & `mwxlib-0.85.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=pD1IjgkwdvD-ebntnAH-6Jo7KY5hDq30Ne6rTE_i9fE,43499
-mwx/framework.py,sha256=axKlqwJG6pi5x6q0-dUtegNtDzBDWqow9QGasGt3vXM,73816
-mwx/graphman.py,sha256=iF1cSVYdQHiu1Wylt1cBGIzbQtZQLSetRN3qw_g6-jA,68716
+mwx/framework.py,sha256=NDrj7pvN0tS1Qb2K1FkvAC8OrZX6CZJDxvmDfwbjefk,73681
+mwx/graphman.py,sha256=vQAO19MyRFdAAQVyaGzEn-WJy5yrkQwtWNr7UKcHgT8,68631
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=vVlBulRQDyYonI9EKfqp-3SpNbGyIJQ6ldkw6bZlalo,27598
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=ajJBsC9o_21DuYuw5mwRGpB4GgwWT2rOjlf-DS-ntLI,138759
-mwx/utilus.py,sha256=ADA8I7qg339TJOvbrWWD91jqICWfc5C-ENFE-a7YBvU,37431
+mwx/nutshell.py,sha256=OfuTU0MBMLlOGSWwwyZEERts2jyyHbyPel9GbyuqP4Q,138916
+mwx/utilus.py,sha256=PDEJhTfDlFrcOe5w6zmU5EHmAfqIDOu74fKewi1rybY,37369
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.84.9.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.84.9.dist-info/METADATA,sha256=Nt7X4C4jS8_safBBRGm2ZcZzk3WEo5B9-czJj-3UIfU,1893
-mwxlib-0.84.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.84.9.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.84.9.dist-info/RECORD,,
+mwxlib-0.85.0.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.85.0.dist-info/METADATA,sha256=6ZxBuu5IFawBD55YWIhxP7rymvy6TUoz6C4rBymPg_k,1893
+mwxlib-0.85.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.85.0.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.85.0.dist-info/RECORD,,
```

