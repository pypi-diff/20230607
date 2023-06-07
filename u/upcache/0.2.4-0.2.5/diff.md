# Comparing `tmp/upcache-0.2.4-py3-none-any.whl.zip` & `tmp/upcache-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 16101 bytes, number of entries: 15
+Zip file size: 16224 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      195 b- defN 22-Dec-17 00:21 upcache/__init__.py
 -rw-r--r--  2.0 unx     3459 b- defN 22-Dec-04 03:59 upcache/cache.py
 -rw-r--r--  2.0 unx      542 b- defN 22-Dec-04 21:48 upcache/daemon.py
 -rw-r--r--  2.0 unx      783 b- defN 22-Dec-04 13:39 upcache/errors.py
 -rw-r--r--  2.0 unx     5355 b- defN 22-Dec-18 03:14 upcache/helpers.py
 -rw-r--r--  2.0 unx       72 b- defN 22-Dec-04 20:34 upcache/networking.py
 -rw-r--r--  2.0 unx      630 b- defN 22-Dec-18 02:01 upcache/server.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-04 20:12 upcache/internal/__init__.py
 -rw-r--r--  2.0 unx     5980 b- defN 23-Jun-07 15:17 upcache/internal/cache.py
 -rw-r--r--  2.0 unx      783 b- defN 22-Dec-04 13:39 upcache/internal/errors.py
--rw-r--r--  2.0 unx    36994 b- defN 23-Jun-07 15:26 upcache/internal/tcp.py
--rw-r--r--  2.0 unx     2970 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-07 16:12 upcache-0.2.4.dist-info/RECORD
-15 files, 59005 bytes uncompressed, 14229 bytes compressed:  75.9%
+-rw-r--r--  2.0 unx    37128 b- defN 23-Jun-07 16:33 upcache/internal/tcp.py
+-rw-r--r--  2.0 unx     2970 b- defN 23-Jun-07 16:34 upcache-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:34 upcache-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-07 16:34 upcache-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-07 16:34 upcache-0.2.5.dist-info/RECORD
+15 files, 59139 bytes uncompressed, 14352 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: upcache/internal/errors.py
 Comment: 
 
 Filename: upcache/internal/tcp.py
 Comment: 
 
-Filename: upcache-0.2.4.dist-info/METADATA
+Filename: upcache-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: upcache-0.2.4.dist-info/WHEEL
+Filename: upcache-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: upcache-0.2.4.dist-info/top_level.txt
+Filename: upcache-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: upcache-0.2.4.dist-info/RECORD
+Filename: upcache-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## upcache/internal/tcp.py

