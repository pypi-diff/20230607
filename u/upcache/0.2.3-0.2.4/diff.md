# Comparing `tmp/upcache-0.2.3-py3-none-any.whl.zip` & `tmp/upcache-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 14701 bytes, number of entries: 15
+Zip file size: 16101 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      195 b- defN 22-Dec-17 00:21 upcache/__init__.py
 -rw-r--r--  2.0 unx     3459 b- defN 22-Dec-04 03:59 upcache/cache.py
 -rw-r--r--  2.0 unx      542 b- defN 22-Dec-04 21:48 upcache/daemon.py
 -rw-r--r--  2.0 unx      783 b- defN 22-Dec-04 13:39 upcache/errors.py
 -rw-r--r--  2.0 unx     5355 b- defN 22-Dec-18 03:14 upcache/helpers.py
 -rw-r--r--  2.0 unx       72 b- defN 22-Dec-04 20:34 upcache/networking.py
 -rw-r--r--  2.0 unx      630 b- defN 22-Dec-18 02:01 upcache/server.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-04 20:12 upcache/internal/__init__.py
--rw-r--r--  2.0 unx     6013 b- defN 22-Dec-17 19:08 upcache/internal/cache.py
+-rw-r--r--  2.0 unx     5980 b- defN 23-Jun-07 15:17 upcache/internal/cache.py
 -rw-r--r--  2.0 unx      783 b- defN 22-Dec-04 13:39 upcache/internal/errors.py
--rw-r--r--  2.0 unx    27310 b- defN 22-Dec-18 03:19 upcache/internal/tcp.py
--rw-r--r--  2.0 unx     2970 b- defN 22-Dec-18 03:22 upcache-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-18 03:22 upcache-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Dec-18 03:22 upcache-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1142 b- defN 22-Dec-18 03:22 upcache-0.2.3.dist-info/RECORD
-15 files, 49354 bytes uncompressed, 12829 bytes compressed:  74.0%
+-rw-r--r--  2.0 unx    36994 b- defN 23-Jun-07 15:26 upcache/internal/tcp.py
+-rw-r--r--  2.0 unx     2970 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/RECORD
+15 files, 59005 bytes uncompressed, 14229 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: upcache/internal/errors.py
 Comment: 
 
 Filename: upcache/internal/tcp.py
 Comment: 
 
-Filename: upcache-0.2.3.dist-info/METADATA
+Filename: upcache-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: upcache-0.2.3.dist-info/WHEEL
+Filename: upcache-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: upcache-0.2.3.dist-info/top_level.txt
+Filename: upcache-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: upcache-0.2.3.dist-info/RECORD
+Filename: upcache-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## upcache/internal/cache.py

