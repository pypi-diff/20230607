# Comparing `tmp/apiiif-0.0.5.tar.gz` & `tmp/apiiif-0.0.6.tar.gz`

## Comparing `apiiif-0.0.5.tar` & `apiiif-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/__init__.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/factory.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.5/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.5/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.6/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.6/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.6/src/apiiif/factory.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 apiiif-0.0.6/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 apiiif-0.0.6/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.6/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.6/PKG-INFO
```

### Comparing `apiiif-0.0.5/src/apiiif/factory.py` & `apiiif-0.0.6/src/apiiif/factory.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.5/src/apiiif/resource_properties.py` & `apiiif-0.0.6/src/apiiif/resource_properties.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-from pydantic import BaseModel, AnyUrl, root_validator
+from pydantic import BaseModel, AnyUrl, root_validator, validator
+
+
+class BaseID(BaseModel):
+
+    @validator('id', pre=True)
+    def slugify(s):
+        if isinstance(s, str):
+            return s.replace(' ', '%20')
+        return s
+
+    id: AnyUrl
 
 
 class LanguageString(BaseModel):
     """A language string is a dictionary with language codes as keys and
     strings as values. The language codes are ISO 2-character codes.
     Add additional languages as needed, but once more than one exists,
     logic is needed to enable all to be optional, but one must be declared."""
@@ -22,52 +33,47 @@
 
 class LabelValue(BaseModel):
     """Used as the value of the requiredStatement and metadata items."""
     label: LanguageString
     value: LanguageString
 
 
-class Image(BaseModel):
-    id: AnyUrl
+class Image(BaseID):
     type: str = 'Image'
     width: int | None
     height: int | None
 
 
 class Thumbnail(Image):
     format: str = 'image/jpeg'
 
 
 class Logo(Image):
     format: str = 'image/png'
 
 
-class Homepage(BaseModel):
-    id: AnyUrl
+class Homepage(BaseID):
     type: str = 'Text'
     label: LanguageString
     format: str = 'text/html'
     language: list[str]
 
 
-class PartOf(BaseModel):
-    id: AnyUrl
+class PartOf(BaseID):
     type: str = 'Collection'
 
 
-class Provider(BaseModel):
-    id: AnyUrl
+class Provider(BaseID):
     type: str = 'Agent'
     label: LanguageString
     homepage: list[Homepage] | None
     logo: list[Logo] | None
 
 
 class Choice(BaseModel):
     type: str = 'Choice'
     items: list = []
 
 
-class ImageService(BaseModel):
-    id: AnyUrl
+class ImageService(BaseID):
     type: str = 'ImageService3'
     profile: str = 'level0'
```

### Comparing `apiiif-0.0.5/src/apiiif/resource_types.py` & `apiiif-0.0.6/src/apiiif/resource_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 from pydantic import BaseModel, AnyUrl, Field
 
 from apiiif.resource_properties import (LanguageString, LabelValue, Provider,
                                         Thumbnail, Homepage, PartOf, Image,
-                                        Choice, ImageService)
+                                        Choice, ImageService, BaseID)
 
 
 class IIIFImage(Image):
     format: str = 'image/jpeg'
     # as other services are defined, add them as options.
     service: list[ImageService] = []
 
 
-class Annotation(BaseModel):
+class Annotation(BaseID):
     context: str = Field(
         default='http://iiif.io/api/presentation/3/context.json',
         alias='@context')
-    id: AnyUrl
     type: str = 'Annotation'
     motivation: str = 'painting'
     target: AnyUrl
     body: IIIFImage | Choice | None = None
 
     def add_image(self, image: IIIFImage):
         if self.body is None:
             self.body = image
         elif isinstance(self.body, Choice):
             self.body.items.append(image)
         else:
             self.body = Choice(items=[self.body, image])
 
 
-class AnnotationPage(BaseModel):
+class AnnotationPage(BaseID):
     context: str = Field(
         default='http://iiif.io/api/presentation/3/context.json',
         alias='@context')
-    id: AnyUrl
     type: str = 'AnnotationPage'
     items: list[Annotation] = []
 
     def add_annotation(self, annotation: Annotation):
         self.items.append(annotation)
 
 
-class Canvas(BaseModel):
-    id: AnyUrl
+class Canvas(BaseID):
     type: str = 'Canvas'
     label: LanguageString
     height: int
     width: int
     behavior: list[str] | None  # ['paged'], ['facing-pages'], ['non-paged']
     items: list = []
 
@@ -57,19 +54,18 @@
 
 # Range should be defined here, but the collections site does not yet support it.
 # Use a range for creating a table of contents within the client (Mirador viewer).
 # For example, printed books could be broken into chapters, and manuscripts could
 # be devided into books or major sections since many manuscripts have non-biblical texts
 
 
-class Manifest(BaseModel):
+class Manifest(BaseID):
     context: str = Field(
         default='http://iiif.io/api/presentation/3/context.json',
         alias='@context')
-    id: AnyUrl
     type: str = 'Manifest'
     label: LanguageString
     metadata: list[LabelValue] = []
     summary: LanguageString | None
     thumbnail: Thumbnail | None
     viewingDirection: str = 'left-to-right'
     behavior: list[str] = ['paged']
@@ -80,19 +76,18 @@
     partOf: PartOf | None
     items: list = []
 
     def add_canvas(self, canvas: Canvas):
         self.items.append(canvas)
 
 
-class Collection(BaseModel):
+class Collection(BaseID):
     context: str = Field(
         default='http://iiif.io/api/presentation/3/context.json',
         alias='@context')
-    id: AnyUrl
     type: str = 'Collection'
     label: LanguageString
     requiredStatement: LabelValue | None
     items: list = []
 
     def add_manifest(self, manifest: Manifest):
         self.items.append(manifest)
```

### Comparing `apiiif-0.0.5/.gitignore` & `apiiif-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.5/LICENSE.txt` & `apiiif-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.5/README.md` & `apiiif-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.5/pyproject.toml` & `apiiif-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.5/PKG-INFO` & `apiiif-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