```diff
@@ -569,14 +569,15 @@
         """
         Waits for an update on a specific key to occur.  If no key
         is specified, it waits for any key to update.
 
         :returns True if an update occurred, False if the connection
                  was closed with no update
         """
+        # TODO: this may get hairy for multiple waiters...
         while True:
             self._update_event.wait()
             self._update_event.clear()
             if self._closed:
                 return False
             elif key is None or self._recent_key == key:
                 return True
@@ -592,32 +593,30 @@
     def subscribe(self, key: Optional[bytes], callback: Callable[[bytes, Optional[bytes]], None]) -> None:
         """
         Enrolls a subscription callback for a specified key or all events if key is None.
 
         :param key optional subscription key filter
         :param callback callback for key-value updates
         """
-        s = self._socket
+        _sendall = self._socket.sendall
         if key is None:
             self._global_callbacks.add(callback)
             with self._lock:
-                s.sendall(_envelope.pack(MAGIC_WORD, CMD_SUB_GLOBAL))
-                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+                _sendall(_envelope.pack(MAGIC_WORD, CMD_SUB_GLOBAL))
         else:
             new_key = False
             cb_list = self._callbacks.get(key)
             if cb_list is None:
                 cb_list = set()
                 self._callbacks[key] = cb_list
                 new_key = True
             cb_list.add(callback)
             if new_key:
                 with self._lock:
-                    s.sendall(_envelope.pack(MAGIC_WORD, CMD_SUB) + _key_header.pack(len(key)) + key)
-                    #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+                    _sendall(_envelope.pack(MAGIC_WORD, CMD_SUB) + _key_header.pack(len(key)) + key)
 
     def unsubscribe(self, key: Optional[bytes], callback: Callable[[bytes, Optional[bytes]], None]) -> None:
         """
         Removes a subscription callback from a specified key subscription list or from all events.
 
         :param key optional subscription key filter
         :param callback callback for key-value updates
@@ -627,29 +626,27 @@
                 self._global_callbacks.remove(callback)
             except:
                 pass
             if self._global_callbacks:
                 return
             with self._lock:
                 self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB_GLOBAL))
-                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
         else:
             cb_list = self._callbacks.get(key)
             if cb_list is None:
                 return
             try:
                 cb_list.remove(callback)
             except:
                 pass
             if cb_list:
                 return
             self._callbacks.pop(key)
             with self._lock:
-                s.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB) + _key_header.pack(len(key)) + key)
-                #mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
+                self._socket.sendall(_envelope.pack(MAGIC_WORD, CMD_UNSUB) + _key_header.pack(len(key)) + key)
 
     def _dispatch(self, key: bytes, value: Optional[bytes]) -> None:
         """
         Handles dispatching key-value updates to the appropriate callbacks.
 
         :param key key updated
         :param value optional value updated (None indicates deletion)
@@ -666,33 +663,42 @@
             for cb in cb_list:
                 cb(key, value)
 
     def _process_incoming(self) -> None:
         """
         Processes incoming updates on a dedicated thread.
         """
+        _envelope_size = _envelope.size
+        _rd_read = self._rd.read
+        _envelope_unpack = _envelope.unpack
+        _key_value_header_unpack = _key_value_header.unpack
+        _key_value_header_size = _key_value_header.size
+        _key_response_unpack = _key_response.unpack
+        _key_response_size = _key_response.size
+        _lock = self._lock
+        _dispatch = self._dispatch
         try:
             while True:
                 # Process commands
-                mw, cmd = _envelope.unpack(self._rd.read(_envelope.size))
-                with self._lock:
+                mw, cmd = _envelope_unpack(_rd_read(_envelope_size))
+                with _lock:
                     if cmd == CMD_NOTIFY_UPDATE:
-                        key_len, value_len = _key_value_header.unpack(self._rd.read(_key_value_header.size))
-                        key = self._rd.read(key_len)
-                        value = self._rd.read(value_len)
+                        key_len, value_len = _key_value_header_unpack(_rd_read(_key_value_header_size))
+                        key = _rd_read(key_len)
+                        value = _rd_read(value_len)
                     elif cmd == CMD_NOTIFY_DELETE:
-                        key_len, = _key_response.unpack(self._rd.read(_key_response.size))
-                        key = self._rd.read(key_len)
+                        key_len, = _key_response_unpack(_rd_read(_key_response_size))
+                        key = _rd_read(key_len)
                         value = None
                     elif cmd == CMD_SUB or cmd == CMD_UNSUB or cmd == CMD_SUB_GLOBAL or cmd == CMD_UNSUB_GLOBAL:
                         continue
                     else:
                         # CMD_INTERRUPT and friends funnel here...
                         break
-                self._dispatch(key, value)
+                _dispatch(key, value)
         except:
             pass
 
     def __del__(self) -> None:
         """
         Handles closure if not directly invoked.
         """
```

## Comparing `upcache-0.2.4.dist-info/METADATA` & `upcache-0.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upcache
-Version: 0.2.4
+Version: 0.2.5
 Summary: In-memory cache with multiprocessing support
 Home-page: https://www.nuradius.com
 Author: Nuradius Software
 Author-email: todd@datacomponents.net
 License: Apache Software License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `upcache-0.2.4.dist-info/RECORD` & `upcache-0.2.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 upcache/errors.py,sha256=jt4DxKkNsbOTWvRx970pZ5XZAbeGOqSJin4ruWvEeJM,783
 upcache/helpers.py,sha256=ShNVK5CkQJA2SNhGRQNyhalTw5V3z4dE6pRnfCg5Qn8,5355
 upcache/networking.py,sha256=O4FfNCOKFUt3eX0MrPFjPMeuTCA5DXItg40xj3rMu6A,72
 upcache/server.py,sha256=EU04kDpnM1HoYI5aO04_pOeQTI_5sdoYagOt8_VtZEM,630
 upcache/internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 upcache/internal/cache.py,sha256=XfVKHoU2E7HFBRyMw6KeIuslsNJaJzuPfARY1bEWRRY,5980
 upcache/internal/errors.py,sha256=jt4DxKkNsbOTWvRx970pZ5XZAbeGOqSJin4ruWvEeJM,783
-upcache/internal/tcp.py,sha256=mTxDa4LljSvslufHuvLDYCDvQbWE2PEuGcUrK_W59Mc,36994
-upcache-0.2.4.dist-info/METADATA,sha256=sYREUlwQxVXCW8FJJLVjfihpMJOH9V9Ymb6R2P20GZU,2970
-upcache-0.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-upcache-0.2.4.dist-info/top_level.txt,sha256=XWEs7c9ubWgJvERCNB8nHI-W1KaAA2bz4PrGDMg3Abs,8
-upcache-0.2.4.dist-info/RECORD,,
+upcache/internal/tcp.py,sha256=Kb8N6w2xiabbRs3nskoLCr88p-fRWpUeZbjcokZ2PHc,37128
+upcache-0.2.5.dist-info/METADATA,sha256=Wcf_MRXt6jQqF1sfm3JZ9hnbdZLBMJkFoUe5C-qpBf0,2970
+upcache-0.2.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+upcache-0.2.5.dist-info/top_level.txt,sha256=XWEs7c9ubWgJvERCNB8nHI-W1KaAA2bz4PrGDMg3Abs,8
+upcache-0.2.5.dist-info/RECORD,,
```