```diff
@@ -43,89 +43,88 @@
         Assigns a value to a key.
 
         :param key the key
         :param value the associated value
         """
         with self._data_lock:
             self._data[key] = value
-            self._on_update(key, value)
-            self._last_key = key
-            self._key_event.set()
+        self._on_update(key, value)
+        self._last_key = key
+        self._key_event.set()
 
     def decrement(self, key: bytes) -> bytes:
         """
         Decrements a value associated with a key.
         If the value is not an integer, a value of -1 is assigned.
 
         :param key the key
         :returns decremented value
         """
-        try:
-            with self._data_lock:
-                v = int(self._data.get(key, b'0').decode()) - 1
-        except:
-            v = -1
-        value = str(v).encode()
         with self._data_lock:
+            try:
+                v = int(self._data.get(key, b'0').decode()) - 1
+            except:
+                v = -1
+            value = str(v).encode()
             self._data[key] = value
-            self._on_update(key, value)
-            self._last_key = key
-            self._key_event.set()
+        self._on_update(key, value)
+        self._last_key = key
+        self._key_event.set()
         return value
     
     def increment(self, key: bytes) -> bytes:
         """
         Increments a value associated with a key.
         If the value is not an integer, a value of 1 is assigned.
 
         :param key the key
         :returns incremented value
         """
-        try:
-            with self._data_lock:
-                v = int(self._data.get(key, b'0').decode()) + 1
-        except:
-            v = 1
-        value = str(v).encode()
         with self._data_lock:
+            try:
+                v = int(self._data.get(key, b'0').decode()) + 1
+            except:
+                v = 1
+            value = str(v).encode()
             self._data[key] = value
-            self._on_update(key, value)
-            self._last_key = key
-            self._key_event.set()
+        self._on_update(key, value)
+        self._last_key = key
+        self._key_event.set()
         return value
 
     def clear(self) -> None:
         """
         Clears all keys from the cache.
         """
         with self._data_lock:
             for k in self._data.keys():
                 self._on_update(k, None)
             self._data = {}
-            # NOTE: None indicates all keys were wiped
-            self._last_key = None
-            self._key_event.set()
+        # NOTE: None indicates all keys were wiped
+        self._last_key = None
+        self._key_event.set()
 
     def drop(self, key: bytes) -> bool:
         """
         Drops a key from the cache.
 
         :param key the key
         :returns True if the key was dropped,
                  False if the key does not exist
         """
+        status = False
         with self._data_lock:
             if key in self._data:
                 self._data.pop(key)
-                self._on_update(key, None)
-                self._last_key = key
-                self._key_event.set()
-                return True
-            else:
-                return False
+                status = True
+        if status:
+            self._on_update(key, None)
+            self._last_key = key
+            self._key_event.set()
+        return status
 
     def exists(self, key: bytes) -> bool:
         """
         Determines if a key exists within the
         cache.
 
         :param key the key
@@ -142,14 +141,15 @@
         :param value wait for associated value
         :param timeout optional timeout
         :returns True if an event for the key fired,
                  False if the cache is closed
         """
         self._key_event.clear()
         if timeout:
+            # TODO: use time.perf_counter()
             timeout_time = datetime.now() + timeout
             while not self._stopped:
                 now = datetime.now()
                 if timeout_time < now or not self._key_event.wait((timeout_time - now).total_seconds()):
                     return False
                 last_key = self._last_key
                 self._key_event.clear()
```

## upcache/internal/tcp.py

