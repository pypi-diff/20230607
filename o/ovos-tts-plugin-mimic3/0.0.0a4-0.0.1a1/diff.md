# Comparing `tmp/ovos_tts_plugin_mimic3-0.0.0a4-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic3-0.0.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21237 bytes, number of entries: 8
--rw-r--r--  2.0 unx    62713 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3/version.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1738 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/WHEEL
--rw-r--r--  2.0 unx      192 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      766 b- defN 23-Mar-14 19:00 ovos_tts_plugin_mimic3-0.0.0a4.dist-info/RECORD
-8 files, 100224 bytes uncompressed, 19871 bytes compressed:  80.2%
+Zip file size: 21250 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    62742 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3/version.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1738 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      766 b- defN 23-Jun-06 22:50 ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD
+8 files, 100253 bytes uncompressed, 19884 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_tts_plugin_mimic3/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic3/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic3-0.0.0a4.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic3/__init__.py

```diff
@@ -103,15 +103,15 @@
         elif lang:
             if lang not in self.default_voices:
                 lang = lang.split("-")[0]
             if lang in self.default_voices:
                 voice = self.default_voices[lang]
             else:
                 raise ValueError(f"Selected lang {lang} is not supported!")
-        elif speaker:
+        elif speaker and isinstance(speaker, str):
             pass  # TODO validate speaker is valid for default voice
         else:
             voice = self.voice
             speaker = self.speaker
 
         if lang:
             a, b = lang.split("-")
```

## ovos_tts_plugin_mimic3/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
-VERSION_BUILD = 0
-VERSION_ALPHA = 4
+VERSION_BUILD = 1
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic3-0.0.0a4.dist-info/LICENSE` & `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic3-0.0.0a4.dist-info/METADATA` & `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic3
-Version: 0.0.0a4
+Version: 0.0.1a1
 Summary: Text to speech plugin for OpenVoiceOS using Mimic3
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic3
 Author: Michael Hansen
 License: AGPL
 Keywords: mycroft plugin tts mimic mimic3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `ovos_tts_plugin_mimic3-0.0.0a4.dist-info/RECORD` & `ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_tts_plugin_mimic3/__init__.py,sha256=SiCVaRSL3B9wLB8s2wfjTPMGBialIuaTZjvDBT4tTZ4,62713
-ovos_tts_plugin_mimic3/version.py,sha256=JN7aD_TugTLEaBIwM5kbDnKdd-QQQx3WIIaO6M_RM2s,177
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/METADATA,sha256=NxnJaKA_uUFT4g1fet80JbgjMUShST2YA5ES_hIhs5M,1738
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/entry_points.txt,sha256=vXVkVOvAevScIuedidXp7Ywp-cmndl7Y5hNSvTzc7QQ,192
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/top_level.txt,sha256=6lmA5NRKPpK3Zlab3O4ZCwwHshZMyqs-QGMzJ7mqC5o,23
-ovos_tts_plugin_mimic3-0.0.0a4.dist-info/RECORD,,
+ovos_tts_plugin_mimic3/__init__.py,sha256=xCuImKD0YvcmKSvcZ-TIScvogMREWSG6r9pKp6RlSm4,62742
+ovos_tts_plugin_mimic3/version.py,sha256=ngFn7CKVyhopdVfKT4gcARfNTt6vFxPLcvHzSZ4vXJY,177
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/METADATA,sha256=9oGtIJU5JodSN8b8JUG3vXG_-laQbN2YIEWSncmHpjI,1738
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/entry_points.txt,sha256=vXVkVOvAevScIuedidXp7Ywp-cmndl7Y5hNSvTzc7QQ,192
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/top_level.txt,sha256=6lmA5NRKPpK3Zlab3O4ZCwwHshZMyqs-QGMzJ7mqC5o,23
+ovos_tts_plugin_mimic3-0.0.1a1.dist-info/RECORD,,
```

