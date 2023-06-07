# Comparing `tmp/EnToFa-1.3.6.tar.gz` & `tmp/EnToFa-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnToFa-1.3.6.tar", last modified: Wed Jun  7 04:26:02 2023, max compression
+gzip compressed data, was "EnToFa-1.4.tar", last modified: Wed Jun  7 04:31:08 2023, max compression
```

## Comparing `EnToFa-1.3.6.tar` & `EnToFa-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:26:02.970311 EnToFa-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-06-07 04:26:02.969311 EnToFa-1.3.6/EnToFa.egg-info/
--rw-rw-rw-   0        0        0      164 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 04:26:02.000000 EnToFa-1.3.6/EnToFa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-06-06 16:33:23.000000 EnToFa-1.3.6/LICENSE
--rw-rw-rw-   0        0        0      164 2023-06-07 04:26:02.969311 EnToFa-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2363 2023-06-06 18:05:47.000000 EnToFa-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 04:26:02.970311 EnToFa-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-06-07 04:25:51.000000 EnToFa-1.3.6/setup.py
--rw-rw-rw-   0        0        0      830 2023-06-06 14:07:12.000000 EnToFa-1.3.6/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:31:08.209662 EnToFa-1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:31:08.209662 EnToFa-1.4/EnToFa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-07 04:30:58.000000 EnToFa-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-07 04:31:08.209662 EnToFa-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-07 04:30:58.000000 EnToFa-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:31:08.209662 EnToFa-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 04:30:58.000000 EnToFa-1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 04:30:58.000000 EnToFa-1.4/translator.py
```

### Comparing `EnToFa-1.3.6/translator.py` & `EnToFa-1.4/translator.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import sys
-import requests
-from win10toast import ToastNotifier
-
-def translate_text(text):
-    url = f"https://translate.googleapis.com/translate_a/single?client=gtx&sl=en&tl=fa&dt=t&q={text}"
-    response = requests.get(url)
-    if response.status_code == 200:
-        data = response.json()
-        translation = data[0][0][0]
-        return translation
-    else:
-        return "Translation failed."
-
-def show_notification(title, message):
-    toaster = ToastNotifier()
-    toaster.show_toast(title, message, duration=10)
-
-def main():
-    text_to_translate = " ".join(sys.argv[1:]) if len(sys.argv) > 1 else input("Enter the text to translate: ")
-    translated_text = translate_text(text_to_translate)
-
-    show_notification(text_to_translate, translated_text)
-
-if __name__ == "__main__":
-    main()
+import sys
+import requests
+from win10toast import ToastNotifier
+
+def translate_text(text):
+    url = f"https://translate.googleapis.com/translate_a/single?client=gtx&sl=en&tl=fa&dt=t&q={text}"
+    response = requests.get(url)
+    if response.status_code == 200:
+        data = response.json()
+        translation = data[0][0][0]
+        return translation
+    else:
+        return "Translation failed."
+
+def show_notification(title, message):
+    toaster = ToastNotifier()
+    toaster.show_toast(title, message, duration=10)
+
+def main():
+    text_to_translate = " ".join(sys.argv[1:]) if len(sys.argv) > 1 else input("Enter the text to translate: ")
+    translated_text = translate_text(text_to_translate)
+
+    show_notification(text_to_translate, translated_text)
+
+if __name__ == "__main__":
+    main()
```