```diff
@@ -1,13 +1,13 @@
 from .cache import Cache
 from .errors import ProtocolError
 from socketserver import BaseRequestHandler, ThreadingTCPServer
 from datetime import timedelta
 from typing import Tuple, List, Optional, Callable, Set, Dict
-from threading import Lock, Thread
+from threading import Lock, Thread, Event
 import atexit
 import os
 import sys
 import json
 import signal
 import socket
 import struct
@@ -26,15 +26,18 @@
 CMD_ALL_KEYS = 10
 CMD_ALL_ITEMS = 11
 CMD_DISCONNECT = 12
 CMD_WAIT_KEY = 13
 CMD_SUB = 14
 CMD_UNSUB = 15
 CMD_NOTIFY_UPDATE = 16
-CMD_NOTIFY_DELETE = 16
+CMD_NOTIFY_DELETE = 17
+CMD_SUB_GLOBAL = 18
+CMD_UNSUB_GLOBAL = 19
+CMD_INTERRUPT = 20
 
 # TCP protocol formatting structs
 _envelope = struct.Struct('II')
 _key_header = struct.Struct('I')
 _key_response = struct.Struct('bI') # exists, length
 _key_value_header = struct.Struct('II')
 _value_response = struct.Struct('I')
@@ -93,14 +96,17 @@
             CMD_DROP_KEY: self._drop_key,
             CMD_COUNT_KEYS: self._count_keys,
             CMD_ALL_KEYS: self._all_keys,
             CMD_ALL_ITEMS: self._all_items,
             CMD_WAIT_KEY: self._wait_key,
             CMD_SUB: self._subscribe,
             CMD_UNSUB: self._unsubscribe,
+            CMD_SUB_GLOBAL: self._subscribe_global,
+            CMD_UNSUB_GLOBAL: self._unsubscribe_global,
+            CMD_INTERRUPT: self._interrupt,
         }
         self._cache_update = Subscriber(self.request)
         self._lock = Lock()
 
     def finish(self) -> None:
         """
         Signals the server that a client disconnected.
@@ -190,14 +196,43 @@
         :returns response
         """
         key_len, = _key_header.unpack(data.read(_key_header.size))
         key = data.read(key_len)
         if len(key) != key_len: raise ProtocolError("length")
         self.server.unsubscribe(key, self._cache_update) # type: ignore[attr-defined]
         return _envelope.pack(MAGIC_WORD, CMD_UNSUB)
+    
+    def _subscribe_global(self, data: SocketReader) -> bytes:
+        """
+        Subscribes to change events for all keys.
+
+        :param data request reader
+        :returns response
+        """
+        self.server.subscribe_all(self._cache_update) # type: ignore[attr-defined]
+        return _envelope.pack(MAGIC_WORD, CMD_SUB_GLOBAL)
+    
+    def _unsubscribe_global(self, data: SocketReader) -> bytes:
+        """
+        Unsubscribes from global change events in the cache.
+
+        :param data request reader
+        :returns response
+        """
+        self.server.unsubscribe_all(self._cache_update) # type: ignore[attr-defined]
+        return _envelope.pack(MAGIC_WORD, CMD_UNSUB_GLOBAL)
+    
+    def _interrupt(self, data: SocketReader) -> bytes:
+        """
+        Generates a "pong" to a "ping" for interrupting a listener thread.
+
+        :param data request reader
+        :returns response
+        """
+        return _envelope.pack(MAGIC_WORD, CMD_INTERRUPT)
 
     def _key_exists(self, data: SocketReader) -> bytes:
         """
         Determines if a key is located in the cache.
 
         :param data request reader
         :returns response
@@ -330,25 +365,26 @@
         """
         Constructs a new Subscriber on top of a socket.
 
         :param socket the socket which will be sent updates
         """
         self._socket = socket
 
-    def on_data(self, data: Optional[bytes]) -> None:
+    def on_data(self, key: bytes, data: Optional[bytes]) -> None:
         """
         Processes updates received from a key-value update
         in the cache.
 
+        :param key key updated
         :param data value bytes to send to socket
         """
         if data:
-            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_NOTIFY_UPDATE) + _value_response.pack(len(data)) + data)
+            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_NOTIFY_UPDATE) + _key_value_header.pack(len(key), len(data)) + key + data)
         else:
-            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_NOTIFY_DELETE))
+            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_NOTIFY_DELETE) + _key_response.pack(len(key)) + key)
 
 class SubscriptionList:
     """
     Maintains a list of subscriptions to a key.
     """
     def __init__(self) -> None:
         """
@@ -381,26 +417,26 @@
         Removes a subscriber from the list.
 
         :param sub subscriber
         """
         with self._lock:
             self._subs.discard(sub)
 
-    def send(self, data: Optional[bytes]) -> None:
+    def send(self, key: bytes, data: Optional[bytes]) -> None:
         """
         Sends a payload to all subscribers.
 
+        :param key key updated
         :param data payload to send
         """
         with self._lock:
             for s in self._subs:
                 try:
-                    s.on_data(data)
+                    s.on_data(key, data)
                 except Exception as e:
-                    print(e)
                     self._remove.append(s)
         if self._remove:
             with self._lock:
                 for item in self._remove:
                     self._subs.discard(item)
             self._remove.clear()
 
@@ -417,25 +453,26 @@
         """
         super().__init__(bind, TCPHandler)
         self.cache = Cache(self._on_cache_update)
         self._auto_kill = auto_kill
         self._num_connected = 0
         self._conn_lock = Lock()
         self._subs : Dict[bytes, SubscriptionList] = {}
+        self._global_subs = SubscriptionList()
 
     def _on_cache_update(self, key: bytes, value: Optional[bytes]) -> None:
         """
         Processes updates to the Cache object.
 
         :param key updated key
         :param value updated value (None to signify deletion)
         """
         subs = self._subs.get(key)
         if subs:
-            subs.send(value)
+            subs.send(key, value)
 
     def subscribe(self, key: bytes, sub: Subscriber) -> None:
         """
         Subscribes to change events associated with a key.
 
         :param key associated key
         :param sub subscriber for receiving updates
@@ -454,14 +491,30 @@
         :param key associated key
         :param sub subscriber to unsubscribe
         """
         subs = self._subs.get(key)
         if subs:
             subs.remove(sub)
             if subs.empty: self._subs.pop(key)
+    
+    def subscribe_all(self, sub: Subscriber) -> None:
+        """
+        Subscribes to all change events.
+
+        :param sub subscriber for receiving updates
+        """
+        self._global_subs.add(sub)
+    
+    def unsubscribe_all(self, sub: Subscriber) -> None:
+        """
+        Unsubscribes a subscriber from all change events.
+
+        :param sub subscriber to unsubscribe
+        """
+        self._global_subs.remove(sub)
 
     def service_actions(self) -> None:
         """
         Processed every loop to determine if the server
         needs to die internally (see auto-kill functionality).
         """
         if self._auto_kill and self._num_connected == 0:
@@ -482,79 +535,265 @@
         with self._conn_lock:
             self._num_connected -= 1
 
 class SubscriptionClient:
     """
     UpCache subscription client
     """
-    def __init__(self, host: str, port: int, key: bytes, callback: Callable[[Optional[bytes]], None]) -> None:
+    def __init__(self, host: str, port: int) -> None:
         """
         Constructs a new TCP-based UpCache client.
 
         :param host TCP host
         :param port TCP port
-        :param calback callback for value updates
         """
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, struct.pack('ii', 1, 0))
         s.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
         s.connect((host, port))
 
-        self._key_header = _key_header.pack(len(key)) + key
+        self._update_event = Event()
+        self._update_event.clear()
+        self._recent_key : Optional[bytes] = None
+
+        self._lock = Lock()
         self._socket = s
-        self._callback = callback
+        self._callbacks : Dict[bytes, Set[Callable[[bytes, Optional[bytes]], None]]] = {}
+        self._global_callbacks : Set[Callable[[bytes, Optional[bytes]], None]] = set()
         self._rd = SocketReader(s, 512)
-        
-        s.sendall(_envelope.pack(MAGIC_WORD, CMD_SUB) + self._key_header)
-        mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
-
+       
         self._process_thread = Thread(target=self._process_incoming)
         self._process_thread.start()
         self._closed = False
 
+    def wait_for_update(self, key: Optional[bytes]) -> bool:
+        """
+        Waits for an update on a specific key to occur.  If no key
+        is specified, it waits for any key to update.
+
+        :returns True if an update occurred, False if the connection
+                 was closed with no update
+        """
+        while True:
+            self._update_event.wait()
+            self._update_event.clear()
+            if self._closed:
+                return False
+            elif key is None or self._recent_key == key:
+                return True
+    
+    def wait_for_close(self) -> None:
+        """
+        Waits for the client to close.
+        """
+        while not self._closed:
+            self._update_event.wait()
+            self._update_event.clear()
+
+    def subscribe(self, key: Optional[bytes], callback: Callable[[bytes, Optional[bytes]], None]) -> None:
+        """
+        Enrolls a subscription callback for a specified key or all events if key is None.
+
+        :param key optional subscription key filter
+        :param callback callback for key-value updates
+        """
+        s = self._socket
+        if key is None:
+            self._global_callbacks.add(callback)
+            with self._lock:
+                s.sendall(_envelope.pack(MAGIC_WORD, CMD_SUB_GLOBAL))
+                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+        else:
+            new_key = False
+            cb_list = self._callbacks.get(key)
+            if cb_list is None:
+                cb_list = set()
+                self._callbacks[key] = cb_list
+                new_key = True
+            cb_list.add(callback)
+            if new_key:
+                with self._lock:
+                    s.sendall(_envelope.pack(MAGIC_WORD, CMD_SUB) + _key_header.pack(len(key)) + key)
+                    #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+
+    def unsubscribe(self, key: Optional[bytes], callback: Callable[[bytes, Optional[bytes]], None]) -> None:
+        """
+        Removes a subscription callback from a specified key subscription list or from all events.
+
+        :param key optional subscription key filter
+        :param callback callback for key-value updates
+        """
+        if key is None:
+            try:
+                self._global_callbacks.remove(callback)
+            except:
+                pass
+            if self._global_callbacks:
+                return
+            with self._lock:
+                self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB_GLOBAL))
+                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+        else:
+            cb_list = self._callbacks.get(key)
+            if cb_list is None:
+                return
+            try:
+                cb_list.remove(callback)
+            except:
+                pass
+            if cb_list:
+                return
+            self._callbacks.pop(key)
+            with self._lock:
+                s.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB) + _key_header.pack(len(key)) + key)
+                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+
+    def _dispatch(self, key: bytes, value: Optional[bytes]) -> None:
+        """
+        Handles dispatching key-value updates to the appropriate callbacks.
+
+        :param key key updated
+        :param value optional value updated (None indicates deletion)
+        """
+
+        # Notify that we have a key-value update
+        self._recent_key = key
+        self._update_event.set()
+
+        for cb in self._global_callbacks:
+            cb(key, value)
+        cb_list = self._callbacks.get(key)
+        if cb_list:
+            for cb in cb_list:
+                cb(key, value)
+
     def _process_incoming(self) -> None:
         """
         Processes incoming updates on a dedicated thread.
         """
         try:
             while True:
+                # Process commands
                 mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
-                if cmd == CMD_NOTIFY_UPDATE:
-                    value_len, = _value_response.unpack(self._rd.read(_value_response.size))
-                    value = self._rd.read(value_len)
-                    self._callback(value)
-                elif cmd == CMD_NOTIFY_DELETE:
-                    self._callback(None)
-                else:
-                    break
+                with self._lock:
+                    if cmd == CMD_NOTIFY_UPDATE:
+                        key_len, value_len = _key_value_header.unpack(self._rd.read(_key_value_header.size))
+                        key = self._rd.read(key_len)
+                        value = self._rd.read(value_len)
+                    elif cmd == CMD_NOTIFY_DELETE:
+                        key_len, = _key_response.unpack(self._rd.read(_key_response.size))
+                        key = self._rd.read(key_len)
+                        value = None
+                    elif cmd == CMD_SUB or cmd == CMD_UNSUB or cmd == CMD_SUB_GLOBAL or cmd == CMD_UNSUB_GLOBAL:
+                        continue
+                    else:
+                        # CMD_INTERRUPT and friends funnel here...
+                        break
+                self._dispatch(key, value)
         except:
             pass
 
     def __del__(self) -> None:
         """
         Handles closure if not directly invoked.
         """
         self.close()
+
+    @property
+    def is_subscribed(self) -> bool:
+        """
+        Returns whether the SubscriptionClient is actively subscribed to any
+        events.
+
+        :returns True if at least one subscription is open
+        """
+        # TODO: check _callbacks here?
+        return len(self._global_callbacks) != 0 or len(self._callbacks) != 0
     
     def close(self) -> None:
         """
         Closes the connection to the TCP server.
         """
         if self._closed: return
 
         # Send unsub which will ACK, so wait for thread to complete
-        self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB) + self._key_header)
+        for k in self._callbacks.keys():
+            with self._lock:
+                self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB) + _key_header.pack(len(k)) + k)
+                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+        self._callbacks.clear()
+        if self._global_callbacks:
+            with self._lock:
+                self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB_GLOBAL))
+                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+            self._global_callbacks.clear()
+
+        # Interrupt the processing thread by poisoning the TCP connection
+        with self._lock:
+            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_INTERRUPT))
         self._process_thread.join()
 
         # Send disconnect and shut down
-        self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_DISCONNECT))
-        self._socket.shutdown(socket.SHUT_RDWR)
-        self._socket.close()
+        with self._lock:
+            self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_DISCONNECT))
+            self._socket.shutdown(socket.SHUT_RDWR)
+            self._socket.close()
         self._closed = True
 
+        # Notify any waiters...
+        self._update_event.set()
+
+class Subscription:
+    """
+    Maintains a subscription and callback to the SubscriptionClient.
+    """
+    def __init__(self, client: SubscriptionClient, key: Optional[bytes], callback: Callable[[bytes, Optional[bytes]], None]) -> None:
+        """
+        Registers a callback for key-value updates to the SubscriptionClient.
+
+        :param client subscription client
+        :param key optional key filter
+        :param callback callback for key-value updates
+        """
+        self._client = client
+        self._key = key
+        self._callback = callback
+        self._client_close_event = Event()
+        self._client_close_event.clear()
+
+        self._client.subscribe(key, callback)
+
+    def close(self) -> None:
+        """
+        Unsubscribes the callback subscription from the subscription client.
+        """
+        self._client.unsubscribe(self._key, self._callback)
+
+        # Notify any waiters...
+        self._client_close_event.set()
+
+        # Don't waste resources...
+        if not self._client.is_subscribed:
+            self._client.close()
+
+    def wait_for_update(self, key: Optional[bytes]) -> bool:
+        """
+        Waits for an update on a specific key to occur.  If no key
+        is specified, it waits for any key to update.
+
+        :returns True if an update occurred, False if the connection
+                 was closed with no update
+        """
+        return self._client.wait_for_update(key)
+    
+    def wait_for_close(self) -> None:
+        """
+        Waits for the client to close.
+        """
+        self._client_close_event.wait()
 
 class Client:
     """
     UpCache client
     """
     def __init__(self, host: str, port: int) -> None:
         """
@@ -564,14 +803,16 @@
         :param port TCP port
         """
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, struct.pack('ii', 1, 0))
         s.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
         s.connect((host, port))
 
+        self._sub_client : Optional[SubscriptionClient] = None
+
         self._lock = Lock()
         self._socket = s
         self._rd = SocketReader(s, 512)
         self._closed = False
         self._refs = 0
 
     def _inc_ref(self) -> None:
@@ -699,25 +940,45 @@
         """
         with self._lock:
             self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_DROP_KEY) + _key_header.pack(len(key)) + key)
             mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
 
             dropped, = struct.unpack('b', self._rd.read(1))
         return dropped == 1
+
+    def _get_subscription_client(self) -> SubscriptionClient:
+        """
+        Creates or returns the existing subscription client for handling
+        client-server subscriptions for key-value updates.
+
+        :returns per-instance SubscriptionClient
+        """
+        if not self._sub_client:
+            host, port = self._socket.getpeername()
+            self._sub_client = SubscriptionClient(host, port)
+        return self._sub_client
     
-    def subscribe(self, key: bytes, callback: Callable[[Optional[bytes]], None]) -> SubscriptionClient:
+    def subscribe(self, key: bytes, callback: Callable[[bytes, Optional[bytes]], None]) -> Subscription:
         """
         Opens a subscription to changes on a key.
 
         :param key the subscription key
-        :param callback associated callback for receiving updates
-        :returns client for maintaining subscription connection
+        :param callback associated callback for receiving key-value updates
+        :returns subscription for maintaining connection details
+        """
+        return Subscription(self._get_subscription_client(), key, callback)
+    
+    def subscribe_all(self, callback: Callable[[bytes, Optional[bytes]], None]) -> Subscription:
         """
-        host, port = self._socket.getpeername()
-        return SubscriptionClient(host, port, key, callback)
+        Opens a subscription to any key changes.
+
+        :param callback associated callback for receiving key-value updates
+        :returns subscription for maintaining connection details
+        """
+        return Subscription(self._get_subscription_client(), None, callback)
     
     def count(self) -> int:
         """
         Returns the total number of key-value pairs in the cache.
 
         :returns number of key-value pairs
         """
@@ -780,14 +1041,18 @@
 
         :param force forces the connection closed
         """
         if self._closed: return
         with self._lock:
             self._refs -= 1
             if force or self._refs <= 0:
+                # Close subscription client
+                if self._sub_client:
+                    self._sub_client.close()
+
                 self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_DISCONNECT))
                 self._socket.shutdown(socket.SHUT_RDWR)
                 self._socket.close()
                 self._refs = 0
             self._closed = True
 
 def _try_unlink(filename: str) -> bool:
```

