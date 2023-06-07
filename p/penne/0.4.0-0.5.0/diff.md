# Comparing `tmp/penne-0.4.0.tar.gz` & `tmp/penne-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penne-0.4.0.tar", last modified: Thu May  4 16:21:34 2023, max compression
+gzip compressed data, was "penne-0.5.0.tar", last modified: Wed Jun  7 21:24:46 2023, max compression
```

## Comparing `penne-0.4.0.tar` & `penne-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,22 @@
--rw-r--r--   0        0        0     5781 2023-05-04 16:21:24.833092 penne-0.4.0/README.md
--rw-r--r--   0        0        0      564 2023-05-04 16:21:24.837092 penne-0.4.0/penne/__init__.py
--rw-r--r--   0        0        0    10169 2023-05-04 16:21:24.837092 penne-0.4.0/penne/core.py
--rw-r--r--   0        0        0    27611 2023-05-04 16:21:24.837092 penne-0.4.0/penne/delegates.py
--rw-r--r--   0        0        0     5470 2023-05-04 16:21:24.837092 penne-0.4.0/penne/handlers.py
--rw-r--r--   0        0        0      737 2023-05-04 16:21:24.837092 penne-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6516 1970-01-01 00:00:00.000000 penne-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2854 2023-06-01 20:08:41.865752 penne-0.5.0/.github/workflows/continuous_integration.yml
+-rw-r--r--   0        0        0     1421 2023-06-01 20:08:41.866554 penne-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1047 2023-06-01 20:08:41.867485 penne-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1084 2023-06-01 20:08:41.868117 penne-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3190 2023-06-01 20:08:41.868765 penne-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1101 2022-07-26 21:32:06.694759 penne-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7539 2023-06-07 18:52:37.200651 penne-0.5.0/README.md
+-rw-r--r--   0        0        0      564 2023-06-07 21:24:43.063336 penne-0.5.0/penne/__init__.py
+-rw-r--r--   0        0        0    12279 2023-06-07 21:14:41.758639 penne-0.5.0/penne/core.py
+-rw-r--r--   0        0        0    29166 2023-06-07 18:06:30.561762 penne-0.5.0/penne/delegates.py
+-rw-r--r--   0        0        0     4575 2023-06-07 21:14:41.735989 penne-0.5.0/penne/handlers.py
+-rw-r--r--   0        0        0      737 2023-06-01 20:08:41.873575 penne-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-06 00:39:00.685439 penne-0.5.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-28 16:49:33.574552 penne-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     6590 2023-06-07 18:44:56.624565 penne-0.5.0/tests/clients.py
+-rw-r--r--   0        0        0     2562 2023-06-07 17:29:34.352182 penne-0.5.0/tests/plottyn_integration.py
+-rw-r--r--   0        0        0      393 2023-06-01 20:08:41.878884 penne-0.5.0/tests/server_conformance.py
+-rw-r--r--   0        0        0     9951 2023-06-06 18:39:21.774324 penne-0.5.0/tests/servers.py
+-rw-r--r--   0        0        0     5600 2023-06-07 21:14:41.753887 penne-0.5.0/tests/test_core.py
+-rw-r--r--   0        0        0     9994 2023-06-07 20:52:06.090169 penne-0.5.0/tests/test_delegates.py
+-rw-r--r--   0        0        0     2117 2023-06-07 15:49:58.585778 penne-0.5.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     8274 1970-01-01 00:00:00.000000 penne-0.5.0/PKG-INFO
```

### Comparing `penne-0.4.0/README.md` & `penne-0.5.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,129 @@
 # PENNE
 
 ![Build Status](https://github.com/InsightCenterNoodles/Penne/workflows/CI/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/Penne)
-![Coverage](tests/coverage/coverage.svg)
-![Coverage](https://github.com/InsightCenterNoodles/Penne/raw/aebac0f/coverage-badge/coverage.svg)
+[![Coverage badge](https://raw.githubusercontent.com/InsightCenterNoodles/Penne/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Penne/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 
 Python Client for NOODLES protocol  
 (Python Encoded Native NOODLES Endpoint)
 
 ## Description
 The client library is based on the NOODLES messaging protocol for communicating with serverside data visualisation applications. The client uses a websocket connection to send CBOR encoded messages. To customize its implementation, the
-library offers hooks in the form of delegates classes which can be extended and overwritten.
+library offers hooks in the form of delegates classes which can be extended.
 
 ## How does the client work?
 When a message is received from the server, the client passes the CBOR encoded message to a handler function which uses
 the message's ID to process it accordingly. Based on this ID, the message can be classified as either a create, delete, 
 update, reply, or invoke message. Upon receiving a create message, the handler creates a new delegate for that object
-which is then stored in the client's state. Delete and update messages manipulate delegates in the client's state as expected. Reply messages indicate whether a method was invoked on the server successfully, and then a callback function can be executed if applicable. Lastly, invoke messages represent signals from the server which are being called on a delegate. The handler essentially sends this signal to the target delgate so it can call a corresponding function. 
-
-To send a message, the user calls a method on a delegate. This method wraps an injected method from the server, and the client can send a message invoking the method.
+which is then stored in the client's state. Delete and update messages manipulate delegates in the client's state as expected. 
+Reply messages indicate whether a method was invoked on the server successfully, and then a callback function can be 
+executed if applicable. Lastly, invoke messages represent signals from the server which are being called on a delegate. 
+The handler sends this signal to the target delegate so it can call a corresponding function. 
+
+To send a message, the user calls a method on a delegate or the document more broadly. Delegates may have injected 
+methods from the server, and the client can send a message invoking the method. For example, the server can define a
+method like insert_row() on a table delegate. The client can then call this method on the delegate, and the server will
+get a message requesting to invoke the method. The server will then respond by updating the state, invoking signals, 
+and sending a reply message to the client. If the server is unable to invoke the method, it will send a reply message
+that contains an exception.
 
 A diagram representing the simplified relationships between the client, server, and delegates is depicted below. 
 
 ```mermaid
-flowchart LR;
-    User-- Request to Invoke Method -->Delegate;
-    User-- Create Custom Delegates --> Client;
-    User-- Create New Plot --> Client;
-    Delegate-- Call Injected Method -->Client;
-    Client-- Send Invoke Method Message -->Server;
-    Server-- Message -->Client;
-    Client-- Create w/ Injection -->Delegate;
-    Client-- Update -->Delegate;
-    Client-- Invoke Signal -->Delegate;
-    Delegate-- Show current state -->User;
+sequenceDiagram
+    participant User
+    participant Delegate
+    participant Client
+    participant Server
+    User->>Delegate: Create Custom Delegates
+    User->>Client: Starts Server with Custom Delegates
+    Client->>Server: Sends Intro Message
+    Server->>Client: Updates the Client with Current State
+    loop until end of session
+        User->>Delegate: Invoke Injected or Custom Method on Delegate or...
+        User->>Client: Invoke Method on Client Directly
+        Client->>Server: Request to Invoke Method
+        Server->>Client: Responds to Update State
+        Client->>Delegate: Invokes Signals, Creates, Updates, and Deletes Delegates
+        Client->>User: Show Current State
+    end
 ```
 
 ## Working with delegates
 >What are delegates? 
 
-NOODLES messages deal with many different objects ranging from tables and plots to lights and materials. To help with 
+NOODLES messages deal with many objects ranging from tables and plots to lights and materials. To help with 
 using these objects, each type has its own delegate class. Each object in a scene corresponds with an instance of a delegate
-which is stored in the client's state. Delegates provide methods specific to each type of object.
-
-Note: PENNE currently offers support primarily for the table delegate class
+which is stored in the client's state. Delegates provide methods specific to each type of object. These objects can contain 
+injected methods and signals from the server. All delegates come with methods `on_new()`, `on_update()`, and `on_remove()`
+which are called automatically when the server sends a message to create, update, or delete an object.
 
 >How can I use custom delegates?
 
-To work with your own delegates, use a custom delegate hash as an argument in `create_client()`. To overide a default
-delegate, use the same key in your dictionary. The library also provides a generic `Delegate` class that
-should be used as the parent class for any delegate. An example of a custom delegate is included in `test_client.py`. Here, the delegate class inherits from `TableDelegate` and uses the pandas library to add table and plotting functionality. 
+To work with your own delegates, simply create a class that inherits from the base delegate. Then, pass a dictionary as
+an argument to the constructor that maps the delegate's type to the new class. In `tests/clients.py` there is a more
+involved example that extends the table delegate. Here, the delegate class 
+inherits from `Table` and uses pandas and matplotlib to add plotting functionality. Below is an even more basic example
+that prints a message whenever a new method is created.
+
+```python
+from penne import Method, Client
+
+
+class CustomMethod(Method):
+  
+  def on_new(self, message: dict):
+    print(f"New method named {self.name} was created")
+    
+      
+with Client(address, {Method: CustomMethod}) as client:
+  # do stuff
+
+```
 
 >How do you call methods on a delegate?
 
 Once instantiated, delegates are injected with methods designated by the server. These methods can be called by using
 public methods on the delegate that essentially wrap the injected ones. Once the method is invoked, the server will 
 respond with a signal that updates the client. Each signal is linked to a method in the delegate which keeps the state of 
 the client up to date. To customize the client's behavior, these methods can be overwritten in a custom delegate. Each 
-public method also accepts a callback function to be executed once a response is received from the server. This way, method calls can be chained together and run in sequence. An example is provided in `test_client.py`.
+public method also accepts a callback function to be executed once a response is received from the server. 
+This way, method calls can be chained together and run in sequence. An example is provided in `tests/plottyn_integration.py`.
 
 ### Tables
 The table delegate comes with several built in methods covering basic table manipulation. The delegate includes...
 ```python
-request_insert(col_list: list=None, row_list: list=None, on_done=None)
+subscribe(on_done=None)
+request_insert(row_list: list=None, on_done=None)
 request_remove(keys: list, on_done=None)
-request_update(data_frame: pandas.DataFrame, on_done=None)
+request_update(keys: List[int], rows: List[List[int]], on_done=None)
 request_clear(on_done=None)
 request_update_selection(name: str, keys: list, on_done=None)
 ```
-Once invoked, signals from the server will update the table in the delegate. When using these methods, the user has the option of including a callback function that will execute once complete.
+When using these methods, the user has the option of including a callback function (on_done) that will execute once complete.
+Once invoked, signals from the server will update the table in the delegate. For the table thereare several signals that
+can be overwritten in a custom delegate. While you can inherit and customize them for your specif implementation of the
+table, they should not be called directly by users. They will be called when indicated by a message from the server. 
+These include...
+```python
+_on_table_init(init_info: dict, on_done=None)
+_reset_table(init_info: dict)
+_remove_rows(keys: list[int])
+_update_rows(keys: list[int], rows: list[list])
+_update_selection(selection: dict)
+```
 
 ## Getting Started
 1. Install the library
 ```python
 pip install penne
 ```
-2. Create a client using `create_client(address, delegate_hash)`
+2. Create a client using 
 ```python
 from penne import Client
 
 with Client(address, delegate_hash) as client:
     # do stuff
 ```
 - (Optional) use delegate hash to map custom delegates
```

### Comparing `penne-0.4.0/penne/__init__.py` & `penne-0.5.0/penne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 Modules:
     core.py
     test_delegates.py
     handlers.py
     messages.py
 """
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 # Imports for easier user access
 from .core import Client
 from .delegates import *
```

### Comparing `penne-0.4.0/penne/delegates.py` & `penne-0.5.0/penne/delegates.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,151 @@
 Follows the specification in the cddl document, and
 implements strict validation
 """
 
 from __future__ import annotations
 
 import logging
-from typing import Literal, Optional, Any, Union, Callable, List, Tuple
-from collections import namedtuple
+from typing import Optional, Any, Union, Callable, List, Tuple, NamedTuple
 from enum import Enum
 from math import pi
 
-from pydantic import BaseModel, root_validator, Extra, validator
+from pydantic import BaseModel, root_validator, Extra, validator, Field
 from pydantic.color import Color
 
 
-""" =============================== ID's ============================= """
+class InjectedMethod(object):
+    """Class for representing injected method in delegate, context automatically set
+
+    Attributes:
+        method (method): method to be called
+        injected (bool): attribute marking method as injected
+    """
+
+    def __init__(self, method_obj) -> None:
+        self.method = method_obj
+        self.injected = True
+
+    def __call__(self, *args, **kwargs):
+        self.method(*args, **kwargs)
+
+
+class LinkedMethod(object):
+    """Class linking target delegate and method's delegate
+
+    make a cleaner function call in injected method, it's like setting the context automatically
+    This is what actually gets called for the injected method
+
+    Attributes:
+        _obj_delegate (delegate):
+            delegate method is being linked to
+        _method_delegate (MethodDelegate):
+            the method's delegate
+    """
+
+    def __init__(self, object_delegate: Delegate, method_delegate: Method):
+        self._obj_delegate = object_delegate
+        self._method_delegate = method_delegate
+
+    def __call__(self, on_done=None, *arguments):
+        self._method_delegate.invoke(self._obj_delegate, list(arguments), callback=on_done)
+
+
+def inject_methods(delegate: Delegate, methods: List[MethodID]):
+    """Inject methods into a delegate class
+
+    Idea is to inject a method that is from the server to put int into a delegate.
+    Now it looks like the delegate has an instance method that actually calls what
+    is on the server. Context, is automatically taken care of by the linked method
+
+    Args:
+        delegate (Delegate):
+            identifier for delegate to be modified
+        methods (list):
+            list of method id's to inject
+    """
+
+    # Clear out old injected methods
+    to_remove = []
+    for field, value in delegate:
+        if hasattr(value, "injected"):
+            logging.debug(f"Deleting: {field} in inject methods")
+            to_remove.append(field)
+    for field in to_remove:
+        delattr(delegate, field)
+
+    for method_id in methods:
 
-IDGroup = namedtuple("IDGroup", ["slot", "gen"])
+        # Get method delegate and manipulate name to exclude noo::
+        method = delegate.client.get_delegate(method_id)
+        if "noo::" in method.name:
+            name = method.name[5:]
+        else:
+            name = method.name
 
+        # Create injected by linking delegates, and creating call method
+        linked = LinkedMethod(delegate, method)
+        injected = InjectedMethod(linked.__call__)
+
+        setattr(delegate, name, injected)
+
+
+def inject_signals(delegate: Delegate, signals: List[SignalID]):
+    """Method to inject signals into delegate
+
+    Args:
+        delegate (delegate):
+            delegate object to be injected
+        signals (list):
+            list of signal id's to be injected
+    """
 
-class ID(IDGroup):
+    for signal_id in signals:
+        signal = delegate.client.state[signal_id]  # refactored state
+        delegate.signals[signal.name] = None
 
-    __slots__ = ()
 
-    def __repr__(self):
-        return f"{self.__class__}|{self.slot}/{self.gen}|"
+def get_context(delegate):
+    """Helper to get context from delegate"""
+
+    if isinstance(delegate, Entity):
+        return {"entity": delegate.id}
+    elif isinstance(delegate, Table):
+        return {"table": delegate.id}
+    elif isinstance(delegate, Plot):
+        return {"plot": delegate.id}
+    else:
+        return None
+
+
+""" =============================== ID's ============================= """
+
+
+class ID(NamedTuple):
+    slot: int
+    gen: int
+
+    def compact_str(self):
+        return f"|{self.slot}/{self.gen}|"
+
+    def __str__(self):
+        return f"{type(self).__name__}{self.compact_str()}"
 
     def __key(self):
         return type(self), self.slot, self.gen
 
-    def __eq__(self, __o: object) -> bool:
-        if isinstance(__o, ID):
-            return self.__key() == __o.__key()
+    def __eq__(self, other: object) -> bool:
+        if type(other) is type(self):
+            return self.__key() == other.__key()
         else:
             return False
 
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
     def __hash__(self):
         return hash(self.__key())
 
 
 class MethodID(ID):
     pass
 
@@ -103,40 +210,33 @@
         """Configuration for Validation"""
 
         arbitrary_types_allowed = True
         use_enum_values = True
         extra = Extra.allow  # Allow injected methods
 
 
-class Component(NoodleObject):
-    """Parent class for all components"""
-
-    id: ID = None
-
-    def __repr__(self):
-        return f"{type(self)} | {self.id}"
-
-
 class Delegate(NoodleObject):
     """Parent class for all delegates
     
     Defines general methods that should be available for all delegates
     
     Attributes:
         client (Client): Client delegate is attached to
+        id: (ID): Unique identifier for delegate
+        name (str): Name of delegate
         signals (dict): Signals that can be called on delegate, method name to callable
     """
 
     client: object = None
     id: ID = None
-    name: Optional[str] = "No-Name Delegate"
+    name: Optional[str] = "No-Name"
     signals: Optional[dict] = {}
 
-    def __repr__(self):
-        return f"{self.name} | {type(self)} | {self.id}"
+    def __str__(self):
+        return f"{self.name} - {type(self).__name__} - {self.id.compact_str()}"
 
     # For all except Document Delegate
     def on_new(self, message: dict):
         pass
 
     # For Document, Table, Entity, Plot, Material, Light Delegates
     def on_update(self, message: dict):
@@ -177,29 +277,58 @@
     vec2 = "VEC2"
     vec3 = "VEC3"
     vec4 = "VEC4"
     mat3 = "MAT3"
     mat4 = "MAT4"
 
 
+class IndexFormat(str, Enum):
+    u8 = "U8"
+    u16 = "U16"
+    u32 = "U32"
+
+
 class PrimitiveType(Enum):
     points = "POINTS"
     lines = "LINES"
     line_loop = "LINE_LOOP"
     line_strip = "LINE_STRIP"
     triangles = "TRIANGLES"
     triangle_strip = "TRIANGLE_STRIP"
 
 
+class ColumnType(str, Enum):
+    text = "TEXT"
+    real = "REAL"
+    integer = "INTEGER"
+
+
+class BufferType(str, Enum):
+    unknown = "UNK"
+    geometry = "GEOMETRY"
+    image = "IMAGE"
+
+
 class SamplerMode(Enum):
     clamp_to_edge = "CLAMP_TO_EDGE"
     mirrored_repeat = "MIRRORED_REPEAT"
     repeat = "REPEAT"
 
 
+class MagFilterTypes(Enum):
+    nearest = "NEAREST"
+    linear = "LINEAR"
+
+
+class MinFilterTypes(Enum):
+    nearest = "NEAREST"
+    linear = "LINEAR"
+    linear_mipmap_linear = "LINEAR_MIPMAP_LINEAR"
+
+
 class SelectionRange(NoodleObject):
     key_from_inclusive: int
     key_to_exclusive: int
 
 
 class Selection(NoodleObject):
     name: str
@@ -254,18 +383,18 @@
     base_color: Optional[Color] = Color('white')
     base_color_texture: Optional[TextureRef] = None  # assume SRGB, no premult alpha
 
     metallic: Optional[float] = 1.0
     roughness: Optional[float] = 1.0
     metal_rough_texture: Optional[TextureRef] = None  # assume linear, ONLY RG used
 
-    @validator("base_color", pre=True)
-    def check_color(cls, value):
+    @validator("base_color", pre=True, allow_reuse=True)
+    def check_color_rgba(cls, value):
 
-        # Raise warning if format is wrong
+        # Raise warning if format is wrong from server
         if len(value) != 4:
             logging.warning(f"Base Color is Wrong Color Format: {value}")
         return value
 
 
 class PointLight(NoodleObject):
     range: float = -1.0
@@ -294,15 +423,15 @@
 
 
 class Index(NoodleObject):
     view: BufferViewID
     count: int
     offset: Optional[int] = 0
     stride: Optional[int] = 0
-    format: Literal["U8", "U16", "U32"]
+    format: IndexFormat
 
 
 class GeometryPatch(NoodleObject):
     attributes: List[Attribute]
     vertex_count: int
     indices: Optional[Index] = None
     type: PrimitiveType
@@ -327,21 +456,21 @@
             raise ValueError("No field provided")
         else:
             return values
 
 
 class TableColumnInfo(NoodleObject):
     name: str
-    type: Literal["TEXT", "REAL", "INTEGER"]
+    type: ColumnType
 
 
 class TableInitData(NoodleObject):
     columns: List[TableColumnInfo]
     keys: List[int]
-    data: List[List[Union[float, int, str]]]
+    data: List[List[Any]]  # Originally tried union, but currently order is used to coerce by pydantic
     selections: Optional[List[Selection]] = None
 
     # too much overhead? - strict mode
     @root_validator
     def types_match(cls, values):
         for row in values['data']:
             for col, i in zip(values['columns'], range(len(row))):
@@ -379,20 +508,20 @@
         if isinstance(on_delegate, Table):
             kind = "table"
         elif isinstance(on_delegate, Plot):
             kind = "plot"
         elif isinstance(on_delegate, Entity):
             kind = "entity"
         else:
-            raise Exception("Invalid delegate context")
+            raise ValueError("Invalid delegate context")
 
         context = {kind: on_delegate.id}
         self.client.invoke_method(self.id, args, context=context, on_done=callback)
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         """Custom string representation for methods"""
 
         rep = f"{self.name}:\n\t{self.doc}\n\tReturns: {self.return_doc}\n\tArgs:"
         for arg in self.arg_doc:
             rep += f"\n\t\t{arg.name}: {arg.doc}"
         return rep
 
@@ -407,14 +536,15 @@
 class Entity(Delegate):
     id: EntityID
     name: Optional[str] = "Unnamed Entity Delegate"
 
     parent: Optional[EntityID] = None
     transform: Optional[Mat4] = None
 
+    null_rep: Optional[Any] = None
     text_rep: Optional[TextRepresentation] = None
     web_rep: Optional[WebRepresentation] = None
     render_rep: Optional[RenderRepresentation] = None
 
     lights: Optional[List[LightID]] = None
     tables: Optional[List[TableID]] = None
     plots: Optional[List[PlotID]] = None
@@ -423,19 +553,24 @@
     signals_list: Optional[List[SignalID]] = None
 
     influence: Optional[BoundingBox] = None
 
     def show_methods(self):
         """Show methods available on the entity"""
 
-        print(f"-- Methods on {self.name} --")
-        print("--------------------------------------")
-        for method_id in self.methods_list:
-            method = self.client.get_component(method_id)
-            print(f">> {method}")
+        if self.methods_list is None:
+            message = "No methods available"
+        else:
+            message = f"-- Methods on {self.name} --\n--------------------------------------\n"
+            for method_id in self.methods_list:
+                method = self.client.get_delegate(method_id)
+                message += f">> {method}"
+
+        print(message)
+        return message
 
 
 class Plot(Delegate):
     id: PlotID
     name: Optional[str] = "Unnamed Plot Delegate"
 
     table: Optional[TableID] = None
@@ -452,19 +587,24 @@
             return values
         else:
             raise ValueError("One plot type must be specified")
 
     def show_methods(self):
         """Show methods available on the entity"""
 
-        print(f"-- Methods on {self.name} --")
-        print("--------------------------------------")
-        for method_id in self.methods_list:
-            method = self.client.get_component(method_id)
-            print(f">> {method}")
+        if self.methods_list is None:
+            message = "No methods available"
+        else:
+            message = f"-- Methods on {self.name} --\n--------------------------------------\n"
+            for method_id in self.methods_list:
+                method = self.client.get_delegate(method_id)
+                message += f">> {method}"
+
+        print(message)
+        return message
 
 
 class Buffer(Delegate):
     id: BufferID
     name: Optional[str] = "Unnamed Buffer Delegate"
     size: int = None
 
@@ -480,27 +620,27 @@
 
 
 class BufferView(Delegate):
     id: BufferViewID
     name: Optional[str] = "Unnamed Buffer-View Delegate"
     source_buffer: BufferID
 
-    type: Literal["UNK", "GEOMETRY", "IMAGE"] = "UNK"
+    type: BufferType = BufferType.unknown
     offset: int
     length: int
 
     @validator("type", pre=True)
     def coerce_type(cls, value):
         if value in ["UNK", "GEOMETRY", "IMAGE"]:
             return value
 
         logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'UNK'")
-        if "GEOMETRY" in value:
+        if "GEOMETRY" in value.upper():
             return "GEOMETRY"
-        elif "IMAGE" in value:
+        elif "IMAGE" in value.upper():
             return "IMAGE"
         else:
             return "UNK"
 
 
 class Material(Delegate):
     id: MaterialID
@@ -543,16 +683,16 @@
     sampler: Optional[SamplerID] = None
 
 
 class Sampler(Delegate):
     id: SamplerID
     name: Optional[str] = "Unnamed Sampler Delegate"
 
-    mag_filter: Optional[Literal["NEAREST", "LINEAR"]] = "LINEAR"
-    min_filter: Optional[Literal["NEAREST", "LINEAR", "LINEAR_MIPMAP_LINEAR"]] = "LINEAR_MIPMAP_LINEAR"
+    mag_filter: Optional[MagFilterTypes] = MagFilterTypes.linear
+    min_filter: Optional[MinFilterTypes] = MinFilterTypes.linear_mipmap_linear
 
     wrap_s: Optional[SamplerMode] = "REPEAT"
     wrap_t: Optional[SamplerMode] = "REPEAT"
 
 
 class Light(Delegate):
     id: LightID
@@ -561,20 +701,20 @@
     color: Optional[Color] = Color('white')
     intensity: Optional[float] = 1.0
 
     point: PointLight = None
     spot: SpotLight = None
     directional: DirectionalLight = None
 
-    @validator("color", pre=True)
-    def check_color(cls, value):
+    @validator("color", pre=True, allow_reuse=True)
+    def check_color_rgb(cls, value):
 
         # Raise warning if format is wrong
         if len(value) != 3:
-            logging.warning(f"Color is Wrong Color Format in Light: {value}")
+            logging.warning(f"Color is not RGB in Light: {value}")
 
         return value
 
     @root_validator
     def one_of(cls, values):
         already_found = False
         for field in ['point', 'spot', 'directional']:
@@ -620,79 +760,82 @@
     tbl_clear: InjectedMethod = None
     tbl_update_selection: InjectedMethod = None
 
     def __init__(self, **kwargs):
         """Override init to link default values with methods"""
         super().__init__(**kwargs)
         self.signals = {
-            "tbl_reset": self._reset_table,
-            "tbl_rows_removed": self._remove_rows,
-            "tbl_updated": self._update_rows,
-            "tbl_selection_updated": self._update_selection
+            "noo::tbl_reset": self._reset_table,
+            "noo::tbl_rows_removed": self._remove_rows,
+            "noo::tbl_updated": self._update_rows,
+            "noo::tbl_selection_updated": self._update_selection
         }
 
     def _on_table_init(self, init_info: dict, on_done=None):
         """Creates table from server response info
 
         Args:
             init_info (Message Obj): 
                 Server response to subscribe which has columns, keys, data, 
                 and possibly selections
         """
 
-        # Extract data from init info and transpose rows to cols
-        row_data = init_info["data"]
-        cols = init_info["columns"]
-        logging.debug(f"Table Initialized with cols: {cols} and row data: {row_data}")
+        init = TableInitData(**init_info)
+        logging.info(f"Table Initialized with cols: {init.columns} and row data: {init.data}")
+        if on_done:
+            on_done()
 
-    def _reset_table(self):
+    def _reset_table(self, init_info: dict = None):
         """Reset dataframe and selections to blank objects
 
         Method is linked to 'tbl_reset' signal
         """
 
         self.selections = {}
+        if init_info:
+            init = TableInitData(**init_info)
+            logging.info(f"Table Reset and Initialized with cols: {init.columns} and row data: {init.data}")
 
-    def _remove_rows(self, key_list: List[int]):
+    def _remove_rows(self, keys: List[int]):
         """Removes rows from table
 
         Method is linked to 'tbl_rows_removed' signal
 
         Args:
-            key_list (list): list of keys corresponding to rows to be removed
+            keys (list): list of keys corresponding to rows to be removed
         """
 
-        logging.debug(f"Removed Rows: {key_list}...\n")
+        logging.info(f"Removed Rows: {keys}...\n")
 
     def _update_rows(self, keys: List[int], rows: list):
         """Update rows in table
 
         Method is linked to 'tbl_updated' signal
 
         Args:
             keys (list): 
                 list of keys to update
             rows (list):
                 list of rows containing the values for each new row
         """
 
-        logging.debug(f"Updated Rows...{keys}\n")
+        logging.info(f"Updated Rows...{keys}\n")
 
-    def _update_selection(self, selection_obj: Selection):
+    def _update_selection(self, selection: dict):
         """Change selection in delegate's state to new selection object
 
         Method is linked to 'tbl_selection_updated' signal
 
         Args:
-            selection_obj (Selection): 
+            selection (Selection): 
                 obj with new selections to replace obj with same name
         """
 
-        self.selections[selection_obj.name] = selection_obj
-        logging.debug(f"Made selection {selection_obj.name} = {selection_obj}")
+        self.selections.setdefault(selection["name"], selection)
+        logging.info(f"Made selection {selection['name']} = {selection}")
 
     def relink_signals(self):
         """Relink the signals for built-in methods
 
         These should always be linked, along with whatever is injected,
         so relink on new and on update messages
         """
@@ -743,16 +886,16 @@
         Raises:
             Exception: Could not subscribe to table
         """
 
         try:
             # Allow for callback after table init
             self.tbl_subscribe(on_done=lambda data: self._on_table_init(data, on_done))
-        except Exception:
-            raise Exception("Could not subscribe to table")
+        except Exception as e:
+            raise Exception(f"Could not subscribe to table {self.id}...{e}")
 
     def request_insert(self, row_list: List[List[int]], on_done=None):
         """Add rows to end of table
 
         User endpoint for interacting with table and invoking method
         For input, row list is list of rows. Also note that tables have
         nine columns by default (x, y, z, r, g, b, sx, sy, sz).
@@ -820,52 +963,62 @@
             name (str):
                 name of the selection object to be updated
             keys (list):
                 list of keys to be in new selection
             on_done (function, optional): 
                 callback function called when complete
         """
-
-        self.tbl_update_selection(on_done, name, {"rows": keys})
+        selection = Selection(name=name, rows=keys)
+        self.tbl_update_selection(on_done, selection.dict())
 
     def show_methods(self):
         """Show methods available on the table"""
 
-        print(f"-- Methods on {self.name} --")
-        print("--------------------------------------")
-        for method_id in self.methods_list:
-            method = self.client.get_component(method_id)
-            print(f">> {method}")
+        if self.methods_list is None:
+            message = "No methods available"
+        else:
+            message = f"-- Methods on {self.name} --\n--------------------------------------\n"
+            for method_id in self.methods_list:
+                method = self.client.get_delegate(method_id)
+                message += f">> {method}"
+
+        print(message)
+        return message
 
 
 class Document(Delegate):
     name: str = "Document"
 
-    methods_list: List[MethodID] = []
+    methods_list: List[MethodID] = []  # Server usually sends as an update
     signals_list: List[SignalID] = []
 
     def on_update(self, message: dict):
         if "methods_list" in message:
             self.methods_list = [MethodID(*element) for element in message["methods_list"]]
         if "signals_list" in message:
             self.signals_list = [SignalID(*element) for element in message["signals_list"]]
 
     def reset(self):
-        self.client.state = {}
+        self.client.state = {"document": self}
         self.methods_list = []
         self.signals_list = []
 
     def show_methods(self):
         """Show methods available on the document"""
 
-        print(f"-- Methods on Document --")
-        print("--------------------------------------")
-        for method_id in self.methods_list:
-            method = self.client.get_component(method_id)
-            print(f">> {method}")
+        if not self.methods_list:
+            message = "No methods available"
+        else:
+            message = f"-- Methods on Document --\n--------------------------------------\n"
+            for method_id in self.methods_list:
+                method = self.client.get_delegate(method_id)
+                message += f">> {method}"
+
+        print(message)
+        return message
 
 
 """ ====================== Communication Objects ====================== """
 
 
 class Invoke(NoodleObject):
     id: SignalID
@@ -886,31 +1039,30 @@
     result: Optional[Any] = None
     method_exception: Optional[MethodException] = None
 
 
 """ ====================== Miscellaneous Objects ====================== """
 
 default_delegates = {
-    "entities": Entity,
-    "tables": Table,
-    "plots": Plot,
-    "signals": Signal,
-    "methods": Method,
-    "materials": Material,
-    "geometries": Geometry,
-    "lights": Light,
-    "images": Image,
-    "textures": Texture,
-    "samplers": Sampler,
-    "buffers": Buffer,
-    "bufferviews": BufferView,
-    "document": Document
+    Entity: Entity,
+    Table: Table,
+    Plot: Plot,
+    Signal: Signal,
+    Method: Method,
+    Material: Material,
+    Geometry: Geometry,
+    Light: Light,
+    Image: Image,
+    Texture: Texture,
+    Sampler: Sampler,
+    Buffer: Buffer,
+    BufferView: BufferView,
+    Document: Document
 }
 
-
 id_map = {
     Method: MethodID,
     Signal: SignalID,
     Table: TableID,
     Plot: PlotID,
     Entity: EntityID,
     Material: MaterialID,
@@ -919,106 +1071,7 @@
     Image: ImageID,
     Texture: TextureID,
     Sampler: SamplerID,
     Buffer: BufferID,
     BufferView: BufferViewID,
     Document: None
 }
-
-
-class InjectedMethod(object):
-    """Class for representing injected method in delegate, context automatically set
-
-    Attributes:
-        method (method): method to be called
-        injected (bool): attribute marking method as injected
-    """
-
-    def __init__(self, method_obj) -> None:
-        self.method = method_obj
-        self.injected = True
-
-    def __call__(self, *args, **kwargs):
-        self.method(*args, **kwargs)
-
-
-class LinkedMethod(object):
-    """Class linking target delegate and method's delegate 
-        
-    make a cleaner function call in injected method, its like setting the context automatically
-    This is what actually gets called for the injected method
-
-    Attributes:
-        _obj_delegate (delegate): 
-            delegate method is being linked to
-        _method_delegate (MethodDelegate): 
-            the method's delegate 
-    """
-
-    def __init__(self, object_delegate: Delegate, method_delegate: Method):
-        self._obj_delegate = object_delegate
-        self._method_delegate = method_delegate
-
-    def __call__(self, on_done=None, *arguments):
-        self._method_delegate.invoke(self._obj_delegate, arguments, callback=on_done)
-
-
-def inject_methods(delegate: Delegate, methods: List[MethodID]):
-    """Inject methods into a delegate class
-
-    Idea is to inject a method that is from the server to put int into a delegate.
-    Now it looks like the delegate has an instance method that actually calls what
-    is on the server. Context, is automatically taken care of by the linked method
-
-    Args:
-        delegate (Delegate):
-            identifier for delegate to be modified
-        methods (list): 
-            list of method id's to inject
-    """
-
-    # Clear out old injected methods
-    for field, value in delegate:
-        if hasattr(value, "injected"):
-            logging.debug(f"Deleting: {field} in inject methods")
-            delattr(delegate, field)
-
-    for method_id in methods:
-
-        # Get method delegate and manipulate name to exclude noo::
-        method = delegate.client.state[method_id]
-        name = method.name[5:]
-
-        # Create injected by linking delegates, and creating call method
-        linked = LinkedMethod(delegate, method)
-        injected = InjectedMethod(linked.__call__)
-
-        setattr(delegate, name, injected)
-
-
-def inject_signals(delegate: Delegate, signals: List[SignalID]):
-    """Method to inject signals into delegate
-
-    Args:
-        delegate (delegate): 
-            delegate object to be injected 
-        signals (list): 
-            list of signal id's to be injected
-    """
-
-    for signal_id in signals:
-        signal = delegate.client.state[signal_id]  # refactored state
-        delegate.signals[signal.name] = None
-
-
-def get_context(delegate):
-    """Helper to get context from delegate"""
-
-    if isinstance(delegate, Entity):
-        return {"entity": delegate.id}
-    elif isinstance(delegate, Table):
-        return {"table": delegate.id}
-    elif isinstance(delegate, Plot):
-        return {"plot": delegate.id}
-    else:
-        return None
-
```

### Comparing `penne-0.4.0/penne/handlers.py` & `penne-0.5.0/penne/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """Module for Handling Raw Messages from the Server"""
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any
-if TYPE_CHECKING:
-    from penne.core import Client
+from typing import Any
 
 import weakref
 import warnings
 import logging
 from pydantic import ValidationError
 
-from penne.delegates import Delegate, id_map, default_delegates
-from penne.delegates import TableID, PlotID, EntityID, ID
+from penne.delegates import Delegate, Document, id_map
+from penne.delegates import ID
 
 
 # Helper Methods
 def update_state(client, message: dict, component_id: ID):
     """Update a delegate in the current state
 
     Args:
@@ -23,53 +21,23 @@
             client to be updated
         message (Message): 
             message containing updates
         component_id (ID):
             ID of the component to be updated
     """
 
-    current_state = client.state[component_id].dict()
+    delegate = client.get_delegate(component_id)
+    current_state = delegate.dict()
     current_state.update(message)
 
-    delegate_type = type(client.state[component_id])
+    delegate_type = type(delegate)
     client.state[component_id] = delegate_type(**current_state)
 
 
-def delegate_from_context(client: Client, context: dict) -> Delegate:
-    """Get delegate object from a context message object
-    
-    Args:
-        client (Client): client to get delegate from
-        context (Message): object containing context
-    
-    Raises:
-        Exception: Couldn't get delegate from context
-    """
-
-    if not context:
-        target_delegate = client.state["document"]
-        return target_delegate
-
-    table = context.get("table")
-    entity = context.get("entity")
-    plot = context.get("plot")
-
-    if table:
-        target_delegate = client.state[TableID(*table)]
-    elif hasattr(context, "entity"):
-        target_delegate = client.state[EntityID(*entity)]
-    elif hasattr(context, "plot"):
-        target_delegate = client.state[PlotID(*plot)]
-    else:
-        raise Exception("Couldn't get delegate from context")
-    
-    return target_delegate
-
-
-def handle(client: Client, message_id, message: dict[str, Any]):
+def handle(client, message_id, message: dict[str, Any]):
     """Handle message from server
 
     'Handle' uses the ID attached to message to get handling info, and uses this info 
     to take proper course of action with message. The function has 5 main sections 
     handling create, delete, and update messages along with signal invocation and reply
     messages.
 
@@ -82,53 +50,51 @@
         message_id (int): id mapping to handle info in client
         message (dict): dict with the message's contents
     """
     
     # Process message using ID from dict
     handle_info = client.server_messages[message_id]
     action = handle_info.action
-    specifier = handle_info.specifier
-    id_type = id_map[default_delegates[specifier]]
-    logging.debug(f"Received Message: {action} {specifier} {message}")
+    delegate_type = handle_info.delegate
+    id_type = id_map[delegate_type]
+    logging.debug(f"Received Message: {action} {delegate_type} {message}")
 
     # Update state based on map info
     if action == "create":
 
         # Create instance of delegate
         reference = weakref.ref(client)
         reference_obj = reference()
         try:
-            delegate: Delegate = client.delegates[specifier](client=reference_obj, **message)
+            delegate: Delegate = client.delegates[delegate_type](client=reference_obj, **message)
             delegate.client = client
             client.state[delegate.id] = delegate
             delegate.on_new(message)
         except ValidationError as e:
 
             warnings.warn(str(e))
 
             if client.strict:
-                raise Exception(f"Could not Create Delegate of type {specifier}")
+                raise Exception(f"Could not Create Delegate of type {delegate_type}")
     
     elif action == "delete":
-        
-        component_id = id_type(*message["id"])
-        state_delegate: Delegate = client.state[component_id]
 
         # Update delegate and state
-        state_delegate.on_remove(message)
-        del state_delegate
+        component_id = id_type(*message["id"])
+        client.state[component_id].on_remove(message)
+        del client.state[component_id]
 
     elif action == "update":
 
-        if specifier != "document":
+        if delegate_type != Document:
             component_id = id_type(*message["id"])
             update_state(client, message, component_id)
             client.state[component_id].on_update(message)
         else:
-            client.state[specifier].on_update(message)
+            client.state["document"].on_update(message)
 
     elif action == "reply":
 
         # Handle callback functions
         exception = message.get("method_exception", False)
         invoke_id = message.get("invoke_id")
         result = message.get("result")
@@ -147,22 +113,26 @@
         # Handle invoke message from server
         signal_data = message["signal_data"]
         signal_id = id_type(*message["id"])
         signal: Delegate = client.state[signal_id]
 
         # Determine the delegate the signal is being invoked on
         context = message.get("context")
-        target_delegate = delegate_from_context(client, context)
+        target_delegate = client.get_delegate_by_context(context)
 
         # Invoke signal attached to target delegate
         logging.debug(f"Invoking {signal.name} w/ args: {signal_data}")
         target_delegate.signals[signal.name](*signal_data)
 
     elif action == "initialized":
 
+        # Set flag that lets context manager start up
+        client.connection_established.set()
+
+        # Start callback if it exists
         if client.on_connected:
             client.callback_queue.put((client.on_connected, None))
 
     else:
         # Document reset messages
         client.state["document"].reset()
         logging.debug("Document Reset")
```

### Comparing `penne-0.4.0/pyproject.toml` & `penne-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "pytest",
     "rigatoni",
     "pandas",
     "matplotlib"
 ]
 
 [project.urls]
-Source = "https://github.com/InsightCenterNoodles/penne"
+Source = "https://github.com/InsightCenterNoodles/Penne"
```

### Comparing `penne-0.4.0/PKG-INFO` & `penne-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penne
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python Client Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,client,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -12,96 +12,139 @@
 Requires-Dist: websockets
 Requires-Dist: cbor2
 Requires-Dist: pydantic
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: rigatoni ; extra == "testing"
 Requires-Dist: pandas ; extra == "testing"
 Requires-Dist: matplotlib ; extra == "testing"
-Project-URL: Source, https://github.com/InsightCenterNoodles/penne
+Project-URL: Source, https://github.com/InsightCenterNoodles/Penne
 Provides-Extra: testing
 
 # PENNE
 
 ![Build Status](https://github.com/InsightCenterNoodles/Penne/workflows/CI/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/Penne)
-![Coverage](tests/coverage/coverage.svg)
-![Coverage](https://github.com/InsightCenterNoodles/Penne/raw/aebac0f/coverage-badge/coverage.svg)
+[![Coverage badge](https://raw.githubusercontent.com/InsightCenterNoodles/Penne/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Penne/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 
 Python Client for NOODLES protocol  
 (Python Encoded Native NOODLES Endpoint)
 
 ## Description
 The client library is based on the NOODLES messaging protocol for communicating with serverside data visualisation applications. The client uses a websocket connection to send CBOR encoded messages. To customize its implementation, the
-library offers hooks in the form of delegates classes which can be extended and overwritten.
+library offers hooks in the form of delegates classes which can be extended.
 
 ## How does the client work?
 When a message is received from the server, the client passes the CBOR encoded message to a handler function which uses
 the message's ID to process it accordingly. Based on this ID, the message can be classified as either a create, delete, 
 update, reply, or invoke message. Upon receiving a create message, the handler creates a new delegate for that object
-which is then stored in the client's state. Delete and update messages manipulate delegates in the client's state as expected. Reply messages indicate whether a method was invoked on the server successfully, and then a callback function can be executed if applicable. Lastly, invoke messages represent signals from the server which are being called on a delegate. The handler essentially sends this signal to the target delgate so it can call a corresponding function. 
-
-To send a message, the user calls a method on a delegate. This method wraps an injected method from the server, and the client can send a message invoking the method.
+which is then stored in the client's state. Delete and update messages manipulate delegates in the client's state as expected. 
+Reply messages indicate whether a method was invoked on the server successfully, and then a callback function can be 
+executed if applicable. Lastly, invoke messages represent signals from the server which are being called on a delegate. 
+The handler sends this signal to the target delegate so it can call a corresponding function. 
+
+To send a message, the user calls a method on a delegate or the document more broadly. Delegates may have injected 
+methods from the server, and the client can send a message invoking the method. For example, the server can define a
+method like insert_row() on a table delegate. The client can then call this method on the delegate, and the server will
+get a message requesting to invoke the method. The server will then respond by updating the state, invoking signals, 
+and sending a reply message to the client. If the server is unable to invoke the method, it will send a reply message
+that contains an exception.
 
 A diagram representing the simplified relationships between the client, server, and delegates is depicted below. 
 
 ```mermaid
-flowchart LR;
-    User-- Request to Invoke Method -->Delegate;
-    User-- Create Custom Delegates --> Client;
-    User-- Create New Plot --> Client;
-    Delegate-- Call Injected Method -->Client;
-    Client-- Send Invoke Method Message -->Server;
-    Server-- Message -->Client;
-    Client-- Create w/ Injection -->Delegate;
-    Client-- Update -->Delegate;
-    Client-- Invoke Signal -->Delegate;
-    Delegate-- Show current state -->User;
+sequenceDiagram
+    participant User
+    participant Delegate
+    participant Client
+    participant Server
+    User->>Delegate: Create Custom Delegates
+    User->>Client: Starts Server with Custom Delegates
+    Client->>Server: Sends Intro Message
+    Server->>Client: Updates the Client with Current State
+    loop until end of session
+        User->>Delegate: Invoke Injected or Custom Method on Delegate or...
+        User->>Client: Invoke Method on Client Directly
+        Client->>Server: Request to Invoke Method
+        Server->>Client: Responds to Update State
+        Client->>Delegate: Invokes Signals, Creates, Updates, and Deletes Delegates
+        Client->>User: Show Current State
+    end
 ```
 
 ## Working with delegates
 >What are delegates? 
 
-NOODLES messages deal with many different objects ranging from tables and plots to lights and materials. To help with 
+NOODLES messages deal with many objects ranging from tables and plots to lights and materials. To help with 
 using these objects, each type has its own delegate class. Each object in a scene corresponds with an instance of a delegate
-which is stored in the client's state. Delegates provide methods specific to each type of object.
-
-Note: PENNE currently offers support primarily for the table delegate class
+which is stored in the client's state. Delegates provide methods specific to each type of object. These objects can contain 
+injected methods and signals from the server. All delegates come with methods `on_new()`, `on_update()`, and `on_remove()`
+which are called automatically when the server sends a message to create, update, or delete an object.
 
 >How can I use custom delegates?
 
-To work with your own delegates, use a custom delegate hash as an argument in `create_client()`. To overide a default
-delegate, use the same key in your dictionary. The library also provides a generic `Delegate` class that
-should be used as the parent class for any delegate. An example of a custom delegate is included in `test_client.py`. Here, the delegate class inherits from `TableDelegate` and uses the pandas library to add table and plotting functionality. 
+To work with your own delegates, simply create a class that inherits from the base delegate. Then, pass a dictionary as
+an argument to the constructor that maps the delegate's type to the new class. In `tests/clients.py` there is a more
+involved example that extends the table delegate. Here, the delegate class 
+inherits from `Table` and uses pandas and matplotlib to add plotting functionality. Below is an even more basic example
+that prints a message whenever a new method is created.
+
+```python
+from penne import Method, Client
+
+
+class CustomMethod(Method):
+  
+  def on_new(self, message: dict):
+    print(f"New method named {self.name} was created")
+    
+      
+with Client(address, {Method: CustomMethod}) as client:
+  # do stuff
+
+```
 
 >How do you call methods on a delegate?
 
 Once instantiated, delegates are injected with methods designated by the server. These methods can be called by using
 public methods on the delegate that essentially wrap the injected ones. Once the method is invoked, the server will 
 respond with a signal that updates the client. Each signal is linked to a method in the delegate which keeps the state of 
 the client up to date. To customize the client's behavior, these methods can be overwritten in a custom delegate. Each 
-public method also accepts a callback function to be executed once a response is received from the server. This way, method calls can be chained together and run in sequence. An example is provided in `test_client.py`.
+public method also accepts a callback function to be executed once a response is received from the server. 
+This way, method calls can be chained together and run in sequence. An example is provided in `tests/plottyn_integration.py`.
 
 ### Tables
 The table delegate comes with several built in methods covering basic table manipulation. The delegate includes...
 ```python
-request_insert(col_list: list=None, row_list: list=None, on_done=None)
+subscribe(on_done=None)
+request_insert(row_list: list=None, on_done=None)
 request_remove(keys: list, on_done=None)
-request_update(data_frame: pandas.DataFrame, on_done=None)
+request_update(keys: List[int], rows: List[List[int]], on_done=None)
 request_clear(on_done=None)
 request_update_selection(name: str, keys: list, on_done=None)
 ```
-Once invoked, signals from the server will update the table in the delegate. When using these methods, the user has the option of including a callback function that will execute once complete.
+When using these methods, the user has the option of including a callback function (on_done) that will execute once complete.
+Once invoked, signals from the server will update the table in the delegate. For the table thereare several signals that
+can be overwritten in a custom delegate. While you can inherit and customize them for your specif implementation of the
+table, they should not be called directly by users. They will be called when indicated by a message from the server. 
+These include...
+```python
+_on_table_init(init_info: dict, on_done=None)
+_reset_table(init_info: dict)
+_remove_rows(keys: list[int])
+_update_rows(keys: list[int], rows: list[list])
+_update_selection(selection: dict)
+```
 
 ## Getting Started
 1. Install the library
 ```python
 pip install penne
 ```
-2. Create a client using `create_client(address, delegate_hash)`
+2. Create a client using 
 ```python
 from penne import Client
 
 with Client(address, delegate_hash) as client:
     # do stuff
 ```
 - (Optional) use delegate hash to map custom delegates
```