## Comparing `upcache-0.2.3.dist-info/METADATA` & `upcache-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upcache
-Version: 0.2.3
+Version: 0.2.4
 Summary: In-memory cache with multiprocessing support
 Home-page: https://www.nuradius.com
 Author: Nuradius Software
 Author-email: todd@datacomponents.net
 License: Apache Software License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `upcache-0.2.3.dist-info/RECORD` & `upcache-0.2.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 upcache/cache.py,sha256=ovwovxJbZmD4cCLd2fAzcuPiO2IDbg31Eyi1Pqk0oOo,3459
 upcache/daemon.py,sha256=i3u8gQNL2eD1Rbb7qNkwc640DN0FiYFArYCHTxKMsDg,542
 upcache/errors.py,sha256=jt4DxKkNsbOTWvRx970pZ5XZAbeGOqSJin4ruWvEeJM,783
 upcache/helpers.py,sha256=ShNVK5CkQJA2SNhGRQNyhalTw5V3z4dE6pRnfCg5Qn8,5355
 upcache/networking.py,sha256=O4FfNCOKFUt3eX0MrPFjPMeuTCA5DXItg40xj3rMu6A,72
 upcache/server.py,sha256=EU04kDpnM1HoYI5aO04_pOeQTI_5sdoYagOt8_VtZEM,630
 upcache/internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-upcache/internal/cache.py,sha256=KxU3YobApnbrZfcYy_N4O-zi5vCJ-xffxt-mHBBar_Y,6013
+upcache/internal/cache.py,sha256=XfVKHoU2E7HFBRyMw6KeIuslsNJaJzuPfARY1bEWRRY,5980
 upcache/internal/errors.py,sha256=jt4DxKkNsbOTWvRx970pZ5XZAbeGOqSJin4ruWvEeJM,783
-upcache/internal/tcp.py,sha256=Of8nZMfGbB8acXyOAf6NiwRvtbhVHMFxGnaBXStixZo,27310
-upcache-0.2.3.dist-info/METADATA,sha256=dT155XqOy0_5wfsLoeUbZ1aCI2lyRBgyE5NSuyJcjNI,2970
-upcache-0.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-upcache-0.2.3.dist-info/top_level.txt,sha256=XWEs7c9ubWgJvERCNB8nHI-W1KaAA2bz4PrGDMg3Abs,8
-upcache-0.2.3.dist-info/RECORD,,
+upcache/internal/tcp.py,sha256=mTxDa4LljSvslufHuvLDYCDvQbWE2PEuGcUrK_W59Mc,36994
+upcache-0.2.4.dist-info/METADATA,sha256=sYREUlwQxVXCW8FJJLVjfihpMJOH9V9Ymb6R2P20GZU,2970
+upcache-0.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+upcache-0.2.4.dist-info/top_level.txt,sha256=XWEs7c9ubWgJvERCNB8nHI-W1KaAA2bz4PrGDMg3Abs,8
+upcache-0.2.4.dist-info/RECORD,,
```

